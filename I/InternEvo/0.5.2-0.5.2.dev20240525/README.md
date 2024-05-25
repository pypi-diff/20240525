# Comparing `tmp/InternEvo-0.5.2.tar.gz` & `tmp/InternEvo-0.5.2.dev20240525.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternEvo-0.5.2.tar", last modified: Mon May 13 03:46:12 2024, max compression
+gzip compressed data, was "InternEvo-0.5.2.dev20240525.tar", last modified: Sat May 25 12:50:03 2024, max compression
```

## Comparing `InternEvo-0.5.2.tar` & `InternEvo-0.5.2.dev20240525.tar`

### file list

```diff
@@ -1,179 +1,186 @@
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:12.030272 InternEvo-0.5.2/
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:10.965394 InternEvo-0.5.2/InternEvo.egg-info/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5169 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4864 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/SOURCES.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/dependency_links.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      178 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/requires.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-13 03:46:10.000000 InternEvo-0.5.2/InternEvo.egg-info/top_level.txt
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-17 04:37:11.000000 InternEvo-0.5.2/LICENSE
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5169 2024-05-13 03:46:12.167481 InternEvo-0.5.2/PKG-INFO
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-22 07:03:00.000000 InternEvo-0.5.2/README.md
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:10.975908 InternEvo-0.5.2/internlm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:33.000000 InternEvo-0.5.2/internlm/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.018832 InternEvo-0.5.2/internlm/accelerator/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/abstract_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/cuda_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/dipu_accelerator.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/accelerator/npu_accelerator.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.040834 InternEvo-0.5.2/internlm/apis/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/internlm/apis/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-01-18 05:06:05.000000 InternEvo-0.5.2/internlm/apis/inference.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.093571 InternEvo-0.5.2/internlm/checkpoint/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/checkpoint/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:15.000000 InternEvo-0.5.2/internlm/checkpoint/checkpoint_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:58.000000 InternEvo-0.5.2/internlm/checkpoint/components.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14172 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/checkpoint/load_funcs.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:31.000000 InternEvo-0.5.2/internlm/checkpoint/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.130052 InternEvo-0.5.2/internlm/core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-17 04:37:12.000000 InternEvo-0.5.2/internlm/core/__init__.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.162033 InternEvo-0.5.2/internlm/core/context/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/core/context/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/core/context/parallel_context.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/core/context/process_group_initializer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/core/context/random.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/core/engine.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/core/gradient_handler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8456 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/naive_amp.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.176696 InternEvo-0.5.2/internlm/core/parallel/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:36.000000 InternEvo-0.5.2/internlm/core/parallel/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3810 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/parallel/shard.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.203598 InternEvo-0.5.2/internlm/core/scheduler/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-06 04:29:21.000000 InternEvo-0.5.2/internlm/core/scheduler/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-04-25 06:33:10.000000 InternEvo-0.5.2/internlm/core/scheduler/base_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.234384 InternEvo-0.5.2/internlm/core/scheduler/comm/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/comm/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/comm/p2p.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4958 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/comm/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8882 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/core/scheduler/no_pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63810 2024-05-11 06:37:47.000000 InternEvo-0.5.2/internlm/core/scheduler/pipeline_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7598 2024-04-19 04:15:43.000000 InternEvo-0.5.2/internlm/core/trainer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.268831 InternEvo-0.5.2/internlm/data/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-04-11 07:24:57.000000 InternEvo-0.5.2/internlm/data/build_dataloader.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.325172 InternEvo-0.5.2/internlm/data/tokenized/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:25.000000 InternEvo-0.5.2/internlm/data/tokenized/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/tokenized/batch_sampler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:49:50.000000 InternEvo-0.5.2/internlm/data/tokenized/collaters.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/tokenized/dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:49:50.000000 InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset_multimodal.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 12:29:02.000000 InternEvo-0.5.2/internlm/data/tokenized/packed_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/tokenized/single_dataset.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/data/train_state.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2546 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/data/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.344261 InternEvo-0.5.2/internlm/eval/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/eval/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:33:26.000000 InternEvo-0.5.2/internlm/eval/evaluation.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.375831 InternEvo-0.5.2/internlm/initialize/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-18 05:06:05.000000 InternEvo-0.5.2/internlm/initialize/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-17 04:37:12.000000 InternEvo-0.5.2/internlm/initialize/initialize_tensor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5934 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/initialize/initialize_trainer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27583 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/initialize/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.393144 InternEvo-0.5.2/internlm/initialize/legacy/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/internlm/initialize/legacy/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/initialize/legacy/launch.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.455857 InternEvo-0.5.2/internlm/model/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.2/internlm/model/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1354 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.484054 InternEvo-0.5.2/internlm/model/llava/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.2/internlm/model/llava/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/llava/clip_builder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/llava/clip_encoder.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/llava/projector_builder.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.502303 InternEvo-0.5.2/internlm/model/losses/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 03:23:14.000000 InternEvo-0.5.2/internlm/model/losses/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1716 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/losses/ce_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16875 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/metrics.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15915 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_internlm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21691 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_internlm2.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20973 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_llama.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10481 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_llava.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17537 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modeling_moe.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.550424 InternEvo-0.5.2/internlm/model/modules/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 03:21:42.000000 InternEvo-0.5.2/internlm/model/modules/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13791 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/embedding.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21583 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27792 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/mha.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4613 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      424 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3277 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/modules/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.586775 InternEvo-0.5.2/internlm/model/moe/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-10 09:03:37.000000 InternEvo-0.5.2/internlm/model/moe/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/model/moe/base_layer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/model/moe/experts.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20335 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/gshard_layer.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.618307 InternEvo-0.5.2/internlm/model/moe/megablock/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:21.000000 InternEvo-0.5.2/internlm/model/moe/megablock/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8669 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/megablock_dmoe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13597 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/megablock_moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2563 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/mlp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11288 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/megablock/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4848 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/moe/moe.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:13.000000 InternEvo-0.5.2/internlm/model/moe/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.662252 InternEvo-0.5.2/internlm/model/ops/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 03:21:42.000000 InternEvo-0.5.2/internlm/model/ops/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    33645 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/attention.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2084 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/cross_entropy.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2400 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/linear.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2489 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/norm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5346 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/rotary_emb.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1670 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/ops/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2952 2024-05-10 09:05:35.000000 InternEvo-0.5.2/internlm/model/registry.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      883 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/model/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.688618 InternEvo-0.5.2/internlm/monitor/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/alert.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/monitor.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/monitor/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.701011 InternEvo-0.5.2/internlm/solver/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/solver/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/solver/activation_checkpoint.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.770758 InternEvo-0.5.2/internlm/solver/optimizer/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:26.000000 InternEvo-0.5.2/internlm/solver/optimizer/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-18 05:06:05.000000 InternEvo-0.5.2/internlm/solver/optimizer/base_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1946 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/solver/optimizer/compatible_adamw.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 09:32:05.000000 InternEvo-0.5.2/internlm/solver/optimizer/fsdp_optimizer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42554 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/solver/optimizer/hybrid_zero_optim.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 09:32:05.000000 InternEvo-0.5.2/internlm/solver/optimizer/store.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:12.000000 InternEvo-0.5.2/internlm/solver/optimizer/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.794767 InternEvo-0.5.2/internlm/solver/schedulers/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/solver/schedulers/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:42:40.000000 InternEvo-0.5.2/internlm/solver/schedulers/beta2_scheduler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/solver/schedulers/lr_scheduler.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.822875 InternEvo-0.5.2/internlm/train/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      601 2024-05-11 06:37:47.000000 InternEvo-0.5.2/internlm/train/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26101 2024-05-11 07:01:18.000000 InternEvo-0.5.2/internlm/train/pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3575 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/train/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.894858 InternEvo-0.5.2/internlm/utils/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/internlm/utils/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7964 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/utils/common.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/gputest.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:15:50.000000 InternEvo-0.5.2/internlm/utils/logger.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/megatron_timers.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3953 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/utils/parallel.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:42:40.000000 InternEvo-0.5.2/internlm/utils/simple_memory_profiler.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/storage_manager.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 03:23:15.000000 InternEvo-0.5.2/internlm/utils/timeout.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4032 2024-05-10 09:05:36.000000 InternEvo-0.5.2/internlm/utils/utils.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 04:30:38.000000 InternEvo-0.5.2/internlm/utils/writer.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-13 03:46:12.170532 InternEvo-0.5.2/setup.cfg
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1235 2024-05-13 03:04:28.000000 InternEvo-0.5.2/setup.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.906807 InternEvo-0.5.2/tests/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-17 04:36:06.000000 InternEvo-0.5.2/tests/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4526 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/common_fixture.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:11.931278 InternEvo-0.5.2/tests/test_core/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.5.2/tests/test_core/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5841 2024-04-23 01:33:18.000000 InternEvo-0.5.2/tests/test_core/test_pipeline.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6968 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_core/utils.py
-drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-13 03:44:12.020983 InternEvo-0.5.2/tests/test_training/
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:58.000000 InternEvo-0.5.2/tests/test_training/7B_check_acc.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 04:30:38.000000 InternEvo-0.5.2/tests/test_training/7B_check_init.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-18 05:04:59.000000 InternEvo-0.5.2/tests/test_training/__init__.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8054 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_forward_output_no_fa.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11809 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_load_ckpt_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14426 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_loss.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3855 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_no_fa_train_temp.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6773 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_norm_weight.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12656 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/test_swap_nb_loss_and_gradnorm.py
--rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14290 2024-05-10 09:05:36.000000 InternEvo-0.5.2/tests/test_training/train_CI.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.268741 InternEvo-0.5.2.dev20240525/
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.205669 InternEvo-0.5.2.dev20240525/InternEvo.egg-info/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5181 2024-05-25 12:50:01.000000 InternEvo-0.5.2.dev20240525/InternEvo.egg-info/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5095 2024-05-25 12:50:01.000000 InternEvo-0.5.2.dev20240525/InternEvo.egg-info/SOURCES.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        1 2024-05-25 12:50:01.000000 InternEvo-0.5.2.dev20240525/InternEvo.egg-info/dependency_links.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      178 2024-05-25 12:50:01.000000 InternEvo-0.5.2.dev20240525/InternEvo.egg-info/requires.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       15 2024-05-25 12:50:01.000000 InternEvo-0.5.2.dev20240525/InternEvo.egg-info/top_level.txt
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13656 2024-01-25 08:28:54.000000 InternEvo-0.5.2.dev20240525/LICENSE
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5181 2024-05-25 12:50:03.480220 InternEvo-0.5.2.dev20240525/PKG-INFO
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4730 2024-01-25 08:28:54.000000 InternEvo-0.5.2.dev20240525/README.md
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.211274 InternEvo-0.5.2.dev20240525/internlm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      267 2024-01-30 08:18:31.000000 InternEvo-0.5.2.dev20240525/internlm/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.252922 InternEvo-0.5.2.dev20240525/internlm/accelerator/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      147 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/accelerator/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4017 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/accelerator/abstract_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11010 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/accelerator/cuda_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11446 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/accelerator/dipu_accelerator.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10866 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/accelerator/npu_accelerator.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.268627 InternEvo-0.5.2.dev20240525/internlm/apis/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-23 09:20:08.000000 InternEvo-0.5.2.dev20240525/internlm/apis/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    37532 2024-05-23 09:22:13.000000 InternEvo-0.5.2.dev20240525/internlm/apis/inference.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.309159 InternEvo-0.5.2.dev20240525/internlm/checkpoint/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       83 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/checkpoint/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27404 2024-04-17 07:54:31.000000 InternEvo-0.5.2.dev20240525/internlm/checkpoint/checkpoint_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20076 2024-04-12 05:43:59.000000 InternEvo-0.5.2.dev20240525/internlm/checkpoint/components.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14172 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/checkpoint/load_funcs.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2474 2024-04-10 07:31:30.000000 InternEvo-0.5.2.dev20240525/internlm/checkpoint/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.352033 InternEvo-0.5.2.dev20240525/internlm/core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      158 2024-01-25 08:28:55.000000 InternEvo-0.5.2.dev20240525/internlm/core/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.390538 InternEvo-0.5.2.dev20240525/internlm/core/context/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1220 2024-03-18 08:30:10.000000 InternEvo-0.5.2.dev20240525/internlm/core/context/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27076 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/core/context/parallel_context.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    38371 2024-03-18 08:30:10.000000 InternEvo-0.5.2.dev20240525/internlm/core/context/process_group_initializer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4295 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/core/context/random.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7458 2024-05-23 09:22:13.000000 InternEvo-0.5.2.dev20240525/internlm/core/engine.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3113 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/core/gradient_handler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8456 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/naive_amp.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.402976 InternEvo-0.5.2.dev20240525/internlm/core/parallel/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-22 08:32:53.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/__init__.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.440417 InternEvo-0.5.2.dev20240525/internlm/core/parallel/comm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-24 18:56:36.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/comm/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    31942 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/comm/isp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13358 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/comm/tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6676 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/comm/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5102 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/comm/zero.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3810 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/parallel/shard.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.468331 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      303 2024-02-08 03:13:39.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5258 2024-05-23 09:22:13.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/base_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.496046 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      884 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22670 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/p2p.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4958 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8882 2024-05-23 09:22:13.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/no_pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    63472 2024-05-23 09:22:13.000000 InternEvo-0.5.2.dev20240525/internlm/core/scheduler/pipeline_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7600 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/core/trainer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.526321 InternEvo-0.5.2.dev20240525/internlm/data/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      209 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/data/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6991 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/data/build_dataloader.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.587267 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      418 2024-03-22 07:04:00.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    15158 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/batch_sampler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4401 2024-04-10 08:53:30.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/collaters.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1714 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1406 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/dummy_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1894 2024-04-10 08:53:30.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/dummy_dataset_multimodal.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22498 2024-04-10 13:25:54.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/packed_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3740 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/data/tokenized/single_dataset.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      454 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/data/train_state.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2546 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/data/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.603121 InternEvo-0.5.2.dev20240525/internlm/eval/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       86 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/eval/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4999 2024-04-11 02:31:26.000000 InternEvo-0.5.2.dev20240525/internlm/eval/evaluation.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.629867 InternEvo-0.5.2.dev20240525/internlm/initialize/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      368 2024-01-25 08:28:55.000000 InternEvo-0.5.2.dev20240525/internlm/initialize/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1793 2024-01-25 08:28:55.000000 InternEvo-0.5.2.dev20240525/internlm/initialize/initialize_tensor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5934 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/initialize/initialize_trainer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27583 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/initialize/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.645133 InternEvo-0.5.2.dev20240525/internlm/initialize/legacy/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.2.dev20240525/internlm/initialize/legacy/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1592 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/initialize/legacy/launch.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.711067 InternEvo-0.5.2.dev20240525/internlm/model/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-22 08:32:53.000000 InternEvo-0.5.2.dev20240525/internlm/model/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1354 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.737976 InternEvo-0.5.2.dev20240525/internlm/model/llava/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-22 08:32:53.000000 InternEvo-0.5.2.dev20240525/internlm/model/llava/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      499 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/llava/clip_builder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2674 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/llava/clip_encoder.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1407 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/llava/projector_builder.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.756366 InternEvo-0.5.2.dev20240525/internlm/model/losses/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       73 2024-03-15 18:58:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/losses/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1716 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/losses/ce_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16875 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/metrics.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    16199 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modeling_internlm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    22009 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modeling_internlm2.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21291 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modeling_llama.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10481 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modeling_llava.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    17821 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modeling_moe.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.811332 InternEvo-0.5.2.dev20240525/internlm/model/modules/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13791 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/embedding.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    21578 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    27857 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/mha.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4613 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      424 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3277 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/modules/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.850790 InternEvo-0.5.2.dev20240525/internlm/model/moe/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-22 08:32:53.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1198 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/base_layer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2762 2024-03-18 08:30:10.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/experts.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20335 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/gshard_layer.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.892709 InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-04-17 08:44:20.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8835 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/megablock_dmoe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    13747 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/megablock_moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2641 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/mlp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11288 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4848 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/moe.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2021 2024-03-18 08:30:10.000000 InternEvo-0.5.2.dev20240525/internlm/model/moe/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.943591 InternEvo-0.5.2.dev20240525/internlm/model/ops/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-03-15 18:57:26.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    33645 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/attention.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2084 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/cross_entropy.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2400 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/linear.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3722 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/norm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10216 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/rotary_emb.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1670 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/ops/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2952 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/registry.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2141 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/model/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.971626 InternEvo-0.5.2.dev20240525/internlm/monitor/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      193 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/monitor/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1479 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/monitor/alert.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10213 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/monitor/monitor.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      776 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/monitor/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:56.986396 InternEvo-0.5.2.dev20240525/internlm/solver/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-15 18:58:59.000000 InternEvo-0.5.2.dev20240525/internlm/solver/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10095 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/solver/activation_checkpoint.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.043264 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      252 2024-03-22 07:04:01.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1080 2024-01-25 08:28:55.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/base_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1946 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/compatible_adamw.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     9173 2024-03-22 08:39:35.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/fsdp_optimizer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    42554 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/hybrid_zero_optim.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4901 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/npu_fused_adamw.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    10132 2024-03-22 08:39:35.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/store.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    20351 2024-04-08 13:12:08.000000 InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.064155 InternEvo-0.5.2.dev20240525/internlm/solver/schedulers/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      272 2024-03-15 18:58:59.000000 InternEvo-0.5.2.dev20240525/internlm/solver/schedulers/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      844 2024-03-26 03:26:29.000000 InternEvo-0.5.2.dev20240525/internlm/solver/schedulers/beta2_scheduler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5940 2024-03-15 18:58:59.000000 InternEvo-0.5.2.dev20240525/internlm/solver/schedulers/lr_scheduler.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.086299 InternEvo-0.5.2.dev20240525/internlm/train/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)      601 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/train/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    26151 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/train/pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3575 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/train/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.158481 InternEvo-0.5.2.dev20240525/internlm/utils/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.2.dev20240525/internlm/utils/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7964 2024-05-23 09:22:14.000000 InternEvo-0.5.2.dev20240525/internlm/utils/common.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6321 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/utils/gputest.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     2112 2024-04-10 11:16:15.000000 InternEvo-0.5.2.dev20240525/internlm/utils/logger.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4156 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/utils/megatron_timers.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3953 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/internlm/utils/parallel.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    24734 2024-03-26 03:26:29.000000 InternEvo-0.5.2.dev20240525/internlm/utils/simple_memory_profiler.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    46133 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/utils/storage_manager.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3126 2024-03-15 18:58:59.000000 InternEvo-0.5.2.dev20240525/internlm/utils/timeout.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4043 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/internlm/utils/utils.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     7117 2024-04-07 02:41:24.000000 InternEvo-0.5.2.dev20240525/internlm/utils/writer.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)       38 2024-05-25 12:50:03.483506 InternEvo-0.5.2.dev20240525/setup.cfg
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     1235 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/setup.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.171060 InternEvo-0.5.2.dev20240525/tests/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.2.dev20240525/tests/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     4526 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/common_fixture.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.192092 InternEvo-0.5.2.dev20240525/tests/test_core/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:45.000000 InternEvo-0.5.2.dev20240525/tests/test_core/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5552 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/tests/test_core/test_pipeline.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6968 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_core/utils.py
+drwxrwxr-x   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-05-25 12:47:57.257808 InternEvo-0.5.2.dev20240525/tests/test_training/
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     5750 2024-04-12 05:43:59.000000 InternEvo-0.5.2.dev20240525/tests/test_training/7B_check_acc.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6360 2024-04-07 02:41:25.000000 InternEvo-0.5.2.dev20240525/tests/test_training/7B_check_init.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)        0 2024-01-25 08:27:46.000000 InternEvo-0.5.2.dev20240525/tests/test_training/__init__.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     8054 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_training/test_forward_output_no_fa.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    11809 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_training/test_load_ckpt_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14426 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_training/test_loss.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     3855 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_training/test_no_fa_train_temp.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)     6773 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_training/test_norm_weight.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    12656 2024-05-22 08:34:58.000000 InternEvo-0.5.2.dev20240525/tests/test_training/test_swap_nb_loss_and_gradnorm.py
+-rw-rw-r--   0 qa-caif-cicd (700000024) qa-caif-cicd (700000024)    14382 2024-05-24 18:58:42.000000 InternEvo-0.5.2.dev20240525/tests/test_training/train_CI.py
```

### Comparing `InternEvo-0.5.2/InternEvo.egg-info/PKG-INFO` & `InternEvo-0.5.2.dev20240525/InternEvo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.5.2
+Version: 0.5.2.dev20240525
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.5.2 Summary: an open-sourced
-lightweight training framework aims to support model pre-training without the
-need for extensive dependencies Classifier: Programming Language :: Python ::
-3.10 Classifier: Intended Audience :: Developers Classifier: Intended Audience
-:: Education Classifier: Intended Audience :: Science/Research Description-
-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.5.2.dev20240525 Summary: an
+open-sourced lightweight training framework aims to support model pre-training
+without the need for extensive dependencies Classifier: Programming Language ::
+Python :: 3.10 Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Education Classifier: Intended Audience :: Science/Research
+Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.5.2/InternEvo.egg-info/SOURCES.txt` & `InternEvo-0.5.2.dev20240525/InternEvo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 internlm/core/trainer.py
 internlm/core/context/__init__.py
 internlm/core/context/parallel_context.py
 internlm/core/context/process_group_initializer.py
 internlm/core/context/random.py
 internlm/core/parallel/__init__.py
 internlm/core/parallel/shard.py
