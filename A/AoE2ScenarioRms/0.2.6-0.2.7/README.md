# Comparing `tmp/AoE2ScenarioRms-0.2.6.tar.gz` & `tmp/AoE2ScenarioRms-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AoE2ScenarioRms-0.2.6.tar", last modified: Mon Jan  1 13:22:56 2024, max compression
+gzip compressed data, was "AoE2ScenarioRms-0.2.7.tar", last modified: Mon Jan  1 14:06:17 2024, max compression
```

## Comparing `AoE2ScenarioRms-0.2.6.tar` & `AoE2ScenarioRms-0.2.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.946485 AoE2ScenarioRms-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.938485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.938485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/core/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/core/aoe2_scenario_rms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.938485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_all_visible.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_no_clutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_state_as_black.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_xs_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.938485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/grouping_method.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.942485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/internal/xs_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/tile_level.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.942485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/errors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/errors/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.942485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/object_clear.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/object_marks.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/terrain_mark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.942485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.942485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/create_object/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/create_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/create_object/create_object_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/create_object/create_object_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/rms_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/rms_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.946485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/grid_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/grid_map_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/scenario_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/tile_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/unit_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/xs_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/xs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:22:56.946485 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-01-01 13:22:56.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-01 13:22:56.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 13:22:56.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-01 13:22:56.000000 AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-01-01 13:22:56.946485 AoE2ScenarioRms-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-01 13:22:44.000000 AoE2ScenarioRms-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 13:22:56.946485 AoE2ScenarioRms-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.637232 AoE2ScenarioRms-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.629233 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.629233 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/core/aoe2_scenario_rms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.629233 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_all_visible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_no_clutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_state_as_black.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_xs_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.633232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/grouping_method.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.633232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/internal/xs_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/tile_level.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.633232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/errors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/errors/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.633232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/object_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/object_marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/terrain_mark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.633232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.633232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/create_object/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/create_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/create_object/create_object_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/create_object/create_object_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/rms_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/rms_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.637232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/grid_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/grid_map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/scenario_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/tile_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/unit_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/xs_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/xs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 14:06:17.637232 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-01-01 14:06:17.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-01 14:06:17.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 14:06:17.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-01 14:06:17.000000 AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-01-01 14:06:17.637232 AoE2ScenarioRms-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-01 14:06:08.000000 AoE2ScenarioRms-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 14:06:17.637232 AoE2ScenarioRms-0.2.7/setup.cfg
```

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/core/aoe2_scenario_rms.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/core/aoe2_scenario_rms.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_all_visible.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_all_visible.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_state_as_black.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_state_as_black.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/debug/apply_xs_print.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/debug/apply_xs_print.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/enums/internal/xs_key.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/enums/internal/xs_key.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/object_clear.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/object_clear.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/flags/terrain_mark.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/flags/terrain_mark.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/create_object/create_object_config.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/create_object/create_object_config.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/create_object/create_object_feature.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/create_object/create_object_feature.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/rms/rms_feature.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/rms/rms_feature.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/data.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/data.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/grid_map.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/grid_map.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/grid_map_factory.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/grid_map_factory.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/locator.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/locator.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/scenario_util.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/scenario_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/tile_util.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/tile_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/unit_util.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/unit_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/xs_container.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/xs_container.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms/util/xs_util.py` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms/util/xs_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/PKG-INFO` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: AoE2ScenarioRms
-Version: 0.2.6
+Version: 0.2.7
 Summary: Add replay-ability to scenarios through random resource placement using triggers & XS!
 Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
 Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
 Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
 Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
+Project-URL: Changelog, https://github.com/KSneijders/AoE2ScenarioRms/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `AoE2ScenarioRms-0.2.6/AoE2ScenarioRms.egg-info/SOURCES.txt` & `AoE2ScenarioRms-0.2.7/AoE2ScenarioRms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/LICENSE` & `AoE2ScenarioRms-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/PKG-INFO` & `AoE2ScenarioRms-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: AoE2ScenarioRms
-Version: 0.2.6
+Version: 0.2.7
 Summary: Add replay-ability to scenarios through random resource placement using triggers & XS!
 Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
 Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
 Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
 Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
+Project-URL: Changelog, https://github.com/KSneijders/AoE2ScenarioRms/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `AoE2ScenarioRms-0.2.6/README.md` & `AoE2ScenarioRms-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.6/pyproject.toml` & `AoE2ScenarioRms-0.2.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "AoE2ScenarioParser>=0.1.60"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AoE2ScenarioRms"
-version = "0.2.6"  # << Also change `AoE2ScenarioRms/version.py`
+version = "0.2.7"  # << Also change `AoE2ScenarioRms/version.py`
 authors = [
     { name = "Kerwin Sneijders", email = "ksneijders-dev@hotmail.com" },
 ]
-description = """
-    Add replay-ability to scenarios through random resource placement using triggers & XS!
-"""
+description = """Add replay-ability to scenarios through random resource placement using triggers & XS!"""
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/KSneijders/AoE2ScenarioRms"
 "Bug Tracker" = "https://github.com/KSneijders/AoE2ScenarioRms/issues"
 "Examples" = "https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples"
+"Changelog" = "https://github.com/KSneijders/AoE2ScenarioRms/blob/main/CHANGELOG.md"
```

