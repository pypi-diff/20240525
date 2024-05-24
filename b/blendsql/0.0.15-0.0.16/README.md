# Comparing `tmp/blendsql-0.0.15.tar.gz` & `tmp/blendsql-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendsql-0.0.15.tar", last modified: Mon May 13 21:39:37 2024, max compression
+gzip compressed data, was "blendsql-0.0.16.tar", last modified: Fri May 24 22:49:35 2024, max compression
```

## Comparing `blendsql-0.0.15.tar` & `blendsql-0.0.16.tar`

### file list

```diff
@@ -1,119 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.787083 blendsql-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 21:39:33.000000 blendsql-0.0.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29129 2024-05-13 21:39:37.787083 blendsql-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27308 2024-05-13 21:39:33.000000 blendsql-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.771083 blendsql-0.0.15/blendsql/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_program.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_smoothie.py
--rw-r--r--   0 runner    (1001) docker     (127)    27468 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_sqlglot.py
--rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/blend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/blend_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/db/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/grammars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/_cfg_grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/_peg_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/grammars/minEarley/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32720 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/ingredients/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/ingredients/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/join/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/join/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/join/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/map/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/map/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/qa/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/validate/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/ingredient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/models/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/local/_llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/local/_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/remote/_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/nl_to_blendsql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/prompts/_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.787083 blendsql-0.0.15/blendsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29129 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-13 21:39:33.000000 blendsql-0.0.15/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.767083 blendsql-0.0.15/research/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/research/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/research/prompts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/prompts/end_to_end_program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/prompts/parser_program.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/bridge_content_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/dataset_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/fetaqa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/fetaqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/fetaqa/fetaqa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/feverous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/feverous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/feverous/feverous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/hybridqa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/hybridqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/hybridqa/hybridqa.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/ottqa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/ottqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/ottqa/ottqa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/all_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/extraction_from_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18590 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/process_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/wikitq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/wikitq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/wikitq/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/wikitq/wikitq.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:39:37.791082 blendsql-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 21:39:33.000000 blendsql-0.0.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.787083 blendsql-0.0.15/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_generic_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17415 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_multi_table_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_single_table_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.952900 blendsql-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 22:49:31.000000 blendsql-0.0.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-05-24 22:49:35.952900 blendsql-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-05-24 22:49:31.000000 blendsql-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.936900 blendsql-0.0.16/blendsql/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/_smoothie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27640 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/_sqlglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40093 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/blend_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/db/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/db/_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/db/_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/db/bridge_content_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/grammars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/_cfg_grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/_peg_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/grammars/minEarley/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/earley.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/earley_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/earley_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32720 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/earley_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/minEarley/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/grammars/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/ingredients/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/ingredients/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/ingredients/builtin/join/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/join/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/join/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/ingredients/builtin/map/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/map/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.940900 blendsql-0.0.16/blendsql/ingredients/builtin/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/qa/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/blendsql/ingredients/builtin/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/builtin/validate/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/ingredients/ingredient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/blendsql/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/blendsql/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/local/_llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/local/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/blendsql/models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/remote/_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/models/remote/_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/blendsql/nl_to_blendsql/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/nl_to_blendsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/nl_to_blendsql/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/nl_to_blendsql/nl_to_blendsql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/blendsql/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/prompts/_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-24 22:49:31.000000 blendsql-0.0.16/blendsql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.952900 blendsql-0.0.16/blendsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-05-24 22:49:35.000000 blendsql-0.0.16/blendsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-24 22:49:35.000000 blendsql-0.0.16/blendsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:49:35.000000 blendsql-0.0.16/blendsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 22:49:35.000000 blendsql-0.0.16/blendsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 22:49:35.000000 blendsql-0.0.16/blendsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 22:49:35.000000 blendsql-0.0.16/blendsql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-24 22:49:31.000000 blendsql-0.0.16/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.932900 blendsql-0.0.16/research/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/research/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.944900 blendsql-0.0.16/research/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/prompts/end_to_end_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/prompts/parser_program.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/bridge_content_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/dataset_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/fetaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/fetaqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/fetaqa/fetaqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/feverous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/feverous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/feverous/feverous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/hybridqa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/hybridqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/hybridqa/hybridqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/ottqa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/ottqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/ottqa/ottqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/sql/all_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/sql/extraction_from_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18590 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/sql/process_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/research/utils/wikitq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/wikitq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/wikitq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-24 22:49:31.000000 blendsql-0.0.16/research/utils/wikitq/wikitq.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:49:35.952900 blendsql-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-24 22:49:31.000000 blendsql-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.948900 blendsql-0.0.16/tests/grammars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/grammars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/grammars/test_cfg_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:35.952900 blendsql-0.0.16/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/models/test_model_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/models/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/models/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/test_generic_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/test_multi_table_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15864 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/test_single_table_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-24 22:49:31.000000 blendsql-0.0.16/tests/utils.py
```

### Comparing `blendsql-0.0.15/LICENSE` & `blendsql-0.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/_constants.py` & `blendsql-0.0.16/blendsql/_constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import Enum, EnumMeta, auto
+from enum import Enum, EnumMeta
 from dataclasses import dataclass
 
 HF_REPO_ID = "parkervg/blendsql-test-dbs"
 
 
 class StrInMeta(EnumMeta):
     def __contains__(cls, item):
@@ -11,18 +11,18 @@
 
 DEFAULT_ANS_SEP = ";"
 DEFAULT_NAN_ANS = "-"
 VALUE_BATCH_SIZE = 5
 
 
 class IngredientType(str, Enum, metaclass=StrInMeta):
-    MAP = auto()
-    STRING = auto()
-    QA = auto()
-    JOIN = auto()
+    MAP = "MAP"
+    STRING = "STRING"
+    QA = "QA"
+    JOIN = "JOIN"
 
 
 @dataclass
 class IngredientKwarg:
     QUESTION = "question"
     CONTEXT = "context"
     VALUES = "values"
```

### Comparing `blendsql-0.0.15/blendsql/_dialect.py` & `blendsql-0.0.16/blendsql/_dialect.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/_smoothie.py` & `blendsql-0.0.16/blendsql/_smoothie.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 Defines output of an executed BlendSQL script
 """
 
 
 @dataclass
 class SmoothieMeta:
     num_values_passed: int  # Number of values passed to a Map/Join/QA ingredient
-    num_prompt_tokens: int  # Number of prompt tokens (counting user and assistant, i.e. input/output)
+    prompt_tokens: int
+    completion_tokens: int
     prompts: List[str]  # Log of prompts submitted to model
     ingredients: Collection[Ingredient]
     query: str
-    db_path: str
+    db_url: str
     contains_ingredient: bool = True
     process_time_seconds: float = None
 
 
 @dataclass
 class Smoothie:
     df: pd.DataFrame
```

### Comparing `blendsql-0.0.15/blendsql/_sqlglot.py` & `blendsql-0.0.16/blendsql/_sqlglot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlglot
 from sqlglot import exp
 from sqlglot.optimizer.scope import build_scope
-from typing import Generator, List, Set, Tuple, Union
+from typing import Generator, List, Set, Tuple, Union, Callable
 from ast import literal_eval
 from sqlglot.optimizer.scope import find_all_in_scope, find_in_scope
 from attr import attrs, attrib
 
 from .utils import recover_blendsql
 from ._constants import DEFAULT_ANS_SEP, DEFAULT_NAN_ANS
 from ._dialect import _parse_one, FTS5SQLite
@@ -627,58 +627,63 @@
         This function identifies that.
 
         Returns:
             dict, with keys:
                 output_type: numeric | string | boolean
                 pattern: regular expression pattern to use in constrained decoding with Model
         """
+
+        def create_pattern(output_type: str) -> Callable[[int], str]:
+            if output_type == "boolean":
+                base_pattern = f"((t|f|{DEFAULT_NAN_ANS}){DEFAULT_ANS_SEP})"
+            elif output_type == "numeric":
+                base_pattern = f"((([0-9]|\.)+|{DEFAULT_NAN_ANS}){DEFAULT_ANS_SEP})"
+            else:
+                raise ValueError(f"Unknown output_type {output_type}")
+            return lambda num_repeats: base_pattern + "{" + str(num_repeats) + "}"
+
         added_kwargs = {}
         ingredient_node = _parse_one(self.sql()[start:end])
         child = None
         for child, _, _ in self.node.walk():
             if child == ingredient_node:
                 break
         if child is None:
             raise ValueError
         ingredient_node_in_context = child
         start_node = ingredient_node_in_context.parent
         # Below handles when we're in a function
         # Example: CAST({{LLMMap('jump distance', 'w::notes')}} AS FLOAT)
         while isinstance(start_node, exp.Func) and start_node is not None:
             start_node = start_node.parent
+        output_type = None
         predicate_literals: List[str] = []
         if start_node is not None:
             predicate_literals = get_predicate_literals(start_node)
         if len(predicate_literals) > 0:
             if all(isinstance(x, bool) for x in predicate_literals):
-                # Add our bool pattern
-                added_kwargs["pattern"] = f"(t|f|{DEFAULT_ANS_SEP}|{DEFAULT_NAN_ANS})+"
-                added_kwargs["output_type"] = "boolean"
+                output_type = "boolean"
             elif all(isinstance(x, (int, float)) for x in predicate_literals):
-                # Add our int/float pattern
-                added_kwargs[
-                    "pattern"
-                ] = f"(([0-9]|\.)+{DEFAULT_ANS_SEP}|{DEFAULT_NAN_ANS}{DEFAULT_ANS_SEP})+"
-                added_kwargs["output_type"] = "numeric"
+                output_type = "numeric"
             else:
                 predicate_literals = [str(i) for i in predicate_literals]
                 added_kwargs["output_type"] = "string"
                 if len(predicate_literals) > 1:
                     added_kwargs["example_outputs"] = DEFAULT_ANS_SEP.join(
                         predicate_literals
                     )
                 else:
                     added_kwargs[
                         "example_outputs"
                     ] = f"{predicate_literals[0]}{DEFAULT_ANS_SEP}{DEFAULT_NAN_ANS}"
+                return added_kwargs
         elif isinstance(
             ingredient_node_in_context.parent, (exp.Order, exp.Ordered, exp.AggFunc)
         ):
-            # Add our int/float pattern
-            added_kwargs[
-                "pattern"
-            ] = f"(([0-9]|\.)+{DEFAULT_ANS_SEP}|{DEFAULT_NAN_ANS}{DEFAULT_ANS_SEP})+"
-            added_kwargs["output_type"] = "numeric"
+            output_type = "numeric"
+        if output_type is not None:
+            added_kwargs["output_type"] = output_type
+            added_kwargs["pattern"] = create_pattern(output_type)
         return added_kwargs
 
     def sql(self, dialect: sqlglot.dialects.Dialect = FTS5SQLite):
         return recover_blendsql(self.node.sql(dialect=dialect))
```

### Comparing `blendsql-0.0.15/blendsql/blend.py` & `blendsql-0.0.16/blendsql/blend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import copy
 import logging
 import time
 import uuid
 import pandas as pd
-import pyparsing
 import re
 from typing import (
     Dict,
     Iterable,
     List,
     Set,
     Tuple,
     Generator,
     Optional,
     Callable,
     Collection,
+    Type,
 )
 from sqlite3 import OperationalError
 import sqlglot.expressions
 from attr import attrs, attrib
 from functools import partial
 from sqlglot import exp
 from colorama import Fore
 import string
 
 from .utils import (
+    logger,
     sub_tablename,
     get_temp_session_table,
     get_temp_subquery_table,
     recover_blendsql,
     get_tablename_colname,
 )
+from ._exceptions import InvalidBlendSQL
 from .db import Database
-from .db.utils import double_quote_escape, single_quote_escape
+from .db.utils import double_quote_escape, select_all_from_table_query
 from ._sqlglot import (
     MODIFIERS,
     get_first_child,
     get_reversed_subqueries,
     replace_join_with_ingredient_single_ingredient,
     replace_join_with_ingredient_multiple_ingredient,
     prune_true_where,
@@ -47,18 +49,15 @@
     remove_ctes,
     is_in_cte,
 )
 from ._dialect import _parse_one, FTS5SQLite
 from .grammars._peg_grammar import grammar
 from .ingredients.ingredient import Ingredient, IngredientException
 from ._smoothie import Smoothie, SmoothieMeta
-from ._constants import (
-    IngredientType,
-    IngredientKwarg,
-)
+from ._constants import IngredientType, IngredientKwarg
 from .models._model import Model
 
 
 @attrs
 class Kitchen(list):
     """Superset of list. A collection of ingredients."""
 
@@ -73,15 +72,15 @@
     def names(self):
         return [i.name for i in self]
 
     def get_from_name(self, name: str):
         for f in self:
             if f.name == name.upper():
                 return f