+internlm/core/parallel/comm/__init__.py
+internlm/core/parallel/comm/isp.py
+internlm/core/parallel/comm/tensor.py
+internlm/core/parallel/comm/utils.py
+internlm/core/parallel/comm/zero.py
 internlm/core/scheduler/__init__.py
 internlm/core/scheduler/base_scheduler.py
 internlm/core/scheduler/no_pipeline_scheduler.py
 internlm/core/scheduler/pipeline_scheduler.py
 internlm/core/scheduler/comm/__init__.py
 internlm/core/scheduler/comm/p2p.py
 internlm/core/scheduler/comm/utils.py
@@ -105,14 +110,15 @@
 internlm/solver/__init__.py
 internlm/solver/activation_checkpoint.py
 internlm/solver/optimizer/__init__.py
 internlm/solver/optimizer/base_optimizer.py
 internlm/solver/optimizer/compatible_adamw.py
 internlm/solver/optimizer/fsdp_optimizer.py
 internlm/solver/optimizer/hybrid_zero_optim.py
+internlm/solver/optimizer/npu_fused_adamw.py
 internlm/solver/optimizer/store.py
 internlm/solver/optimizer/utils.py
 internlm/solver/schedulers/__init__.py
 internlm/solver/schedulers/beta2_scheduler.py
 internlm/solver/schedulers/lr_scheduler.py
 internlm/train/__init__.py
 internlm/train/pipeline.py
