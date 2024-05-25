# Comparing `tmp/openai_python_client-0.1.0.tar.gz` & `tmp/openai_python_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_python_client-0.1.0.tar", last modified: Thu May  9 11:29:08 2024, max compression
+gzip compressed data, was "openai_python_client-0.2.0.tar", last modified: Sat May 25 20:44:56 2024, max compression
```

## Comparing `openai_python_client-0.1.0.tar` & `openai_python_client-0.2.0.tar`

### file list

```diff
@@ -1,519 +1,519 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.774142 openai_python_client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-09 11:29:08.774142 openai_python_client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:29:08.774142 openai_python_client-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.686142 openai_python_client-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.774142 openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-09 11:29:08.000000 openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32316 2024-05-09 11:29:08.000000 openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:29:08.000000 openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 11:29:08.000000 openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 11:29:08.000000 openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.690142 openai_python_client-0.1.0/src/openai_python_client/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.690142 openai_python_client-0.1.0/src/openai_python_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.694142 openai_python_client-0.1.0/src/openai_python_client/api/assistants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/cancel_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_thread_and_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/delete_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/delete_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/delete_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_run_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_assistants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_run_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/assistants/submit_tool_ouputs_to_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.694142 openai_python_client-0.1.0/src/openai_python_client/api/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/audio/create_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/audio/create_transcription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/audio/create_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.698142 openai_python_client-0.1.0/src/openai_python_client/api/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/batch/cancel_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/batch/create_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/batch/list_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/batch/retrieve_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.698142 openai_python_client-0.1.0/src/openai_python_client/api/chat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/chat/create_chat_completion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.698142 openai_python_client-0.1.0/src/openai_python_client/api/completions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/completions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/completions/create_completion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.698142 openai_python_client-0.1.0/src/openai_python_client/api/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/embeddings/create_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.698142 openai_python_client-0.1.0/src/openai_python_client/api/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/files/create_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/files/delete_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/files/download_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/files/list_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/files/retrieve_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.698142 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/cancel_fine_tuning_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/create_fine_tuning_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_job_checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/list_paginated_fine_tuning_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/retrieve_fine_tuning_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.702142 openai_python_client-0.1.0/src/openai_python_client/api/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/images/create_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/images/create_image_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/images/create_image_variation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.702142 openai_python_client-0.1.0/src/openai_python_client/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/models/delete_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/models/list_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/models/retrieve_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.702142 openai_python_client-0.1.0/src/openai_python_client/api/moderations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/moderations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/moderations/create_moderation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.702142 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/cancel_vector_store_file_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/create_vector_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/create_vector_store_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/create_vector_store_file_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/delete_vector_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/delete_vector_store_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/get_vector_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/get_vector_store_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/get_vector_store_file_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8278 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/list_files_in_vector_store_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/list_vector_store_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/list_vector_stores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/modify_vector_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:29:08.774142 openai_python_client-0.1.0/src/openai_python_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    44246 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_incomplete_details_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_incomplete_details_type_0_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_last_error_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_last_error_type_0_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0_submit_tool_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_message_function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistant_tool_resources_type_0_file_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_api_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_api_response_format_option_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_api_response_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_api_tool_choice_option_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_named_tool_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_named_tool_choice_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/assistants_named_tool_choice_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_errors_data_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_input_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output_error_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output_response_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output_response_type_0_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/batch_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_function_call_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_named_tool_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_named_tool_choice_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_named_tool_choice_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_response_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_response_message_function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_response_message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_options_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_response_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_response_delta_function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_response_delta_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_token_logprob.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_token_logprob_top_logprobs_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_tool_choice_option_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_tool_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_image_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_image_output_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_image_output_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_log_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_log_output_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool_call_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool_call_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/completion_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_batch_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_batch_body_completion_window.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_batch_body_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_batch_body_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_function_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_function_response_choices_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_function_response_choices_item_finish_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_function_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_image_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    31609 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_function_call_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_logit_bias_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_response_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response_choices_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response_choices_item_finish_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response_choices_item_logprobs_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item_finish_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item_logprobs_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    23024 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_request_logit_bias_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item_finish_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0_top_logprobs_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_request_encoding_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_response_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_file_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_file_request_purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters_batch_size_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters_learning_rate_multiplier_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters_n_epochs_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item_type_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item_wandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_edit_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_edit_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_edit_request_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_edit_request_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_request_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_request_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_request_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_request_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_variation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_variation_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_variation_request_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_image_variation_request_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_message_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_message_request_attachments_type_0_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_message_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_message_request_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response_results_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response_results_item_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response_results_item_category_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_run_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_run_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_run_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_speech_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_speech_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_speech_request_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_speech_request_voice.py
--rw-r--r--   0 runner    (1001) docker     (127)    23692 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_file_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_request_response_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_request_timestamp_granularities_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_response_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_response_verbose_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_translation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_translation_request_model_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_translation_response_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_translation_response_verbose_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_file_batch_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_file_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_assistant_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_assistant_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_file_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_message_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_thread_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_thread_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_vector_store_file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_vector_store_file_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_vector_store_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/delete_vector_store_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/done_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/done_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/done_event_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/embedding_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/error_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/error_event_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_citation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_citation_file_citation.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_citation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_path_file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_path_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool_call_file_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool_call_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_checkpoint_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_checkpoint_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_error_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_event_level.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_event_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_hyperparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_hyperparameters_n_epochs_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_integration_wandb.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_tool_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_tool_call_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_tool_call_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/function_tool_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_content_part.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_content_part_image_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_content_part_image_url_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_content_part_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_file_image_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/image_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/images_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_assistants_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_assistants_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_batches_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_batches_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_files_in_vector_store_batch_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_files_in_vector_store_batch_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_files_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_files_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_fine_tuning_job_checkpoints_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_fine_tuning_job_checkpoints_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_fine_tuning_job_events_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_fine_tuning_job_events_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_messages_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_messages_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_models_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_paginated_fine_tuning_jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_paginated_fine_tuning_jobs_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_run_steps_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_run_steps_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_runs_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_threads_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_vector_store_files_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_vector_store_files_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_vector_store_files_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_vector_stores_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/list_vector_stores_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_creation_message_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_creation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_0_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_1_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_2_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_3_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_4_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/model_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_file_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_message_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_message_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_run_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_run_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_file_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/open_ai_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/open_ai_file_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/open_ai_file_purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/open_ai_file_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_completion_usage_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_completion_usage_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_0_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_1_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_2_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_3_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_4_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_5_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_6_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps_last_error_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps_last_error_type_0_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_steps_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_0_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_1_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_2_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_3_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_4_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_5_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_6.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_6_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_7.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_7_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_8.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_8_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_tool_call_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_tool_call_object_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/run_tool_call_object_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/submit_tool_outputs_run_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/submit_tool_outputs_run_request_tool_outputs_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/system_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/system_message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/text_content_part.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/text_content_part_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/text_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/text_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_attachments_type_0_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_incomplete_details_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_incomplete_details_type_0_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_stream_event_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_stream_event_type_0_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_tool_resources_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_tool_resources_type_0_code_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_tool_resources_type_0_file_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_truncation_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/thread_truncation_controls_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/tool_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/tool_calls_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/tool_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/tool_message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/transcription_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/transcription_word.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/update_vector_store_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/update_vector_store_request_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/user_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/user_message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_expiration_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_expiration_policy_anchor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_batch_file_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_batch_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_batch_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files_last_error_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files_last_error_type_0_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_metadata_type_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/models/vector_store_status.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-09 11:28:53.000000 openai_python_client-0.1.0/src/openai_python_client/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.846904 openai_python_client-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-25 20:44:56.846904 openai_python_client-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:44:56.846904 openai_python_client-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.774904 openai_python_client-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.846904 openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-25 20:44:56.000000 openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32316 2024-05-25 20:44:56.000000 openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:44:56.000000 openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-25 20:44:56.000000 openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 20:44:56.000000 openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.778904 openai_python_client-0.2.0/src/openai_python_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.778904 openai_python_client-0.2.0/src/openai_python_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.782904 openai_python_client-0.2.0/src/openai_python_client/api/assistants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/cancel_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_thread_and_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/delete_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/delete_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/delete_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_run_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_assistants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_run_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/assistants/submit_tool_ouputs_to_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.782904 openai_python_client-0.2.0/src/openai_python_client/api/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/audio/create_speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/audio/create_transcription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/audio/create_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.782904 openai_python_client-0.2.0/src/openai_python_client/api/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/batch/cancel_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/batch/create_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/batch/list_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/batch/retrieve_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.782904 openai_python_client-0.2.0/src/openai_python_client/api/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/chat/create_chat_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.782904 openai_python_client-0.2.0/src/openai_python_client/api/completions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/completions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/completions/create_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.782904 openai_python_client-0.2.0/src/openai_python_client/api/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/embeddings/create_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.786904 openai_python_client-0.2.0/src/openai_python_client/api/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/files/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/files/delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/files/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/files/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/files/retrieve_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.786904 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/cancel_fine_tuning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/create_fine_tuning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_job_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/list_paginated_fine_tuning_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/retrieve_fine_tuning_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.786904 openai_python_client-0.2.0/src/openai_python_client/api/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/images/create_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/images/create_image_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/images/create_image_variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.786904 openai_python_client-0.2.0/src/openai_python_client/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/models/delete_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/models/list_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/models/retrieve_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.786904 openai_python_client-0.2.0/src/openai_python_client/api/moderations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/moderations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/moderations/create_moderation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.790904 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/cancel_vector_store_file_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/create_vector_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/create_vector_store_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/create_vector_store_file_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/delete_vector_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/delete_vector_store_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/get_vector_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/get_vector_store_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/get_vector_store_file_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8278 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/list_files_in_vector_store_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/list_vector_store_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/list_vector_stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/modify_vector_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:44:56.846904 openai_python_client-0.2.0/src/openai_python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    44246 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_incomplete_details_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_incomplete_details_type_0_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_last_error_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_last_error_type_0_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0_submit_tool_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_message_function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistant_tool_resources_type_0_file_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_api_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_api_response_format_option_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_api_response_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_api_tool_choice_option_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_named_tool_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_named_tool_choice_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/assistants_named_tool_choice_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_errors_data_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_input_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output_error_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output_response_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output_response_type_0_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/batch_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_function_call_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_named_tool_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_named_tool_choice_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_named_tool_choice_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_response_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_response_message_function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_response_message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_options_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_response_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_response_delta_function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_response_delta_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_token_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_token_logprob_top_logprobs_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_tool_choice_option_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_tool_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_image_output_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_image_output_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_log_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_log_output_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool_call_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/completion_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_batch_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_batch_body_completion_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_batch_body_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_batch_body_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_function_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_function_response_choices_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_function_response_choices_item_finish_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_function_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31609 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_function_call_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_logit_bias_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_response_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response_choices_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response_choices_item_finish_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response_choices_item_logprobs_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item_finish_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item_logprobs_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23024 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_request_logit_bias_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item_finish_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0_top_logprobs_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_request_encoding_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_response_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_file_request_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters_batch_size_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters_learning_rate_multiplier_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters_n_epochs_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item_type_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item_wandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_edit_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_edit_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_edit_request_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_edit_request_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_request_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_request_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_request_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_request_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_variation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_variation_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_variation_request_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_image_variation_request_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_message_request_attachments_type_0_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_message_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_message_request_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response_results_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response_results_item_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response_results_item_category_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23990 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_run_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_run_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_run_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_speech_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_speech_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_speech_request_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_speech_request_voice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23692 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_file_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_request_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_request_timestamp_granularities_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_response_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_response_verbose_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_translation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_translation_request_model_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_translation_response_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_translation_response_verbose_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_file_batch_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_assistant_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_assistant_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_file_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_message_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_thread_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_thread_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_vector_store_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_vector_store_file_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_vector_store_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/delete_vector_store_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/done_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/done_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/done_event_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/embedding_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/error_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/error_event_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_citation_file_citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_citation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_path_file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_path_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool_call_file_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_checkpoint_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_checkpoint_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_error_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_event_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_event_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_hyperparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_hyperparameters_n_epochs_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_integration_wandb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_tool_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_tool_call_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_tool_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/function_tool_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_content_part.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_content_part_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_content_part_image_url_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_content_part_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_file_image_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/image_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/images_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_assistants_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_assistants_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_batches_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_batches_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_files_in_vector_store_batch_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_files_in_vector_store_batch_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_files_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_files_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_fine_tuning_job_checkpoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_fine_tuning_job_checkpoints_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_fine_tuning_job_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_fine_tuning_job_events_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_messages_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_messages_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_models_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_paginated_fine_tuning_jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_paginated_fine_tuning_jobs_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_run_steps_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_run_steps_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_runs_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_threads_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_vector_store_files_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_vector_store_files_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_vector_store_files_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_vector_stores_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/list_vector_stores_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_creation_message_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_creation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_0_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_1_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_2_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_3_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_4_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/model_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_file_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_message_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_message_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_run_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_run_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_file_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/open_ai_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/open_ai_file_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/open_ai_file_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/open_ai_file_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_completion_usage_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_completion_usage_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_0_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_1_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_2_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_3_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_4_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_5_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_6_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11246 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps_last_error_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps_last_error_type_0_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_steps_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_0_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_1_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_2_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_3_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_4_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_5_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_6_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_7_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_8_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_tool_call_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_tool_call_object_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/run_tool_call_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/submit_tool_outputs_run_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/submit_tool_outputs_run_request_tool_outputs_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/system_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/system_message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/text_content_part.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/text_content_part_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/text_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_attachments_type_0_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_incomplete_details_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_incomplete_details_type_0_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_stream_event_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_stream_event_type_0_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_tool_resources_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_tool_resources_type_0_code_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_tool_resources_type_0_file_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_truncation_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/thread_truncation_controls_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/tool_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/tool_calls_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/tool_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/tool_message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/transcription_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/transcription_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/update_vector_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/update_vector_store_request_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/user_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/user_message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_expiration_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_expiration_policy_anchor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_batch_file_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_batch_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_batch_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files_last_error_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files_last_error_type_0_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_metadata_type_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/models/vector_store_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-25 20:44:43.000000 openai_python_client-0.2.0/src/openai_python_client/types.py
```

### Comparing `openai_python_client-0.1.0/PKG-INFO` & `openai_python_client-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OpenAI-Python-Client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pure-python implementation built from OpenAPI-Python-Client Generator https://github.com/openapi-generators/openapi-python-client and OpenAI's published OpenAPI spec https://github.com/openai/openai-openapi
 Author-email: Ian Goforth <ian.goforth@gmail.com>
 License: MIT