-        raise pyparsing.ParseException(
+        raise InvalidBlendSQL(
             f"Ingredient '{name}' called, but not found in passed `ingredient` arg!"
         )
 
     def extend(self, ingredients: Iterable[Ingredient]) -> None:
         try:
             if not all(issubclass(x, Ingredient) for x in ingredients):
                 raise IngredientException(
@@ -141,41 +140,40 @@
             continue
     # Now re-parse with sqlglot
     _query: exp.Expression = _parse_one(query)
     original_query = copy.deepcopy(recover_blendsql(_query.sql(dialect=FTS5SQLite)))
     return (_query, original_query)
 
 
-def preprocess_blendsql(
-    query: str, blender_args: dict, blender: Model
-) -> Tuple[str, dict, set]:
+def preprocess_blendsql(query: str, blender: Model) -> Tuple[str, dict, set]:
     """Parses BlendSQL string with our pyparsing grammar and returns objects
     required for interpretation and execution.
 
     Args:
         query: The BlendSQL query to preprocess
-        blender_args: Arguments used as default in ingredient calls with LLMs
         blender: Model object, which we attach to each parsed_dict
 
     Returns:
         Tuple, containing:
 
             - query
 
             - ingredient_alias_to_parsed_dict
 
             - tables_in_ingredients
 
     Examples:
-          >>> preprocess_blendsql(
-          >>>  query=" SELECT * FROM documents JOIN {{LLMJoin(left_on='w::player', right_on='documents::title')}} WHERE rank = 2",
-          >>>  blender_args={},
-          >>>  blender=blender
-          >>> )
-          (
+        ```python
+        preprocess_blendsql(
+            query="SELECT * FROM documents JOIN {{LLMJoin(left_on='w::player', right_on='documents::title')}} WHERE rank = 2",
+            blender=blender
+        )
+        ```
+        ```text
+        (
             'SELECT documents.title AS \'Player\' , documents.content FROM documents JOIN {{A()}} WHERE w. "rank" = 2',
             {
                 '{{A()}}': {
                     'function': 'LLMJoin',
                     'args': [],
                     'ingredient_aliasname': 'A',
                     'raw': "{{ LLMJoin ( left_on= 'w::player' , right_on= 'documents::title' ) }}",
@@ -183,15 +181,16 @@
                         'left_on': 'w::player',
                         'right_on': 'documents::title',
                         'llm': AzureOpenaiLLM(model_name_or_path='gpt-4', ...)
                     }
                 }
             },
             {'documents', 'w'}
-          )
+        )
+        ```
     """
     ingredient_alias_to_parsed_dict: Dict[str, dict] = {}
     ingredient_str_to_alias: Dict[str, str] = {}
     tables_in_ingredients: Set[str] = set()
     query = re.sub(r"(\s+)", " ", query)
     reversed_scan_res = [scan_res for scan_res in grammar.scanString(query)][::-1]
     for idx, (parse_results, start, end) in enumerate(reversed_scan_res):
@@ -234,32 +233,26 @@
                     else:
                         parsed_results_dict[arg_type][idx][
                             -1
                         ] = formatted_curr_arg  # kwargs gets returned as ['limit', '=', 10] sort of list
             # So we need to parse by indices in dict expression
             # maybe if I was better at pp.Suppress we wouldn't need this
             kwargs_dict = {x[0]: x[-1] for x in parsed_results_dict["kwargs"]}
-            # Optionally modify kwargs dict, depending on blend() blender_args
-            if blender_args is not None:
-                for k, v in blender_args.items():
-                    if k in kwargs_dict:
-                        logging.debug(
-                            Fore.YELLOW
-                            + f"Overriding passed arg for '{k}'!"
-                            + Fore.RESET
-                        )
-                    kwargs_dict[k] = v
             kwargs_dict[IngredientKwarg.MODEL] = blender
             context_arg = kwargs_dict.get(
                 IngredientKwarg.CONTEXT,
-                parsed_results_dict["args"][1]
-                if len(parsed_results_dict["args"]) > 1
-                else parsed_results_dict["args"][1]
-                if len(parsed_results_dict["args"]) > 1
-                else None,
+                (
+                    parsed_results_dict["args"][1]
+                    if len(parsed_results_dict["args"]) > 1
+                    else (
+                        parsed_results_dict["args"][1]
+                        if len(parsed_results_dict["args"]) > 1
+                        else None
+                    )
+                ),
             )
             for arg in {
                 context_arg,
                 kwargs_dict.get("left_on", None),
                 kwargs_dict.get("right_on", None),
             }:
                 if arg is None:
@@ -375,27 +368,26 @@
     **kwargs,
 ):
     """
     Used to disambiguate anonymized BlendSQL function and execute in a recursive context.
     """
     for alias, d in ingredient_alias_to_parsed_dict.items():
         query = re.sub(re.escape(alias), d["raw"], query)
-    logging.debug(
+    logger.debug(
         Fore.CYAN + f"Executing `{query}` and setting to `{aliasname}`..." + Fore.RESET
     )
     return _blend(query=query, **kwargs)
 
 
 def _blend(
     query: str,
     db: Database,
     blender: Optional[Model] = None,
-    ingredients: Optional[Collection[Ingredient]] = None,
+    ingredients: Optional[Collection[Type[Ingredient]]] = None,
     verbose: bool = False,
-    blender_args: Optional[Dict[str, str]] = None,
     infer_gen_constraints: bool = True,
     table_to_title: Optional[Dict[str, str]] = None,
     schema_qualify: bool = True,
     _prev_passed_values: int = 0,
 ) -> Smoothie:
     """Invoked from blend(), this contains the recursive logic to execute
     a BlendSQL query and return a `Smoothie` object.
@@ -407,15 +399,15 @@
     # Create our Kitchen
     kitchen = Kitchen(db=db, session_uuid=session_uuid)
     kitchen.extend(ingredients)
     (
         query,
         ingredient_alias_to_parsed_dict,
         tables_in_ingredients,
-    ) = preprocess_blendsql(query, blender_args=blender_args, blender=blender)
+    ) = preprocess_blendsql(query=query, blender=blender)
     try:
         # Try to parse as a normal SQLite query
         _query: exp.Expression = _parse_one(query)
         original_query = copy.deepcopy(recover_blendsql(_query.sql(dialect=FTS5SQLite)))
         query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
     except sqlglot.errors.ParseError:
         # If we hit an error, wrap in SQLite logic so it's able to be executed
@@ -424,46 +416,49 @@
             kitchen=kitchen,
             ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
         )
         query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
 
     # Preliminary check - we can't have anything that modifies database state
     if _query.find(MODIFIERS):
-        raise ValueError("BlendSQL query cannot have `DELETE` clause!")
+        raise InvalidBlendSQL("BlendSQL query cannot have `DELETE` clause!")
 
     # If there's no `SELECT` and just a QAIngredient, wrap it in a `SELECT CASE` query
     if _query.find(exp.Select) is None:
         _query, original_query = autowrap_query(
             query=query,
             kitchen=kitchen,
             ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
         )
         query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
 
     # If we don't have any ingredient calls, execute as normal SQL
     if len(ingredients) == 0 or len(ingredient_alias_to_parsed_dict) == 0:
         return Smoothie(
-            df=db.execute_query(query),
+            df=db.execute_to_df(query),
             meta=SmoothieMeta(
                 num_values_passed=0,
-                num_prompt_tokens=0,
+                prompt_tokens=blender.prompt_tokens if blender is not None else 0,
+                completion_tokens=(
+                    blender.completion_tokens if blender is not None else 0
+                ),
                 prompts=blender.prompts if blender is not None else [],
                 ingredients=[],
                 query=original_query,
-                db_path=db.db_path,
+                db_url=str(db.db_url),
                 contains_ingredient=False,
             ),
         )
     _get_temp_session_table: Callable = partial(get_temp_session_table, session_uuid)
     # Mapping from {"QA('does this company...', 'constituents::Name')": 'does this company'...})
     function_call_to_res: Dict[str, str] = {}
     session_modified_tables = set()
     # TODO: Currently, as we traverse upwards from deepest subquery,
     #   if any lower subqueries have an ingredient, we deem the current
-    #   as inelligible for optimization. Maybe this can be improved in the future.
+    #   as ineligible for optimization. Maybe this can be improved in the future.
     prev_subquery_has_ingredient = False
     for subquery_idx, subquery in enumerate(get_reversed_subqueries(_query)):
         # At this point, we should have already handled cte statements and created associated tables
         if subquery.find(exp.With) is not None:
             subquery = subquery.transform(remove_ctes)
         # Only cache executed_ingredients within the same subquery
         # The same ingredient may have different results within a different subquery context
@@ -480,15 +475,15 @@
             ]
             if len(parent_select_tablenames) == 1:
                 subquery_str = recover_blendsql(
                     f"SELECT * FROM {parent_select_tablenames[0]} WHERE "
                     + get_first_child(subquery).sql(dialect=FTS5SQLite)
                 )
             else:
-                logging.debug(
+                logger.debug(
                     Fore.YELLOW
                     + "Encountered subquery without `SELECT`, and more than 1 table!\nCannot optimize yet, skipping this step."
                 )
                 continue
         else:
             subquery_str = recover_blendsql(subquery.sql(dialect=FTS5SQLite))
 
@@ -522,60 +517,59 @@
                     aliasname=tablename,
                     query=_query,
                     blender=blender,
                     db=db,
                     ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
                     # Below are in case we need to call blend() again
                     ingredients=ingredients,
-                    blender_args=blender_args,
                     infer_gen_constraints=infer_gen_constraints,
                     table_to_title=table_to_title,
                     verbose=verbose,
                     _prev_passed_values=_prev_passed_values,
                 )
                 query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
             if abstracted_query is not None:
-                logging.debug(
+                logger.debug(
                     Fore.CYAN
                     + f"Executing `{abstracted_query}` and setting to `{_get_temp_subquery_table(tablename)}`..."
                     + Fore.RESET
                 )
                 try:
                     db.to_temp_table(
-                        df=db.execute_query(abstracted_query),
+                        df=db.execute_to_df(abstracted_query),
                         tablename=_get_temp_subquery_table(tablename),
                     )
                 except OperationalError as e:
                     # Fallback to naive execution
-                    logging.debug(Fore.RED + e + Fore.RESET)
-                    logging.debug(
+                    logger.debug(Fore.RED + e + Fore.RESET)
+                    logger.debug(
                         Fore.RED + "Falling back to naive execution..." + Fore.RESET
                     )
                     naive_execution = True
         # Be sure to handle those remaining aliases, which didn't have abstracted queries
         for aliasname, aliased_subquery in scm.alias_to_subquery.items():
             _query = set_subquery_to_alias(
                 subquery=aliased_subquery,
                 aliasname=aliasname,
                 query=_query,
                 blender=blender,
                 db=db,
                 ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
                 # Below are in case we need to call blend() again
                 ingredients=ingredients,
-                blender_args=blender_args,
                 infer_gen_constraints=infer_gen_constraints,
                 table_to_title=table_to_title,
                 verbose=verbose,
                 _prev_passed_values=_prev_passed_values,
             )
             query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
         if prev_subquery_has_ingredient:
             scm.set_node(scm.node.transform(maybe_set_subqueries_to_true))
 
+        # lazy_limit: Union[int, None] = scm.get_lazy_limit()
         # After above processing of AST, sync back to string repr
         subquery_str = scm.sql()
         # Now, 1) Find all ingredients to execute (e.g. '{{f(a, b, c)}}')
         # 2) Track when we've created a new table from a MapIngredient call
         #   only at the end of parsing a subquery, we can merge to the original session_uuid table
         tablename_to_map_out: Dict[str, List[pd.DataFrame]] = {}
         for (
@@ -615,29 +609,32 @@
             # Optionally, recursively call blend() again to get subtable
             # This applies to `context` and `options`
             for i, unpack_kwarg in enumerate(
                 [IngredientKwarg.CONTEXT, IngredientKwarg.OPTIONS]
             ):
                 unpack_value = kwargs_dict.get(
                     unpack_kwarg,
-                    parsed_results_dict["args"][i + 1]
-                    if len(parsed_results_dict["args"]) > i + 1
-                    else parsed_results_dict["args"][i]
-                    if len(parsed_results_dict["args"]) > i
-                    else "",
+                    (
+                        parsed_results_dict["args"][i + 1]
+                        if len(parsed_results_dict["args"]) > i + 1
+                        else (
+                            parsed_results_dict["args"][i]
+                            if len(parsed_results_dict["args"]) > i
+                            else ""
+                        )
+                    ),
                 )
                 if isinstance(unpack_value, str) and unpack_value.upper().startswith(
                     ("SELECT", "WITH")
                 ):
                     _smoothie = _blend(
                         query=unpack_value,
                         db=db,
                         blender=blender,
                         ingredients=ingredients,
-                        blender_args=blender_args,
                         infer_gen_constraints=infer_gen_constraints,
                         table_to_title=table_to_title,
                         verbose=verbose,
                         _prev_passed_values=_prev_passed_values,
                     )
                     _prev_passed_values = _smoothie.meta.num_values_passed
                     subtable = _smoothie.df
@@ -737,22 +734,22 @@
         for tablename, llm_outs in tablename_to_map_out.items():
             if len(llm_outs) > 0:
                 # Once we finish parsing this subquery, write to our session_uuid table
                 # Below, we differ from Binder, which seems to replace the old table
                 # On their left join merge command: https://github.com/HKUNLP/Binder/blob/9eede69186ef3f621d2a50572e1696bc418c0e77/nsql/database.py#L196
                 # We create a new temp table to avoid a potentially self-destructive operation
                 base_tablename = tablename
-                _base_table: pd.DataFrame = db.execute_query(
-                    f'SELECT * FROM "{double_quote_escape(base_tablename)}";'
+                _base_table: pd.DataFrame = db.execute_to_df(
+                    select_all_from_table_query(base_tablename)
                 )
                 base_table = _base_table
                 if db.has_temp_table(_get_temp_session_table(tablename)):
                     base_tablename = _get_temp_session_table(tablename)
-                    base_table: pd.DataFrame = db.execute_query(
-                        f"SELECT * FROM '{single_quote_escape(base_tablename)}';",
+                    base_table: pd.DataFrame = db.execute_to_df(
+                        select_all_from_table_query(base_tablename)
                     )
                 previously_added_columns = base_table.columns.difference(
                     _base_table.columns
                 )
                 assert len(set([len(x) for x in llm_outs])) == 1
                 llm_out_df = pd.concat(llm_outs, axis=1)
                 llm_out_df = llm_out_df.loc[:, ~llm_out_df.columns.duplicated()]
@@ -790,100 +787,138 @@
         )
     for a, t in scm.alias_to_tablename.items():
         if t in session_modified_tables:
             query = sub_tablename(
                 a, f'"{double_quote_escape(_get_temp_session_table(t))}"', query
             )
 
-    logging.debug("")
-    logging.debug(
+    logger.debug("")
+    logger.debug(
         "**********************************************************************************"
     )
-    logging.debug(Fore.LIGHTGREEN_EX + f"Final Query:\n{query}" + Fore.RESET)
-    logging.debug(
+    logger.debug(Fore.LIGHTGREEN_EX + f"Final Query:\n{query}" + Fore.RESET)
+    logger.debug(
         "**********************************************************************************"
     )
-    logging.debug("")
+    logger.debug("")
 
-    df = db.execute_query(query)
+    df = db.execute_to_df(query)
 
     return Smoothie(
         df=df,
         meta=SmoothieMeta(
             process_time_seconds=time.time() - start,
             num_values_passed=sum(
                 [
                     i.num_values_passed
                     for i in kitchen
                     if hasattr(i, "num_values_passed")
                 ]
             )
             + _prev_passed_values,
-            num_prompt_tokens=blender.num_prompt_tokens if blender is not None else 0,
+            prompt_tokens=blender.prompt_tokens if blender is not None else 0,
+            completion_tokens=blender.completion_tokens if blender is not None else 0,
             prompts=blender.prompts if blender is not None else [],
             ingredients=ingredients,
             query=original_query,
-            db_path=db.db_path,
+            db_url=str(db.db_url),
         ),
     )
 
 
 def blend(
     query: str,
     db: Database,
     blender: Optional[Model] = None,
-    ingredients: Optional[Collection[Ingredient]] = None,
+    ingredients: Optional[Collection[Type[Ingredient]]] = None,
     verbose: bool = False,
-    blender_args: Optional[Dict[str, str]] = None,
     infer_gen_constraints: bool = True,
     table_to_title: Optional[Dict[str, str]] = None,
     schema_qualify: bool = True,
 ) -> Smoothie:
-    """The `blend()` function is used to execute a BlendSQL query against a database and
+    '''The `blend()` function is used to execute a BlendSQL query against a database and
     return the final result, in addition to the intermediate reasoning steps taken.
     Execution is done on a database given an ingredient context.
 
     Args:
         query: The BlendSQL query to execute
         db: Database connector object
-        ingredients: List of ingredient objects, to use in interpreting BlendSQL query
-        verbose: Boolean defining whether to run in logging.debug mode
-        blender: Optionally override whatever llm argument we pass to Model ingredient.
-            Useful for research applications, where we don't (necessarily) want the parser to choose endpoints.
+        ingredients: Collection of ingredient objects, to use in interpreting BlendSQL query
+        verbose: Boolean defining whether to run with logger in debug mode
+        blender: Which BlendSQL model to use in performing ingredient tasks in the current query
         infer_gen_constraints: Optionally infer the output format of an `IngredientMap` call, given the predicate context
             For example, in `{{LLMMap('convert to date', 'w::listing date')}} <= '1960-12-31'`
-            We can infer the output format should look like '1960-12-31'
-                and put this in the `example_outputs` kwarg
+            We can infer the output format should look like '1960-12-31' and both:
+                1) Put this string in the `example_outputs` kwarg
+                2) If we have a LocalModel, pass the '\d{4}-\d{2}-\d{2}' pattern to outlines.generate.regex
         table_to_title: Optional mapping from table name to title of table.
             Useful for datasets like WikiTableQuestions, where relevant info is stored in table title.
         schema_qualify: Optional bool, determines if we run qualify_columns() from sqlglot
             This enables us to write BlendSQL scripts over multi-table databases without manually qualifying columns ourselves
             However, we need to call db.get_sqlglot_schema() if schema_qualify=True, which may add some latency.
             With single-table queries, we can set this to False.
 
     Returns:
         smoothie: `Smoothie` dataclass containing pd.DataFrame output and execution metadata
-    """
+
+    Examples:
+        ```python
+        from blendsql import blend, LLMMap, LLMQA, LLMJoin
+        from blendsql.db import SQLite
+        from blendsql.models import OpenaiLLM
+        from blendsql.utils import fetch_from_hub
+
+        blendsql = """
+        SELECT * FROM w
+        WHERE city = {{
+            LLMQA(
+                'Which city is located 120 miles west of Sydney?',
+                (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+                options='w::city'
+            )
+        }}
+        """
+        smoothie = blend(
+            query=blendsql,
+            db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+            ingredients={LLMMap, LLMQA, LLMJoin},
+            blender=OpenaiLLM("gpt-3.5-turbo"),
+            # Optional args below
+            infer_gen_constraints=True,
+            silence_db_exec_errors=False,
+            verbose=True
+        )
+        ```
+    '''
     if verbose:
-        logging.getLogger().setLevel(logging.DEBUG)
+        logger.setLevel(logging.DEBUG)
     else:
-        logging.getLogger().setLevel(logging.ERROR)
+        logger.setLevel(logging.ERROR)
     start = time.time()
     try:
         smoothie = _blend(
             query=query,
             db=db,
             blender=blender,
             ingredients=ingredients,
-            blender_args=blender_args,
             infer_gen_constraints=infer_gen_constraints,
             table_to_title=table_to_title,
             schema_qualify=schema_qualify,
         )
     except Exception as error:
+        if not isinstance(error, (InvalidBlendSQL, IngredientException)):
+            from .grammars.minEarley.parser import EarleyParser
+            from .grammars.utils import load_cfg_parser
+
+            # Parse with CFG and try to get helpful recommendations
+            parser: EarleyParser = load_cfg_parser(ingredients)
+            try:
+                parser.parse(query)
+            except Exception as parser_error:
+                raise parser_error
         raise error
     finally:
         # In the case of a recursive `_blend()` call,
         #   this logic allows temp tables to persist until
         #   the final base case is fulfilled.
         db._reset_connection()
     smoothie.meta.process_time_seconds = time.time() - start
```

### Comparing `blendsql-0.0.15/blendsql/blend_cli.py` & `blendsql-0.0.16/blendsql/blend_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 import os
 import argparse
 import importlib
-import json
 
 from blendsql import blend
 from blendsql.db import SQLite
+from blendsql.db.utils import truncate_df_content
 from blendsql.utils import tabulate
-from blendsql.models import LlamaCppLLM
-from blendsql.ingredients.builtin import LLMQA, LLMMap, LLMJoin, DT
+from blendsql.models import (
+    OpenaiLLM,
+    TransformersLLM,
+    AzureOpenaiLLM,
+    LlamaCppLLM,
+    OllamaLLM,
+)
+from blendsql.ingredients.builtin import LLMQA, LLMMap, LLMJoin
 
 _has_readline = importlib.util.find_spec("readline") is not None
 
+MODEL_TYPE_TO_CLASS = {
+    "openai": OpenaiLLM,
+    "azure_openai": AzureOpenaiLLM,
+    "llama_cpp": LlamaCppLLM,
+    "transformers": TransformersLLM,
+    "ollama": OllamaLLM,
+}
+
 
 def print_msg_box(msg, indent=1, width=None, title=None):
     """Print message-box with optional title."""
     lines = msg.split("\n")
     space = " " * indent
     if not width:
         width = max(map(len, lines))
@@ -33,16 +47,29 @@
 
 def main():
     if _has_readline:
         import readline
 
         _ = readline
     parser = argparse.ArgumentParser()
-    parser.add_argument("db_path", nargs="?")
-    parser.add_argument("secrets_path", nargs="?", default="./secrets.json")
+    parser.add_argument("db_path", nargs="?", help="Database path")
+    parser.add_argument(
+        "model_type",
+        nargs="?",
+        default="openai",
+        choices=list(MODEL_TYPE_TO_CLASS.keys()),
+        help="Model type, for the Blender to use in executing the BlendSQL query.",
+    )
+    parser.add_argument(
+        "model_name_or_path",
+        nargs="?",
+        default="gpt-3.5-turbo",
+        help="Model identifier to pass to the selected model_type class.",
+    )
+    parser.add_argument("-v", action="store_true", help="Flag to run in verbose mode.")
     args = parser.parse_args()
 
     db = SQLite(db_path=args.db_path)
     print_msg_box(f"Beginning BlendSQL session with '{args.db_path}'...")
     print()
     while True:
         lines = []
@@ -57,34 +84,18 @@
             cls()
             print_msg_box("Beginning BlendSQL session...")
             continue
         try:
             smoothie = blend(
                 query=text,
                 db=db,
-                ingredients={LLMQA, LLMMap, LLMJoin, DT},
-                blender=LlamaCppLLM(
-                    "./lark-constrained-parsing/tinyllama-1.1b-chat-v1.0.Q2_K.gguf"
+                ingredients={LLMQA, LLMMap, LLMJoin},
+                blender=MODEL_TYPE_TO_CLASS.get(args.model_type)(
+                    args.model_name_or_path
                 ),
                 infer_gen_constraints=True,
-                verbose=True,
+                verbose=args.v,
             )
             print()
-            print(tabulate(smoothie.df.iloc[:10]))
-            print()
-            print(json.dumps(smoothie.meta.prompts, indent=4))
+            print(tabulate(truncate_df_content(smoothie.df, 50)))
         except Exception as error:
             print(error)
-
-
-"""
-SELECT "common name" AS 'State Flower' FROM w 
-WHERE state = {{
-    LLMQA(
-        'Which is the smallest state by area?',
-        (SELECT title, content FROM documents WHERE documents MATCH 'smallest OR state OR area' LIMIT 3),
-        options='w::state'
-    )
-}}
-
-SELECT Symbol, Description, Quantity FROM portfolio WHERE {{LLMMap('Do they manufacture cell phones?', 'portfolio::Description')}} = TRUE AND portfolio.Symbol in (SELECT Symbol FROM constituents WHERE Sector = 'Information Technology')
-"""
```

### Comparing `blendsql-0.0.15/blendsql/db/_sqlite.py` & `blendsql-0.0.16/blendsql/db/_sqlite.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from sqlalchemy.engine import make_url, URL
 
 from .utils import double_quote_escape
 from ._database import Database
 
 
 class SQLite(Database):
     """A SQLite database connection.
@@ -12,20 +13,22 @@
         ```python
         from blendsql.db import SQLite
         db = SQLite("./path/to/database.db")
         ```
     """
 
     def __init__(self, db_path: str):
-        super().__init__(db_path=Path(db_path).resolve(), db_prefix="sqlite:///")
+        self._raw_db_path = Path(db_path).resolve()
+        db_url: URL = make_url(f"sqlite:///{self._raw_db_path}")
+        super().__init__(db_url=db_url)
 
     def has_temp_table(self, tablename: str) -> bool:
         return (
             tablename
-            in self.execute_query(
+            in self.execute_to_df(
                 "SELECT name FROM sqlite_temp_master WHERE type='table';"
             )["name"].unique()
         )
 
     def get_sqlglot_schema(self) -> dict:
         """Returns database schema as a dictionary, in the format that
         sqlglot.optimizer expects.
@@ -33,15 +36,15 @@
         Examples:
             >>> db.get_sqlglot_schema()
             {"x": {"A": "INT", "B": "INT", "C": "INT", "D": "INT", "Z": "STRING"}}
         """
         schema = {}
         for tablename in self.tables():
             schema[f'"{double_quote_escape(tablename)}"'] = {}
-            for _, row in self.execute_query(
+            for _, row in self.execute_to_df(
                 f"""
             SELECT name, type FROM pragma_table_info(:t)
             """,
                 {"t": tablename},
             ).iterrows():
                 schema[f'"{double_quote_escape(tablename)}"'][
                     '"' + row["name"] + '"'
```

### Comparing `blendsql-0.0.15/blendsql/grammars/_cfg_grammar.lark` & `blendsql-0.0.16/blendsql/grammars/_cfg_grammar.lark`

 * *Files 9% similar despite different names*

```diff
@@ -62,30 +62,34 @@
 
 ?expression_math: expression_product
                | expression_math "+" expression_product -> expression_add
                | expression_math "-" expression_product -> expression_sub
                | "CASE"i (when_then)+ "ELSE"i expression_math "END"i -> case_expression
                | "CAST"i "(" expression_math "AS"i TYPENAME ")" -> as_type
                | "CAST"i "(" literal "AS"i TYPENAME ")" -> literal_cast
-               | AGGREGATION_FUNCTIONS expression_math ")" [window_form] -> sql_aggregation
+               | AGGREGATE_FUNCTIONS expression_math ")" [window_form] -> sql_aggregation
                | SCALAR_FUNCTIONS [(expression_math ",")*] expression_math ")" -> sql_scalar
                | blendsql_aggregation_expr -> blendsql_aggregation
+               | blendsql_scalar_expr -> blendsql_scalar
                | "RANK"i "(" ")" window_form -> rank_expression
                | "DENSE_RANK"i "(" ")" window_form -> dense_rank_expression
                | "|" "|" expression_math
 
-BLENDSQL_AGGREGATION: ("LLMQA("i | "LLMVerify("i)
-BLENDSQL_JOIN: ("LLMJoin("i)
+BLENDSQL_AGGREGATE_FUNCTIONS: $blendsql_aggregate_functions
+BLENDSQL_JOIN_FUNCTIONS: $blendsql_join_functions
+BLENDSQL_SCALAR_FUNCTIONS: $blendsql_scalar_functions
 left_on_arg: "left_on" "=" string
 right_on_arg: "right_on" "=" string
-blendsql_arg: (name "=" literal | literal | "(" start ")")
+blendsql_arg: (literal | "(" start ")")
+blendsql_argnames: ("context"|"question"|"options")
 
-blendsql_expression_math: blendsql_arg ("," blendsql_arg)*
-blendsql_aggregation_expr: "{{" BLENDSQL_AGGREGATION blendsql_expression_math ")" "}}"
-blendsql_join_expr: "{{" BLENDSQL_JOIN (left_on_arg "," right_on_arg|right_on_arg "," left_on_arg) ")" "}}"
+blendsql_expression_math: [blendsql_argnames "="] blendsql_arg ("," [blendsql_argnames "="] blendsql_arg)*
+blendsql_aggregation_expr: blendsql_function_begin BLENDSQL_AGGREGATE_FUNCTIONS blendsql_expression_math ")" blendsql_function_end
+blendsql_scalar_expr: blendsql_function_begin BLENDSQL_SCALAR_FUNCTIONS blendsql_expression_math ")" blendsql_function_end
+blendsql_join_expr: blendsql_function_begin BLENDSQL_JOIN_FUNCTIONS (left_on_arg "," right_on_arg|right_on_arg "," left_on_arg) ")" blendsql_function_end
 
 window_form: "OVER"i "(" ["PARTITION"i "BY"i (expression_math ",")* expression_math] ["ORDER"i "BY"i (order ",")* order [ row_range_clause ] ] ")"
 
 row_range_clause: ( ROWS | RANGE ) frame_extent
 frame_extent: frame_between | frame_preceding
 frame_between: "BETWEEN"i frame_bound "AND"i frame_bound
 frame_bound: frame_preceding | frame_following | "CURRENT"i "ROW"i
@@ -121,15 +125,15 @@
          | "timestamp"i
          | "time"i
          | "date"i
          | "category"i
          | "string"i
 
 // https://www.sqlite.org/lang_expr.html#*funcinexpr
-AGGREGATION_FUNCTIONS: ("sum("i | "avg("i | "min("i | "max("i | "count("i ["distinct"i] )
+AGGREGATE_FUNCTIONS: ("sum("i | "avg("i | "min("i | "max("i | "count("i ["distinct"i] )
 SCALAR_FUNCTIONS: ("trim("i | "coalesce("i | "abs("i)
 
 alias: string -> alias_string
 _window_name: name
 limit_count: integer_ -> limit_count
 skip_rows: integer_
 bool_expression: bool_parentheses
@@ -181,13 +185,17 @@
 DAY: /[0-9]{2}/
 time: HOURS ":" MINUTES ":" SECONDS
 HOURS: /[0-9]{2}/
 MINUTES: /[0-9]{2}/
 SECONDS: /[0-9]{2}/
 name: CNAME | ESCAPED_STRING | | /`([^`]|\s)+`|``/
 SEMICOLON: ";"
+CURLY_BRACKET_OPEN: "{"
+CURLY_BRACKET_CLOSE: "}"
+blendsql_function_begin: CURLY_BRACKET_OPEN ~ 2
+blendsql_function_end: CURLY_BRACKET_CLOSE ~ 2
 
 %import common.ESCAPED_STRING
 %import common.CNAME
 %import common.NUMBER
 %import common.WS
 %ignore WS
```

### Comparing `blendsql-0.0.15/blendsql/grammars/_peg_grammar.py` & `blendsql-0.0.16/blendsql/grammars/_peg_grammar.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/grammars/minEarley/earley.py` & `blendsql-0.0.16/blendsql/grammars/minEarley/earley.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/grammars/minEarley/earley_analyzer.py` & `blendsql-0.0.16/blendsql/grammars/minEarley/earley_analyzer.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/grammars/minEarley/earley_exceptions.py` & `blendsql-0.0.16/blendsql/grammars/minEarley/earley_exceptions.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/grammars/minEarley/earley_forest.py` & `blendsql-0.0.16/blendsql/grammars/minEarley/earley_forest.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/grammars/minEarley/parser.py` & `blendsql-0.0.16/blendsql/grammars/minEarley/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,18 @@
 
     def handle_error(self, e):
         CANDIDATE_LIMIT = 64
 
         def regex_to_candidates(regex):
             candidates = set()
             if exrex.count(regex) > CANDIDATE_LIMIT:
-                logger.warning(f"regex {regex} has too many candidates")
+                logger.warning(
+                    f"regex {regex} has too many candidates. ignoring this pattern"
+                )
+                return candidates
             for candidate in exrex.generate(regex, limit=CANDIDATE_LIMIT):
                 candidates.add(candidate)
             return candidates
 
         def pattern_to_candidates(pattern: Pattern):
             candidates = set()
             if isinstance(pattern, PatternStr):
```

### Comparing `blendsql-0.0.15/blendsql/grammars/minEarley/tree.py` & `blendsql-0.0.16/blendsql/grammars/minEarley/tree.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/blendsql/ingredients/builtin/join/main.py` & `blendsql-0.0.16/blendsql/ingredients/builtin/join/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,169 @@
-from typing import List, Optional
-from guidance import gen
-from textwrap import dedent
+from typing import List, Optional, Tuple
+import outlines
+import re
+from colorama import Fore
 
-from blendsql.models._model import Model
-from blendsql._program import Program
+from blendsql.models import Model, LocalModel, OllamaLLM
+from blendsql._program import Program, return_ollama_response
 from blendsql import _constants as CONST
 from blendsql.ingredients.ingredient import JoinIngredient
+from blendsql.utils import logger, newline_dedent
 
 
 class JoinProgram(Program):
     def __call__(
         self,
+        model: Model,
         join_criteria: str,
         left_values: List[str],
         right_values: List[str],
         sep: str,
         **kwargs,
-    ):
-        _model = self.model
-        left_values = "\n".join(left_values)
-        right_values = "\n".join(right_values)
-        with self.systemcontext:
-            _model += "You are a database expert in charge of performing a modified `LEFT JOIN` operation. This `LEFT JOIN` is based on a semantic criteria given by the user."
-            _model += f"\nThe left and right value alignment should be separated by '{sep}', with each new `JOIN` alignment goin on a newline. If a given left value has no corresponding right value, give '-' as a response."
-        with self.usercontext:
-            if self.few_shot:
-                _model += dedent(
-                    """
-                Criteria: Join to same topics.
-
-                Left Values:
-                joshua fields
-                bob brown
-                ron ryan
-
-                Right Values:
-                ron ryan
-                colby mules
-                bob brown (ice hockey)
-                josh fields (pitcher)
-
-                Output:
-                joshua fields;josh fields (pitcher)
-                bob brown;bob brown (ice hockey)
-                ron ryan;ron ryan
-
-                ---
-
-                Criteria: Align the fruit to their corresponding colors.
-
-                Left Values:
-                apple
-                banana
-                blueberry
-                orange
-
-                Right Values:
-                blue
-                yellow
-                red
-
-                Output:
-                apple;red
-                banana;yellow
-                blueberry;blue
-                orange;-
+    ) -> Tuple[str, str]:
+        prompt = ""
+        prompt += "You are a database expert in charge of performing a modified `LEFT JOIN` operation. This `LEFT JOIN` is based on a semantic criteria given by the user."
+        prompt += f"\nThe left and right value alignment should be separated by '{sep}', with each new `JOIN` alignment goin on a newline. If a given left value has no corresponding right value, give '-' as a response."
+        prompt += newline_dedent(
+            """
+        Criteria: Join to same topics.
+
+        Left Values:
+        joshua fields
+        bob brown
+        ron ryan
+
+        Right Values:
+        ron ryan
+        colby mules
+        bob brown (ice hockey)
+        josh fields (pitcher)
+
+        Output:
+        joshua fields;josh fields (pitcher)
+        bob brown;bob brown (ice hockey)
+        ron ryan;ron ryan
+
+        ---
+
+        Criteria: Align the fruit to their corresponding colors.
+
+        Left Values:
+        apple
+        banana
+        blueberry
+        orange
+
+        Right Values:
+        blue
+        yellow
+        red
+
+        Output:
+        apple;red
+        banana;yellow
+        blueberry;blue
+        orange;-
 
-                ---
-                """
+        ---
+        """
+        )
+        prompt += newline_dedent(
+            """
+            Criteria: {}
+
+            Left Values:
+            {}
+
+            Right Values:
+            {}
+
+            Output:
+            """.format(
+                join_criteria, "\n".join(left_values), "\n".join(right_values)
+            )
+        )
+        # Create this pattern on the fly, and not in infer_gen_constraints
+        # since it depends on what our left/right values are
+        regex = (
+            lambda num_repeats: "(({}){}({})\n)".format(
+                "|".join([re.escape(i) for i in left_values]),
+                CONST.DEFAULT_ANS_SEP,
+                "|".join(
+                    [re.escape(i) for i in right_values] + [CONST.DEFAULT_NAN_ANS]
+                ),
+            )
+            + "{"
+            + str(num_repeats)
+            + "}"
+        )
+        max_tokens = (
+            len(
+                model.tokenizer.encode(
+                    "".join(left_values)
+                    + "".join(right_values)
+                    + (CONST.DEFAULT_ANS_SEP * len(left_values)),
                 )
-            _model += dedent(
-                f"""
-                Criteria: {join_criteria}
-
-                Left Values:
-                {left_values}
-
-                Right Values:
-                {right_values}
+            )
+            if model.tokenizer is not None
+            else None
+        )
 
-                Output:
-                """
+        if isinstance(model, LocalModel):
+            generator = outlines.generate.regex(
+                model.logits_generator, regex(len(left_values))
             )
-        with self.assistantcontext:
-            _model += gen(name="result", **self.gen_kwargs)
-        return _model
+        else:
+            if isinstance(model, OllamaLLM):
+                # Handle call to ollama
+                return return_ollama_response(
+                    logits_generator=model.logits_generator,
+                    prompt=prompt,
+                    max_tokens=max_tokens,
+                    temperature=0.0,
+                )
+            generator = outlines.generate.text(model.logits_generator)
+
+        result = generator(
+            prompt,
+            max_tokens=max_tokens,
+            stop_at=["---"],
+        )
+        logger.debug(Fore.CYAN + prompt + Fore.RESET)
+        logger.debug(Fore.LIGHTCYAN_EX + result + Fore.RESET)
+        return (result, prompt)
 
 
 class LLMJoin(JoinIngredient):
     DESCRIPTION = """
     If we need to do a `join` operation where there is imperfect alignment between table values, use the new function:
         `{{LLMJoin(left_on='table::column', right_on='table::column')}}`
     """
 
     def run(
         self,
         left_values: List[str],
         right_values: List[str],
         model: Model,
-        question: Optional[str] = "Join to same topics.",
+        question: Optional[str] = None,
         **kwargs,
     ) -> dict:
-        res = model.predict(
+        if question is None:
+            question = "Join to same topics."
+        result = model.predict(
             program=JoinProgram,
             sep=CONST.DEFAULT_ANS_SEP,
             left_values=left_values,
             right_values=right_values,
             join_criteria=question,
             **kwargs,
         )
 
-        _result = res["result"].split("\n")
-        result: dict = {}
+        _result = result.split("\n")
+        mapping: dict = {}
         for item in _result:
             if CONST.DEFAULT_ANS_SEP in item:
                 k, v = item.rsplit(CONST.DEFAULT_ANS_SEP, 1)
                 if any(pred == CONST.DEFAULT_NAN_ANS for pred in {k, v}):
                     continue
-                result[k] = v
-        return result
+                mapping[k] = v
+        return mapping
```

### Comparing `blendsql-0.0.15/blendsql/ingredients/builtin/map/main.py` & `blendsql-0.0.16/blendsql/ingredients/builtin/map/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,138 @@
 import logging
-from typing import Union, Iterable, Any, Dict, Optional, List
+from typing import Union, Iterable, Any, Dict, Optional, List, Callable, Tuple
 
+import json
 import pandas as pd
 from colorama import Fore
 from tqdm import tqdm
-from textwrap import dedent
-from guidance import gen
+import outlines
 
-from blendsql.models._model import Model
-from blendsql.models import OpenaiLLM
+from blendsql.utils import logger, newline_dedent
+from blendsql.models import Model, LocalModel, RemoteModel, OpenaiLLM, OllamaLLM
 from ast import literal_eval
 from blendsql import _constants as CONST
 from blendsql.ingredients.ingredient import MapIngredient
-from blendsql._program import Program
+from blendsql._program import Program, return_ollama_response
 
 
 class MapProgram(Program):
     def __call__(
         self,
+        model: Model,
         question: str,
         values: List[str],
         sep: str,
         include_tf_disclaimer: bool = False,
+        max_tokens: int = None,
+        regex: Callable[[int], str] = None,
         output_type: str = None,
         example_outputs: str = None,
         table_title: str = None,
         colname: str = None,
         **kwargs,
-    ):
-        _model = self.model
-        with self.systemcontext:
-            _model += """Given a set of values from a database, answer the question row-by-row, in order."""
-            if include_tf_disclaimer:
-                _model += " If the question can be answered with 'true' or 'false', select `t` for 'true' or `f` for 'false'."
-            _model += dedent(
-                f"""
-            The answer should be a list separated by '{sep}', and have {len(values)} items in total.
-            When you have given all {len(values)} answers, stop responding.
-            If a given value has no appropriate answer, give '-' as a response.
+    ) -> Tuple[str, str]:
+        prompt = ""
+        prompt += """Given a set of values from a database, answer the question row-by-row, in order."""
+        if include_tf_disclaimer:
+            prompt += " If the question can be answered with 'true' or 'false', select `t` for 'true' or `f` for 'false'."
+        prompt += newline_dedent(
+            f"""
+        The answer should be a list separated by '{sep}', and have {len(values)} items in total.
+        When you have given all {len(values)} answers, stop responding.
+        If a given value has no appropriate answer, give '-' as a response.
+        """
+        )
+        prompt += newline_dedent(
             """
-            )
-        with self.usercontext:
-            if self.few_shot:
-                _model += dedent(
-                    """
-                ---
-
-                The following values come from the column 'Home Town', in a table titled '2010\u201311 North Carolina Tar Heels men's basketball team'.
-                Q: What state is this?
-                Values:
-                `Ames, IA`
-                `Carrboro, NC`
-                `Kinston, NC`
-                `Encino, CA`
-
-                Output type: string
-                Here are some example outputs: `MA;CA;-;`
-
-                A: IA;NC;NC;CA
-
-                ---
-
-                The following values come from the column 'Penalties (P+P+S+S)', in a table titled 'Biathlon World Championships 2013 \u2013 Men's pursuit'.
-                Q: Total penalty count?
-                Values:
-                `1 (0+0+0+1)`
-                `10 (5+3+2+0)`
-                `6 (2+2+2+0)`
-
-                Output type: numeric
-                Here are some example outputs: `9;-`
-
-                A: 1;10;6
-
-                ---
-
-                The following values come from the column 'term', in a table titled 'Electoral district of Lachlan'.
-                Q: how long did it last?
-                Values:
-                `1859–1864`
-                `1864–1869`
-                `1869–1880`
-
-                Output type: numeric
-
-                A: 5;5;11
-
-                ---
-
-                The following values come from the column 'Length of use', in a table titled 'Crest Whitestrips'.
-                Q: Is the time less than a week?
-                Values:
-                `14 days`
-                `10 days`
-                `daily`
-                `2 hours`
+        ---
 
-                Output type: boolean
-                A: f;f;t;t
+        The following values come from the column 'Home Town', in a table titled '2010\u201311 North Carolina Tar Heels men's basketball team'.
+        Q: What state is this?
+        Values:
+        `Ames, IA`
+        `Carrboro, NC`
+        `Kinston, NC`
+        `Encino, CA`
 
-                ---
-                """
-                )
-            if table_title:
-                _model += dedent(
-                    f"The following values come from the column '{colname}', in a table titled '{table_title}'."
+        Output type: string
+        Here are some example outputs: `MA;CA;-;`
+
+        A: IA;NC;NC;CA
+
+        ---
+
+        The following values come from the column 'Penalties (P+P+S+S)', in a table titled 'Biathlon World Championships 2013 \u2013 Men's pursuit'.
+        Q: Total penalty count?
+        Values:
+        `1 (0+0+0+1)`
+        `10 (5+3+2+0)`
+        `6 (2+2+2+0)`
+
+        Output type: numeric
+        Here are some example outputs: `9;-`
+
+        A: 1;10;6
+
+        ---
+
+        The following values come from the column 'term', in a table titled 'Electoral district of Lachlan'.
+        Q: how long did it last?
+        Values:
+        `1859–1864`
+        `1864–1869`
+        `1869–1880`
+
+        Output type: numeric
+
+        A: 5;5;11
+
+        ---
+
+        The following values come from the column 'Length of use', in a table titled 'Crest Whitestrips'.
+        Q: Is the time less than a week?
+        Values:
+        `14 days`
+        `10 days`
+        `daily`
+        `2 hours`
+
+        Output type: boolean
+        A: f;f;t;t
+
+        ---
+        """
+        )
+        if table_title:
+            prompt += newline_dedent(
+                f"The following values come from the column '{colname}', in a table titled '{table_title}'."
+            )
+        prompt += newline_dedent(f"""Q: {question}\nValues:\n""")
+        for value in values:
+            prompt += f"`{value}`\n"
+        if output_type:
+            prompt += f"\nOutput type: {output_type}"
+        if example_outputs:
+            prompt += f"\nHere are some example outputs: {example_outputs}\n"
+        prompt += "\nA:"
+        if isinstance(model, LocalModel) and regex is not None:
+            generator = outlines.generate.regex(
+                model.logits_generator, regex(len(values))
+            )
+        else:
+            if isinstance(model, OllamaLLM):
+                # Handle call to ollama
+                return return_ollama_response(
+                    logits_generator=model.logits_generator,
+                    prompt=prompt,
+                    max_tokens=max_tokens,
+                    temperature=0.0,
                 )
-            _model += dedent(f"""Q: {question}\nValues:\n""")
-            for value in values:
-                _model += f"`{value}`\n"
-            if output_type:
-                _model += f"\nOutput type: {output_type}"
-            if example_outputs:
-                _model += f"\nHere are some example outputs: {example_outputs}\n"
-            _model += "\nA:"
-        with self.assistantcontext:
-            _model += gen(name="result", **self.gen_kwargs)
-        return _model
+            generator = outlines.generate.text(model.logits_generator)
+        return (generator(prompt, max_tokens=max_tokens), prompt)
 
 
 class LLMMap(MapIngredient):
     DESCRIPTION = """
     If question-relevant column(s) contents are not suitable for SQL comparisons or calculations, map it to a new column using the scalar function:
         `{{LLMMap('question', 'table::column')}}`
     """
@@ -149,67 +161,66 @@
             table_to_title: Mapping from tablename to a title providing some more context.
 
         Returns:
             Iterable[Any] containing the output of the Model for each value.
         """
         # Unpack default kwargs
         tablename, colname = self.unpack_default_kwargs(**kwargs)
-        # OpenAI endpoints can't use patterns
-        pattern = None if isinstance(model, OpenaiLLM) else pattern
+        # Remote endpoints can't use patterns
+        pattern = None if isinstance(model, RemoteModel) else pattern
         if value_limit is not None:
             values = values[:value_limit]
         values = [value if not pd.isna(value) else "-" for value in values]
         table_title = None
         if table_to_title is not None:
             if tablename not in table_to_title:
-                logging.debug(f"Tablename {tablename} not in given table_to_title!")
+                logger.debug(f"Tablename {tablename} not in given table_to_title!")
             else:
                 table_title = table_to_title[tablename]
         split_results = []
         # Only use tqdm if we're in debug mode
         context_manager = (
             tqdm(
                 range(0, len(values), CONST.VALUE_BATCH_SIZE),
                 total=len(values) // CONST.VALUE_BATCH_SIZE,
                 desc=f"Making calls to Model with batch_size {CONST.VALUE_BATCH_SIZE}",
                 bar_format="{l_bar}%s{bar}%s{r_bar}" % (Fore.CYAN, Fore.RESET),
             )
-            if logging.DEBUG >= logging.root.level
+            if logger.level >= logging.DEBUG
             else range(0, len(values), CONST.VALUE_BATCH_SIZE)
         )
 
         for i in context_manager:
             answer_length = len(values[i : i + CONST.VALUE_BATCH_SIZE])
             max_tokens = answer_length * 15
             include_tf_disclaimer = False
 
-            if pattern is not None:
-                if pattern.startswith("(t|f"):
-                    include_tf_disclaimer = True
-                    # max_tokens = answer_length * 2
+            if output_type == "boolean":
+                include_tf_disclaimer = True
             elif isinstance(model, OpenaiLLM):
                 include_tf_disclaimer = True
 
-            res = model.predict(
+            result = model.predict(
                 program=MapProgram,
                 question=question,
                 sep=CONST.DEFAULT_ANS_SEP,
                 values=values[i : i + CONST.VALUE_BATCH_SIZE],
                 example_outputs=example_outputs,
                 output_type=output_type,
                 include_tf_disclaimer=include_tf_disclaimer,
                 table_title=table_title,
-                gen_kwargs={"max_tokens": max_tokens, "regex": pattern},
+                regex=pattern,
+                max_tokens=max_tokens,
                 **kwargs,
             )
             _r = [
                 i.strip()
-                for i in res["result"]
-                .strip(CONST.DEFAULT_ANS_SEP)
-                .split(CONST.DEFAULT_ANS_SEP)
+                for i in result.strip(CONST.DEFAULT_ANS_SEP).split(
+                    CONST.DEFAULT_ANS_SEP
+                )
             ]
             # Try to map to booleans and `None`
             _r = [
                 {
                     "t": True,
                     "f": False,
                     "true": True,
@@ -220,28 +231,30 @@
                     "no": False,
                     CONST.DEFAULT_NAN_ANS: None,
                 }.get(i.lower(), i)
                 for i in _r
             ]
             expected_len = len(values[i : i + CONST.VALUE_BATCH_SIZE])
             if len(_r) != expected_len:
-                logging.debug(
+                logger.debug(
                     Fore.YELLOW
                     + f"Mismatch between length of values and answers!\nvalues:{expected_len}, answers:{len(_r)}"
                     + Fore.RESET
                 )
-                logging.debug(_r)
+                logger.debug(_r)
             # Cut off, in case we over-predicted
             _r = _r[:expected_len]
             # Add, in case we under-predicted
             while len(_r) < expected_len:
                 _r.append(None)
             split_results.extend(_r)
         for idx, i in enumerate(split_results):
             try:
                 split_results[idx] = literal_eval(i)
             except (ValueError, SyntaxError):
                 continue
-        logging.debug(
-            Fore.YELLOW + f"Finished with values {split_results[:10]}" + Fore.RESET
+        logger.debug(
+            Fore.YELLOW
+            + f"Finished with values:\n{json.dumps(dict(zip(values[:10], split_results[:10])), indent=4)}"
+            + Fore.RESET
         )
         return split_results
```

### Comparing `blendsql-0.0.15/blendsql/ingredients/builtin/qa/main.py` & `blendsql-0.0.16/blendsql/ingredients/builtin/qa/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,87 @@
 import copy
-from typing import Dict, Union, Optional, Set, List
-from guidance import gen, select
+from typing import Dict, Union, Optional, Set, List, Tuple
 import pandas as pd
+import outlines
 import re
-from blendsql.models._model import Model
-from blendsql._program import Program
+
+from blendsql.models import Model, OllamaLLM
+from blendsql._exceptions import InvalidBlendSQL
+from blendsql._program import Program, return_ollama_response
 from blendsql.ingredients.ingredient import QAIngredient
 from blendsql.db.utils import single_quote_escape
 
 
 class QAProgram(Program):
     def __call__(
         self,
+        model: Model,
         question: str,
         context: Optional[pd.DataFrame] = None,
         options: Optional[List[str]] = None,
         long_answer: Optional[bool] = False,
         table_title: Optional[str] = None,
+        max_tokens: int = None,
         **kwargs,
-    ):
-        _model = self.model
+    ) -> Tuple[str, str]:
+        prompt = ""
         serialized_db = context.to_string() if context is not None else ""
-        with self.systemcontext:
-            _model += "Answer the question for the table. "
-            if long_answer:
-                _model += "Make the answer as concrete as possible, providing more context and reasoning using the entire table.\n"
-            else:
-                _model += "Keep the answers as short as possible, without leading context. For example, do not say 'The answer is 2', simply say '2'.\n"
-            if options is not None:
-                _model += "Your answer should be a selection from one of the following options:\n"
-                int_prefix_options = []
-                for _idx, option in enumerate(options):
-                    int_prefix_option = f"{option}"
-                    int_prefix_options.append(int_prefix_option)
-                    _model += f"{int_prefix_option}\n"
-                # Add in title case, since this helps with selection
-                modified_option_to_original = {}
-                _options = copy.deepcopy(options)
-                # Below we check to see if our options have a unique first word
-                # sometimes, the model will generate 'Frank' instead of 'Frank Smith'
-                # We still want to align that, in this case
-                add_first_word = False
-                if len(set([i.split(" ")[0] for i in options])) == len(options):
-                    add_first_word = True
-                for option in options:
-                    option = str(option)
-                    for modified_option in [option.title(), option.upper()]:
-                        _options.add(modified_option)
-                        modified_option_to_original[modified_option] = option
-                    if add_first_word:
-                        modified_option_to_original[option.split(" ")[0]] = option
-                options = _options
-        with self.usercontext:
-            _model += f"\n\nQuestion: {question}"
-            if table_title is not None:
-                _model += f"\n\nContext: \n Table Description: {table_title} \n {serialized_db}"
-            else:
-                _model += f"\n\nContext: \n {serialized_db}"
-        with self.assistantcontext:
-            if options is not None:
-                _model += select(options=[str(i) for i in options], name="result")
-            else:
-                _model += gen(name="result", **self.gen_kwargs)
-        if options:
-            _model._variables["result"] = modified_option_to_original.get(
-                _model._variables["result"], _model._variables["result"]
+        prompt += "Answer the question for the table. "
+        if long_answer:
+            prompt += "Make the answer as concrete as possible, providing more context and reasoning using the entire table.\n"
+        else:
+            prompt += "Keep the answers as short as possible, without leading context. For example, do not say 'The answer is 2', simply say '2'.\n"
+        if options is not None:
+            # Add in title case, since this helps with selection
+            modified_option_to_original = {}
+            _options = copy.deepcopy(options)
+            # Below we check to see if our options have a unique first word
+            # sometimes, the model will generate 'Frank' instead of 'Frank Smith'
+            # We still want to align that, in this case
+            add_first_word = False
+            if len(set([i.split(" ")[0] for i in options])) == len(options):
+                add_first_word = True
+            for option in options:
+                option = str(option)
+                for modified_option in [option.title(), option.upper()]:
+                    _options.add(modified_option)
+                    modified_option_to_original[modified_option] = option
+                if add_first_word:
+                    modified_option_to_original[option.split(" ")[0]] = option
+            options = _options
+        prompt += f"\n\nQuestion: {question}"
+        if table_title is not None:
+            prompt += (
+                f"\n\nContext: \n Table Description: {table_title} \n {serialized_db}"
             )
-        return _model
+        else:
+            prompt += f"\n\nContext: \n {serialized_db}"
+        if options is not None:
+            if isinstance(model, OllamaLLM):
+                raise InvalidBlendSQL(
+                    "Can't use `options` argument in LLMQA with an Ollama model!"
+                )
+            generator = outlines.generate.choice(
+                model.logits_generator, [re.escape(str(i)) for i in options]
+            )
+            result = generator(prompt, max_tokens=max_tokens)
+            # Map from modified options to original, as they appear in DB
+            result = modified_option_to_original.get(result, result)
+        else:
+            if isinstance(model, OllamaLLM):
+                # Handle call to ollama
+                return return_ollama_response(
+                    logits_generator=model.logits_generator,
+                    prompt=prompt,
+                    max_tokens=max_tokens,
+                    temperature=0.0,
+                )
+            generator = outlines.generate.text(model.logits_generator)
+            result = generator(prompt, max_tokens=max_tokens)
+        return (result, prompt)
 
 
 class LLMQA(QAIngredient):
     DESCRIPTION = """
     If mapping to a new column still cannot answer the question with valid SQL, turn to an end-to-end solution using the aggregate function:
         `{{LLMQA('question', (blendsql))}}`
         Optionally, this function can take an `options` argument to restrict its output to an existing SQL column.
@@ -87,19 +98,17 @@
         table_to_title: Optional[Dict[str, str]] = None,
         long_answer: bool = False,
         **kwargs,
     ) -> Union[str, int, float]:
         if context is not None:
             if value_limit is not None:
                 context = context.iloc[:value_limit]
-        res = model.predict(
+        result = model.predict(
             program=QAProgram,
             options=options,
             question=question,
             context=context,
             long_answer=long_answer,
             table_title=None,
             **kwargs,
         )
-        return "'{}'".format(
-            single_quote_escape(re.sub(r"^\d+\):", "", res["result"]).strip().lower())
-        )
+        return "'{}'".format(single_quote_escape(result.strip().lower()))
```

### Comparing `blendsql-0.0.15/blendsql/ingredients/builtin/validate/main.py` & `blendsql-0.0.16/blendsql/ingredients/builtin/validate/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from typing import Dict, Union, Optional
+from typing import Dict, Union, Optional, Tuple
 import pandas as pd
-from guidance import select
+import outlines
 
-from blendsql.models._model import Model
+from blendsql.models import Model
 from blendsql._program import Program
 from blendsql.ingredients.ingredient import QAIngredient
 
 
 class ValidateProgram(Program):
     def __call__(
         self,
+        model: Model,
         question: str,
         context: pd.DataFrame = None,
         table_title: str = None,
         **kwargs,
-    ):
+    ) -> Tuple[str, str]:
         serialized_db = context.to_string() if context is not None else ""
-        _model = self.model
-        with self.systemcontext:
-            _model += "You are a database expert in charge of validating a claim given a context. Given a claim and associated database context, you will respond 'true' if the claim is factual given the context, and 'false' if not."
-        with self.usercontext:
-            _model += f"Claim: {question}"
-            if table_title:
-                _model += f"\nTable Description: {table_title}"
-            _model += f"\n{serialized_db}\n\nAnswer:"
-        with self.assistantcontext:
-            _model += select(options=["true", "false"], name="result")
-        return _model
+        prompt = ""
+        prompt += "You are a database expert in charge of validating a claim given a context. Given a claim and associated database context, you will respond 'true' if the claim is factual given the context, and 'false' if not."
+        prompt += f"Claim: {question}"
+        if table_title:
+            prompt += f"\nTable Description: {table_title}"
+        prompt += f"\n{serialized_db}\n\nAnswer:"
+        generator = outlines.generate.choice(model.logits_generator, ["true", "false"])
+        return (generator(prompt), prompt)
 
 
 class LLMValidate(QAIngredient):
     def run(
         self,
         question: str,
         model: Model,
@@ -39,15 +37,15 @@
         table_to_title: Optional[Dict[str, str]] = None,
         long_answer: bool = False,
         **kwargs,
     ) -> Union[str, int, float]:
         if context is not None:
             if value_limit is not None:
                 context = context.iloc[:value_limit]
-        res = model.predict(
+        response = model.predict(
             program=ValidateProgram,
             question=question,
             context=context,
             table_title=None,
             **kwargs,
         )
-        return int(res["result"] == "true")
+        return int(response == "true")
```

### Comparing `blendsql-0.0.15/blendsql/ingredients/ingredient.py` & `blendsql-0.0.16/blendsql/ingredients/ingredient.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,42 +12,28 @@
     Set,
     Collection,
     Optional,
 )
 import uuid
 from typeguard import check_type
 
+from .._exceptions import IngredientException
 from .. import utils
 from .._constants import IngredientKwarg, IngredientType
 from ..db import Database
-from ..db.utils import double_quote_escape
-
-
-class IngredientException(ValueError):
-    pass
+from ..db.utils import select_all_from_table_query
 
 
 def unpack_default_kwargs(**kwargs):
     return (
         kwargs.get("tablename"),
         kwargs.get("colname"),
     )
 
 
-def align_to_real_columns(db: Database, colname: str, tablename: str) -> str:
-    table_columns = db.execute_query(f'SELECT * FROM "{tablename}" LIMIT 1').columns
-    if colname not in table_columns:
-        # Try to align with column, according to some normalization rules
-        cleaned_to_original = {
-            col.replace("\\n", " ").replace("\xa0", " "): col for col in table_columns
-        }
-        colname = cleaned_to_original[colname]
-    return colname
-
-
 @attrs
 class Ingredient(ABC):
     name: str = attrib()
     ingredient_type: str = attrib(init=False)
     allowed_output_types: Tuple[Type] = attrib(init=False)
     # Below gets passed via `Kitchen.extend()`
     db: Database = attrib(init=False)
@@ -114,44 +100,38 @@
         new_arg_column = question
         while (
             new_arg_column in set(self.db.iter_columns(tablename))
             or new_arg_column in prev_subquery_map_columns
         ):
             new_arg_column = "_" + new_arg_column
 
-        original_table = self.db.execute_query(f'SELECT * FROM "{tablename}"')
+        original_table = self.db.execute_to_df(select_all_from_table_query(tablename))
 
         # Get a list of values to map
         # First, check if we've already dumped some `MapIngredient` output to the main session table
         if temp_session_table_exists:
-            temp_session_table = self.db.execute_query(
-                f'SELECT * FROM "{double_quote_escape(temp_session_tablename)}"'
-            )
-            colname = align_to_real_columns(
-                db=self.db, colname=colname, tablename=temp_session_tablename
+            temp_session_table = self.db.execute_to_df(
+                select_all_from_table_query(temp_session_tablename)
             )
             # We don't need to run this function on everything,
             #   if a previous subquery already got to certain values
             if new_arg_column in temp_session_table.columns:
-                values = self.db.execute_query(
+                values = self.db.execute_to_list(
                     f'SELECT DISTINCT "{colname}" FROM "{temp_session_tablename}" WHERE "{new_arg_column}" IS NULL',
-                )[colname].tolist()
+                )
             # Base case: this is the first time we've used this particular ingredient
             # BUT, temp_session_tablename still exists
             else:
-                values = self.db.execute_query(
-                    f'SELECT DISTINCT "{colname}" FROM "{temp_session_tablename}"'
-                )[colname].tolist()
+                values = self.db.execute_to_list(
+                    f'SELECT DISTINCT "{colname}" FROM "{temp_session_tablename}"',
+                )
         else:
-            colname = align_to_real_columns(
-                db=self.db, colname=colname, tablename=value_source_tablename
+            values = self.db.execute_to_list(
+                f'SELECT DISTINCT "{colname}" FROM "{value_source_tablename}"',
             )
-            values = self.db.execute_query(
-                f'SELECT DISTINCT "{colname}" FROM "{value_source_tablename}"'
-            )[colname].tolist()
 
         # No need to run ingredient if we have no values to map onto
         if len(values) == 0:
             original_table[new_arg_column] = None
             return (new_arg_column, tablename, colname, original_table)
 
         kwargs[IngredientKwarg.VALUES] = values
@@ -207,52 +187,62 @@
         **kwargs,
     ) -> tuple:
         # Unpack kwargs
         aliases_to_tablenames: Dict[str, str] = kwargs.get("aliases_to_tablenames")
         get_temp_subquery_table: Callable = kwargs.get("get_temp_subquery_table")
         get_temp_session_table: Callable = kwargs.get("get_temp_session_table")
 
+        # Depending on the size of the underlying data, it may be optimal to swap
+        #   the order of 'left_on' and 'right_on' columns during processing
+        swapped = False
         values = []
         original_lr_identifiers = []
         modified_lr_identifiers = []
-        left_values, right_values = [], []
         mapping = {}
         for on_arg in [left_on, right_on]:
             tablename, colname = utils.get_tablename_colname(on_arg)
             tablename = aliases_to_tablenames.get(tablename, tablename)
             original_lr_identifiers.append((tablename, colname))
             tablename, _ = self.maybe_get_temp_table(
                 temp_table_func=get_temp_subquery_table,
                 tablename=tablename,
             )
             values.append(
-                set(
-                    [
-                        str(i)
-                        for i in self.db.execute_query(
-                            f'SELECT DISTINCT "{colname}" FROM "{tablename}"'
-                        )[colname].tolist()
-                    ]
+                self.db.execute_to_list(
+                    f'SELECT DISTINCT "{colname}" FROM "{tablename}"', to_type=str
                 )
             )
             modified_lr_identifiers.append((tablename, colname))
 
         if question is None:
             # First, check which values we actually need to call Model on
             # We don't want to join when there's already an intuitive alignment
+            # First, make sure outer loop is shorter of the two lists
+            outer, inner = sorted(values, key=len)
+            _outer = []
+            inner = set(inner)
             mapping = {}
-            left_values, right_values = values
-            for l in left_values:
-                if l in right_values:
+            for l in outer:
+                if l in inner:
                     # Define this mapping, and remove from Model inference call
                     mapping[l] = l
+                    inner.remove(l)
+                else:
+                    _outer.append(l)
+                if len(inner) == 0:
+                    break
+            to_compare = [inner, _outer]
+        else:
+            to_compare = values
 
-            processed_values = set(list(mapping.keys()))
-            left_values = left_values.difference(processed_values)
-            right_values = right_values.difference(processed_values)
+        # Finally, order by new (remaining) length and check if we swapped places from original
+        sorted_values = sorted(to_compare, key=len)
+        if sorted_values != values:
+            swapped = True
+        left_values, right_values = sorted_values
 
         kwargs["left_values"] = left_values
         kwargs["right_values"] = right_values
 
         (left_tablename, left_colname), (
             right_tablename,
             right_colname,
@@ -270,24 +260,29 @@
 
             kwargs[IngredientKwarg.QUESTION] = question
             _mapping: Dict[str, str] = self._run(*args, **kwargs)
             mapping = mapping | _mapping
 
         # Using mapped left/right values, create intermediary mapping table
         temp_join_tablename = get_temp_session_table(str(uuid.uuid4())[:4])
+        # Below, we check to see if 'swapped' is True
+        # If so, we need to inverse what is 'left', and what is 'right'
         joined_values_df = pd.DataFrame(
-            data={"left": mapping.keys(), "right": mapping.values()}
+            data={
+                "left" if not swapped else "right": mapping.keys(),
+                "right" if not swapped else "left": mapping.values(),
+            }
         )
         self.db.to_temp_table(df=joined_values_df, tablename=temp_join_tablename)
         return (
             left_tablename,
             right_tablename,
             f"""JOIN "{temp_join_tablename}" ON "{right_tablename}"."{right_colname}" = "{temp_join_tablename}".right
-                           JOIN "{left_tablename}" ON "{left_tablename}"."{left_colname}" = "{temp_join_tablename}".left
-                           """,
+               JOIN "{left_tablename}" ON "{left_tablename}"."{left_colname}" = "{temp_join_tablename}".left
+               """,
             temp_join_tablename,
         )
 
     @abstractmethod
     def run(self, *args, **kwargs) -> dict:
         ...
 
@@ -309,41 +304,44 @@
         # Unpack kwargs
         aliases_to_tablenames: Dict[str, str] = kwargs.get("aliases_to_tablenames")
 
         subtable = context
         if context is not None:
             if isinstance(context, str):
                 tablename, colname = utils.get_tablename_colname(context)
-                subtable = self.db.execute_query(
+                subtable = self.db.execute_to_df(
                     f'SELECT "{colname}" FROM "{tablename}"'
                 )
             elif not isinstance(context, pd.DataFrame):
                 raise ValueError(
                     f"Unknown type for `identifier` arg in QAIngredient: {type(context)}"
                 )
             if subtable.empty:
                 raise IngredientException("Empty subtable passed to QAIngredient!")
         unpacked_options = options
         if options is not None:
             if not isinstance(options, list):
                 try:
                     tablename, colname = utils.get_tablename_colname(options)
                     tablename = aliases_to_tablenames.get(tablename, tablename)
-                    unpacked_options = self.db.execute_query(
+                    unpacked_options = self.db.execute_to_list(
                         f'SELECT DISTINCT "{colname}" FROM "{tablename}"'
-                    )[colname].tolist()
+                    )
                 except ValueError:
                     unpacked_options = options.split(";")
             unpacked_options = set(unpacked_options)
         self.num_values_passed += len(subtable) if subtable is not None else 0
         kwargs[IngredientKwarg.OPTIONS] = unpacked_options
         kwargs[IngredientKwarg.CONTEXT] = subtable
         kwargs[IngredientKwarg.QUESTION] = question
         response: Union[str, int, float] = self._run(*args, **kwargs)
         return response
+        # response = response.replace("\x00", "").replace(":", "\:")
+        # return response
+        # return f"'{response}'"
 
     @abstractmethod
     def run(self, *args, **kwargs) -> Union[str, int, float]:
         ...
 
 
 @attrs
```

### Comparing `blendsql-0.0.15/blendsql/models/_model.py` & `blendsql-0.0.16/blendsql/models/_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import functools
-from typing import Any, List
-import guidance
+from typing import Any, List, Optional, Type
 import pandas as pd
 from attr import attrib, attrs
 from pathlib import Path
 from dotenv import load_dotenv
 from colorama import Fore
 import time
 import threading
 from diskcache import Cache
 import platformdirs
 import hashlib
 from abc import abstractmethod
+from outlines.models import LogitsGenerator
 
+from ..utils import logger
 from .._program import Program, program_to_str
 from .._constants import IngredientKwarg
 from ..db.utils import truncate_df_content
 
 CONTEXT_TRUNCATION_LIMIT = 100
 
 
@@ -39,34 +40,37 @@
 @attrs
 class Model:
     """Parent class for all BlendSQL Models."""
 
     model_name_or_path: str = attrib()
     tokenizer: Any = attrib(default=None)
     requires_config: bool = attrib(default=False)
-    refresh_interval_min: int = attrib(default=None)
+    refresh_interval_min: Optional[int] = attrib(default=None)
+    load_model_kwargs: Optional[dict] = attrib(default={})
     env: str = attrib(default=".")
     caching: bool = attrib(default=True)
 
-    model: guidance.models.Model = attrib(init=False)
+    logits_generator: LogitsGenerator = attrib(init=False)
     prompts: list = attrib(init=False)
+    prompt_tokens: int = attrib(init=False)
+    completion_tokens: int = attrib(init=False)
+    num_calls: int = attrib(init=False)
     cache: Cache = attrib(init=False)
     run_setup_on_load: bool = attrib(default=True)
 
-    gen_kwargs: dict = {}
-    num_llm_calls: int = 0
-    num_prompt_tokens: int = 0
-
     def __attrs_post_init__(self):
         if self.caching:
             self.cache = Cache(
                 Path(platformdirs.user_cache_dir("blendsql"))
                 / f"{self.model_name_or_path}.diskcache"
             )
         self.prompts: List[str] = []
+        self.prompt_tokens = 0
+        self.completion_tokens = 0
+        self.num_calls = 0
         if self.requires_config:
             if self.env is None:
                 self.env = "."
             _env = Path(self.env)
             env_filepath = _env / ".env" if _env.is_dir() else _env
             if env_filepath.is_file():
                 load_dotenv(str(env_filepath))
@@ -81,49 +85,52 @@
             timer.start()
         if self.tokenizer is not None:
             assert hasattr(self.tokenizer, "encode") and callable(
                 self.tokenizer.encode
             ), f"`tokenizer` passed to {self.__class__} should have `encode` method!"
         if self.run_setup_on_load:
             self._setup()
-        self.model = self._load_model()
+        self.logits_generator: LogitsGenerator = self._load_model(
+            **self.load_model_kwargs
+        )
 
-    def predict(self, program: Program, **kwargs) -> dict:
+    def predict(self, program: Type[Program], **kwargs) -> dict:
         """Takes a `Program` and some kwargs, and evaluates it with context of
         current Model.
 
         Args:
-            program: guidance program used to generate Model output
+            program: The `Program` object used to generate Model output
             **kwargs: any additional kwargs will get passed to the program
 
         Returns:
             dict containing all Model variable names and their values.
 
         Examples:
-            >>> llm.predict(program, **kwargs)
-            {"result": '"This is Model generated output"'}
+            >>> model.predict(program, **kwargs)
+            "This is model generated output"
         """
         if self.caching:
             # First, check our cache
             key = self._create_key(program, **kwargs)
             if key in self.cache:
+                logger.debug(Fore.MAGENTA + "Using cache..." + Fore.RESET)
                 self.prompts.insert(
                     -1, self.format_prompt(self.cache.get(key), **kwargs)
                 )
                 return self.cache.get(key)
         # Modify fields used for tracking Model usage
-        self.num_llm_calls += 1
-        model = program(model=self.model, **kwargs)
+        response, prompt = program(model=self, **kwargs)
+        self.prompts.insert(-1, self.format_prompt(response, **kwargs))
+        self.num_calls += 1
         if self.tokenizer is not None:
-            prompt = model._current_prompt()
-            self.num_prompt_tokens += len(self.tokenizer.encode(prompt))
-        self.prompts.insert(-1, self.format_prompt(model._variables, **kwargs))
+            self.prompt_tokens += len(self.tokenizer.encode(prompt))
+            self.completion_tokens += len(self.tokenizer.encode(response))
         if self.caching:
-            self.cache[key] = model._variables
-        return model._variables
+            self.cache[key] = response
+        return response
 
     def _create_key(self, program: Program, **kwargs) -> str:
         """Generates a hash to use in diskcache Cache.
         This way, we don't need to send our prompts to the same Model
         if our context of Model + program + kwargs is the same.
 
         Returns:
@@ -145,32 +152,43 @@
             program_to_str(program),
             options_str,
         ).encode()
         hasher.update(combined)
         return hasher.hexdigest()
 
     @staticmethod
-    def format_prompt(res, **kwargs) -> dict:
-        d = {"answer": res}
+    def format_prompt(response: str, **kwargs) -> dict:
+        d = {"answer": response}
         if IngredientKwarg.QUESTION in kwargs:
             d[IngredientKwarg.QUESTION] = kwargs.get(IngredientKwarg.QUESTION)
         if IngredientKwarg.CONTEXT in kwargs:
             context = kwargs.get(IngredientKwarg.CONTEXT)
             if isinstance(context, pd.DataFrame):
                 context = truncate_df_content(context, CONTEXT_TRUNCATION_LIMIT)
                 d[IngredientKwarg.CONTEXT] = context.to_dict(orient="records")
         if IngredientKwarg.VALUES in kwargs:
             d[IngredientKwarg.VALUES] = kwargs.get(IngredientKwarg.VALUES)
         return d
 
     @abstractmethod
-    def _setup(self, **kwargs) -> None:
+    def _setup(self, *args, **kwargs) -> None:
         """Any additional setup required to get this Model up and functioning
         should go here. For example, in the AzureOpenaiLLM, we have some logic
         to refresh our client secrets every 30 min.
         """
         ...
 
     @abstractmethod
-    def _load_model(self) -> Any:
-        """Logic for instantiating the guidance model class goes here."""
+    def _load_model(self, *args, **kwargs) -> Any:
+        """Logic for instantiating the model class goes here.
+        Will most likely be an outlines.LogitsGenerator object,
+        but in some cases (like OllamaLLM) we make an exception.
+        """
         ...
+
+
+class LocalModel(Model):
+    pass
+
+
+class RemoteModel(Model):
+    pass
```

### Comparing `blendsql-0.0.15/blendsql/models/local/_transformers.py` & `blendsql-0.0.16/blendsql/models/local/_transformers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,43 @@
-import logging
 import importlib.util
-from guidance.models import Transformers, Model
+from outlines.models import transformers, LogitsGenerator
 
-from .._model import Model
-
-logging.getLogger("guidance").setLevel(logging.CRITICAL)
+from .._model import LocalModel
 
 _has_transformers = importlib.util.find_spec("transformers") is not None
 
 
-class TransformersLLM(Model):
+class TransformersLLM(LocalModel):
     """Class for Transformers local Model.
 
     Args:
         model_name_or_path: Name of the model on HuggingFace, or the path to a local model
+        caching: Bool determining whether we access the model's cache
+
+    Examples:
+        ```python
+        from blendsql.models import TransformersLLM
+        model = TransformersLLM("Qwen/Qwen1.5-0.5B")
+        ```
     """
 
-    def __init__(self, model_name_or_path: str, **kwargs):
+    def __init__(self, model_name_or_path: str, caching: bool = True, **kwargs):
         if not _has_transformers:
             raise ImportError(
                 "Please install transformers with `pip install transformers`!"
             ) from None
         import transformers
 
         super().__init__(
             model_name_or_path=model_name_or_path,
             requires_config=False,
             tokenizer=transformers.AutoTokenizer.from_pretrained(model_name_or_path),
+            caching=caching,
             **kwargs
         )
 
-    def _load_model(self) -> Model:
-        return Transformers(self.model_name_or_path, echo=False)
+    def _load_model(self) -> LogitsGenerator:
+        # https://huggingface.co/blog/how-to-generate
+        return transformers(
+            self.model_name_or_path,
+            model_kwargs={"do_sample": True, "temperature": 0.0, "top_p": 1.0},
+        )
```

### Comparing `blendsql-0.0.15/blendsql/utils.py` & `blendsql-0.0.16/blendsql/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from typing import Tuple
 import re
 from tabulate import tabulate
 from functools import partial
-
+import logging
 
 from ._constants import HF_REPO_ID
 
+logging.basicConfig()
+logger = logging.getLogger("blendsql")
 tabulate = partial(tabulate, headers="keys", showindex="never", tablefmt="orgtbl")
+newline_dedent = lambda x: "\n".join([m.lstrip() for m in x.split("\n")])
 
 
 def fetch_from_hub(filename: str):
     try:
         from huggingface_hub import hf_hub_download
     except ImportError:
         raise ImportError(
             f"You need huggingface_hub to run this!\n`pip install huggingface_hub`"
         ) from None
     return hf_hub_download(
-        repo_id=HF_REPO_ID, filename=filename, repo_type="dataset", force_download=True
+        repo_id=HF_REPO_ID, filename=filename, repo_type="dataset", force_download=False
     )
 
 
 def get_tablename_colname(s: str) -> Tuple[str, str]:
     """Takes as input a string in the format `{tablename}::{colname}`
     Returns individual parts, but raises error if `s` is in the wrong format.
     """
```

### Comparing `blendsql-0.0.15/blendsql.egg-info/SOURCES.txt` & `blendsql-0.0.16/blendsql.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 blendsql/__init__.py
 blendsql/_constants.py
 blendsql/_dialect.py
+blendsql/_exceptions.py
 blendsql/_program.py
 blendsql/_smoothie.py
 blendsql/_sqlglot.py
 blendsql/blend.py
 blendsql/blend_cli.py
-blendsql/nl_to_blendsql.py
 blendsql/utils.py
 blendsql.egg-info/PKG-INFO
 blendsql.egg-info/SOURCES.txt
 blendsql.egg-info/dependency_links.txt
 blendsql.egg-info/entry_points.txt
 blendsql.egg-info/requires.txt
 blendsql.egg-info/top_level.txt
 blendsql/db/__init__.py
 blendsql/db/_database.py
 blendsql/db/_postgres.py
 blendsql/db/_sqlite.py
+blendsql/db/bridge_content_encoder.py
 blendsql/db/utils.py
 blendsql/grammars/__init__.py
 blendsql/grammars/_cfg_grammar.lark
 blendsql/grammars/_peg_grammar.py
+blendsql/grammars/utils.py
 blendsql/grammars/minEarley/__init__.py
 blendsql/grammars/minEarley/earley.py
 blendsql/grammars/minEarley/earley_analyzer.py
 blendsql/grammars/minEarley/earley_exceptions.py
 blendsql/grammars/minEarley/earley_forest.py
 blendsql/grammars/minEarley/parser.py
 blendsql/grammars/minEarley/tree.py
@@ -47,15 +49,19 @@
 blendsql/ingredients/builtin/validate/main.py
 blendsql/models/__init__.py
 blendsql/models/_model.py
 blendsql/models/local/__init__.py
 blendsql/models/local/_llama_cpp.py
 blendsql/models/local/_transformers.py
 blendsql/models/remote/__init__.py
+blendsql/models/remote/_ollama.py
 blendsql/models/remote/_openai.py
+blendsql/nl_to_blendsql/__init__.py
+blendsql/nl_to_blendsql/args.py
+blendsql/nl_to_blendsql/nl_to_blendsql.py
 blendsql/prompts/__init__.py
 blendsql/prompts/_prompts.py
 research/metrics/__init__.py
 research/prompts/__init__.py
 research/prompts/end_to_end_program.py
 research/prompts/parser_program.py
 research/utils/__init__.py
@@ -77,14 +83,17 @@
 research/utils/sql/all_keywords.py
 research/utils/sql/extraction_from_sql.py
 research/utils/sql/process_sql.py
 research/utils/wikitq/__init__.py
 research/utils/wikitq/utils.py
 research/utils/wikitq/wikitq.py
 tests/__init__.py
-tests/test_end_to_end.py
 tests/test_generic_blendsql.py
-tests/test_grammar.py
-tests/test_model.py
 tests/test_multi_table_blendsql.py
 tests/test_single_table_blendsql.py
-tests/utils.py
+tests/utils.py
+tests/grammars/__init__.py
+tests/grammars/test_cfg_grammar.py
+tests/models/__init__.py
+tests/models/test_model_caching.py
+tests/models/test_ollama.py
+tests/models/test_transformers.py
```

### Comparing `blendsql-0.0.15/pyproject.toml` & `blendsql-0.0.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/prompts/end_to_end_program.py` & `blendsql-0.0.16/research/prompts/end_to_end_program.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/prompts/parser_program.py` & `blendsql-0.0.16/research/prompts/parser_program.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/args.py` & `blendsql-0.0.16/research/utils/args.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/bridge_content_encoder.py` & `blendsql-0.0.16/research/utils/bridge_content_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
     """
     key = (table_name, column_name)
     if key in cache:
         return cache[key]
     fetch_sql = 'SELECT DISTINCT `{}` FROM "{}"'.format(
         column_name, double_quote_escape(table_name)
     )
-    picklist = set(db.execute_query(fetch_sql).values.flat)
+    picklist = set(db.execute_to_df(fetch_sql).values.flat)
     picklist = list(picklist)
     cache[key] = picklist
     return picklist
 
 
 def align_title_to_content(contents: List[str], db_path: str) -> list:
     titles = []
```

### Comparing `blendsql-0.0.15/research/utils/database.py` & `blendsql-0.0.16/research/utils/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,21 @@
             )
             serialized_db.append("/*")
             if whole_table:
                 serialized_db.append("Entire table:")
             else:
                 serialized_db.append(f"{num_rows} example rows:")
             serialized_db.append(f"{get_rows_query}")
-            rows = db.execute_query(get_rows_query)
+            rows = db.execute_to_df(get_rows_query)
             if truncate_content is not None:
                 # Truncate long strings
                 rows = rows.map(
-                    lambda x: f"{str(x)[:truncate_content]}..."
-                    if isinstance(x, str) and len(str(x)) > truncate_content
-                    else x
+                    lambda x: (
+                        f"{str(x)[:truncate_content]}..."
+                        if isinstance(x, str) and len(str(x)) > truncate_content
+                        else x
+                    )
                 )
             serialized_db.append(f"{rows.to_string(index=False)}")
             serialized_db.append("*/\n")
     serialized_db = "\n".join(serialized_db).strip()
     return serialized_db
```

### Comparing `blendsql-0.0.15/research/utils/dataset.py` & `blendsql-0.0.16/research/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/dataset_loader.py` & `blendsql-0.0.16/research/utils/dataset_loader.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/fetaqa/fetaqa.py` & `blendsql-0.0.16/research/utils/fetaqa/fetaqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,19 @@
                         )
                     )
         bridge_hints = "\n".join(bridge_hints)
     db.con.close()
     return (
         db_path,
         {
-            "examples": blendsql_examples
-            if model_args.blender_model_name_or_path is not None
-            else sql_examples,
+            "examples": (
+                blendsql_examples
+                if model_args.blender_model_name_or_path is not None
+                else sql_examples
+            ),
             "question": question,
             "serialized_db": serialized_db,
             "bridge_hints": bridge_hints,
             "extra_task_description": "Provide concrete reasoning to the answer",
         },
     )
```

### Comparing `blendsql-0.0.15/research/utils/feverous/feverous.py` & `blendsql-0.0.16/research/utils/feverous/feverous.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,19 @@
             "ingredients_prompt": open(
                 "./research/prompts/feverous/ingredients.txt"
             ).read(),
             "question": statement,
             "serialized_db": serialized_db,
             "entire_serialized_db": entire_serialized_db,
             "bridge_hints": bridge_hints,
-            "extra_task_description": f"Additionally, we have the table `{DOCS_TABLE_NAME}` at our disposal, which contains Wikipedia articles providing more details about the values in our table."
-            if contains_documents
-            else "",
+            "extra_task_description": (
+                f"Additionally, we have the table `{DOCS_TABLE_NAME}` at our disposal, which contains Wikipedia articles providing more details about the values in our table."
+                if contains_documents
+                else ""
+            ),
         },
     )
 
 
 def feverous_pre_process_function(
     batch: dict, data_training_args: DataTrainingArguments, model_args: ModelArguments
 ) -> dict:
```

### Comparing `blendsql-0.0.15/research/utils/hybridqa/hybridqa.py` & `blendsql-0.0.16/research/utils/hybridqa/hybridqa.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/normalizer.py` & `blendsql-0.0.16/research/utils/normalizer.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/ottqa/ottqa.py` & `blendsql-0.0.16/research/utils/ottqa/ottqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     question: str,
     question_id: str,
     db_path: str,
     data_training_args: DataTrainingArguments,
     model_args: ModelArguments,
 ) -> Tuple[str, dict]:
     if "docs_tablesize" not in cache:
-        cache["docs_tablesize"] = db.execute_query(
+        cache["docs_tablesize"] = db.execute_to_df(
             f"SELECT COUNT(*) FROM {DOCS_TABLE_NAME}"
         ).values[0][0]
     cache["docs_tablesize"]
     chosen_tables = ottqa_question_id_to_retriever_results[question_id]
     chosen_tables = [
         table_id_to_tablename["_".join(item["title"].split("_")[:-1])]
         for item in chosen_tables
```

### Comparing `blendsql-0.0.15/research/utils/sql/extraction_from_sql.py` & `blendsql-0.0.16/research/utils/sql/extraction_from_sql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/sql/process_sql.py` & `blendsql-0.0.16/research/utils/sql/process_sql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/wikitq/utils.py` & `blendsql-0.0.16/research/utils/wikitq/utils.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.15/research/utils/wikitq/wikitq.py` & `blendsql-0.0.16/research/utils/wikitq/wikitq.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,19 @@
                         )
                     )
         bridge_hints = "\n".join(bridge_hints)
     db.con.close()
     return (
         db_path,
         {
-            "examples": blendsql_examples
-            if model_args.blender_model_name_or_path is not None
-            else sql_examples,
+            "examples": (
+                blendsql_examples
+                if model_args.blender_model_name_or_path is not None
+                else sql_examples
+            ),
             "question": question,
             "serialized_db": serialized_db,
             "bridge_hints": bridge_hints,
             "extra_task_description": None,
         },
     )
```

### Comparing `blendsql-0.0.15/setup.py` & `blendsql-0.0.16/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,40 +29,47 @@
     author="Parker Glenn",
     author_email="parkervg5@gmail.com",
     description="Query language to blend SQL logic and LLM reasoning across multi-modal data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     packages=find_packages(exclude=["examples", "research", "img"]),
+    include_package_data=True,
     data_files=["blendsql/grammars/_cfg_grammar.lark"],
     install_requires=[
-        "guidance>=0.1.0",
+        "outlines",
         "pyparsing==3.1.1",
-        "pandas==1.5.3",
+        "pandas>=2.0.0",
         "bottleneck>=1.3.6",
         "python-dotenv==1.0.1",
         "sqlglot==18.13.0",
         "sqlalchemy>=2.0.0",
+        "huggingface_hub",
+        "lark",
+        "exrex",
         "platformdirs",
         "attrs",
         "tqdm",
         "colorama",
         "tabulate",
         "typeguard",
+        "rapidfuzz",
     ],
     extras_require={
-        "nl_to_blendsql": ["exrex", "lark"],
+        "llama-cpp": ["llama-cpp-python"],
+        "ollama": ["ollama"],
+        "openai": ["openai>1.0.0"],
+        "transformers": ["transformers>=4.0.0", "datasets", "torch>=2.3.0"],
         "research": [
             "datasets==2.16.1",
             "nltk",
             "wikiextractor",
             "rouge_score",
             "rapidfuzz",
             "records",
-            "SQLAlchemy",
             "recognizers-text",
             "recognizers-text-suite",
             "emoji==1.7.0",
         ],
         "test": ["pytest", "huggingface_hub", "pre-commit"],
         "docs": [
             "mkdocs-material",
```

### Comparing `blendsql-0.0.15/tests/test_end_to_end.py` & `blendsql-0.0.16/tests/models/test_transformers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 import pytest
-from typing import Set
 
 from blendsql import blend, LLMQA, LLMMap, LLMJoin
-from blendsql.ingredients import Ingredient
 from blendsql._smoothie import Smoothie
 from blendsql.db import SQLite
 from blendsql.utils import fetch_from_hub
 from blendsql.models import TransformersLLM
 
-TEST_TRANSFORMERS_LLM = "Qwen/Qwen1.5-0.5B"
+TEST_TRANSFORMERS_LLM = "hf-internal-testing/tiny-random-PhiForCausalLM"
 
 
 @pytest.fixture(scope="session")
 def db() -> SQLite:
     return SQLite(
         fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")
     )
 
 
 @pytest.fixture(scope="session")
-def ingredients() -> Set[Ingredient]:
+def ingredients() -> set:
     return {LLMQA, LLMMap, LLMJoin}
 
 
 @pytest.fixture(scope="session")
 def model() -> TransformersLLM:
     return TransformersLLM(TEST_TRANSFORMERS_LLM, caching=False)
```

### Comparing `blendsql-0.0.15/tests/test_generic_blendsql.py` & `blendsql-0.0.16/tests/test_generic_blendsql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import pandas as pd
 import sqlite3
 from pathlib import Path
 from blendsql import blend
 from blendsql.db import SQLite
-from blendsql.ingredients.ingredient import IngredientException
+from blendsql._exceptions import IngredientException, InvalidBlendSQL
 
 
 @pytest.fixture(scope="session")
 def db() -> SQLite:
     """Create a dummy sqlite db to use in tests."""
     dbpath = "./test_generic.db"
     df = pd.DataFrame({"Name": ["Danny", "Emma", "Tony"], "Age": [23, 26, 19]})
@@ -19,27 +19,27 @@
     Path(dbpath).unlink()
 
 
 def test_error_on_delete1(db):
     blendsql = """
     DELETE FROM w WHERE TRUE;
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(InvalidBlendSQL):
         _ = blend(
             query=blendsql,
             db=db,
             ingredients=set(),
         )
 
 
 def test_error_on_delete2(db):
     blendsql = """
     DROP TABLE w;
     """
-    with pytest.raises(ValueError):
+    with pytest.raises(InvalidBlendSQL):
         _ = blend(
             query=blendsql,
             db=db,
             ingredients=set(),
         )
```

### Comparing `blendsql-0.0.15/tests/test_grammar.py` & `blendsql-0.0.16/tests/grammars/test_cfg_grammar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import pytest
-from blendsql.grammars.minEarley.parser import EarleyParser
+from blendsql import LLMQA, LLMJoin, LLMMap
+from blendsql.grammars.utils import load_cfg_parser, EarleyParser
 from blendsql.grammars.minEarley.earley_exceptions import UnexpectedInput
 
 
 @pytest.fixture(scope="session")
 def parser() -> EarleyParser:
-    return EarleyParser.open("./blendsql/grammars/_cfg_grammar.lark", start="start")
+    return load_cfg_parser({LLMQA, LLMJoin, LLMMap})
 
 
 accept_queries = [
     """
     {{
         LLMQA(
             'What year was the player born?',
@@ -78,14 +79,26 @@
                 ), d AS (
                     SELECT * FROM documents JOIN t WHERE documents MATCH t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5
                 ) SELECT d.content, t.player AS 'Rangers Player' FROM d JOIN t
             )
         )
     }}
     """,
+    # Named arguments should work
+    """
+    {{
+        LLMQA(
+            question='Tell me why the sky is blue',
+            context=(SELECT * FROM w LIMIT 10)
+        )
+    }}
+    """,
+    """
+    SELECT * FROM w WHERE 1+1 = 2 AND {{LLMMap('more than 30 points?', 'w::score')}} = TRUE
+    """,
     "select count(`driver`) from w",
     "with t as (SELECT count(`driver`) from w), d as (SELECT * FROM w) SELECT * FROM t;",
     "select w.driver || w.constructor from w",
 ]
 
 reject_queries = [
     # not_an_arg
@@ -138,19 +151,61 @@
     """
     select * from w where x 'string';
     """,
     # Duplicate 'with' in CTE
     "with t as (SELECT count(`driver`) from w), with d as (SELECT * FROM w) SELECT * FROM t;",
     # Invalid use of concat
     "select driver from w || t;",
+    # Can't use LLMMap here
+    "SELECT * FROM w JOIN {{LLMMap('more than 30 points?', 'table::column')}}",
 ]
 
 
 @pytest.mark.parametrize("q", accept_queries)
 def test_accept(parser, q):
     parser.parse(q)
 
 
 @pytest.mark.parametrize("q", reject_queries)
 def test_reject(parser, q):
     with pytest.raises(UnexpectedInput):
         parser.parse(q)
+
+
+def test_unspecified_ingredient_reject():
+    """We pass in LLMQA to load_cfg_parser, but then use LLMap.
+    This should raise a grammar error.
+    """
+    parser = load_cfg_parser(ingredients={LLMQA})
+    with pytest.raises(UnexpectedInput):
+        parser.parse(
+            """
+            SELECT * FROM w WHERE {{LLMMap('more than 30 points?', 'w::score')}} = TRUE
+            """
+        )
+
+
+def test_no_ingredients_reject():
+    """If we don't pass any ingredients into load_cfg_parser,
+    we essentially just have a SQLite CFG grammar.
+    """
+    parser = load_cfg_parser()
+    with pytest.raises(UnexpectedInput):
+        parser.parse(
+            """
+            {{
+                LLMQA(
+                    'What year was the player born?',
+                    (
+                        SELECT documents.title AS 'Player', documents.content FROM documents
+                        JOIN {{
+                            LLMJoin(
+                                left_on = 'w::winner',
+                                right_on = 'documents::title'
+                            )
+                        }}
+                        WHERE w.year = '1971-72'
+                    )
+                )
+            }}
+            """
+        )
```

### Comparing `blendsql-0.0.15/tests/test_model.py` & `blendsql-0.0.16/tests/models/test_model_caching.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import uuid
 from dataclasses import dataclass
+
 from blendsql.models import Model
 from blendsql._program import Program
 
 TEST_QUESTION = "The quick brown fox jumps over the lazy dog"
 
 MODEL_A = "a"
 MODEL_B = "b"
@@ -31,121 +32,111 @@
     def __new__(
         self,
         **kwargs,
     ):
         return self.__call__(self, **kwargs)
 
     def __call__(self, question: str, **kwargs):
-        return DummyModelOutput({"uuid": str(uuid.uuid4())})
+        return (DummyModelOutput({"uuid": str(uuid.uuid4())}), None)
 
 
 class DifferentDummyProgram(Program):
     def __new__(
         self,
         **kwargs,
     ):
         return self.__call__(self, **kwargs)
 
     def __call__(self, question: str, unused: str = None, **kwargs):
-        return DummyModelOutput({"uuid": str(uuid.uuid4())})
+        return (DummyModelOutput({"uuid": str(uuid.uuid4())}), None)
 
 
 class DummyProgramWithGlobal(Program):
     def __new__(
         self,
         **kwargs,
     ):
         return self.__call__(self, **kwargs)
 
     def __call__(self, question: str, **kwargs):
         print(TEST_GLOBAL)
-        return DummyModelOutput({"uuid": str(uuid.uuid4())})
+        return (DummyModelOutput({"uuid": str(uuid.uuid4())}), None)
 
 
 def test_simple_cache():
-    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
-        "uuid"
-    ]
+    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)
 
     model_b = DummyModel(MODEL_A)
-    b = model_b.predict(program=DummyProgram, question=TEST_QUESTION)["uuid"]
+    b = model_b.predict(program=DummyProgram, question=TEST_QUESTION)
 
     assert a == b
-    assert model_b.num_llm_calls == 0
+    assert model_b.num_calls == 0
 
 
 def test_different_models():
-    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
-        "uuid"
-    ]
-
-    b = DummyModel(MODEL_B).predict(program=DummyProgram, question=TEST_QUESTION)[
-        "uuid"
-    ]
+    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)
+
+    b = DummyModel(MODEL_B).predict(program=DummyProgram, question=TEST_QUESTION)
 
     assert a != b
 
 
 def test_different_arguments():
-    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
-        "uuid"
-    ]
+    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)
 
     b = DummyModel(MODEL_A).predict(
         program=DummyProgram, question="This is a different question"
-    )["uuid"]
+    )
 
     assert a != b
 
 
 def test_different_programs():
-    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
-        "uuid"
-    ]
+    a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)
 
     b = DummyModel(MODEL_A).predict(
         program=DifferentDummyProgram, question=TEST_QUESTION
-    )["uuid"]
+    )
 
     assert a != b
 
 
 def test_same_global_vars():
     global TEST_GLOBAL
     TEST_GLOBAL = "This is the same value"
     a = DummyModel(MODEL_A).predict(
         program=DummyProgramWithGlobal, question=TEST_QUESTION
-    )["uuid"]
+    )
 
     TEST_GLOBAL = "This is the same value"
     model_b = DummyModel(MODEL_A)
-    b = model_b.predict(program=DummyProgramWithGlobal, question=TEST_QUESTION)["uuid"]
+    b = model_b.predict(program=DummyProgramWithGlobal, question=TEST_QUESTION)
 
     assert a == b
-    assert model_b.num_llm_calls == 0
+    assert model_b.num_calls == 0
 
 
 def test_different_global_vars():
     global TEST_GLOBAL
     TEST_GLOBAL = "This is one value"
     a = DummyModel(MODEL_A).predict(
         program=DummyProgramWithGlobal, question=TEST_QUESTION
-    )["uuid"]
+    )
 
     TEST_GLOBAL = "This is a different value"
     b = DummyModel(MODEL_A).predict(
         program=DummyProgramWithGlobal, question=TEST_QUESTION
-    )["uuid"]
+    )
 
     assert a != b
 
 
 def test_with_set_vars():
     a = DummyModel(MODEL_A).predict(
         program=DummyProgram, question=TEST_QUESTION, random_set={"a", "b", "c"}
-    )["uuid"]
+    )
 
     b = DummyModel(MODEL_A).predict(
         program=DummyProgram, question=TEST_QUESTION, random_set={"b", "c", "a"}
-    )["uuid"]
+    )
 
     assert a == b
```

### Comparing `blendsql-0.0.15/tests/test_multi_table_blendsql.py` & `blendsql-0.0.16/tests/test_multi_table_blendsql.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,27 +58,27 @@
         )
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["A"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE Symbol in
     (
         SELECT Symbol FROM constituents
                 WHERE sector = 'Information Technology'
     )
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_join_multi_exec(db, ingredients):
     blendsql = """
     SELECT "Run Date", Account, Action, ROUND("Amount ($)", 2) AS 'Total Dividend Payout ($$)', Name
         FROM account_history
         LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
@@ -95,23 +95,23 @@
         AND lower(account_history.Action) like "%dividend%"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["A"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT Name) FROM constituents WHERE Sector = 'Information Technology'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_join_not_qualified_multi_exec(db, ingredients):
     """Same test as test_join_multi_exec(), but without qualifying columns if we don't need to.
     i.e. 'Action' and 'Sector' don't have tablename preceding them.
     commit fefbc0a
     """
@@ -132,23 +132,23 @@
         AND lower(Action) like "%dividend%"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["A"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT Name) FROM constituents WHERE Sector = 'Information Technology'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_select_multi_exec(db, ingredients):
     blendsql = """
     SELECT "Run Date", Account, Action, ROUND("Amount ($)", 2) AS 'Total Dividend Payout ($$)', Name
         FROM account_history
         LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
@@ -166,15 +166,15 @@
         AND lower(account_history.Action) like "%dividend%"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_complex_multi_exec(db, ingredients):
     blendsql = """
     SELECT DISTINCT constituents.Symbol, Action FROM constituents
     LEFT JOIN account_history ON constituents.Symbol = account_history.Symbol
@@ -194,15 +194,15 @@
     ORDER BY LENGTH(constituents.Name) LIMIT 1
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_complex_not_qualified_multi_exec(db, ingredients):
     """Same test as test_complex_multi_exec(), but without qualifying columns if we don't need to.
     commit fefbc0a
     """
@@ -225,15 +225,15 @@
     ORDER BY LENGTH(Name) LIMIT 1
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_join_ingredient_multi_exec(db, ingredients):
     blendsql = """
     SELECT Account, Quantity FROM returns
     JOIN {{
@@ -247,15 +247,15 @@
     SELECT Account, Quantity FROM returns JOIN account_history ON returns."Annualized Returns" = account_history."Account"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_qa_equals_multi_exec(db, ingredients):
     blendsql = """
     SELECT Action FROM account_history
     WHERE Symbol = {{return_aapl()}}
@@ -265,15 +265,15 @@
     WHERE Symbol = "AAPL"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_table_alias_multi_exec(db, ingredients):
     blendsql = """
     SELECT Symbol FROM portfolio AS w
         WHERE {{starts_with('A', 'w::Symbol')}} = TRUE
@@ -285,23 +285,23 @@
         AND LENGTH(w.Symbol) > 3
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["A"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE LENGTH(Symbol) > 3
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_subquery_alias_multi_exec(db, ingredients):
     blendsql = """
     SELECT Symbol FROM (
         SELECT DISTINCT Symbol FROM portfolio WHERE Symbol IN (
             SELECT Symbol FROM portfolio WHERE Quantity > 200
@@ -316,23 +316,23 @@
     ) AS w WHERE w.Symbol LIKE 'F%' AND LENGTH(w.Symbol) > 3
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["F"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE LENGTH(Symbol) > 3 AND Quantity > 200
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_cte_qa_multi_exec(db, ingredients):
     blendsql = """
    {{
         get_table_size(
             (
@@ -351,23 +351,35 @@
     ) SELECT COUNT(*) FROM a WHERE LENGTH(a.Symbol) > 2
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["F"])
     # Make sure we only pass what's necessary to our ingredient
-    # passed_to_ingredient = db.execute_query(
-    #     """
-    # SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE LENGTH(Symbol) > 3 AND Quantity > 200
-    # """
-    # )
-    # assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    passed_to_map_ingredient = db.execute_to_list(
+        """
+    SELECT COUNT(DISTINCT Symbol) FROM portfolio
+    """
+    )[0]
+    # We also need to factor in what we passed to QA ingredient
+    passed_to_qa_ingredient = db.execute_to_list(
+        """
+    WITH a AS (
+        SELECT * FROM (SELECT DISTINCT * FROM portfolio) as w
+            WHERE w.Symbol LIKE 'F%'
+    ) SELECT COUNT(*) FROM a WHERE LENGTH(a.Symbol) > 2
+    """
+    )[0]
+    assert (
+        smoothie.meta.num_values_passed
+        == passed_to_qa_ingredient + passed_to_map_ingredient
+    )
 
 
 def test_cte_qa_named_multi_exec(db, ingredients):
     blendsql = """
    {{
         get_table_size(
             (
@@ -386,23 +398,33 @@
     ) SELECT COUNT(*) FROM a WHERE LENGTH(a.Symbol) > 2
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["F"])
     # Make sure we only pass what's necessary to our ingredient
-    # passed_to_ingredient = db.execute_query(
-    #     """
-    # SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE LENGTH(Symbol) > 3 AND Quantity > 200
-    # """
-    # )
-    # assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    passed_to_map_ingredient = db.execute_to_list(
+        """
+        SELECT COUNT(DISTINCT Symbol) FROM portfolio
+        """
+    )[0]
+    passed_to_qa_ingredient = db.execute_to_list(
+        """
+    WITH a AS (
+        SELECT * FROM (SELECT DISTINCT * FROM portfolio) as w
+            WHERE w.Symbol LIKE 'F%'
+    ) SELECT COUNT(*) FROM a WHERE LENGTH(a.Symbol) > 2
+    """
+    )[0]
+    assert smoothie.meta.num_values_passed == (
+        passed_to_map_ingredient + passed_to_qa_ingredient
+    )
 
 
 def test_ingredient_in_select_with_join_multi_exec(db, ingredients):
     """If the query only has an ingredient in the `SELECT` statement, and `JOIN` clause,
     we should run the `JOIN` statement first, and then call the ingredient.
 
     commit de4a7bc
@@ -418,25 +440,25 @@
         WHERE account_history.Action like "%dividend%"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT constituents.Name)
     FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
     WHERE account_history.Action like "%dividend%"
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_ingredient_in_select_with_join_multi_select_multi_exec(db, ingredients):
     """A modified version of the above
 
     commit de4a7bc
     """
@@ -451,52 +473,52 @@
         WHERE Action like "%dividend%"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT constituents.Name)
     FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
     WHERE account_history.Action like "%dividend%"
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
-# def test_subquery_alias_with_join_multi_exec(db, ingredients):
-#     blendsql = """
-#     SELECT w."Percent of Account" FROM (SELECT * FROM "portfolio" WHERE Quantity > 200 OR "Today''s Gain/Loss Percent" > 0.05) as w
-#     JOIN {{
-#         do_join(
-#             left_on='w::Symbol',
-#             right_on='geographic::Symbol'
-#         )
-#     }} WHERE {{starts_with('F', 'w::Symbol')}}
-#     AND w."Percent of Account" < 0.2
-#     """
-#
-#     sql = """
-#     SELECT w."Percent of Account" FROM (SELECT * FROM "portfolio" WHERE Quantity > 200 OR "Today''s Gain/Loss Percent" > 0.05) as w
-#     JOIN geographic ON w.Symbol = geographic.Symbol
-#     WHERE w.Symbol LIKE 'F%'
-#     AND w."Percent of Account" < 0.2
-#     """
-#     smoothie = blend(
-#         query=blendsql,
-#         db=db,
-#         ingredients=ingredients,
-#     )
-#     sql_df = db.execute_query(sql)
-#     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["F"])
-#     # Make sure we only pass what's necessary to our ingredient
-#     # passed_to_ingredient = db.execute_query(
-#     #     """
-#     # SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE LENGTH(Symbol) > 3
-#     # """
-#     # )
-#     # assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+def test_subquery_alias_with_join_multi_exec(db, ingredients):
+    blendsql = """
+    SELECT w."Percent of Account" FROM (SELECT * FROM "portfolio" WHERE Quantity > 200 OR "Today''s Gain/Loss Percent" > 0.05) as w
+    JOIN {{
+        do_join(
+            left_on='geographic::Symbol',
+            right_on='w::Symbol'
+        )
+    }} WHERE {{starts_with('F', 'w::Symbol')}}
+    AND w."Percent of Account" < 0.2
+    """
+
+    sql = """
+    SELECT w."Percent of Account" FROM (SELECT * FROM "portfolio" WHERE Quantity > 200 OR "Today''s Gain/Loss Percent" > 0.05) as w
+    JOIN geographic ON w.Symbol = geographic.Symbol
+    WHERE w.Symbol LIKE 'F%'
+    AND w."Percent of Account" < 0.2
+    """
+    smoothie = blend(
+        query=blendsql,
+        db=db,
+        ingredients=ingredients,
+    )
+    sql_df = db.execute_to_df(sql)
+    assert_equality(smoothie=smoothie, sql_df=sql_df, args=["F"])
+    # Make sure we only pass what's necessary to our ingredient
+    passed_to_ingredient = db.execute_to_list(
+        """
+    SELECT COUNT(DISTINCT Symbol) FROM portfolio WHERE (Quantity > 200 OR "Today''s Gain/Loss Percent" > 0.05) AND "Percent of Account" < 0.2 
+    """
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
```

### Comparing `blendsql-0.0.15/tests/test_single_table_blendsql.py` & `blendsql-0.0.16/tests/test_single_table_blendsql.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     SELECT * FROM transactions WHERE merchant LIKE "Z%";
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["Z"])
 
 
 def test_simple_ingredient_exec_at_end(db, ingredients):
     blendsql = """
     SELECT * FROM transactions WHERE {{starts_with('Z', 'transactions::merchant')}}
     """
@@ -80,34 +80,34 @@
     SELECT * FROM transactions WHERE merchant LIKE "Z%";
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["Z"])
 
 
 def test_simple_ingredient_exec_in_select(db, ingredients):
     blendsql = """
     SELECT {{starts_with('Z', 'transactions::merchant')}} FROM transactions WHERE parent_category = 'Auto & Transport'
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions WHERE parent_category = 'Auto & Transport'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_nested_ingredient_exec(db, ingredients):
     blendsql = """
     SELECT DISTINCT merchant FROM transactions WHERE
         merchant in (
             SELECT merchant FROM transactions
@@ -124,26 +124,33 @@
         );
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["Z"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions WHERE amount > 100
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_nonexistent_column_exec(db, ingredients):
+    """
+    NOTE: Converting to CNF would break this one
+    since we would get:
+        SELECT DISTINCT merchant, child_category FROM transactions WHERE
+        (child_category = 'Gifts' OR STRUCT(STRUCT(A())) = 1) AND
+        (child_category = 'Gifts' OR child_category = 'this does not exist')
+    """
     blendsql = """
     SELECT DISTINCT merchant, child_category FROM transactions WHERE
        (
            {{starts_with('Z', 'transactions::merchant')}} = 1
            AND child_category = 'this does not exist'
        )
        OR child_category = 'Gifts'
@@ -157,23 +164,23 @@
        OR child_category = 'Gifts'
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["Z"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions WHERE child_category = 'this does not exist'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_nested_and_exec(db, ingredients):
     blendsql = """
     SELECT DISTINCT merchant, child_category FROM transactions WHERE
        (
            {{starts_with('O', 'transactions::merchant')}} = 1
@@ -190,23 +197,23 @@
        OR child_category = 'Gifts'
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["O"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions WHERE child_category = 'Restaurants & Dining'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_multiple_nested_ingredients(db, ingredients):
     blendsql = """
     SELECT DISTINCT child_category, merchant FROM transactions WHERE
         (
             {{starts_with('A', 'transactions::merchant')}} = 1
@@ -225,23 +232,23 @@
         OR child_category = 'Gifts'
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df, args=["A", "T"])
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) + COUNT(DISTINCT child_category) FROM transactions WHERE parent_category = 'Food'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_length_ingredient(db, ingredients):
     blendsql = """
     SELECT {{get_length('length', 'transactions::merchant')}}, merchant
         FROM transactions
         WHERE {{get_length('length', 'transactions::merchant')}} > 1;
@@ -252,23 +259,23 @@
         WHERE LENGTH(merchant) > 1;
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_max_length(db, ingredients):
     blendsql = """
     SELECT MAX({{get_length('length', 'transactions::merchant')}}) as max_length, merchant
         FROM transactions
         WHERE {{get_length('length', 'transactions::merchant')}} > 1;
@@ -279,23 +286,23 @@
         WHERE LENGTH(merchant) > 1;
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_limit(db, ingredients):
     blendsql = """
     SELECT DISTINCT merchant, child_category FROM transactions WHERE
        {{starts_with('P', 'transactions::merchant')}} = 1
        AND child_category = 'Restaurants & Dining'
@@ -308,23 +315,23 @@
         LIMIT 1
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions WHERE child_category = 'Restaurants & Dining'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_select(db, ingredients):
     blendsql = """
     SELECT DISTINCT merchant, child_category FROM transactions WHERE
        merchant = {{select_first_sorted(options='transactions::merchant')}}
     """
@@ -333,15 +340,15 @@
         ORDER BY merchant LIMIT 1
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_ingredient_in_select_stmt(db, ingredients):
     blendsql = """
     SELECT MAX({{get_length('length', 'transactions::merchant')}}) as l FROM transactions 
     """
@@ -349,23 +356,23 @@
     SELECT MAX(LENGTH(merchant)) as l FROM transactions
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions 
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_ingredient_in_select_stmt_with_filter(db, ingredients):
     # commit de4a7bc
     blendsql = """
     SELECT MAX({{get_length('length', 'transactions::merchant')}}) as l FROM transactions WHERE child_category = 'Restaurants & Dining'
     """
@@ -373,46 +380,46 @@
     SELECT MAX(LENGTH(merchant)) as l FROM transactions WHERE child_category = 'Restaurants & Dining'
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions WHERE child_category = 'Restaurants & Dining'
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_nested_duplicate_map_calls(db, ingredients):
     blendsql = """
     SELECT merchant FROM transactions WHERE {{get_length('length', 'transactions::merchant')}} > (SELECT {{get_length('length', 'transactions::merchant')}} FROM transactions WHERE merchant = 'Paypal')
     """
     sql = """
     SELECT merchant FROM transactions WHERE LENGTH(merchant) > (SELECT LENGTH(merchant) FROM transactions WHERE merchant = 'Paypal')
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT COUNT(DISTINCT merchant) FROM transactions
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_many_duplicate_map_calls(db, ingredients):
     blendsql = """
     SELECT 
         {{get_length('length', 'transactions::merchant')}} AS l1,
         {{get_length('length', 'transactions::cash_flow')}} AS l2,
@@ -429,27 +436,27 @@
     FROM transactions WHERE amount > 1300    
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT
     (SELECT COUNT(DISTINCT merchant) FROM transactions WHERE amount > 1300)
     + (SELECT COUNT(DISTINCT cash_flow) FROM transactions WHERE amount > 1300)
     + (SELECT COUNT(DISTINCT child_category) FROM transactions WHERE amount > 1300)
     + (SELECT COUNT(DISTINCT date) FROM transactions WHERE amount > 1300)
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_exists_isolated_qa_call(db, ingredients):
     # commit 7a19e39
     blendsql = """
     SELECT NOT EXISTS (
         SELECT * FROM transactions WHERE {{get_length('length', 'transactions::merchant')}} > 4 AND amount > 500
@@ -468,23 +475,23 @@
     )   
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
-    sql_df = db.execute_query(sql)
+    sql_df = db.execute_to_df(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
-    passed_to_ingredient = db.execute_query(
+    passed_to_ingredient = db.execute_to_list(
         """
     SELECT (SELECT COUNT(DISTINCT merchant) FROM transactions WHERE amount > 500) + (SELECT COUNT(*) FROM transactions WHERE amount < 500)
     """
-    )
-    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+    )[0]
+    assert smoothie.meta.num_values_passed == passed_to_ingredient
 
 
 def test_query_options_arg(db, ingredients):
     # commit 5ffa26d
     blendsql = """
     {{
         select_first_option(
```

### Comparing `blendsql-0.0.15/tests/utils.py` & `blendsql-0.0.16/tests/utils.py`

 * *Files identical despite different names*