```

### Comparing `InternEvo-0.5.2/LICENSE` & `InternEvo-0.5.2.dev20240525/LICENSE`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/PKG-INFO` & `InternEvo-0.5.2.dev20240525/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternEvo
-Version: 0.5.2
+Version: 0.5.2.dev20240525
 Summary: an open-sourced lightweight training framework aims to support model pre-training without the need for extensive dependencies
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: InternEvo Version: 0.5.2 Summary: an open-sourced
-lightweight training framework aims to support model pre-training without the
-need for extensive dependencies Classifier: Programming Language :: Python ::
-3.10 Classifier: Intended Audience :: Developers Classifier: Intended Audience
-:: Education Classifier: Intended Audience :: Science/Research Description-
-Content-Type: text/markdown License-File: LICENSE # InternEvo
+Metadata-Version: 2.1 Name: InternEvo Version: 0.5.2.dev20240525 Summary: an
+open-sourced lightweight training framework aims to support model pre-training
+without the need for extensive dependencies Classifier: Programming Language ::
+Python :: 3.10 Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Education Classifier: Intended Audience :: Science/Research
+Description-Content-Type: text/markdown License-File: LICENSE # InternEvo
                              [./doc/imgs/logo.svg]
                                       Â 
                                  IInntteerrnnEEvvoo _H_O_T
                                       Â 
   [![Documentation Status](https://readthedocs.org/projects/internevo/badge/
 ?version=latest)](https://internevo.readthedocs.io/zh_CN/latest/?badge=latest)
 [![license](./doc/imgs/license.svg)](./LICENSE) [ðUsage](./doc/en/usage.md)
```

