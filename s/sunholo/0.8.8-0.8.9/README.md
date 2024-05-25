# Comparing `tmp/sunholo-0.8.8.tar.gz` & `tmp/sunholo-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunholo-0.8.8.tar", last modified: Fri Jan 12 13:40:46 2024, max compression
+gzip compressed data, was "sunholo-0.8.9.tar", last modified: Fri Jan 12 15:21:41 2024, max compression
```

## Comparing `sunholo-0.8.8.tar` & `sunholo-0.8.9.tar`

### file list

```diff
@@ -1,95 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.009710 sunholo-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-12 13:40:37.000000 sunholo-0.8.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-01-12 13:40:46.009710 sunholo-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-01-12 13:40:37.000000 sunholo-0.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-12 13:40:46.009710 sunholo-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-12 13:40:37.000000 sunholo-0.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:45.997710 sunholo-0.8.8/sunholo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:45.997710 sunholo-0.8.8/sunholo/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/dispatch_to_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/agents/flask/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/flask/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/flask/qna_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/langserve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/agents/special_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/archive/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/archive/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/auth/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/bots/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/bots/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/bots/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/chunker/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/data_to_embed_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/message_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/pdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/chunker/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/components/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/components/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/components/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/components/retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/components/vectorstore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.001710 sunholo-0.8.8/sunholo/database/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6694 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:45.993709 sunholo-0.8.8/sunholo/database/sql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/database/sql/sb/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/sql/sb/create_function.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/sql/sb/create_function_time.sql
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/sql/sb/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/sql/sb/delete_source_row.sql
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/sql/sb/return_sources.sql
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/database/sql/sb/setup.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/embedder/embed_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/lookup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/lookup/model_lookup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/patches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/patches/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/patches/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/patches/langchain/vertexai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/pubsub/process_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/pubsub/pubsub_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/qna/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/qna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/qna/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/qna/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/streaming/content_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/streaming/langserve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/streaming/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/summarise/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/summarise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/summarise/summarise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.005710 sunholo-0.8.8/sunholo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/utils/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-12 13:40:37.000000 sunholo-0.8.8/sunholo/utils/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 13:40:46.009710 sunholo-0.8.8/sunholo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-01-12 13:40:45.000000 sunholo-0.8.8/sunholo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-12 13:40:45.000000 sunholo-0.8.8/sunholo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 13:40:45.000000 sunholo-0.8.8/sunholo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-12 13:40:45.000000 sunholo-0.8.8/sunholo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-12 13:40:45.000000 sunholo-0.8.8/sunholo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.843159 sunholo-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-12 15:21:33.000000 sunholo-0.8.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-01-12 15:21:41.843159 sunholo-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-01-12 15:21:33.000000 sunholo-0.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-12 15:21:41.843159 sunholo-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-01-12 15:21:33.000000 sunholo-0.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.831159 sunholo-0.8.9/sunholo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.831159 sunholo-0.8.9/sunholo/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/dispatch_to_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.831159 sunholo-0.8.9/sunholo/agents/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/fastapi/qna_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/agents/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/flask/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/flask/qna_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/langserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/agents/special_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/archive/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/auth/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/bots/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/bots/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/bots/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/chunker/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/data_to_embed_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/message_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/pdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/chunker/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/components/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/components/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/components/retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/components/vectorstore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.835159 sunholo-0.8.9/sunholo/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6694 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.827159 sunholo-0.8.9/sunholo/database/sql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/database/sql/sb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/sql/sb/create_function.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/sql/sb/create_function_time.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/sql/sb/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/sql/sb/delete_source_row.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/sql/sb/return_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/database/sql/sb/setup.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/embedder/embed_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/lookup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/lookup/model_lookup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/patches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/patches/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/patches/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/patches/langchain/vertexai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/pubsub/process_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/pubsub/pubsub_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/qna/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/qna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/qna/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/qna/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/streaming/content_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/streaming/langserve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/streaming/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.839159 sunholo-0.8.9/sunholo/summarise/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/summarise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/summarise/summarise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.843159 sunholo-0.8.9/sunholo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/utils/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-12 15:21:33.000000 sunholo-0.8.9/sunholo/utils/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:21:41.843159 sunholo-0.8.9/sunholo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-01-12 15:21:41.000000 sunholo-0.8.9/sunholo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-12 15:21:41.000000 sunholo-0.8.9/sunholo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 15:21:41.000000 sunholo-0.8.9/sunholo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-12 15:21:41.000000 sunholo-0.8.9/sunholo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-12 15:21:41.000000 sunholo-0.8.9/sunholo.egg-info/top_level.txt
```

### Comparing `sunholo-0.8.8/LICENSE.txt` & `sunholo-0.8.9/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [2023] [Holosun ApS]
+   Copyright [2024] [Holosun ApS]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sunholo-0.8.8/PKG-INFO` & `sunholo-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sunholo
-Version: 0.8.8
+Version: 0.8.9
 Summary: Large Language Model DevOps - a package to help deploy LLMs to the Cloud.
 Home-page: https://github.com/sunholo-data/sunholo-py
