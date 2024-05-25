# Comparing `tmp/torchtnt_nightly-2024.5.23.tar.gz` & `tmp/torchtnt_nightly-2024.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtnt_nightly-2024.5.23.tar", last modified: Thu May 23 11:27:19 2024, max compression
+gzip compressed data, was "torchtnt_nightly-2024.5.24.tar", last modified: Fri May 24 11:27:35 2024, max compression
```

## Comparing `torchtnt_nightly-2024.5.23.tar` & `torchtnt_nightly-2024.5.24.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.960678 torchtnt_nightly-2024.5.23/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-23 11:27:19.960678 torchtnt_nightly-2024.5.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:27:19.960678 torchtnt_nightly-2024.5.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.940679 torchtnt_nightly-2024.5.23/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.944679 torchtnt_nightly-2024.5.23/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/_loop_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/_unit_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.948679 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/_checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/base_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/checkpointer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/dcp_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/empty_cuda_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/iteration_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/memory_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/progress_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/slow_rank_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/throughput_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/time_limit_interrupter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/time_wait_for_batch_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/torch_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.952679 torchtnt_nightly-2024.5.23/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.956678 torchtnt_nightly-2024.5.23/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/data/profile_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/data/synthetic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    23329 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/fsdp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.956678 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/memory_snapshot_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/prepare_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-23 11:25:13.000000 torchtnt_nightly-2024.5.23/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:27:19.956678 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-23 11:27:19.000000 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-23 11:27:19.000000 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:27:19.000000 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 11:27:19.000000 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 11:27:19.000000 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:27:19.000000 torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.950475 torchtnt_nightly-2024.5.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-24 11:27:35.950475 torchtnt_nightly-2024.5.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:27:35.950475 torchtnt_nightly-2024.5.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.934475 torchtnt_nightly-2024.5.24/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.938475 torchtnt_nightly-2024.5.24/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/_loop_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/_unit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36138 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.942474 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/_checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/base_checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/checkpointer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15782 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/dcp_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/empty_cuda_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/iteration_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/memory_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/progress_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/slow_rank_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8965 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/throughput_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/time_limit_interrupter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/time_wait_for_batch_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/torch_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17312 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22471 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.946474 torchtnt_nightly-2024.5.24/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29240 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.946474 torchtnt_nightly-2024.5.24/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21149 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/data/profile_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/data/synthetic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11546 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23329 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/fsdp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.946474 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/memory_snapshot_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27230 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14932 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/prepare_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-24 11:25:29.000000 torchtnt_nightly-2024.5.24/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:27:35.950475 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-24 11:27:35.000000 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-24 11:27:35.000000 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:27:35.000000 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-24 11:27:35.000000 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 11:27:35.000000 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:27:35.000000 torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt_nightly-2024.5.23/LICENSE` & `torchtnt_nightly-2024.5.24/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/PKG-INFO` & `torchtnt_nightly-2024.5.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2024.5.23
+Version: 2024.5.24
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.5.23 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.5.24 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt_nightly-2024.5.23/README.md` & `torchtnt_nightly-2024.5.24/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/setup.py` & `torchtnt_nightly-2024.5.24/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/__init__.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/_callback_handler.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/_callback_handler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/_loop_utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/_loop_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/_test_utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/_unit_utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/_unit_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/auto_unit.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/auto_unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callback.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/__init__.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/_checkpoint_utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/_checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/base_checkpointer.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/base_checkpointer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/checkpointer_types.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/checkpointer_types.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/dcp_saver.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/dcp_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/early_stopping.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/empty_cuda_cache.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/empty_cuda_cache.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/iteration_time_logger.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/iteration_time_logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/memory_snapshot.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/memory_snapshot.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/module_summary.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/progress_reporter.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/slow_rank_detector.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/slow_rank_detector.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/throughput_logger.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/throughput_logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/time_limit_interrupter.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/time_limit_interrupter.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/time_wait_for_batch_logger.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/time_wait_for_batch_logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/torch_compile.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/torch_compile.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/evaluate.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/fit.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/predict.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/state.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/train.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/unit.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/framework/utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/__init__.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/checkpoint.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/data/__init__.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/data/data_prefetcher.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/data/iterators.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/data/multi_dataloader.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/data/profile_dataloader.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/data/profile_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/data/synthetic_data.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/device.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/distributed.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/early_stop_checker.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/env.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/flops.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/flops.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/fsdp_utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/fsdp_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/fsspec.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/__init__.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/csv.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/file.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/in_memory.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/json.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/logger.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/stdout.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/tensorboard.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/loggers/utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/lr_scheduler.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/memory.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/memory_snapshot_profiler.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/memory_snapshot_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/misc.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/module_summary.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/oom.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/optimizer.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/optimizer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/precision.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/precision.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/prepare_module.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/prepare_module.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/progress.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/rank_zero_log.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/stateful.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/stateful.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/swa.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/swa.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/test_utils.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/timer.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/tqdm.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt/utils/version.py` & `torchtnt_nightly-2024.5.24/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2024.5.23
+Version: 2024.5.24
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.5.23 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2024.5.24 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt_nightly-2024.5.23/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt_nightly-2024.5.24/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