### Comparing `InternEvo-0.5.2/README.md` & `InternEvo-0.5.2.dev20240525/README.md`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/accelerator/abstract_accelerator.py` & `InternEvo-0.5.2.dev20240525/internlm/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/accelerator/cuda_accelerator.py` & `InternEvo-0.5.2.dev20240525/internlm/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/accelerator/dipu_accelerator.py` & `InternEvo-0.5.2.dev20240525/internlm/accelerator/dipu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/accelerator/npu_accelerator.py` & `InternEvo-0.5.2.dev20240525/internlm/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/apis/inference.py` & `InternEvo-0.5.2.dev20240525/internlm/apis/inference.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/checkpoint/checkpoint_manager.py` & `InternEvo-0.5.2.dev20240525/internlm/checkpoint/checkpoint_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/checkpoint/components.py` & `InternEvo-0.5.2.dev20240525/internlm/checkpoint/components.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/checkpoint/load_funcs.py` & `InternEvo-0.5.2.dev20240525/internlm/checkpoint/load_funcs.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/checkpoint/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/context/__init__.py` & `InternEvo-0.5.2.dev20240525/internlm/core/context/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/context/parallel_context.py` & `InternEvo-0.5.2.dev20240525/internlm/core/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/context/process_group_initializer.py` & `InternEvo-0.5.2.dev20240525/internlm/core/context/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/context/random.py` & `InternEvo-0.5.2.dev20240525/internlm/core/context/random.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/engine.py` & `InternEvo-0.5.2.dev20240525/internlm/core/engine.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/gradient_handler.py` & `InternEvo-0.5.2.dev20240525/internlm/core/gradient_handler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/naive_amp.py` & `InternEvo-0.5.2.dev20240525/internlm/core/naive_amp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/parallel/shard.py` & `InternEvo-0.5.2.dev20240525/internlm/core/parallel/shard.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/scheduler/base_scheduler.py` & `InternEvo-0.5.2.dev20240525/internlm/core/scheduler/base_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/scheduler/comm/__init__.py` & `InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/scheduler/comm/p2p.py` & `InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/p2p.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/scheduler/comm/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/core/scheduler/comm/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/scheduler/no_pipeline_scheduler.py` & `InternEvo-0.5.2.dev20240525/internlm/core/scheduler/no_pipeline_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/core/scheduler/pipeline_scheduler.py` & `InternEvo-0.5.2.dev20240525/internlm/core/scheduler/pipeline_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,15 +564,15 @@
             moe_losses.append(moe_loss)
         # Before running 1F1B, need to receive first forward tensor.
         # If all microbatches are run in warmup / cooldown phase, then no need to
         # receive this tensor here.
         if num_1f1b_micropairs > 0:
             if not gpc.is_first_rank(ParallelMode.PIPELINE):
                 if forward_recv_shapes is None:
-                    forward_recv_shapes = comm.recv_obj_meta(forward_recv_shapes)
+                    forward_recv_shapes = comm.recv_obj_meta()
                 input_obj = comm.recv_forward(
                     forward_recv_shapes,
                     dtype=self.dtype,
                     scatter_gather_tensors=self.scatter_gather_tensors,
                 )
             else:
                 input_obj = None
@@ -810,23 +810,15 @@
         micro_batch_data, micro_batch_label = self._load_micro_batch(
             data=self.batch_data,
             label=self.batch_label,
             offset=self.microbatch_offset[model_chunk_id],
             bsz_stride=self.bsz_stride,
         )
         if self.data_process_func:
-            micro_batch_data["input_ids"] = self.data_process_func(
-                micro_batch_data["input_ids"], micro_batch_data["cu_seqlens"]
-            )
-            micro_batch_label = self.data_process_func(
-                micro_batch_label, micro_batch_data["cu_seqlens"], padding_v=-100
-            )
-
-            micro_batch_data.pop("cu_seqlens")
-            micro_batch_data.pop("indexes")
+            micro_batch_data, micro_batch_label = self.data_process_func(micro_batch_data, micro_batch_label)
 
         micro_batch_data["label"] = micro_batch_label
         self.microbatch_offset[model_chunk_id] += self.bsz_stride
         return move_to_device(micro_batch_data)
 
     def _forward_step(self, engine, chunk_id):
         """Forward step for passed-in model. If it is the first stage, the input tensor
@@ -966,15 +958,15 @@
             num_warmup_microsteps (int): The number of warm-up microsteps.
             receive_extra_backward (bool, optional): Whether to receive extra backward input for the 1F1B stage.
                                                      Default is False.
             forward_only (bool, optional): Whether to only perform forward pass. Default is False.
         """
         if not gpc.is_pipeline_first_stage():
             if self._input_obj_shapes[0] is None:
-                self._input_obj_shapes[0] = comm.recv_obj_meta(self._input_obj_shapes[0])
+                self._input_obj_shapes[0] = comm.recv_obj_meta()
             self._input_objs[0].append(
                 comm.recv_forward(
                     self._input_obj_shapes[0],
                     dtype=self.dtype,
                     scatter_gather_tensors=self.scatter_gather_tensors,
                 )
             )
```

### Comparing `InternEvo-0.5.2/internlm/core/trainer.py` & `InternEvo-0.5.2.dev20240525/internlm/core/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if batch_sampler:
             self.init_batch_sampler(batch_sampler)
 
         # tgs statistic
         self.tgs_statistic = {
             "sum_step": 0,
             "sum_tg": 0,
-            "sum_time": 0,
+            "total_time": 0,
             "sum_last_tg_10": 0,
             "sum_last_time_10": 0,
             "sum_last_tg_50": 0,
             "sum_last_time_50": 0,
             "SMA_tg_50": 0,
             "SMA_time_50": 0,
             "SMA_tg_50_list": deque(),
```

### Comparing `InternEvo-0.5.2/internlm/data/build_dataloader.py` & `InternEvo-0.5.2.dev20240525/internlm/data/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/batch_sampler.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/batch_sampler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/collaters.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/collaters.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/dataset.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/dummy_dataset_multimodal.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/dummy_dataset_multimodal.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/packed_dataset.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/packed_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/tokenized/single_dataset.py` & `InternEvo-0.5.2.dev20240525/internlm/data/tokenized/single_dataset.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/data/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/data/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/eval/evaluation.py` & `InternEvo-0.5.2.dev20240525/internlm/eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/initialize/initialize_tensor.py` & `InternEvo-0.5.2.dev20240525/internlm/initialize/initialize_tensor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/initialize/initialize_trainer.py` & `InternEvo-0.5.2.dev20240525/internlm/initialize/initialize_trainer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/initialize/launch.py` & `InternEvo-0.5.2.dev20240525/internlm/initialize/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/initialize/legacy/launch.py` & `InternEvo-0.5.2.dev20240525/internlm/initialize/legacy/launch.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/builder.py` & `InternEvo-0.5.2.dev20240525/internlm/model/builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/llava/clip_encoder.py` & `InternEvo-0.5.2.dev20240525/internlm/model/llava/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/llava/projector_builder.py` & `InternEvo-0.5.2.dev20240525/internlm/model/llava/projector_builder.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/losses/ce_loss.py` & `InternEvo-0.5.2.dev20240525/internlm/model/losses/ce_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/metrics.py` & `InternEvo-0.5.2.dev20240525/internlm/model/metrics.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/modeling_internlm.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modeling_internlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from internlm.initialize.initialize_tensor import normal_, scaled_init_method_normal
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import MHA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
 from internlm.model.utils import (
+    convert_attn_args_to_kwargs,
+    convert_attn_kwargs_to_args,
     internlm1_mha_pre_load_convert,
     internlm1_mha_save_convert,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
@@ -158,19 +160,21 @@
                     if self.use_scaled_init and "fc1" not in name:
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
                         normal_(std=0.006 if "fc1" in name else 0.0015)(param.data)
 
     def forward(self, hidden_states, **kwargs):
         if self.checkpoint and self.training:
-            return activation_checkpoint(self._forward, False, hidden_states, **kwargs)
+            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
+            args = convert_attn_kwargs_to_args(kwargs)
+            return activation_checkpoint(self._forward, False, hidden_states, *args)
         else:
             return self._forward(hidden_states, **kwargs)
 
-    def _forward(self, hidden_states=None, **kwargs):
+    def _forward(self, hidden_states, *args, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -186,15 +190,16 @@
             residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, hidden_states)
         else:
             residual, hidden_states = _dropout_and_norm_attn(hidden_states)
 
         if self.residual_in_fp32:
             residual = residual.to(torch.float32)
 
-        hidden_states = self.mixer(hidden_states, **kwargs)
+        mixer_kwargs = convert_attn_args_to_kwargs(args, kwargs)
+        hidden_states = self.mixer(hidden_states, **mixer_kwargs)
 
         def _dropout_and_norm_ffn(_residual, _hidden_states):
             _dropped = self.dropout2(_hidden_states)
             _residual = (_dropped + _residual) if _residual is not None else _dropped
             _hidden_states = self.norm2(_residual.float())
             return _residual, _hidden_states
```

### Comparing `InternEvo-0.5.2/internlm/model/modeling_internlm2.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modeling_internlm2.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     uniform_,
 )
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import GQA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
+from internlm.model.utils import (
+    convert_attn_args_to_kwargs,
+    convert_attn_kwargs_to_args,
+)
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
 
 
 class InternLM2Decoder(nn.Module):
@@ -193,19 +197,21 @@
                     else:
                         self.init_func(std=self.ffn_uplayer_init_std if "fc1" in name else self.ffn_other_init_std)(
                             param.data
                         )
 
     def forward(self, hidden_states, residual=None, **kwargs):
         if self.checkpoint and self.training:
-            return activation_checkpoint(self._forward, False, hidden_states, residual, **kwargs)
+            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
+            args = convert_attn_kwargs_to_args(kwargs)
+            return activation_checkpoint(self._forward, False, hidden_states, residual, *args)
         else:
             return self._forward(hidden_states, residual, **kwargs)
 
-    def _forward(self, hidden_states=None, residual=None, **kwargs):
+    def _forward(self, hidden_states, residual, *args, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -223,15 +229,16 @@
                 residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, residual, hidden_states)
             else:
                 residual, hidden_states = _dropout_and_norm_attn(residual, hidden_states)
 
             if self.residual_in_fp32:
                 residual = residual.to(torch.float32)
 
-            hidden_states = self.attention(hidden_states, **kwargs)
+            attn_kwargs = convert_attn_args_to_kwargs(args, kwargs)
+            hidden_states = self.attention(hidden_states, **attn_kwargs)
 
             if not isinstance(self.feed_forward, nn.Identity):
                 if not self.fused_dropout_add_ln:
 
                     def _dropout_and_norm_ffn(_residual, _hidden_states):
                         _dropped = self.dropout2(_hidden_states)
                         _residual = (_dropped + _residual) if _residual is not None else _dropped
```

### Comparing `InternEvo-0.5.2/internlm/model/modeling_llama.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modeling_llama.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     uniform_,
 )
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import GQA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
+from internlm.model.utils import (
+    convert_attn_args_to_kwargs,
+    convert_attn_kwargs_to_args,
+)
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
 
 
 class Llama2Decoder(nn.Module):