-Download-URL: https://github.com/sunholo-data/sunholo-py/archive/refs/tags/v0.8.8.tar.gz
+Download-URL: https://github.com/sunholo-data/sunholo-py/archive/refs/tags/v0.8.9.tar.gz
 Author: Holosun ApS
 Author-email: llmops@sunholo.com
 License: Apache License, Version 2.0
 Keywords: llms,devops,google_cloud_platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -74,15 +74,15 @@
 ## Configuration
 
 The library uses the config specifications that some examples are given in the `config/` folder.
 
 When using the functions, make sure to have the `config/` folder in the root of where your application is running (usually `$HOME/config`)
 
 ```
-   Copyright [2023] [Holosun ApS]
+   Copyright [2024] [Holosun ApS]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sunholo-0.8.8/README.md` & `sunholo-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ## Configuration
 
 The library uses the config specifications that some examples are given in the `config/` folder.
 
 When using the functions, make sure to have the `config/` folder in the root of where your application is running (usually `$HOME/config`)
 
 ```
-   Copyright [2023] [Holosun ApS]
+   Copyright [2024] [Holosun ApS]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sunholo-0.8.8/setup.py` & `sunholo-0.8.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 # Define your base version
-version = '0.8.8'
+version = '0.8.9'
 
 setup(
     name='sunholo',
     version=version,
     packages=find_packages(),
     license='Apache License, Version 2.0',
     long_description=open('README.md').read(),
```

### Comparing `sunholo-0.8.8/sunholo/agents/chat_history.py` & `sunholo-0.8.9/sunholo/agents/chat_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/agents/dispatch_to_qa.py` & `sunholo-0.8.9/sunholo/agents/dispatch_to_qa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,15 +45,15 @@
 
     return qna_endpoint, qna_data
 
 def send_to_qa(user_input, vector_name, chat_history, stream=False, **kwargs):
 
     qna_endpoint, qna_data = prep_request_payload(user_input, chat_history, vector_name, stream, **kwargs)
     header = get_header()
-    
+
     try:
         qna_response = requests.post(qna_endpoint, json=qna_data, stream=stream, headers=header)
         qna_response.raise_for_status()
 
         if stream:
             # If streaming, return a generator that yields response content chunks
             def content_generator():
```

### Comparing `sunholo-0.8.8/sunholo/agents/flask/qna_routes.py` & `sunholo-0.8.9/sunholo/agents/flask/qna_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/agents/langserve.py` & `sunholo-0.8.9/sunholo/agents/langserve.py`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/agents/pubsub.py` & `sunholo-0.8.9/sunholo/agents/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/agents/route.py` & `sunholo-0.8.9/sunholo/agents/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/agents/special_commands.py` & `sunholo-0.8.9/sunholo/agents/special_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/archive/archive.py` & `sunholo-0.8.9/sunholo/archive/archive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/auth/run.py` & `sunholo-0.8.9/sunholo/auth/run.py`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/bots/discord.py` & `sunholo-0.8.9/sunholo/bots/discord.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/bots/webapp.py` & `sunholo-0.8.9/sunholo/bots/webapp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/chunker/data_to_embed_pubsub.py` & `sunholo-0.8.9/sunholo/chunker/data_to_embed_pubsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/chunker/gcs.py` & `sunholo-0.8.9/sunholo/chunker/gcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/chunker/loaders.py` & `sunholo-0.8.9/sunholo/chunker/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/chunker/message_data.py` & `sunholo-0.8.9/sunholo/chunker/message_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/chunker/pdfs.py` & `sunholo-0.8.9/sunholo/chunker/pdfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/chunker/publish.py` & `sunholo-0.8.9/sunholo/chunker/publish.py`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/chunker/splitter.py` & `sunholo-0.8.9/sunholo/chunker/splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/components/llm.py` & `sunholo-0.8.9/sunholo/components/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/components/prompt.py` & `sunholo-0.8.9/sunholo/components/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/components/retriever.py` & `sunholo-0.8.9/sunholo/components/retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/components/vectorstore.py` & `sunholo-0.8.9/sunholo/components/vectorstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/database/database.py` & `sunholo-0.8.9/sunholo/database/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/database/sql/sb/create_function.sql` & `sunholo-0.8.9/sunholo/database/sql/sb/create_function.sql`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/database/sql/sb/create_function_time.sql` & `sunholo-0.8.9/sunholo/database/sql/sb/create_function_time.sql`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/embedder/embed_chunk.py` & `sunholo-0.8.9/sunholo/embedder/embed_chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/logging.py` & `sunholo-0.8.9/sunholo/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/lookup/model_lookup.yaml` & `sunholo-0.8.9/sunholo/lookup/model_lookup.yaml`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/patches/langchain/vertexai.py` & `sunholo-0.8.9/sunholo/patches/langchain/vertexai.py`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/pubsub/process_pubsub.py` & `sunholo-0.8.9/sunholo/pubsub/process_pubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/pubsub/pubsub_manager.py` & `sunholo-0.8.9/sunholo/pubsub/pubsub_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/qna/parsers.py` & `sunholo-0.8.9/sunholo/qna/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/qna/retry.py` & `sunholo-0.8.9/sunholo/qna/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/streaming/content_buffer.py` & `sunholo-0.8.9/sunholo/streaming/content_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/streaming/langserve.py` & `sunholo-0.8.9/sunholo/streaming/langserve.py`

 * *Files identical despite different names*

### Comparing `sunholo-0.8.8/sunholo/streaming/streaming.py` & `sunholo-0.8.9/sunholo/streaming/streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/summarise/summarise.py` & `sunholo-0.8.9/sunholo/summarise/summarise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/utils/config.py` & `sunholo-0.8.9/sunholo/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/utils/gcp.py` & `sunholo-0.8.9/sunholo/utils/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo/utils/parsers.py` & `sunholo-0.8.9/sunholo/utils/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#   Copyright [2023] [Holosun ApS]
+#   Copyright [2024] [Holosun ApS]
 #
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `sunholo-0.8.8/sunholo.egg-info/PKG-INFO` & `sunholo-0.8.9/sunholo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sunholo
-Version: 0.8.8
+Version: 0.8.9
 Summary: Large Language Model DevOps - a package to help deploy LLMs to the Cloud.
 Home-page: https://github.com/sunholo-data/sunholo-py
-Download-URL: https://github.com/sunholo-data/sunholo-py/archive/refs/tags/v0.8.8.tar.gz
+Download-URL: https://github.com/sunholo-data/sunholo-py/archive/refs/tags/v0.8.9.tar.gz
 Author: Holosun ApS
 Author-email: llmops@sunholo.com
 License: Apache License, Version 2.0
 Keywords: llms,devops,google_cloud_platform
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -74,15 +74,15 @@
 ## Configuration
 
 The library uses the config specifications that some examples are given in the `config/` folder.
 
 When using the functions, make sure to have the `config/` folder in the root of where your application is running (usually `$HOME/config`)
 
 ```
-   Copyright [2023] [Holosun ApS]
+   Copyright [2024] [Holosun ApS]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sunholo-0.8.8/sunholo.egg-info/SOURCES.txt` & `sunholo-0.8.9/sunholo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 sunholo/agents/__init__.py
 sunholo/agents/chat_history.py
 sunholo/agents/dispatch_to_qa.py
 sunholo/agents/langserve.py
 sunholo/agents/pubsub.py
 sunholo/agents/route.py
 sunholo/agents/special_commands.py
+sunholo/agents/fastapi/__init__.py
+sunholo/agents/fastapi/qna_routes.py
 sunholo/agents/flask/__init__.py
 sunholo/agents/flask/base.py
 sunholo/agents/flask/qna_routes.py
 sunholo/archive/__init__.py
 sunholo/archive/archive.py
 sunholo/auth/__init__.py
 sunholo/auth/run.py
```