-Requires-Python: ==3.11.*
+Requires-Python: ==3.12.*
 Description-Content-Type: text/markdown
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: python-dateutil>=2.9.0.post0
 
 # OpenAI-Python-Client
 A client library for accessing OpenAI API
```

### Comparing `openai_python_client-0.1.0/README.md` & `openai_python_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/pyproject.toml` & `openai_python_client-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "OpenAI-Python-Client"
-version = "0.1.0"
+version = "0.2.0"
 description = "A pure-python implementation built from OpenAPI-Python-Client Generator https://github.com/openapi-generators/openapi-python-client and OpenAI's published OpenAPI spec https://github.com/openai/openai-openapi"
 authors = [
     {name = "Ian Goforth", email = "ian.goforth@gmail.com"},
 ]
 dependencies = [
     "httpx>=0.27.0",
     "attrs>=23.2.0",
     "python-dateutil>=2.9.0.post0",
 ]
-requires-python = "==3.11.*"
+requires-python = "==3.12.*"
 readme = "README.md"
 license = {text = "MIT"}
 
 
 [tool.pdm]
 distribution = true
```

### Comparing `openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/PKG-INFO` & `openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: OpenAI-Python-Client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pure-python implementation built from OpenAPI-Python-Client Generator https://github.com/openapi-generators/openapi-python-client and OpenAI's published OpenAPI spec https://github.com/openai/openai-openapi
 Author-email: Ian Goforth <ian.goforth@gmail.com>
 License: MIT
