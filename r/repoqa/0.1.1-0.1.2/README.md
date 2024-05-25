# Comparing `tmp/repoqa-0.1.1.tar.gz` & `tmp/repoqa-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repoqa-0.1.1.tar", last modified: Sun May 19 19:28:07 2024, max compression
+gzip compressed data, was "repoqa-0.1.2.tar", last modified: Sat May 25 06:02:56 2024, max compression
```

## Comparing `repoqa-0.1.1.tar` & `repoqa-0.1.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3194 2024-04-24 00:46:21.000000 repoqa-0.1.1/.gitignore
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      913 2024-04-24 00:46:21.000000 repoqa-0.1.1/.pre-commit-config.yaml
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    11558 2024-04-24 00:46:21.000000 repoqa-0.1.1/LICENSE
--rw-r--r--   0 ganler    (1000) ganler    (1000)     6273 2024-05-19 19:28:07.287425 repoqa-0.1.1/PKG-INFO
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5375 2024-05-19 19:27:40.000000 repoqa-0.1.1/README.md
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/docs/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2575 2024-04-24 00:46:21.000000 repoqa-0.1.1/docs/curate_dataset.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      825 2024-04-24 00:46:21.000000 repoqa-0.1.1/docs/dev_note.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-04-24 00:46:21.000000 repoqa-0.1.1/pyproject.toml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/repoqa/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      208 2024-04-24 00:46:21.000000 repoqa-0.1.1/repoqa/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      411 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa/_version.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    13467 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/compute_score.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1639 2024-04-26 09:19:08.000000 repoqa-0.1.1/repoqa/data.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      600 2024-04-24 00:46:21.000000 repoqa-0.1.1/repoqa/metric.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/repoqa/provider/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      136 2024-04-24 19:42:11.000000 repoqa-0.1.1/repoqa/provider/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1023 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/anthropic.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      332 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/base.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1435 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/google.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2487 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/hf.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1522 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/openai.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/repoqa/provider/request/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      649 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/request/__init__.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2038 2024-04-26 09:19:08.000000 repoqa-0.1.1/repoqa/provider/request/anthropic.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1857 2024-04-24 22:48:39.000000 repoqa-0.1.1/repoqa/provider/request/google.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1704 2024-04-26 09:19:08.000000 repoqa-0.1.1/repoqa/provider/request/openai.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1620 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/provider/vllm.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    13669 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/search_needle_function.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2527 2024-05-19 19:27:40.000000 repoqa-0.1.1/repoqa/utility.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/repoqa.egg-info/
--rw-r--r--   0 ganler    (1000) ganler    (1000)     6273 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/PKG-INFO
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2040 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/SOURCES.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        1 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/dependency_links.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/entry_points.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      234 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/requires.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-05-19 19:28:07.000000 repoqa-0.1.1/repoqa.egg-info/top_level.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-05-19 19:27:40.000000 repoqa-0.1.1/requirements.txt
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/results/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       13 2024-04-24 00:46:21.000000 repoqa-0.1.1/results/.gitignore
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      675 2024-04-24 00:46:21.000000 repoqa-0.1.1/results/README.md
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/cherrypick/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      720 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/cherrypick/README.md
--rw-rw-r--   0 ganler    (1000) ganler    (1000)    12868 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/cherrypick/lists.json
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1986 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/dataset_ensemble_clone.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2480 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dataset_ensemble_gh_api.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4086 2024-04-19 09:21:06.000000 repoqa-0.1.1/scripts/curate/dep_analysis/cpp.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/data/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/data/.gitignore
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/go-analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3118 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/dep_analysis/go-analysis/dependency_analysis.go
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2843 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/dep_analysis/go.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1652 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.283425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/java-lib/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)  6013426 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2984 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/pom.xml
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.279425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5415 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2199 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/java.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2610 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/python.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     5579 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/dep_analysis/rust.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4294 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/dep_analysis/typescript.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4163 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/function_analysis.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3980 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/curate/github_fetch.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1589 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/merge_annotation.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     1173 2024-04-16 20:28:57.000000 repoqa-0.1.1/scripts/curate/merge_dep.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     4756 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/needle_annotation.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3223 2024-04-19 09:21:06.000000 repoqa-0.1.1/scripts/curate/needle_selection.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     3378 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/curate/obfuscate_nl.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/requirements.txt
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      320 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/curate/utility.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/demos/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      751 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/demos/model_request_oai.py
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/dev/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)       84 2024-02-25 13:11:01.000000 repoqa-0.1.1/scripts/dev/license-hdr.txt
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/eval/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      502 2024-05-19 19:27:40.000000 repoqa-0.1.1/scripts/eval/recompute_all_scores.sh
-drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-19 19:28:07.287425 repoqa-0.1.1/scripts/misc/
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      877 2024-04-06 02:26:24.000000 repoqa-0.1.1/scripts/misc/estimate_max_char.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)     2432 2024-04-24 00:46:21.000000 repoqa-0.1.1/scripts/misc/repo_token_size.py
--rw-rw-r--   0 ganler    (1000) ganler    (1000)      980 2024-05-19 19:28:07.287425 repoqa-0.1.1/setup.cfg
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3194 2024-04-24 00:46:21.000000 repoqa-0.1.2/.gitignore
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      913 2024-04-24 00:46:21.000000 repoqa-0.1.2/.pre-commit-config.yaml
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    11558 2024-04-24 00:46:21.000000 repoqa-0.1.2/LICENSE
+-rw-r--r--   0 ganler    (1000) ganler    (1000)     7864 2024-05-25 06:02:56.770351 repoqa-0.1.2/PKG-INFO
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     6941 2024-05-25 06:02:04.000000 repoqa-0.1.2/README.md
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/docs/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2575 2024-04-24 00:46:21.000000 repoqa-0.1.2/docs/curate_dataset.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      825 2024-04-24 00:46:21.000000 repoqa-0.1.2/docs/dev_note.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-04-24 00:46:21.000000 repoqa-0.1.2/pyproject.toml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/repoqa/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      208 2024-04-24 00:46:21.000000 repoqa-0.1.2/repoqa/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      411 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa/_version.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    13467 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/compute_score.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1639 2024-04-26 09:19:08.000000 repoqa-0.1.2/repoqa/data.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      600 2024-04-24 00:46:21.000000 repoqa-0.1.2/repoqa/metric.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/repoqa/provider/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      136 2024-04-24 19:42:11.000000 repoqa-0.1.2/repoqa/provider/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1023 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/provider/anthropic.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      332 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/provider/base.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1435 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/provider/google.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2546 2024-05-25 06:02:04.000000 repoqa-0.1.2/repoqa/provider/hf.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1522 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/provider/openai.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/repoqa/provider/request/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      649 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/provider/request/__init__.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2038 2024-04-26 09:19:08.000000 repoqa-0.1.2/repoqa/provider/request/anthropic.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1857 2024-04-24 22:48:39.000000 repoqa-0.1.2/repoqa/provider/request/google.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1704 2024-04-26 09:19:08.000000 repoqa-0.1.2/repoqa/provider/request/openai.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1679 2024-05-25 06:02:04.000000 repoqa-0.1.2/repoqa/provider/vllm.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    13669 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/search_needle_function.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2527 2024-05-19 19:27:40.000000 repoqa-0.1.2/repoqa/utility.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/repoqa.egg-info/
+-rw-r--r--   0 ganler    (1000) ganler    (1000)     7864 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa.egg-info/PKG-INFO
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2040 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa.egg-info/SOURCES.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        1 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa.egg-info/dependency_links.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa.egg-info/entry_points.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      244 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa.egg-info/requires.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-05-25 06:02:56.000000 repoqa-0.1.2/repoqa.egg-info/top_level.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      134 2024-05-25 06:02:04.000000 repoqa-0.1.2/requirements.txt
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/results/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       13 2024-04-24 00:46:21.000000 repoqa-0.1.2/results/.gitignore
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      675 2024-04-24 00:46:21.000000 repoqa-0.1.2/results/README.md
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/cherrypick/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      720 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/cherrypick/README.md
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)    12868 2024-05-19 19:27:40.000000 repoqa-0.1.2/scripts/cherrypick/lists.json
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.766351 repoqa-0.1.2/scripts/curate/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1986 2024-05-19 19:27:40.000000 repoqa-0.1.2/scripts/curate/dataset_ensemble_clone.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2480 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/curate/dataset_ensemble_gh_api.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.766351 repoqa-0.1.2/scripts/curate/dep_analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4086 2024-04-19 09:21:06.000000 repoqa-0.1.2/scripts/curate/dep_analysis/cpp.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.766351 repoqa-0.1.2/scripts/curate/dep_analysis/data/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)        7 2024-04-16 20:28:57.000000 repoqa-0.1.2/scripts/curate/dep_analysis/data/.gitignore
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.766351 repoqa-0.1.2/scripts/curate/dep_analysis/go-analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3118 2024-05-19 19:27:40.000000 repoqa-0.1.2/scripts/curate/dep_analysis/go-analysis/dependency_analysis.go
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2843 2024-05-19 19:27:40.000000 repoqa-0.1.2/scripts/curate/dep_analysis/go.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.766351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1652 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.766351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/java-lib/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)  6013426 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2984 2024-04-16 20:28:57.000000 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/pom.xml
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.762351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5415 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2199 2024-04-16 20:28:57.000000 repoqa-0.1.2/scripts/curate/dep_analysis/java.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2610 2024-04-16 20:28:57.000000 repoqa-0.1.2/scripts/curate/dep_analysis/python.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     5579 2024-04-16 20:28:57.000000 repoqa-0.1.2/scripts/curate/dep_analysis/rust.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4294 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/curate/dep_analysis/typescript.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4163 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/curate/function_analysis.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3980 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/curate/github_fetch.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1589 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/curate/merge_annotation.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     1173 2024-04-16 20:28:57.000000 repoqa-0.1.2/scripts/curate/merge_dep.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     4756 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/curate/needle_annotation.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3223 2024-04-19 09:21:06.000000 repoqa-0.1.2/scripts/curate/needle_selection.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     3378 2024-05-19 19:27:40.000000 repoqa-0.1.2/scripts/curate/obfuscate_nl.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      129 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/curate/requirements.txt
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      320 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/curate/utility.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/scripts/demos/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      751 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/demos/model_request_oai.py
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/scripts/dev/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)       84 2024-02-25 13:11:01.000000 repoqa-0.1.2/scripts/dev/license-hdr.txt
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/scripts/eval/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      502 2024-05-19 19:27:40.000000 repoqa-0.1.2/scripts/eval/recompute_all_scores.sh
+drwxrwxr-x   0 ganler    (1000) ganler    (1000)        0 2024-05-25 06:02:56.770351 repoqa-0.1.2/scripts/misc/
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      877 2024-04-06 02:26:24.000000 repoqa-0.1.2/scripts/misc/estimate_max_char.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)     2432 2024-04-24 00:46:21.000000 repoqa-0.1.2/scripts/misc/repo_token_size.py
+-rw-rw-r--   0 ganler    (1000) ganler    (1000)      991 2024-05-25 06:02:56.770351 repoqa-0.1.2/setup.cfg
```

### Comparing `repoqa-0.1.1/.gitignore` & `repoqa-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/.pre-commit-config.yaml` & `repoqa-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/LICENSE` & `repoqa-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/PKG-INFO` & `repoqa-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: repoqa
-Version: 0.1.1
+Version: 0.1.2
 Summary: "RepoQA for Evaluating Long-Context Code Understanding"
 Home-page: https://github.com/evalplus/repoqa
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tempdir>=0.7.1
 Requires-Dist: appdirs>=1.4.4