@@ -185,19 +189,21 @@
                     else:
                         self.init_func(std=self.ffn_uplayer_init_std if "fc1" in name else self.ffn_other_init_std)(
                             param.data
                         )
 
     def forward(self, hidden_states, residual=None, **kwargs):
         if self.checkpoint and self.training:
-            return activation_checkpoint(self._forward, False, hidden_states, residual, **kwargs)
+            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
+            args = convert_attn_kwargs_to_args(kwargs)
+            return activation_checkpoint(self._forward, False, hidden_states, residual, *args)
         else:
             return self._forward(hidden_states, residual, **kwargs)
 
-    def _forward(self, hidden_states=None, residual=None, **kwargs):
+    def _forward(self, hidden_states, residual, *args, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -215,15 +221,16 @@
                 residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, residual, hidden_states)
             else:
                 residual, hidden_states = _dropout_and_norm_attn(residual, hidden_states)
 
             if self.residual_in_fp32:
                 residual = residual.to(torch.float32)
 
-            hidden_states = self.attention(hidden_states, **kwargs)
+            attn_kwargs = convert_attn_args_to_kwargs(args, kwargs)
+            hidden_states = self.attention(hidden_states, **attn_kwargs)
 
             if not isinstance(self.feed_forward, nn.Identity):
                 if not self.fused_dropout_add_ln:
 
                     def _dropout_and_norm_ffn(_residual, _hidden_states):
                         _dropped = self.dropout2(_hidden_states)
                         _residual = (_dropped + _residual) if _residual is not None else _dropped
```

### Comparing `InternEvo-0.5.2/internlm/model/modeling_llava.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modeling_llava.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/modeling_moe.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modeling_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from internlm.model.modules.embedding import Embedding1D
 from internlm.model.modules.linear import new_linear
 from internlm.model.modules.mha import MHA
 from internlm.model.modules.mlp import new_feed_forward
 from internlm.model.modules.norm import new_layer_norm
 from internlm.model.moe.moe import MoE
 from internlm.model.utils import (
+    convert_attn_args_to_kwargs,
+    convert_attn_kwargs_to_args,
     internlm1_mha_pre_load_convert,
     internlm1_mha_save_convert,
 )
 from internlm.solver.activation_checkpoint import activation_checkpoint
 from internlm.utils.logger import get_logger
 
 logger = get_logger(__file__)
@@ -175,19 +177,21 @@
                         scaled_init_method_normal(sigma=0.006, num_layers=self.layer_idx + 1)(param.data)
                     else:
                         normal_(std=0.006 if "fc1" in name else 0.0015)(param.data)
 
     def forward(self, hidden_states, **kwargs):
         if self.checkpoint and self.training:
             # TODO: check whether this will be affected by moe
-            return activation_checkpoint(self._forward, False, hidden_states, **kwargs)
+            # NOTICE: activation_checkpiont do not support kwargs when use_reentrant = True.
+            args = convert_attn_kwargs_to_args(kwargs)
+            return activation_checkpoint(self._forward, False, hidden_states, *args)
         else:
             return self._forward(hidden_states, **kwargs)
 