-Requires-Python: ==3.11.*
+Requires-Python: ==3.12.*
 Description-Content-Type: text/markdown
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: python-dateutil>=2.9.0.post0
 
 # OpenAI-Python-Client
 A client library for accessing OpenAI API
```

### Comparing `openai_python_client-0.1.0/src/OpenAI_Python_Client.egg-info/SOURCES.txt` & `openai_python_client-0.2.0/src/OpenAI_Python_Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/cancel_run.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/cancel_run.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_assistant.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_assistant.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_message.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_run.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_run.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_thread.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_thread.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/create_thread_and_run.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/create_thread_and_run.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/delete_assistant.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/delete_assistant.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/delete_message.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/delete_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/delete_thread.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/delete_thread.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_assistant.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_assistant.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_message.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_run.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_run.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_run_step.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_run_step.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/get_thread.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/get_thread.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_assistants.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_assistants.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_messages.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_messages.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_run_steps.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/list_runs.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/list_runs.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_assistant.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_assistant.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_message.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_run.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_run.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/modify_thread.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/modify_thread.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/assistants/submit_tool_ouputs_to_run.py` & `openai_python_client-0.2.0/src/openai_python_client/api/assistants/submit_tool_ouputs_to_run.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/audio/create_speech.py` & `openai_python_client-0.2.0/src/openai_python_client/api/audio/create_speech.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/audio/create_transcription.py` & `openai_python_client-0.2.0/src/openai_python_client/api/audio/create_transcription.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/audio/create_translation.py` & `openai_python_client-0.2.0/src/openai_python_client/api/audio/create_translation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/batch/cancel_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/batch/cancel_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/batch/create_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/batch/create_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/batch/list_batches.py` & `openai_python_client-0.2.0/src/openai_python_client/api/batch/list_batches.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/batch/retrieve_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/batch/retrieve_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/chat/create_chat_completion.py` & `openai_python_client-0.2.0/src/openai_python_client/api/chat/create_chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/completions/create_completion.py` & `openai_python_client-0.2.0/src/openai_python_client/api/completions/create_completion.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/embeddings/create_embedding.py` & `openai_python_client-0.2.0/src/openai_python_client/api/embeddings/create_embedding.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/files/create_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/files/create_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/files/delete_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/files/delete_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/files/download_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/files/download_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/files/list_files.py` & `openai_python_client-0.2.0/src/openai_python_client/api/files/list_files.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/files/retrieve_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/files/retrieve_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/cancel_fine_tuning_job.py` & `openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/cancel_fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/create_fine_tuning_job.py` & `openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/create_fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_events.py` & `openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_events.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_job_checkpoints.py` & `openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/list_fine_tuning_job_checkpoints.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/list_paginated_fine_tuning_jobs.py` & `openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/list_paginated_fine_tuning_jobs.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/fine_tuning/retrieve_fine_tuning_job.py` & `openai_python_client-0.2.0/src/openai_python_client/api/fine_tuning/retrieve_fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/images/create_image.py` & `openai_python_client-0.2.0/src/openai_python_client/api/images/create_image.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/images/create_image_edit.py` & `openai_python_client-0.2.0/src/openai_python_client/api/images/create_image_edit.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/images/create_image_variation.py` & `openai_python_client-0.2.0/src/openai_python_client/api/images/create_image_variation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/models/delete_model.py` & `openai_python_client-0.2.0/src/openai_python_client/api/models/delete_model.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/models/list_models.py` & `openai_python_client-0.2.0/src/openai_python_client/api/models/list_models.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/models/retrieve_model.py` & `openai_python_client-0.2.0/src/openai_python_client/api/models/retrieve_model.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/moderations/create_moderation.py` & `openai_python_client-0.2.0/src/openai_python_client/api/moderations/create_moderation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/cancel_vector_store_file_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/cancel_vector_store_file_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/create_vector_store.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/create_vector_store.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/create_vector_store_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/create_vector_store_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/create_vector_store_file_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/create_vector_store_file_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/delete_vector_store.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/delete_vector_store.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/delete_vector_store_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/delete_vector_store_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/get_vector_store.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/get_vector_store.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/get_vector_store_file.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/get_vector_store_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/get_vector_store_file_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/get_vector_store_file_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/list_files_in_vector_store_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/list_files_in_vector_store_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/list_vector_store_files.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/list_vector_store_files.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/list_vector_stores.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/list_vector_stores.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/api/vector_stores/modify_vector_store.py` & `openai_python_client-0.2.0/src/openai_python_client/api/vector_stores/modify_vector_store.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/client.py` & `openai_python_client-0.2.0/src/openai_python_client/client.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/errors.py` & `openai_python_client-0.2.0/src/openai_python_client/errors.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/__init__.py` & `openai_python_client-0.2.0/src/openai_python_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread.py` & `openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_incomplete_details_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_incomplete_details_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_last_error_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_last_error_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0_submit_tool_outputs.py` & `openai_python_client-0.2.0/src/openai_python_client/models/a_run_on_a_thread_required_action_type_0_submit_tool_outputs.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant_message.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant_message_function_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant_message_function_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistant_tool_resources_type_0_file_search.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistant_tool_resources_type_0_file_search.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistants_api_response_format.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistants_api_response_format.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistants_named_tool_choice.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistants_named_tool_choice.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/assistants_named_tool_choice_function.py` & `openai_python_client-0.2.0/src/openai_python_client/models/assistants_named_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_errors.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_errors.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_errors_data_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_errors_data_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_request_counts.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_request_counts.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_request_input.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_request_input.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output_error_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output_error_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output_response_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output_response_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/batch_request_output_response_type_0_body.py` & `openai_python_client-0.2.0/src/openai_python_client/models/batch_request_output_response_type_0_body.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_function_call_option.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_function_call_option.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_functions.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_functions.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk_function.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_chunk_function.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_message_tool_call_function.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_message_tool_call_function.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_named_tool_choice.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_named_tool_choice.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_named_tool_choice_function.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_named_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_response_message.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_response_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_response_message_function_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_response_message_function_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_options_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_options_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_response_delta.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_response_delta.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_stream_response_delta_function_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_stream_response_delta_function_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_token_logprob.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_token_logprob.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_token_logprob_top_logprobs_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_token_logprob_top_logprobs_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/chat_completion_tool.py` & `openai_python_client-0.2.0/src/openai_python_client/models/chat_completion_tool.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_image_output.py` & `openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_image_output.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_image_output_image.py` & `openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_image_output_image.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_log_output.py` & `openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_log_output.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool.py` & `openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/code_interpreter_tool_call_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/code_interpreter_tool_call_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/completion_usage.py` & `openai_python_client-0.2.0/src/openai_python_client/models/completion_usage.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_model_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_model_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_assistant_request_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_batch_body.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_batch_body.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_batch_body_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_batch_body_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_function_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_function_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_function_response_choices_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_function_response_choices_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_image_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_image_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_logit_bias_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_logit_bias_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_model_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_model_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_request_response_format.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_request_response_format.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response_choices_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response_choices_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_response_choices_item_logprobs_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_response_choices_item_logprobs_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item_logprobs_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_choices_item_logprobs_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_chat_completion_stream_response_usage.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_chat_completion_stream_response_usage.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_completion_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_completion_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_completion_request_logit_bias_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_completion_request_logit_bias_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0_top_logprobs_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_completion_response_choices_item_logprobs_type_0_top_logprobs_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_embedding_response_usage.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_embedding_response_usage.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_file_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_file_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item_wandb.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_fine_tuning_job_request_integrations_type_0_item_wandb.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_image_edit_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_image_edit_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_image_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_image_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_image_variation_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_image_variation_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_message_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_message_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_message_request_attachments_type_0_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_message_request_attachments_type_0_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_message_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_message_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response_results_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response_results_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response_results_item_categories.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response_results_item_categories.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_moderation_response_results_item_category_scores.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_moderation_response_results_item_category_scores.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_run_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_run_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_run_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_run_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_run_request_model_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_run_request_model_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_speech_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_speech_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_model_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_model_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_file_search.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_and_run_request_tool_resources_type_0_file_search.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_thread_request_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_response_json.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_response_json.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_transcription_response_verbose_json.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_transcription_response_verbose_json.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_translation_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_translation_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_translation_response_json.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_translation_response_json.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_translation_response_verbose_json.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_translation_response_verbose_json.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_file_batch_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_file_batch_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_file_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_file_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/create_vector_store_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/create_vector_store_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_assistant_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_assistant_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_file_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_file_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_message_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_message_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_model_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_model_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_thread_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_thread_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_vector_store_file_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_vector_store_file_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/delete_vector_store_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/delete_vector_store_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/done_event.py` & `openai_python_client-0.2.0/src/openai_python_client/models/done_event.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/embedding.py` & `openai_python_client-0.2.0/src/openai_python_client/models/embedding.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/error.py` & `openai_python_client-0.2.0/src/openai_python_client/models/error.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/error_event.py` & `openai_python_client-0.2.0/src/openai_python_client/models/error_event.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/error_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_citation.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_citation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_citation_file_citation.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_citation_file_citation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_path.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_path.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_path_file_path.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_path_file_path.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/file_search_tool_call_file_search.py` & `openai_python_client-0.2.0/src/openai_python_client/models/file_search_tool_call_file_search.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_checkpoint.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_checkpoint.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_checkpoint_metrics.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_checkpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_error_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_error_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_event.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_event.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_hyperparameters.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_integration.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_integration.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/fine_tuning_job_integration_wandb.py` & `openai_python_client-0.2.0/src/openai_python_client/models/fine_tuning_job_integration_wandb.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/function_message.py` & `openai_python_client-0.2.0/src/openai_python_client/models/function_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/function_object.py` & `openai_python_client-0.2.0/src/openai_python_client/models/function_object.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/function_parameters.py` & `openai_python_client-0.2.0/src/openai_python_client/models/function_parameters.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/function_tool.py` & `openai_python_client-0.2.0/src/openai_python_client/models/function_tool.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/function_tool_call.py` & `openai_python_client-0.2.0/src/openai_python_client/models/function_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/function_tool_call_function.py` & `openai_python_client-0.2.0/src/openai_python_client/models/function_tool_call_function.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/image.py` & `openai_python_client-0.2.0/src/openai_python_client/models/image.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/image_content_part.py` & `openai_python_client-0.2.0/src/openai_python_client/models/image_content_part.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/image_content_part_image_url.py` & `openai_python_client-0.2.0/src/openai_python_client/models/image_content_part_image_url.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/image_file.py` & `openai_python_client-0.2.0/src/openai_python_client/models/image_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/image_file_image_file.py` & `openai_python_client-0.2.0/src/openai_python_client/models/image_file_image_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/images_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/images_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_assistants_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_assistants_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_batches_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_batches_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_files_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_files_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_fine_tuning_job_checkpoints_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_fine_tuning_job_checkpoints_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_fine_tuning_job_events_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_fine_tuning_job_events_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_messages_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_messages_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_models_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_paginated_fine_tuning_jobs_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_paginated_fine_tuning_jobs_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_run_steps_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_run_steps_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_runs_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_runs_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_threads_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_threads_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_vector_store_files_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_vector_store_files_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/list_vector_stores_response.py` & `openai_python_client-0.2.0/src/openai_python_client/models/list_vector_stores_response.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/message_creation.py` & `openai_python_client-0.2.0/src/openai_python_client/models/message_creation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/message_creation_message_creation.py` & `openai_python_client-0.2.0/src/openai_python_client/models/message_creation_message_creation.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_3.py` & `openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_3.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/message_stream_event_type_4.py` & `openai_python_client-0.2.0/src/openai_python_client/models/message_stream_event_type_4.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/model.py` & `openai_python_client-0.2.0/src/openai_python_client/models/model.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_file_search.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_assistant_request_tool_resources_type_0_file_search.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_message_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_message_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_message_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_message_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_run_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_run_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_run_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_run_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_file_search.py` & `openai_python_client-0.2.0/src/openai_python_client/models/modify_thread_request_tool_resources_type_0_file_search.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/open_ai_file.py` & `openai_python_client-0.2.0/src/openai_python_client/models/open_ai_file.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_completion_usage_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_completion_usage_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_completion_usage_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_completion_usage_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_3.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_3.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_4.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_4.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_5.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_5.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_step_stream_event_type_6.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_step_stream_event_type_6.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_steps.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_steps_last_error_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_steps_last_error_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_steps_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_steps_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_1.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_1.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_2.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_2.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_3.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_3.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_4.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_4.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_5.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_5.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_6.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_6.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_7.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_7.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_stream_event_type_8.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_stream_event_type_8.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_tool_call_object.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_tool_call_object.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/run_tool_call_object_function.py` & `openai_python_client-0.2.0/src/openai_python_client/models/run_tool_call_object_function.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/submit_tool_outputs_run_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/submit_tool_outputs_run_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/submit_tool_outputs_run_request_tool_outputs_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/submit_tool_outputs_run_request_tool_outputs_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/system_message.py` & `openai_python_client-0.2.0/src/openai_python_client/models/system_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/text.py` & `openai_python_client-0.2.0/src/openai_python_client/models/text.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/text_content_part.py` & `openai_python_client-0.2.0/src/openai_python_client/models/text_content_part.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/text_text.py` & `openai_python_client-0.2.0/src/openai_python_client/models/text_text.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/the_message_object.py` & `openai_python_client-0.2.0/src/openai_python_client/models/the_message_object.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_attachments_type_0_item.py` & `openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_attachments_type_0_item.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_incomplete_details_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_incomplete_details_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/the_message_object_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/the_message_object_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread_stream_event_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread_stream_event_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread_tool_resources_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread_tool_resources_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread_tool_resources_type_0_code_interpreter.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread_tool_resources_type_0_code_interpreter.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread_tool_resources_type_0_file_search.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread_tool_resources_type_0_file_search.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/thread_truncation_controls.py` & `openai_python_client-0.2.0/src/openai_python_client/models/thread_truncation_controls.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/tool_calls.py` & `openai_python_client-0.2.0/src/openai_python_client/models/tool_calls.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/tool_message.py` & `openai_python_client-0.2.0/src/openai_python_client/models/tool_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/transcription_segment.py` & `openai_python_client-0.2.0/src/openai_python_client/models/transcription_segment.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/transcription_word.py` & `openai_python_client-0.2.0/src/openai_python_client/models/transcription_word.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/update_vector_store_request.py` & `openai_python_client-0.2.0/src/openai_python_client/models/update_vector_store_request.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/update_vector_store_request_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/update_vector_store_request_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/user_message.py` & `openai_python_client-0.2.0/src/openai_python_client/models/user_message.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_expiration_policy.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_expiration_policy.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_batch.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_batch.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_batch_file_counts.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_batch_file_counts.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_file_counts.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_file_counts.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_files_last_error_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_files_last_error_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/models/vector_store_metadata_type_0.py` & `openai_python_client-0.2.0/src/openai_python_client/models/vector_store_metadata_type_0.py`

 * *Files identical despite different names*

### Comparing `openai_python_client-0.1.0/src/openai_python_client/types.py` & `openai_python_client-0.2.0/src/openai_python_client/types.py`

 * *Files identical despite different names*