+Requires-Dist: wget>=3.2
 Requires-Dist: fire>=0.6.0
 Requires-Dist: nltk>=3.8.1
 Requires-Dist: rich>=13.5.2
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: tree_sitter_languages>=1.10.2
 Requires-Dist: transformers>=4.40.0
 Requires-Dist: openai>=1.23.2
@@ -61,28 +62,34 @@
 ```
 
 </div>
 </details>
 
 ## 🏁 Search Needle Function (SNF)
 
-Search Needle Function is the first RepoQA task which aims to practice LLMs' ability of **long-context code understanding and retrieval**.
-Its corresponding real-life application is to perform precise code search from user intent rather than simple keyword match.
+Search Needle Function is the first and base RepoQA task which aims to practice LLMs' ability of **long-context code understanding and retrieval**.
+Its corresponding real-life scenario is to perform precise code search from function description.
 
-> [!Important]
+<details><summary>🔎 More dataset details <i>:: click to expand ::</i></summary>
+<div>
+
+> [!Note]
 >
-> SNF includes 500 tests (5 programming languages x 10 repositories x 10 needle functions) where an LLM is given:
+> SNF includes 500 tests (5 programming languages x 10 repos x 10 needle functions) where an LLM is given:
 >
 > 1. A large code context sorted in file dependency
 > 2. A NL description of the needle function without revealing keywords like function names
 > 3. An instruction to retrieve the described function
 >
 > The evaluator passes a test if the searched function is syntactically closest to the ground-truth compared against
 > other functions (systematically parsed by `treesitter`) and the similarity is greater than a user defined threshold (by default 0.8).
 
+</div>
+</details>
+
 You can run the SNF evaluation using various backends:
 
 ### OpenAI Compatible Servers
 
 ```bash
 repoqa.search_needle_function --model "gpt4-turbo" --backend openai
 # 💡 If you use openai API compatible server such as vLLM servers:
@@ -98,38 +105,70 @@
 
 ### vLLM
 
 ```bash
 repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --backend vllm
 ```
 
-> [!Tip]
->
-> You can unlock the model's context using [dynamic RoPE scaling](https://blog.eleuther.ai/yarn/#dynamic-scaling).
-> For example, `Meta-Llama-3-8B-Instruct` has 8k context but running the default 16k test needs more (approx. 20k).
+<details><summary>🔎 Context extension for small-ctx models <i>:: click to expand ::</i></summary>
+<div>
+
+> There are two ways to unlock a model's context at inference time:
 >
-> To extend the context to 32k, in its config file (`hub/models--meta-llama--Meta-Llama-3-8B-Instruct/snapshots/[hash]/config.json`) set:
+> 1. **Direct Extension**: Edit `max_positional_embedding` of the model's `config.json` (e.g., `hub/models--meta-llama--Meta-Llama-3-8B-Instruct/snapshots/[hash]/config.json`) to something like `22528`.
+> 2. **[Dynamic RoPE Scaling](https://blog.eleuther.ai/yarn/#dynamic-scaling)**:
+>    To extend `Meta-Llama-3-8B-Instruct` from 8k to 32k (4x), edit the `config.json`:
 >
 > `"rope_scaling": {"type": "dynamic", "factor": 4.0}`
 >
 > Note: This works for vLLM `<0.4.3` and HuggingFace transformers. RepoQA will automatically configure dynamic RoPE for vLLM `>= 0.4.3`
 
+</div>
+</details>
+
 > [!Note]
 >
 > Reference evaluation time:
 >
 > - Llama3-8B-Instruct: 45 minutes on 2xA6000 (PCIe NVLink)
 > - Llama3-70B-Instruct: 100 minutes on 4xA100 (PCIe NVLink)
 
 ### HuggingFace transformers
 
 ```bash
 repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --backend hf --trust-remote-code
 ```
 
+> [!Tip]
+>
+> Installing [flash-attn](https://github.com/Dao-AILab/flash-attention) and
+> additionally set `--attn-implementation "flash_attention_2"` can largely
+> lower the memory requirement.
+
+<details><summary>🔨 Having trouble installing `flash-attn`? <i>:: click to expand ::</i></summary>
+<div>
+
+> If you have trouble with `pip install flash-attn --no-build-isolation`,
+> you can try to directly use [pre-built wheels](https://github.com/Dao-AILab/flash-attention/releases):
+>
+> ```shell
+> export FLASH_ATTN_VER=2.5.8 # check latest version at https://github.com/Dao-AILab/flash-attention/releases
+> export CUDA_VER="cu122"     # check available ones at https://github.com/Dao-AILab/flash-attention/releases
+> export TORCH_VER=$(python -c "import torch; print('.'.join(torch.__version__.split('.')[:2]))")
+> export PY_VER=$(python -c "import platform; print(''.join(platform.python_version().split('.')[:2]))")
+> export OS_ARCH=$(python -c "import platform; print(f'{platform.system().lower()}_{platform.machine()}')")
+>
+> export WHEEL=flash_attn-${FLASH_ATTN_VER}+${CUDA_VER}torch${TORCH_VER}cxx11abiFALSE-cp${PY_VER}-cp${PY_VER}-${OS_ARCH}.whl
+> wget https://github.com/Dao-AILab/flash-attention/releases/download/v${FLASH_ATTN_VER}/${WHEEL}
+> pip install ${WHEEL}
+> ```
+
+</div>
+</details>
+
 ### Google Generative AI API (Gemini)
 
 ```bash
 repoqa.search_needle_function --model "gemini-1.5-pro-latest" --backend google
 ```
 
 ### CLI Usage
```

### Comparing `repoqa-0.1.1/README.md` & `repoqa-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -33,28 +33,34 @@
 ```
 
 </div>
 </details>
 
 ## 🏁 Search Needle Function (SNF)
 
-Search Needle Function is the first RepoQA task which aims to practice LLMs' ability of **long-context code understanding and retrieval**.
-Its corresponding real-life application is to perform precise code search from user intent rather than simple keyword match.
+Search Needle Function is the first and base RepoQA task which aims to practice LLMs' ability of **long-context code understanding and retrieval**.
+Its corresponding real-life scenario is to perform precise code search from function description.
 
-> [!Important]
+<details><summary>🔎 More dataset details <i>:: click to expand ::</i></summary>
+<div>
+
+> [!Note]
 >
-> SNF includes 500 tests (5 programming languages x 10 repositories x 10 needle functions) where an LLM is given:
+> SNF includes 500 tests (5 programming languages x 10 repos x 10 needle functions) where an LLM is given:
 >
 > 1. A large code context sorted in file dependency
 > 2. A NL description of the needle function without revealing keywords like function names
 > 3. An instruction to retrieve the described function
 >
 > The evaluator passes a test if the searched function is syntactically closest to the ground-truth compared against
 > other functions (systematically parsed by `treesitter`) and the similarity is greater than a user defined threshold (by default 0.8).
 
+</div>
+</details>
+
 You can run the SNF evaluation using various backends:
 
 ### OpenAI Compatible Servers
 
 ```bash
 repoqa.search_needle_function --model "gpt4-turbo" --backend openai
 # 💡 If you use openai API compatible server such as vLLM servers:
@@ -70,38 +76,70 @@
 
 ### vLLM
 
 ```bash
 repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --backend vllm
 ```
 
-> [!Tip]
->
-> You can unlock the model's context using [dynamic RoPE scaling](https://blog.eleuther.ai/yarn/#dynamic-scaling).
-> For example, `Meta-Llama-3-8B-Instruct` has 8k context but running the default 16k test needs more (approx. 20k).
+<details><summary>🔎 Context extension for small-ctx models <i>:: click to expand ::</i></summary>
+<div>
+
+> There are two ways to unlock a model's context at inference time:
 >
-> To extend the context to 32k, in its config file (`hub/models--meta-llama--Meta-Llama-3-8B-Instruct/snapshots/[hash]/config.json`) set:
+> 1. **Direct Extension**: Edit `max_positional_embedding` of the model's `config.json` (e.g., `hub/models--meta-llama--Meta-Llama-3-8B-Instruct/snapshots/[hash]/config.json`) to something like `22528`.
+> 2. **[Dynamic RoPE Scaling](https://blog.eleuther.ai/yarn/#dynamic-scaling)**:
+>    To extend `Meta-Llama-3-8B-Instruct` from 8k to 32k (4x), edit the `config.json`:
 >
 > `"rope_scaling": {"type": "dynamic", "factor": 4.0}`
 >
 > Note: This works for vLLM `<0.4.3` and HuggingFace transformers. RepoQA will automatically configure dynamic RoPE for vLLM `>= 0.4.3`
 
+</div>
+</details>
+
 > [!Note]
 >
 > Reference evaluation time:
 >
 > - Llama3-8B-Instruct: 45 minutes on 2xA6000 (PCIe NVLink)
 > - Llama3-70B-Instruct: 100 minutes on 4xA100 (PCIe NVLink)
 
 ### HuggingFace transformers
 
 ```bash
 repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --backend hf --trust-remote-code
 ```
 
+> [!Tip]
+>
+> Installing [flash-attn](https://github.com/Dao-AILab/flash-attention) and
+> additionally set `--attn-implementation "flash_attention_2"` can largely
+> lower the memory requirement.
+
+<details><summary>🔨 Having trouble installing `flash-attn`? <i>:: click to expand ::</i></summary>
+<div>
+
+> If you have trouble with `pip install flash-attn --no-build-isolation`,
+> you can try to directly use [pre-built wheels](https://github.com/Dao-AILab/flash-attention/releases):
+>
+> ```shell
+> export FLASH_ATTN_VER=2.5.8 # check latest version at https://github.com/Dao-AILab/flash-attention/releases
+> export CUDA_VER="cu122"     # check available ones at https://github.com/Dao-AILab/flash-attention/releases
+> export TORCH_VER=$(python -c "import torch; print('.'.join(torch.__version__.split('.')[:2]))")
+> export PY_VER=$(python -c "import platform; print(''.join(platform.python_version().split('.')[:2]))")
+> export OS_ARCH=$(python -c "import platform; print(f'{platform.system().lower()}_{platform.machine()}')")
+>
+> export WHEEL=flash_attn-${FLASH_ATTN_VER}+${CUDA_VER}torch${TORCH_VER}cxx11abiFALSE-cp${PY_VER}-cp${PY_VER}-${OS_ARCH}.whl
+> wget https://github.com/Dao-AILab/flash-attention/releases/download/v${FLASH_ATTN_VER}/${WHEEL}
+> pip install ${WHEEL}
+> ```
+
+</div>
+</details>
+
 ### Google Generative AI API (Gemini)
 
 ```bash
 repoqa.search_needle_function --model "gemini-1.5-pro-latest" --backend google
 ```
 
 ### CLI Usage
```

### Comparing `repoqa-0.1.1/docs/curate_dataset.md` & `repoqa-0.1.2/docs/curate_dataset.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/docs/dev_note.md` & `repoqa-0.1.2/docs/dev_note.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/compute_score.py` & `repoqa-0.1.2/repoqa/compute_score.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/data.py` & `repoqa-0.1.2/repoqa/data.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/metric.py` & `repoqa-0.1.2/repoqa/metric.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/anthropic.py` & `repoqa-0.1.2/repoqa/provider/anthropic.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/google.py` & `repoqa-0.1.2/repoqa/provider/google.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/hf.py` & `repoqa-0.1.2/repoqa/provider/hf.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 from repoqa.provider.base import BaseProvider
 from repoqa.provider.request import construct_message_list, hacky_assistant_stop_seq
 
 
 class HfProvider(BaseProvider):
     def __init__(self, model, trust_remote_code=False, attn_implementation=None):
-        self.tokenizer = AutoTokenizer.from_pretrained(model)
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            model, trust_remote_code=trust_remote_code
+        )
         self.hf_model = AutoModelForCausalLM.from_pretrained(
             model,
             trust_remote_code=trust_remote_code,
             attn_implementation=attn_implementation,
             torch_dtype="auto",
         ).cuda()
         self.stop_sequencer = StopSequencer(
```

### Comparing `repoqa-0.1.1/repoqa/provider/openai.py` & `repoqa-0.1.2/repoqa/provider/openai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/request/__init__.py` & `repoqa-0.1.2/repoqa/provider/request/__init__.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/request/anthropic.py` & `repoqa-0.1.2/repoqa/provider/request/anthropic.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/request/google.py` & `repoqa-0.1.2/repoqa/provider/request/google.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/request/openai.py` & `repoqa-0.1.2/repoqa/provider/request/openai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/provider/vllm.py` & `repoqa-0.1.2/repoqa/provider/vllm.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from repoqa.provider.request import construct_message_list, hacky_assistant_stop_seq
 
 
 class VllmProvider(BaseProvider):
     def __init__(
         self, model, tensor_parallel_size, max_model_len=None, trust_remote_code=False
     ):
-        self.tokenizer = AutoTokenizer.from_pretrained(model)
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            model, trust_remote_code=trust_remote_code
+        )
         self.llm = LLM(
             model=model,
             tensor_parallel_size=tensor_parallel_size,
             max_model_len=max_model_len,
             trust_remote_code=trust_remote_code,
         )
         self.stop_seq = []
```

### Comparing `repoqa-0.1.1/repoqa/search_needle_function.py` & `repoqa-0.1.2/repoqa/search_needle_function.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa/utility.py` & `repoqa-0.1.2/repoqa/utility.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/repoqa.egg-info/PKG-INFO` & `repoqa-0.1.2/repoqa.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: repoqa
-Version: 0.1.1
+Version: 0.1.2
 Summary: "RepoQA for Evaluating Long-Context Code Understanding"
 Home-page: https://github.com/evalplus/repoqa
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tempdir>=0.7.1
 Requires-Dist: appdirs>=1.4.4
+Requires-Dist: wget>=3.2
 Requires-Dist: fire>=0.6.0
 Requires-Dist: nltk>=3.8.1
 Requires-Dist: rich>=13.5.2
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: tree_sitter_languages>=1.10.2
 Requires-Dist: transformers>=4.40.0
 Requires-Dist: openai>=1.23.2
@@ -61,28 +62,34 @@
 ```
 
 </div>
 </details>
 
 ## 🏁 Search Needle Function (SNF)
 
-Search Needle Function is the first RepoQA task which aims to practice LLMs' ability of **long-context code understanding and retrieval**.
-Its corresponding real-life application is to perform precise code search from user intent rather than simple keyword match.
+Search Needle Function is the first and base RepoQA task which aims to practice LLMs' ability of **long-context code understanding and retrieval**.
+Its corresponding real-life scenario is to perform precise code search from function description.
 
-> [!Important]
+<details><summary>🔎 More dataset details <i>:: click to expand ::</i></summary>
+<div>
+
+> [!Note]
 >
-> SNF includes 500 tests (5 programming languages x 10 repositories x 10 needle functions) where an LLM is given:
+> SNF includes 500 tests (5 programming languages x 10 repos x 10 needle functions) where an LLM is given:
 >
 > 1. A large code context sorted in file dependency
 > 2. A NL description of the needle function without revealing keywords like function names
 > 3. An instruction to retrieve the described function
 >
 > The evaluator passes a test if the searched function is syntactically closest to the ground-truth compared against
 > other functions (systematically parsed by `treesitter`) and the similarity is greater than a user defined threshold (by default 0.8).
 
+</div>
+</details>
+
 You can run the SNF evaluation using various backends:
 
 ### OpenAI Compatible Servers
 
 ```bash
 repoqa.search_needle_function --model "gpt4-turbo" --backend openai
 # 💡 If you use openai API compatible server such as vLLM servers:
@@ -98,38 +105,70 @@
 
 ### vLLM
 
 ```bash
 repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --backend vllm
 ```
 
-> [!Tip]
->
-> You can unlock the model's context using [dynamic RoPE scaling](https://blog.eleuther.ai/yarn/#dynamic-scaling).
-> For example, `Meta-Llama-3-8B-Instruct` has 8k context but running the default 16k test needs more (approx. 20k).
+<details><summary>🔎 Context extension for small-ctx models <i>:: click to expand ::</i></summary>
+<div>
+
+> There are two ways to unlock a model's context at inference time:
 >
-> To extend the context to 32k, in its config file (`hub/models--meta-llama--Meta-Llama-3-8B-Instruct/snapshots/[hash]/config.json`) set:
+> 1. **Direct Extension**: Edit `max_positional_embedding` of the model's `config.json` (e.g., `hub/models--meta-llama--Meta-Llama-3-8B-Instruct/snapshots/[hash]/config.json`) to something like `22528`.
+> 2. **[Dynamic RoPE Scaling](https://blog.eleuther.ai/yarn/#dynamic-scaling)**:
+>    To extend `Meta-Llama-3-8B-Instruct` from 8k to 32k (4x), edit the `config.json`:
 >
 > `"rope_scaling": {"type": "dynamic", "factor": 4.0}`
 >
 > Note: This works for vLLM `<0.4.3` and HuggingFace transformers. RepoQA will automatically configure dynamic RoPE for vLLM `>= 0.4.3`
 
+</div>
+</details>
+
 > [!Note]
 >
 > Reference evaluation time:
 >
 > - Llama3-8B-Instruct: 45 minutes on 2xA6000 (PCIe NVLink)
 > - Llama3-70B-Instruct: 100 minutes on 4xA100 (PCIe NVLink)
 
 ### HuggingFace transformers
 
 ```bash
 repoqa.search_needle_function --model "Qwen/CodeQwen1.5-7B-Chat" --backend hf --trust-remote-code
 ```
 
+> [!Tip]
+>
+> Installing [flash-attn](https://github.com/Dao-AILab/flash-attention) and
+> additionally set `--attn-implementation "flash_attention_2"` can largely
+> lower the memory requirement.
+
+<details><summary>🔨 Having trouble installing `flash-attn`? <i>:: click to expand ::</i></summary>
+<div>
+
+> If you have trouble with `pip install flash-attn --no-build-isolation`,
+> you can try to directly use [pre-built wheels](https://github.com/Dao-AILab/flash-attention/releases):
+>
+> ```shell
+> export FLASH_ATTN_VER=2.5.8 # check latest version at https://github.com/Dao-AILab/flash-attention/releases
+> export CUDA_VER="cu122"     # check available ones at https://github.com/Dao-AILab/flash-attention/releases
+> export TORCH_VER=$(python -c "import torch; print('.'.join(torch.__version__.split('.')[:2]))")
+> export PY_VER=$(python -c "import platform; print(''.join(platform.python_version().split('.')[:2]))")
+> export OS_ARCH=$(python -c "import platform; print(f'{platform.system().lower()}_{platform.machine()}')")
+>
+> export WHEEL=flash_attn-${FLASH_ATTN_VER}+${CUDA_VER}torch${TORCH_VER}cxx11abiFALSE-cp${PY_VER}-cp${PY_VER}-${OS_ARCH}.whl
+> wget https://github.com/Dao-AILab/flash-attention/releases/download/v${FLASH_ATTN_VER}/${WHEEL}
+> pip install ${WHEEL}
+> ```
+
+</div>
+</details>
+
 ### Google Generative AI API (Gemini)
 
 ```bash
 repoqa.search_needle_function --model "gemini-1.5-pro-latest" --backend google
 ```
 
 ### CLI Usage
```

### Comparing `repoqa-0.1.1/repoqa.egg-info/SOURCES.txt` & `repoqa-0.1.2/repoqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/results/README.md` & `repoqa-0.1.2/results/README.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/cherrypick/README.md` & `repoqa-0.1.2/scripts/cherrypick/README.md`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/cherrypick/lists.json` & `repoqa-0.1.2/scripts/cherrypick/lists.json`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dataset_ensemble_clone.py` & `repoqa-0.1.2/scripts/curate/dataset_ensemble_clone.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dataset_ensemble_gh_api.py` & `repoqa-0.1.2/scripts/curate/dataset_ensemble_gh_api.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/cpp.py` & `repoqa-0.1.2/scripts/curate/dep_analysis/cpp.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/go-analysis/dependency_analysis.go` & `repoqa-0.1.2/scripts/curate/dep_analysis/go-analysis/dependency_analysis.go`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/go.py` & `repoqa-0.1.2/scripts/curate/dep_analysis/go.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml` & `repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/dependency-reduced-pom.xml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar` & `repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/java-lib/java-analysis-1.0-SNAPSHOT.jar`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/pom.xml` & `repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/pom.xml`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java` & `repoqa-0.1.2/scripts/curate/dep_analysis/java-analysis/src/main/java/edu/cs/illinois/repoqa/DepAnalyze.java`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/java.py` & `repoqa-0.1.2/scripts/curate/dep_analysis/java.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/python.py` & `repoqa-0.1.2/scripts/curate/dep_analysis/python.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/rust.py` & `repoqa-0.1.2/scripts/curate/dep_analysis/rust.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/dep_analysis/typescript.py` & `repoqa-0.1.2/scripts/curate/dep_analysis/typescript.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/function_analysis.py` & `repoqa-0.1.2/scripts/curate/function_analysis.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/github_fetch.py` & `repoqa-0.1.2/scripts/curate/github_fetch.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/merge_annotation.py` & `repoqa-0.1.2/scripts/curate/merge_annotation.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/merge_dep.py` & `repoqa-0.1.2/scripts/curate/merge_dep.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/needle_annotation.py` & `repoqa-0.1.2/scripts/curate/needle_annotation.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/needle_selection.py` & `repoqa-0.1.2/scripts/curate/needle_selection.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/curate/obfuscate_nl.py` & `repoqa-0.1.2/scripts/curate/obfuscate_nl.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/demos/model_request_oai.py` & `repoqa-0.1.2/scripts/demos/model_request_oai.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/misc/estimate_max_char.py` & `repoqa-0.1.2/scripts/misc/estimate_max_char.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/scripts/misc/repo_token_size.py` & `repoqa-0.1.2/scripts/misc/repo_token_size.py`

 * *Files identical despite different names*

### Comparing `repoqa-0.1.1/setup.cfg` & `repoqa-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 [options]
 packages = find:
 python_requires = >=3.8
 dependency_links = 
 install_requires = 
 	tempdir>=0.7.1
 	appdirs>=1.4.4
+	wget>=3.2
 	fire>=0.6.0
 	nltk>=3.8.1
 	rich>=13.5.2
 	numpy>=1.25.2
 	tree_sitter_languages>=1.10.2
 	transformers>=4.40.0
 	openai>=1.23.2
```