-    def _forward(self, hidden_states=None, **kwargs):
+    def _forward(self, hidden_states, *args, **kwargs):
         r"""Pass the input through the encoder layer.
 
         Args:
             hidden_states: the sequence to the encoder layer (required).
             residual: hidden_states = Attn/MLP(LN(residual))
             cu_seqlens: 1d LongTensor, len(cu_seqlens) = hidden_states + 1
             indexes: the length of index is same as hidden states, which stand for the current position
@@ -203,15 +207,16 @@
             residual, hidden_states = activation_checkpoint(_dropout_and_norm_attn, False, hidden_states)
         else:
             residual, hidden_states = _dropout_and_norm_attn(hidden_states)
 
         if self.residual_in_fp32:
             residual = residual.to(torch.float32)
 
-        hidden_states = self.mixer(hidden_states, **kwargs)
+        mixer_kwargs = convert_attn_args_to_kwargs(args, kwargs)
+        hidden_states = self.mixer(hidden_states, **mixer_kwargs)
 
         def _dropout_and_norm_ffn(_residual, _hidden_states):
             _dropped = self.dropout2(_hidden_states)
             _residual = (_dropped + _residual) if _residual is not None else _dropped
             _hidden_states = self.norm2(_residual.float())
             return _residual, _hidden_states
```

### Comparing `InternEvo-0.5.2/internlm/model/modules/embedding.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/modules/linear.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modules/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,15 +488,15 @@
                     self.first_eval_flag = False
                     self.tmp_weight = nn.functional.normalize(weight)
 
                 weight = self.tmp_weight
 
         return fused_dense_func(
             input,
-            self.weight,
+            weight,
             communicator=self._communicator,
             module=self,
             bias=self.bias,
         )
 
 
 class RewardModelLinear(ScaleColumnParallelLinear):
```

### Comparing `InternEvo-0.5.2/internlm/model/modules/mha.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modules/mha.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,26 +180,30 @@
 
         cu_seqlens_q = cu_seqlens
         cu_seqlens_k = cu_seqlens
 
         max_seqlen_q = attention_mask.shape[-1]
         max_seqlen_k = attention_mask.shape[-1]
 
-        q_packed = q.masked_select(attention_mask.view(batch_size, -1, 1, 1)).view(-1, q.shape[-2], q.shape[-1])
-        kv_packed = kv.masked_select(attention_mask.view(batch_size, -1, 1, 1, 1)).view(
-            -1, kv.shape[-3], kv.shape[-2], kv.shape[-1]
+        q_packed = (
+            q.masked_select(attention_mask.view(batch_size, -1, 1, 1)).view(-1, q.shape[-2], q.shape[-1]).unsqueeze(0)
+        )
+        kv_packed = (
+            kv.masked_select(attention_mask.view(batch_size, -1, 1, 1, 1))
+            .view(-1, kv.shape[-3], kv.shape[-2], kv.shape[-1])
+            .unsqueeze(0)
         )
 
         return q_packed, kv_packed, cu_seqlens_q, cu_seqlens_k, max_seqlen_q, max_seqlen_k
 
     def _inference(self, x, inference_params, **kwargs):  # pylint: disable=W0613
         assert inference_params is not None, "inference_params is required for inference"
         assert self.layer_idx is not None, "Generation requires layer_idx in the constructor"
-        attention_mask = inference_params.get("attention_mask", None)
-        sequence_len_offset = inference_params.get("sequence_len_offset", 0)
+        attention_mask = inference_params.attention_mask
+        sequence_len_offset = inference_params.sequence_len_offset
         batch_size = x.shape[0]
 
         # wqkv, output: q, kv
         if self.enable_qkv_fusion:
             qkv = self.wqkv(x)
             qkv = rearrange(qkv, "b s (three h d) -> b s three h d", three=3, d=self.head_dim)
 
@@ -226,29 +230,29 @@
                         f"{self.max_position_embeddings}, which will cause deviations in dynamic ntk calculations."
                     )
 
                 if self.rotary_emb_dim > 0:
                     q = self.rotary_emb(
                         q, offsets=sequence_len_offset, cache_type="query", interleaved=self.interleaved
                     )
-                    k = kv[:, :, 0].squeueze(2)
+                    k = kv[:, :, 0].squeeze(2)
                     self.rotary_emb(
                         k, offsets=0, cache_type="key", interleaved=self.interleaved, in_place=True
                     )  # in-place is important
             else:
                 if self.rotary_emb_dim > 0:
                     q = self.rotary_emb(q, offsets=0, cache_type="query", interleaved=self.interleaved)
-                    k = kv[:, :, 0].squeueze(2)
+                    k = kv[:, :, 0].squeeze(2)
                     self.rotary_emb(
                         k, offsets=0, cache_type="key", interleaved=self.interleaved, in_place=True
                     )  # in-place is important
         else:
             assert self.rotary_emb_dim > 0, "You should use rotary_emb."
 
-            k, v = kv[:, :, 0].squeueze(2), kv[:, :, 1].squeueze(2)
+            k, v = kv[:, :, 0].squeeze(2), kv[:, :, 1].squeeze(2)
 
             if attention_mask is None:
                 q = self.rotary_emb(q, offsets=sequence_len_offset, cache_type="query", interleaved=self.interleaved)
                 k = self.rotary_emb(k, offsets=sequence_len_offset, cache_type="key", interleaved=self.interleaved)
             else:
                 if sequence_len_offset == 0:
                     q = self.rotary_emb(
@@ -470,35 +474,39 @@
 
         cu_seqlens_q = cu_seqlens
         cu_seqlens_k = cu_seqlens
 
         max_seqlen_q = attention_mask.shape[-1]
         max_seqlen_k = attention_mask.shape[-1]
 
-        q_packed = q.masked_select(attention_mask.view(batch_size, -1, 1, 1)).view(-1, q.shape[-2], q.shape[-1])
-        kv_packed = kv.masked_select(attention_mask.view(batch_size, -1, 1, 1, 1)).view(
-            -1, kv.shape[-3], kv.shape[-2], kv.shape[-1]
+        q_packed = (
+            q.masked_select(attention_mask.view(batch_size, -1, 1, 1)).view(-1, q.shape[-2], q.shape[-1]).unsqueeze(0)
+        )
+        kv_packed = (
+            kv.masked_select(attention_mask.view(batch_size, -1, 1, 1, 1))
+            .view(-1, kv.shape[-3], kv.shape[-2], kv.shape[-1])
+            .unsqueeze(0)
         )
 
         return q_packed, kv_packed, cu_seqlens_q, cu_seqlens_k, max_seqlen_q, max_seqlen_k
 
     def _inference(self, x, inference_params, **kwargs):  # pylint: disable=W0613
         assert inference_params is not None, "inference_params is required for inference"
         assert self.layer_idx is not None, "Generation requires layer_idx in the constructor"
-        attention_mask = inference_params.get("attention_mask", None)
-        sequence_len_offset = inference_params.get("sequence_len_offset", 0)
-        window_size = inference_params.get("window_size", None)
+        attention_mask = inference_params.attention_mask
+        sequence_len_offset = inference_params.sequence_len_offset
+        window_size = inference_params.window_size
 
         batch_size = x.shape[0]
 
         # wqkv, output: q, k, v
         if self.enable_qkv_fusion:
             qkv = self.wqkv(x)
             qkv = rearrange(qkv, "b s (h gs d) -> b s h gs d", gs=self.q_per_kv + 2, d=self.head_dim)
-            q, k, v = (qkv[..., : self.q_per_kv, :], qkv[..., -2, :].unsqueeze(-2), qkv[..., -1, :].unsqueeze(-2))
+            q, k, v = (qkv[..., : self.q_per_kv, :], qkv[..., -2, :], qkv[..., -1, :])
             q = rearrange(q, "b s h gs d -> b s (h gs) d")
         else:
             q, k, v = self.wq(x), self.wk(x), self.wv(x)
             q = rearrange(q, "b s (h d) -> b s h d", d=self.head_dim)
             k = rearrange(k, "b s (h d) -> b s h d", d=self.head_dim)
             v = rearrange(v, "b s (h d) -> b s h d", d=self.head_dim)
```

### Comparing `InternEvo-0.5.2/internlm/model/modules/mlp.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/modules/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/model/modules/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/moe/base_layer.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/base_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/moe/experts.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/experts.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/moe/gshard_layer.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/gshard_layer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/moe/megablock/megablock_dmoe.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/megablock_dmoe.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from internlm.model.moe.megablock.utils import promote_scalar
 
 try:
     import stk
     from megablocks import ops
 except (ModuleNotFoundError, ImportError):
     stk = None
-    megablocks = None
+    ops = None
 
 
 class MegaBlockdMoE(MegaBlockMoE):
     """
     Built on the paper and library Megablocks as described in
     https://arxiv.org/abs/2211.15841. This implementation is
     strictly equivalent to standard MoE with full capacity (no
@@ -29,41 +29,45 @@
     (1) drop tokens at the cost of reduced performance or (2) set
     capacity factor to number of experts and thus waste computation
     and memory on padding.
     """
 
     def __init__(  # pylint: disable=W0231
         self,
-        hidden_size: int,
+        in_features: int,
+        hidden_features: int,
+        out_features: int,
+        num_experts: int,
         ep_group: Optional[torch.distributed.ProcessGroup],
         ep_size: int,
-        num_experts: int,
         top_k: int = 1,
         parallel_mode: str = "tensor",
         device: Optional[torch.device] = None,
         dtype: Optional[torch.device] = None,
         multiple_of: int = 256,
     ) -> None:
         assert gpc.expert_parallel_size == 1, "do not support expert parallel"
+        assert ops is not None and stk is not None, "MegaBlocks not found, please run " '"pip install megablocks".'
         self.top_k = top_k
         self.num_experts = num_experts
 
         tp_size = gpc.get_world_size(ParallelMode.TENSOR)
-        self.ffn_dim = multiple_of * ((int(hidden_size * gpc.config.model.mlp_ratio) + multiple_of - 1) // multiple_of)
+        self.ffn_dim = multiple_of * ((hidden_features + multiple_of - 1) // multiple_of)
         assert self.ffn_dim % tp_size == 0
         if parallel_mode == "tensor":
             self.ffn_dim_per_row = self.ffn_dim // tp_size // ep_size
         else:
             self.ffn_dim_per_row = self.ffn_dim // ep_size
         BaseMoELayer.__init__(  # pylint: disable=W0233
             self,
-            torch.nn.Linear(hidden_size, num_experts, bias=False),
+            torch.nn.Linear(in_features, num_experts, bias=False),
             MegaBlockGroupedFeedForward(
-                hidden_size,
+                in_features,
                 (self.ffn_dim // tp_size) * (num_experts // ep_size),
+                out_features,
                 parallel_mode,
                 device,
                 dtype,
             ),
             ep_group,
             ep_size,
             1,
```

### Comparing `InternEvo-0.5.2/internlm/model/moe/megablock/megablock_moe.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/megablock_moe.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,39 +27,43 @@
     (1) drop tokens at the cost of reduced performance or (2) set
     capacity factor to number of experts and thus waste computation
     and memory on padding.
     """
 
     def __init__(
         self,
-        hidden_size: int,
+        in_features: int,
+        hidden_features: int,
+        out_features: int,
+        num_experts: int,
         ep_group: Optional[torch.distributed.ProcessGroup],
         ep_size: int,
-        num_experts: int,
         top_k: int = 1,
         capacity_factor: float = 1.0,
         drop_tokens: bool = True,
         device: Optional[torch.device] = None,
         dtype: Optional[torch.device] = None,
         multiple_of: int = 256,
     ) -> None:
         assert not gpc.config.parallel.sequence_parallel, "do not support sequence parallel"
+        assert ops is not None, 'MegaBlocks not found, please run "pip install megablocks".'
         self.top_k = top_k
         self.num_experts = num_experts
 
         tp_size = gpc.get_world_size(ParallelMode.TENSOR)
-        self.ffn_dim = multiple_of * ((int(hidden_size * gpc.config.model.mlp_ratio) + multiple_of - 1) // multiple_of)
+        self.ffn_dim = multiple_of * ((hidden_features + multiple_of - 1) // multiple_of)
         self.capacity_factor = capacity_factor
         self.drop_tokens = drop_tokens
         assert self.ffn_dim % tp_size == 0
         super().__init__(
-            torch.nn.Linear(hidden_size, num_experts, bias=False),
+            torch.nn.Linear(in_features, num_experts, bias=False),
             MegaBlockFeedForward(
-                hidden_size,
+                in_features,
                 self.ffn_dim // tp_size,
+                out_features,
                 num_experts // ep_size,
                 device,
                 dtype,
             ),
             ep_group,
             ep_size,
             1,
```

### Comparing `InternEvo-0.5.2/internlm/model/moe/megablock/mlp.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,27 @@
     Feed forward using megablock kernel
     """
 
     def __init__(
         self,
         in_features: int,
         hidden_features: int,
+        out_features: int,
         num_local_experts: int,
         device=None,
         dtype=None,
     ):
         super().__init__()
 
         # merged expert weights, all of size  (ffn_dim * n_experts, model_dim)
         self.w1 = nn.Parameter(torch.empty(num_local_experts, in_features, hidden_features, device=device, dtype=dtype))
-        self.w2 = nn.Parameter(torch.empty(num_local_experts, in_features, hidden_features, device=device, dtype=dtype))
-        self.w3 = nn.Parameter(torch.empty(num_local_experts, hidden_features, in_features, device=device, dtype=dtype))
+        self.w3 = nn.Parameter(torch.empty(num_local_experts, in_features, hidden_features, device=device, dtype=dtype))
+        self.w2 = nn.Parameter(
+            torch.empty(num_local_experts, hidden_features, out_features, device=device, dtype=dtype)
+        )
 
     def forward(self, x):
         # TODO w2 and w3 should swap
         w1_o = tensor_parallel_bmm(x, self.w1, group=gpc.get_group(ParallelMode.TENSOR))
         w3_o = tensor_parallel_bmm(x, self.w3, group=gpc.get_group(ParallelMode.TENSOR))
         out = tensor_parallel_bmm(Silu(w1_o, w3_o), self.w2)
         torch.distributed.all_reduce(out, group=gpc.get_group(ParallelMode.TENSOR))
@@ -47,23 +50,24 @@
     Feed forward using megablock kernel
     """
 
     def __init__(
         self,
         in_features: int,
         hidden_features: int,
+        out_features: int,
         parallel_mode="tensor",
         device=None,
         dtype=None,
     ):
         super().__init__()
 
         # merged expert weights, all of size  (ffn_dim * n_experts, model_dim)
         self.w1 = nn.Parameter(torch.empty(hidden_features, in_features, device=device, dtype=dtype))
-        self.w2 = nn.Parameter(torch.empty(hidden_features, in_features, device=device, dtype=dtype))
+        self.w2 = nn.Parameter(torch.empty(hidden_features, out_features, device=device, dtype=dtype))
         self.w3 = nn.Parameter(torch.empty(hidden_features, in_features, device=device, dtype=dtype))
 
         self.parallel_mode = parallel_mode
 
     def forward(self, x, topo):
         # TODO w2 and w3 should swap
         w1_o = sdd_nt(x, self.w1, topo, gpc.get_group(ParallelMode.TENSOR), self.parallel_mode)
```

### Comparing `InternEvo-0.5.2/internlm/model/moe/megablock/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/megablock/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/moe/moe.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/moe.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/moe/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/model/moe/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/ops/attention.py` & `InternEvo-0.5.2.dev20240525/internlm/model/ops/attention.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/ops/cross_entropy.py` & `InternEvo-0.5.2.dev20240525/internlm/model/ops/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/ops/linear.py` & `InternEvo-0.5.2.dev20240525/internlm/model/ops/linear.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/ops/norm.py` & `InternEvo-0.5.2.dev20240525/internlm/model/ops/norm.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,21 @@
 try:
     from deeplink_ext.internevo_ops import MixedFusedRMSNorm
 
     deeplink_rmsnorm_impl = True
 except (ModuleNotFoundError, ImportError):
     deeplink_rmsnorm_impl = False
 
+try:
+    from torch_npu import npu_rms_norm
+
+    torchnpu_rmsnorm_impl = True
+except (ModuleNotFoundError, ImportError):
+    torchnpu_rmsnorm_impl = False
+
 
 def manual_rms_norm(my_input, weight, normalized_shape, eps):
     # layer norm should always be calculated in float32
     dims = tuple(i for i in range(-1, -len(normalized_shape) - 1, -1))
     variance = my_input.to(torch.float32).pow(2).mean(dims, keepdim=True)
     my_input = my_input * torch.rsqrt(variance + eps)
 
@@ -68,13 +75,42 @@
     def reset_parameters(self):
         init.ones_(self.weight)
 
     def extra_repr(self):
         return f"{self.normalized_shape}, eps={self.eps}, "
 
 
+class _RMSNormNPU(torch.nn.Module):
+    """A custom NPU module for RMS normalization."""
+
+    def __init__(self, normalized_shape, eps=1e-5):
+        super().__init__()
+
+        if isinstance(normalized_shape, numbers.Integral):
+            normalized_shape = (normalized_shape,)
+        self.normalized_shape = torch.Size(normalized_shape)
+        self.eps = eps
+        self.weight = Parameter(torch.empty(*normalized_shape))
+        self.reset_parameters()
+        self.rmsorm_npu_forward = npu_rms_norm
+
+    def forward(self, _input: torch.Tensor):
+        weight_fp32 = self.weight.to(torch.float32)
+        input_fp32 = _input.to(torch.float32)
+        output = self.rmsorm_npu_forward(input_fp32, gamma=weight_fp32, epsilon=self.eps)[0].to(self.weight.dtype)
+        return output
+
+    def reset_parameters(self):
+        init.ones_(self.weight)
+
+    def extra_repr(self):
+        return f"{self.normalized_shape}, eps={self.eps}, ".format(**self.__dict__)
+
+
 # TODO: Support deeplink in a more unified manner
-RMSNorm = (
-    MixedFusedRMSNorm
-    if internlm_accelerator.get_accelerator_backend() == AcceleratorType.DIPU and deeplink_rmsnorm_impl
-    else _RMSNorm
-)
+backend = internlm_accelerator.get_accelerator_backend()
+if backend == AcceleratorType.DIPU and deeplink_rmsnorm_impl:
+    RMSNorm = MixedFusedRMSNorm
+elif backend == AcceleratorType.NPU and torchnpu_rmsnorm_impl:
+    RMSNorm = _RMSNormNPU
+else:
+    RMSNorm = _RMSNorm
```

### Comparing `InternEvo-0.5.2/internlm/model/ops/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/model/ops/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/model/registry.py` & `InternEvo-0.5.2.dev20240525/internlm/model/registry.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/monitor/alert.py` & `InternEvo-0.5.2.dev20240525/internlm/monitor/alert.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/monitor/monitor.py` & `InternEvo-0.5.2.dev20240525/internlm/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/monitor/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/activation_checkpoint.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/optimizer/base_optimizer.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/optimizer/compatible_adamw.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/compatible_adamw.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/optimizer/fsdp_optimizer.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/fsdp_optimizer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/optimizer/hybrid_zero_optim.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/hybrid_zero_optim.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/optimizer/store.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/store.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/optimizer/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/schedulers/beta2_scheduler.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/schedulers/beta2_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/solver/schedulers/lr_scheduler.py` & `InternEvo-0.5.2.dev20240525/internlm/solver/schedulers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/train/__init__.py` & `InternEvo-0.5.2.dev20240525/internlm/train/__init__.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/train/pipeline.py` & `InternEvo-0.5.2.dev20240525/internlm/train/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,14 +504,15 @@
     batch_count,
     batch,
     train_state,
     optimizer,
     beta2_scheduler,
     trainer,
     start_time,
+    very_begining_time,
     loss,
     moe_loss,
     grad_norm,
     metric,
 ):
     """
     Print some training metrics of current batch.
@@ -542,15 +543,15 @@
         tk_per_gpu = round(
             num_tokens_in_batch * gpc.get_world_size(ParallelMode.DATA) / gpc.get_world_size(ParallelMode.GLOBAL),
             4,
         )
         tgs_statistic = train_state.tgs_statistic
         tgs_statistic["sum_step"] += 1
         tgs_statistic["sum_tg"] += tk_per_gpu
-        tgs_statistic["sum_time"] += time_cost
+        tgs_statistic["total_time"] = time.time() - very_begining_time
         tgs_statistic["sum_last_tg_10"] += tk_per_gpu
         tgs_statistic["sum_last_time_10"] += time_cost
         tgs_statistic["sum_last_tg_50"] += tk_per_gpu
         tgs_statistic["sum_last_time_50"] += time_cost
         tgs_statistic["SMA_tg_50"] += tk_per_gpu
         tgs_statistic["SMA_time_50"] += time_cost
         tgs_statistic["SMA_tg_50_list"].append(tk_per_gpu)
@@ -573,15 +574,15 @@
             tgs_statistic["last_tgs_50"] = round(tgs_statistic["sum_last_tg_50"] / tgs_statistic["sum_last_time_50"], 2)
             tgs_statistic["sum_last_tg_50"] = 0
             tgs_statistic["sum_last_time_50"] = 0
 
         last_tgs_10 = tgs_statistic["last_tgs_10"]
         last_tgs_50 = tgs_statistic["last_tgs_50"]
 
-        tgs_all = round(tgs_statistic["sum_tg"] / tgs_statistic["sum_time"], 2)
+        tgs_all = round(tgs_statistic["sum_tg"] / tgs_statistic["total_time"], 2)
         tgs_avg = round(tgs_statistic["sum_tgs"] / tgs_statistic["sum_step"], 2)
         tgs_SMA = round(tgs_statistic["SMA_tg_50"] / tgs_statistic["SMA_time_50"], 2)
 
         tflops = get_tflops_func(time_cost)
 
         tgs_origin = round(
             num_tokens_in_batch
```

### Comparing `InternEvo-0.5.2/internlm/train/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/train/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/common.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/common.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/gputest.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/gputest.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/logger.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/logger.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/megatron_timers.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/megatron_timers.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/parallel.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/simple_memory_profiler.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/simple_memory_profiler.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/storage_manager.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/storage_manager.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/timeout.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/timeout.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/internlm/utils/utils.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,34 +58,35 @@
     def __kv_checker(num_args: int):
         if num_args < 3:
             return "kv" in kwargs
         else:
             # kv: [batch, seqlen, 3, n_head, headdim]
             return len(args[2].shape) == 5
 
-    def __cu_seqlens_checker(num_args: int, check_idx: int):
+    def __cu_seqlens_checker(args, check_idx: int):
+        num_args = len(args)
         if num_args < (check_idx + 1):
             if check_idx == 2:
                 return "cu_seqlens" in kwargs and kwargs["cu_seqlens"] is not None
             else:
                 return "cu_seqlens_q" in kwargs and kwargs["cu_seqlens_q"] is not None
         else:
-            return isinstance(num_args[check_idx], torch.Tensor)
+            return isinstance(args[check_idx], torch.Tensor)
 
     if __qkv_checker(len(args)):
         # qkv packed, and we should check cu_seqlens with index 2
         qkv_pack_type = int(QKVPackType.QKVPACKED)
     elif __kv_checker(len(args)):
         # kv packed, and we should check cu_seqlens with index 3
         qkv_pack_type = int(QKVPackType.KVPACKED)
     else:
         # qkv splited, and we should check cu_seqlens with index 4
         qkv_pack_type = int(QKVPackType.QKVSPLITED)
 
-    with_cu_seqlens = __cu_seqlens_checker(len(args), qkv_pack_type)
+    with_cu_seqlens = __cu_seqlens_checker(args, qkv_pack_type)
 
     return str(qkv_pack_type), str(with_cu_seqlens)
 
 
 def params_dispatch_with_condition(condition: Callable, func: Callable = None):
 
     if func is None:
```

### Comparing `InternEvo-0.5.2/internlm/utils/writer.py` & `InternEvo-0.5.2.dev20240525/internlm/utils/writer.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/setup.py` & `InternEvo-0.5.2.dev20240525/setup.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/common_fixture.py` & `InternEvo-0.5.2.dev20240525/tests/common_fixture.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_core/test_pipeline.py` & `InternEvo-0.5.2.dev20240525/tests/test_core/test_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import multiprocessing as mp
 
 import pytest
 import torch
 
-from internlm.accelerator import AcceleratorType, get_accelerator
 from internlm.core.context import ParallelMode
 from internlm.core.context import global_context as gpc
 from internlm.core.context.parallel_context import Config
+from internlm.solver.optimizer.compatible_adamw import new_compatible_adamw
 from internlm.utils.common import get_current_device
 from tests.test_core.utils import (
     MlpModel,
     MyLoss,
     build_environment,
     init_model_and_optim,
     loose_close,
@@ -119,42 +119,38 @@
     yx = torch.tensor(y_list).to(device).to(dtype)
 
     input_list = [{"input_ids": xs}, yx]
 
     # pp forward and backward
     output_list = []
     for _ in range(10):
-        output, _, loss = scheduler.forward_backward_step(
-            engine, input_list, forward_only=False, return_loss=True, return_output_label=True
+        res = scheduler.forward_backward_step(
+            engine,
+            input_list,
+            forward_only=False,
+            return_loss=True,
+            return_output_label=True,
         )
+        output = res[0]
+        loss = res[2]
         output_list.append(output)
 
     # engine.step()
 
     # torch related
     if gpc.is_last_rank(ParallelMode.PIPELINE):
         torch_xs = torch.tensor(x_list).to(device).to(torch.float32)
         torch_ys = torch.tensor(y_list).to(device).to(torch.float32)
         torch_model = MlpModel(0, 32, "torch").to(device)
-        adam_extra_kwargs = {}
-        if get_accelerator().get_accelerator_backend() == AcceleratorType.NPU:
-            import torch_npu
-
-            internlm_adamw = torch_npu.optim.NpuFusedAdamW
-        else:
-            internlm_adamw = torch.optim.AdamW
-            if torch.__version__ >= "2.1.0":
-                adam_extra_kwargs["fused"] = True
 
-        torch_optimizer = internlm_adamw(
+        torch_optimizer = new_compatible_adamw(
             params=[{"params": torch_model.parameters(), "weight_decay": config.adam.weight_decay}],
             lr=config.adam.lr,
             betas=(config.adam.adam_beta1, config.adam.adam_beta2),
             eps=config.adam.adam_eps,
-            **adam_extra_kwargs,
         )
 
         # check only forward logits
         first_output = output_list[0]
         for i in range(1, 10):
             assert torch.equal(first_output, output_list[i])
```

### Comparing `InternEvo-0.5.2/tests/test_core/utils.py` & `InternEvo-0.5.2.dev20240525/tests/test_core/utils.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/7B_check_acc.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/7B_check_acc.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/7B_check_init.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/7B_check_init.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/test_forward_output_no_fa.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/test_forward_output_no_fa.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/test_load_ckpt_loss.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/test_load_ckpt_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/test_loss.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/test_loss.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/test_no_fa_train_temp.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/test_no_fa_train_temp.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/test_norm_weight.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/test_norm_weight.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/test_swap_nb_loss_and_gradnorm.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/test_swap_nb_loss_and_gradnorm.py`

 * *Files identical despite different names*

### Comparing `InternEvo-0.5.2/tests/test_training/train_CI.py` & `InternEvo-0.5.2.dev20240525/tests/test_training/train_CI.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                 logger.warning(f"The old key {key} no longer exists!")
 
     if gpc.is_rank_for_log():
         logger.info("Weight check passed")
 
 
 def main(args):
+    very_begining_time = time.time()
     # init setting
     skip_batches = gpc.config.data.skip_batches
     total_steps = gpc.config.data.total_steps
     valid_every = gpc.config.data.valid_every
     label_smoothing = gpc.config.loss.label_smoothing
 
     get_tflops_func = partial(
@@ -301,14 +302,15 @@
                 success_update=success_update,
                 batch_count=batch_count,
                 batch=batch,
                 train_state=train_state,
                 optimizer=optimizer,
                 beta2_scheduler=beta2_scheduler,
                 trainer=trainer,
+                very_begining_time=very_begining_time,
                 start_time=start_time,
                 loss=loss,
                 moe_loss=moe_loss,
                 grad_norm=grad_norm_groups,
                 metric=metric,
             )
```

