# Comparing `tmp/AoE2ScenarioParser-0.1.8.tar.gz` & `tmp/AoE2ScenarioParser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AoE2ScenarioParser-0.1.8.tar", last modified: Sat May  1 08:30:03 2021, max compression
+gzip compressed data, was "AoE2ScenarioParser-0.1.9.tar", last modified: Wed Jun  2 18:41:35 2021, max compression
```

## Comparing `AoE2ScenarioParser-0.1.8.tar` & `AoE2ScenarioParser-0.1.9.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.766268 AoE2ScenarioParser-0.1.8/
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.165974 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/
--rw-rw-rw-   0        0        0      963 2021-03-27 14:31:07.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/aoe2_scenario.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.311638 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/
--rw-rw-rw-   0        0        0     8312 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/buildings.py
--rw-rw-rw-   0        0        0     6304 2021-04-30 20:20:41.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/conditions.py
--rw-rw-rw-   0        0        0    17060 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/effects.py
--rw-rw-rw-   0        0        0     7492 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/heroes.py
--rw-rw-rw-   0        0        0     2021 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/other.py
--rw-rw-rw-   0        0        0      373 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/players.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.335799 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/scripts/
--rw-rw-rw-   0        0        0     2530 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/scripts/get_icon_ids.py
--rw-rw-rw-   0        0        0    11106 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/scripts/object_parser.py
--rw-rw-rw-   0        0        0    10263 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/techs.py
--rw-rw-rw-   0        0        0     2173 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/terrains.py
--rw-rw-rw-   0        0        0    28872 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/trigger_lists.py
--rw-rw-rw-   0        0        0    17587 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/units.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.422358 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/
--rw-rw-rw-   0        0        0     4255 2021-04-22 21:36:52.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/bytes_conversions.py
--rw-rw-rw-   0        0        0     4310 2021-04-24 18:51:10.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/bytes_parser.py
--rw-rw-rw-   0        0        0      459 2021-04-25 08:58:39.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/exceptions.py
--rw-rw-rw-   0        0        0     1753 2021-04-25 09:07:15.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/helper.py
--rw-rw-rw-   0        0        0     1081 2021-04-03 12:50:00.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/incremental_generator.py
--rw-rw-rw-   0        0        0      450 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/list_functions.py
--rw-rw-rw-   0        0        0     1677 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/pretty_format.py
--rw-rw-rw-   0        0        0     1028 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/printers.py
--rw-rw-rw-   0        0        0     1682 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/string_manipulations.py
--rw-rw-rw-   0        0        0      326 2020-12-30 15:45:24.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/local_config.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.440359 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/
--rw-rw-rw-   0        0        0     4389 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/aoe2_object.py
--rw-rw-rw-   0        0        0     1746 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/aoe2_object_manager.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.487362 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/
--rw-rw-rw-   0        0        0     6320 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/condition.py
--rw-rw-rw-   0        0        0    12753 2021-04-14 08:36:35.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/effect.py
--rw-rw-rw-   0        0        0      731 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/terrain_tile.py
--rw-rw-rw-   0        0        0    15269 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/trigger.py
--rw-rw-rw-   0        0        0     3834 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/unit.py
--rw-rw-rw-   0        0        0      641 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/variable.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.512358 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.534363 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/de/
--rw-rw-rw-   0        0        0     1541 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/de/map_manager_de.py
--rw-rw-rw-   0        0        0     3683 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/de/trigger_manager_de.py
--rw-rw-rw-   0        0        0      505 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/de/unit_manager_de.py
--rw-rw-rw-   0        0        0     3522 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/map_manager.py
--rw-rw-rw-   0        0        0    26530 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/trigger_manager.py
--rw-rw-rw-   0        0        0     8553 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/unit_manager.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.573543 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.581554 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/enums/
--rw-rw-rw-   0        0        0     1955 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/enums/group_by.py
--rw-rw-rw-   0        0        0    11344 2021-04-30 20:20:41.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/new_condition.py
--rw-rw-rw-   0        0        0    41217 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/new_effect.py
--rw-rw-rw-   0        0        0      781 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/tile.py
--rw-rw-rw-   0        0        0     1418 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/trigger_ce_lock.py
--rw-rw-rw-   0        0        0     1355 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/trigger_select.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.596543 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/scenarios/
--rw-rw-rw-   0        0        0      903 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/scenarios/aoe2_de_scenario.py
--rw-rw-rw-   0        0        0    12202 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/scenarios/aoe2_scenario.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.613678 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/
--rw-rw-rw-   0        0        0    11580 2021-04-12 17:47:06.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/aoe2_file_section.py
--rw-rw-rw-   0        0        0     1240 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/aoe2_struct_model.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.650077 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/
--rw-rw-rw-   0        0        0     2571 2021-04-12 17:42:07.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency.py
--rw-rw-rw-   0        0        0      136 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency_action.py
--rw-rw-rw-   0        0        0      767 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency_eval.py
--rw-rw-rw-   0        0        0     1224 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency_target.py
--rw-rw-rw-   0        0        0     2079 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/retriever_dependency.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.683435 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/
--rw-rw-rw-   0        0        0     4515 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/datatype.py
--rw-rw-rw-   0        0        0     7599 2021-04-24 18:48:41.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/retriever.py
--rw-rw-rw-   0        0        0     8735 2021-04-12 17:34:15.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/retriever_object_link.py
--rw-rw-rw-   0        0        0     1441 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/support.py
--rw-rw-rw-   0        0        0       58 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/settings.py
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.116433 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.690434 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/
--rw-rw-rw-   0        0        0     6038 2021-03-25 21:47:53.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/changelog.md
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.715263 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/
--rw-rw-rw-   0        0        0    21742 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/conditions.json
--rw-rw-rw-   0        0        0   106831 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/effects.json
--rw-rw-rw-   0        0        0   117887 2021-04-24 18:48:41.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/structure.json
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.739477 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/
--rw-rw-rw-   0        0        0    28679 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/conditions.json
--rw-rw-rw-   0        0        0   138904 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/effects.json
--rw-rw-rw-   0        0        0   122992 2021-04-24 18:48:41.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/structure.json
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.762111 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/
--rw-rw-rw-   0        0        0    28679 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/conditions.json
--rw-rw-rw-   0        0        0   138904 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/effects.json
--rw-rw-rw-   0        0        0   123225 2021-04-24 18:48:41.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/structure.json
-drwxrwxrwx   0        0        0        0 2021-05-01 08:30:03.205484 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/
--rw-rw-rw-   0        0        0     7286 2021-05-01 08:30:02.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3495 2021-05-01 08:30:02.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-01 08:30:02.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2021-05-01 08:30:02.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2021-05-01 08:30:02.000000 AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       47 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7286 2021-05-01 08:30:03.764277 AoE2ScenarioParser-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6067 2021-04-12 15:04:01.000000 AoE2ScenarioParser-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2021-05-01 08:30:03.766268 AoE2ScenarioParser-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      907 2021-05-01 08:30:02.000000 AoE2ScenarioParser-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.811573 AoE2ScenarioParser-0.1.9/
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.205580 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/
+-rw-rw-rw-   0        0        0      963 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/aoe2_scenario.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.349571 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/
+-rw-rw-rw-   0        0        0     7530 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/buildings.py
+-rw-rw-rw-   0        0        0     6288 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/conditions.py
+-rw-rw-rw-   0        0        0    16903 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/effects.py
+-rw-rw-rw-   0        0        0     7767 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/heroes.py
+-rw-rw-rw-   0        0        0     8704 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/other.py
+-rw-rw-rw-   0        0        0      373 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/players.py
+-rw-rw-rw-   0        0        0     6216 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/projectiles.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.369569 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/scripts/
+-rw-rw-rw-   0        0        0     2530 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/scripts/get_icon_ids.py
+-rw-rw-rw-   0        0        0    11106 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/scripts/object_parser.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.381580 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/support/
+-rw-rw-rw-   0        0        0     2043 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/support/info_dataset_base.py
+-rw-rw-rw-   0        0        0    10304 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/techs.py
+-rw-rw-rw-   0        0        0     2173 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/terrains.py
+-rw-rw-rw-   0        0        0    33857 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/trigger_lists.py
+-rw-rw-rw-   0        0        0    17785 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/units.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.459580 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/
+-rw-rw-rw-   0        0        0     4255 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/bytes_conversions.py
+-rw-rw-rw-   0        0        0     4290 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/bytes_parser.py
+-rw-rw-rw-   0        0        0      459 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/exceptions.py
+-rw-rw-rw-   0        0        0     1753 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/helper.py
+-rw-rw-rw-   0        0        0     1081 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/incremental_generator.py
+-rw-rw-rw-   0        0        0      450 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/list_functions.py
+-rw-rw-rw-   0        0        0     1677 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/pretty_format.py
+-rw-rw-rw-   0        0        0     1028 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/printers.py
+-rw-rw-rw-   0        0        0     1682 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/string_manipulations.py
+-rw-rw-rw-   0        0        0      326 2020-12-30 15:45:24.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/local_config.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.473572 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/
+-rw-rw-rw-   0        0        0     4389 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/aoe2_object.py
+-rw-rw-rw-   0        0        0     1746 2021-05-31 22:42:03.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/aoe2_object_manager.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.520572 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/
+-rw-rw-rw-   0        0        0     6300 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/condition.py
+-rw-rw-rw-   0        0        0    12733 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/effect.py
+-rw-rw-rw-   0        0        0      731 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/terrain_tile.py
+-rw-rw-rw-   0        0        0    15261 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/trigger.py
+-rw-rw-rw-   0        0        0     3975 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/unit.py
+-rw-rw-rw-   0        0        0      641 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/variable.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.546570 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.570572 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/de/
+-rw-rw-rw-   0        0        0     1541 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/de/map_manager_de.py
+-rw-rw-rw-   0        0        0     3683 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/de/trigger_manager_de.py
+-rw-rw-rw-   0        0        0      505 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/de/unit_manager_de.py
+-rw-rw-rw-   0        0        0     3522 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/map_manager.py
+-rw-rw-rw-   0        0        0    26530 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/trigger_manager.py
+-rw-rw-rw-   0        0        0     9095 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/unit_manager.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.614572 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.621570 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/enums/
+-rw-rw-rw-   0        0        0     1955 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/enums/group_by.py
+-rw-rw-rw-   0        0        0    14009 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/new_condition.py
+-rw-rw-rw-   0        0        0    50525 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/new_effect.py
+-rw-rw-rw-   0        0        0      781 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/tile.py
+-rw-rw-rw-   0        0        0     1418 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/trigger_ce_lock.py
+-rw-rw-rw-   0        0        0     1355 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/trigger_select.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.636570 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/scenarios/
+-rw-rw-rw-   0        0        0      903 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/scenarios/aoe2_de_scenario.py
+-rw-rw-rw-   0        0        0    12676 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/scenarios/aoe2_scenario.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.652568 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/
+-rw-rw-rw-   0        0        0    10770 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/aoe2_file_section.py
+-rw-rw-rw-   0        0        0     1231 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/aoe2_struct_model.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.699572 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/
+-rw-rw-rw-   0        0        0     2495 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency.py
+-rw-rw-rw-   0        0        0      136 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency_action.py
+-rw-rw-rw-   0        0        0      767 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency_eval.py
+-rw-rw-rw-   0        0        0     1224 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency_target.py
+-rw-rw-rw-   0        0        0     2079 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/retriever_dependency.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.733574 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/
+-rw-rw-rw-   0        0        0     4515 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/datatype.py
+-rw-rw-rw-   0        0        0     7800 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/retriever.py
+-rw-rw-rw-   0        0        0     8613 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/retriever_object_link.py
+-rw-rw-rw-   0        0        0     1441 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/support.py
+-rw-rw-rw-   0        0        0       58 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/settings.py
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.166570 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.742569 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/
+-rw-rw-rw-   0        0        0     6038 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/changelog.md
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.764569 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/
+-rw-rw-rw-   0        0        0    21630 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/conditions.json
+-rw-rw-rw-   0        0        0   106477 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/effects.json
+-rw-rw-rw-   0        0        0   117879 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/structure.json
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.786569 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/
+-rw-rw-rw-   0        0        0    28543 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/conditions.json
+-rw-rw-rw-   0        0        0   138454 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/effects.json
+-rw-rw-rw-   0        0        0   122984 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/structure.json
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.808579 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/
+-rw-rw-rw-   0        0        0    28543 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/conditions.json
+-rw-rw-rw-   0        0        0   138454 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/effects.json
+-rw-rw-rw-   0        0        0   123217 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/structure.json
+drwxrwxrwx   0        0        0        0 2021-06-02 18:41:35.239568 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/
+-rw-rw-rw-   0        0        0     6658 2021-06-02 18:41:34.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3595 2021-06-02 18:41:34.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-02 18:41:34.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2021-06-02 18:41:34.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2021-06-02 18:41:34.000000 AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       47 2021-05-02 15:57:23.000000 AoE2ScenarioParser-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6658 2021-06-02 18:41:35.810568 AoE2ScenarioParser-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5471 2021-06-02 18:40:48.000000 AoE2ScenarioParser-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-06-02 18:41:35.811573 AoE2ScenarioParser-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      907 2021-06-02 18:41:34.000000 AoE2ScenarioParser-0.1.9/setup.py
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/aoe2_scenario.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/aoe2_scenario.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/buildings.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/buildings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,217 +1,153 @@
-from enum import Enum
+from AoE2ScenarioParser.datasets.support.info_dataset_base import InfoDatasetBase
 
 
-class BuildingInfo(Enum):
-    @property
-    def ID(self):
-        return self.value[0]
-
-    @classmethod
-    def from_id(cls, value: int):
-        if type(value) is not int:
-            raise TypeError(f"from_id expected int, got {type(value)}")
-        if value == -1:
-            raise ValueError("-1 is not a valid id value")
-        for x in cls._member_map_.values():
-            if x.value[0] == value:
-                return x
-        raise ValueError(f"{value} is not a valid id value")
-
-    @property
-    def ICON_ID(self):
-        return self.value[1]
-
-    @classmethod
-    def from_icon_id(cls, value: int):
-        if type(value) is not int:
-            raise TypeError(f"from_icon_id expected int, got {type(value)}")
-        if value == -1:
-            raise ValueError("-1 is not a valid icon_id value")
-        for x in cls._member_map_.values():
-            if x.value[1] == value:
-                return x
-        raise ValueError(f"{value} is not a valid icon_id value")
-
-    @property
-    def DEAD_ID(self):
-        return self.value[2]
-
-    @classmethod
-    def from_dead_id(cls, value: int):
-        if type(value) is not int:
-            raise TypeError(f"from_dead_id expected int, got {type(value)}")
-        if value == -1:
-            raise ValueError("-1 is not a valid dead_id value")
-        for x in cls._member_map_.values():
-            if x.value[2] == value:
-                return x
-        raise ValueError(f"{value} is not a valid dead_id value")
-
-    @property
-    def IS_GAIA_ONLY(self):
-        return self.value[3]
-
-    @staticmethod
-    def gaia_only():
-        result = []
-        for x in BuildingInfo:
-            if x.IS_GAIA:
-                result.append(x)
-        return result
-
-    @staticmethod
-    def non_gaia():
-        result = []
-        for x in BuildingInfo:
-            if not x.IS_GAIA:
-                result.append(x)
-        return result
-
-    RUINS = 345, -1, -1, True
-    AACHEN_CATHEDRAL = 1622, 37, 1517, False
-    AMPHITHEATRE = 251, 58, 1514, False
-    AQUEDUCT = 231, 52, 1522, False
-    ARCH_OF_CONSTANTINE = 899, 37, 1485, False
-    ARCHERY_RANGE = 87, 0, 1415, False
-    ARMY_TENT_A = 1196, 76, 1467, False
-    ARMY_TENT_B = 1197, 76, 1468, False
-    ARMY_TENT_C = 1198, 77, 1469, False
-    ARMY_TENT_D = 1199, 77, 1470, False
-    ARMY_TENT_E = 1200, 77, 1471, False
-    BARRACKS = 12, 2, 1402, False
-    BLACKSMITH = 103, 4, 1419, False
-    BOMBARD_TOWER = 236, 42, 1439, False
-    BRIDGE_A_BOTTOM = 607, -1, 144, False
-    BRIDGE_A_BROKEN_BOTTOM = 740, -1, 144, False
-    BRIDGE_A_BROKEN_TOP = 739, -1, 144, False
-    BRIDGE_A_CRACKED = 738, -1, 144, False
-    BRIDGE_A_MIDDLE = 606, -1, 144, False
-    BRIDGE_A_TOP = 605, -1, 144, False
-    BRIDGE_B_BOTTOM = 610, -1, 144, False
-    BRIDGE_B_BROKEN_BOTTOM = 743, -1, 144, False
-    BRIDGE_B_BROKEN_TOP = 742, -1, 144, False
-    BRIDGE_B_CRACKED = 741, -1, 144, False
-    BRIDGE_B_MIDDLE = 609, -1, 144, False
-    BRIDGE_B_TOP = 608, -1, 144, False
-    BRIDGE_C_BOTTOM = 1206, -1, 144, False
-    BRIDGE_C_BROKEN_BOTTOM = 1212, -1, 144, False
-    BRIDGE_C_BROKEN_TOP = 1211, -1, 144, False
-    BRIDGE_C_CRACKED = 1210, -1, 144, False
-    BRIDGE_C_MIDDLE = 1205, -1, 144, False
-    BRIDGE_C_TOP = 1204, -1, 144, False
-    BRIDGE_D_BOTTOM = 1209, -1, 144, False
-    BRIDGE_D_BROKEN_BOTTOM = 1215, -1, 144, False
-    BRIDGE_D_BROKEN_TOP = 1214, -1, 144, False
-    BRIDGE_D_CRACKED = 1213, -1, 144, False
-    BRIDGE_D_MIDDLE = 1208, -1, 144, False
-    BRIDGE_D_TOP = 1207, -1, 144, False
-    BRIDGE_E_BOTTOM = 1552, -1, 144, False
-    BRIDGE_E_BROKEN_BOTTOM = 1558, -1, 144, False
-    BRIDGE_E_BROKEN_TOP = 1557, -1, 144, False
-    BRIDGE_E_CRACKED = 1556, -1, 144, False
-    BRIDGE_E_MIDDLE = 1551, -1, 144, False
-    BRIDGE_E_TOP = 1550, -1, 144, False
-    BRIDGE_F_BOTTOM = 1555, -1, 144, False
-    BRIDGE_F_BROKEN_BOTTOM = 1561, -1, 144, False
-    BRIDGE_F_BROKEN_TOP = 1560, -1, 144, False
-    BRIDGE_F_CRACKED = 1559, -1, 144, False
-    BRIDGE_F_MIDDLE = 1554, -1, 144, False
-    BRIDGE_F_TOP = 1553, -1, 144, False
-    CASTLE = 82, 7, 1430, False
-    CATHEDRAL = 599, 11, 1480, False
-    CHAIN_WEST_TO_EAST = 1398, 72, 144, False
-    CHAIN_SOUTHWEST_TO_NORTHEAST = 1396, 72, 144, False
-    CHAIN_NORTH_TO_SOUTH = 1399, 72, 144, False
-    CHAIN_NORTHWEST_TO_SOUTHEAST = 1397, 72, 144, False
-    CITY_GATE_WEST_TO_EAST = 1587, 36, 1512, False
-    CITY_GATE_SOUTHWEST_TO_NORTHEAST = 1579, 36, 1510, False
-    CITY_GATE_NORTH_TO_SOUTH = 1591, 36, 1513, False
-    CITY_GATE_NORTHWEST_TO_SOUTHEAST = 1583, 36, 1511, False
-    CITY_WALL = 370, 31, 143, False
-    COLOSSEUM = 263, 58, 1520, False
-    DOCK = 45, 13, -1, False
-    DORMITION_CATHEDRAL = 1369, 37, 1493, False
-    FARM = 50, 35, 357, False
-    FEITORIA = 1021, 53, 1446, False
-    FENCE = 1062, 30, 1065, False
-    FIRE_TOWER = 190, 26, 1438, False
-    FISH_TRAP = 199, 41, 278, False
-    FORTIFIED_PALISADE_WALL = 119, 30, 143, False
-    FORTIFIED_TOWER = 1102, 45, 1444, False
-    FORTIFIED_WALL = 155, 31, 1509, False
-    FORTRESS = 33, 8, 1486, False
-    GATE_NORTHWEST_TO_SOUTHEAST = 88, 36, 1501, False
-    GATE_WEST_TO_EAST = 659, 36, 1502, False
-    GATE_SOUTHWEST_TO_NORTHEAST = 64, 36, 1500, False
-    GATE_NORTH_TO_SOUTH = 667, 36, 1503, False
-    GOL_GUMBAZ = 1217, 37, 1487, False
-    GUARD_TOWER = 234, 25, 1437, False
-    HARBOR = 1189, 56, -1, False
-    HOUSE = 70, 34, 1403, False
-    HUT_A = 1082, 75, 1455, False
-    HUT_B = 1083, 75, 1456, False
-    HUT_C = 1084, 74, 1457, False
-    HUT_D = 1085, 75, 1458, False
-    HUT_E = 1086, 75, 1459, False
-    HUT_F = 1087, 75, 1460, False
-    HUT_G = 1088, 75, 1461, False
-    KEEP = 235, 26, 1438, False
-    KREPOST = 1251, 55, 1479, False
-    LUMBER_CAMP = 562, 40, 1409, False
-    MARKET = 84, 16, 1422, False
-    MILL = 68, 19, 1404, False
-    MINING_CAMP = 584, 39, 1410, False
-    MONASTERY = 104, 10, 1421, False
-    MONUMENT = 826, 37, -1, False
-    OUTPOST = 598, 38, 1405, False
-    PALISADE_GATE_SOUTHWEST_TO_NORTHEAST = 793, 44, 1441, False
-    PALISADE_GATE_WEST_TO_EAST = 797, 44, 1442, False
-    PALISADE_GATE_NORTHWEST_TO_SOUTHEAST = 789, 44, 1440, False
-    PALISADE_GATE_NORTH_TO_SOUTH = 801, 44, 1443, False
-    PALISADE_WALL = 72, 30, 1407, False
-    PYRAMID = 689, 57, 1515, False
-    QUIMPER_CATHEDRAL = 872, 37, 1489, False
-    RICE_FARM = 1187, 35, 1188, False
-    ROCK_CHURCH = 1378, 341, -1, False
-    SANCHI_STUPA = 1216, 37, 1490, False
-    SANKORE_MADRASAH = 1367, 37, 1491, False
-    SEA_GATE_SOUTHWEST_TO_NORTHEAST = 1379, 71, -1, False
-    SEA_GATE_NORTH_TO_SOUTH = 1391, 71, -1, False
-    SEA_GATE_WEST_TO_EAST = 1387, 71, -1, False
-    SEA_GATE_NORTHWEST_TO_SOUTHEAST = 1383, 71, -1, False
-    SEA_TOWER = 785, 25, -1, False
-    SEA_WALL = 788, 30, -1, False
-    SHRINE = 1264, 12, 1483, False
-    SIEGE_WORKSHOP = 49, 22, 1425, False
-    STABLE = 101, 23, 1417, False
-    STONE_WALL = 117, 31, 1508, False
-    STORAGE = 1081, 59, 1484, False
-    TEMPLE_OF_HEAVEN = 637, 11, 1481, False
-    TENT_A = 1097, 78, 1462, False
-    TENT_B = 1098, 83, 1463, False
-    TENT_C = 1099, 83, 1464, False
-    TENT_D = 1100, 83, 1465, False
-    TENT_E = 1101, 83, 1466, False
-    TOWER_OF_LONDON = 1368, 37, 1492, False
-    TOWN_CENTER = 109, 28, 1408, False
-    TRADE_WORKSHOP = 110, 17, 1429, False
-    UNIVERSITY = 209, 32, 1427, False
-    WATCH_TOWER = 79, 25, 1436, False
-    WONDER = 276, 37, 1445, False
-    WOODEN_BRIDGE_A_BOTTOM = 1311, -1, 144, False
-    WOODEN_BRIDGE_A_MIDDLE = 1310, -1, 144, False
-    WOODEN_BRIDGE_A_TOP = 1309, -1, 144, False
-    WOODEN_BRIDGE_B_BOTTOM = 1314, -1, 144, False
-    WOODEN_BRIDGE_B_MIDDLE = 1313, -1, 144, False
-    WOODEN_BRIDGE_B_TOP = 1312, -1, 144, False
-    YURT_A = 712, 81, 1447, False
-    YURT_B = 713, 82, 1448, False
-    YURT_C = 714, 82, 1449, False
-    YURT_D = 715, 82, 1450, False
-    YURT_E = 716, 80, 1451, False
-    YURT_F = 717, 80, 1452, False
-    YURT_G = 718, 80, 1453, False
-    YURT_H = 719, 79, 1454, False
-    DONJON = 1665, 84, 1524, False
-    TRADE_WORKSHOP_BR = 1647, 17, 1429, False
-    TRADE_WORKSHOP_TG = 179, 17, 1429, False
+class BuildingInfo(InfoDatasetBase):
+    RUINS = 345, -1, -1, 16393, True
+    AACHEN_CATHEDRAL = 1622, 37, 1517, 16182, False
+    AMPHITHEATRE = 251, 58, 1514, 16572, False
+    AQUEDUCT = 231, 52, 1522, 16201, False
+    ARCH_OF_CONSTANTINE = 899, 37, 1485, 16572, False
+    ARCHERY_RANGE = 87, 0, 1415, 16128, False
+    ARMY_TENT_A = 1196, 76, 1467, 16521, False
+    ARMY_TENT_B = 1197, 76, 1468, 16521, False
+    ARMY_TENT_C = 1198, 77, 1469, 16522, False
+    ARMY_TENT_D = 1199, 77, 1470, 16523, False
+    ARMY_TENT_E = 1200, 77, 1471, 16522, False
+    BARRACKS = 12, 2, 1402, 16135, False
+    BLACKSMITH = 103, 4, 1419, 16131, False
+    BOMBARD_TOWER = 236, 42, 1439, 16156, False
+    BRIDGE_A_BOTTOM = 607, -1, 144, 16513, False
+    BRIDGE_A_BROKEN_BOTTOM = 740, -1, 144, 16643, False
+    BRIDGE_A_BROKEN_TOP = 739, -1, 144, 16642, False
+    BRIDGE_A_CRACKED = 738, -1, 144, 16641, False
+    BRIDGE_A_MIDDLE = 606, -1, 144, 16512, False
+    BRIDGE_A_TOP = 605, -1, 144, 16511, False
+    BRIDGE_B_BOTTOM = 610, -1, 144, 16516, False
+    BRIDGE_B_BROKEN_BOTTOM = 743, -1, 144, 16646, False
+    BRIDGE_B_BROKEN_TOP = 742, -1, 144, 16645, False
+    BRIDGE_B_CRACKED = 741, -1, 144, 16644, False
+    BRIDGE_B_MIDDLE = 609, -1, 144, 16515, False
+    BRIDGE_B_TOP = 608, -1, 144, 16514, False
+    BRIDGE_C_BOTTOM = 1206, -1, 144, 16513, False
+    BRIDGE_C_BROKEN_BOTTOM = 1212, -1, 144, 16643, False
+    BRIDGE_C_BROKEN_TOP = 1211, -1, 144, 16642, False
+    BRIDGE_C_CRACKED = 1210, -1, 144, 16641, False
+    BRIDGE_C_MIDDLE = 1205, -1, 144, 16512, False
+    BRIDGE_C_TOP = 1204, -1, 144, 16511, False
+    BRIDGE_D_BOTTOM = 1209, -1, 144, 16516, False
+    BRIDGE_D_BROKEN_BOTTOM = 1215, -1, 144, 16646, False
+    BRIDGE_D_BROKEN_TOP = 1214, -1, 144, 16645, False
+    BRIDGE_D_CRACKED = 1213, -1, 144, 16644, False
+    BRIDGE_D_MIDDLE = 1208, -1, 144, 16515, False
+    BRIDGE_D_TOP = 1207, -1, 144, 16514, False
+    BRIDGE_E_BOTTOM = 1552, -1, 144, 16513, False
+    BRIDGE_E_BROKEN_BOTTOM = 1558, -1, 144, 16643, False
+    BRIDGE_E_BROKEN_TOP = 1557, -1, 144, 16642, False
+    BRIDGE_E_CRACKED = 1556, -1, 144, 16641, False
+    BRIDGE_E_MIDDLE = 1551, -1, 144, 16512, False
+    BRIDGE_E_TOP = 1550, -1, 144, 16511, False
+    BRIDGE_F_BOTTOM = 1555, -1, 144, 16516, False
+    BRIDGE_F_BROKEN_BOTTOM = 1561, -1, 144, 16646, False
+    BRIDGE_F_BROKEN_TOP = 1560, -1, 144, 16645, False
+    BRIDGE_F_CRACKED = 1559, -1, 144, 16644, False
+    BRIDGE_F_MIDDLE = 1554, -1, 144, 16515, False
+    BRIDGE_F_TOP = 1553, -1, 144, 16514, False
+    CASTLE = 82, 7, 1430, 16142, False
+    CATHEDRAL = 599, 11, 1480, 16505, False
+    CHAIN_WEST_TO_EAST = 1398, 72, 144, 16186, False
+    CHAIN_SOUTHWEST_TO_NORTHEAST = 1396, 72, 144, 16186, False
+    CHAIN_NORTH_TO_SOUTH = 1399, 72, 144, 16186, False
+    CHAIN_NORTHWEST_TO_SOUTHEAST = 1397, 72, 144, 16186, False
+    CITY_GATE_WEST_TO_EAST = 1587, 36, 1512, 16044, False
+    CITY_GATE_SOUTHWEST_TO_NORTHEAST = 1579, 36, 1510, 16044, False
+    CITY_GATE_NORTH_TO_SOUTH = 1591, 36, 1513, 16044, False
+    CITY_GATE_NORTHWEST_TO_SOUTHEAST = 1583, 36, 1511, 16044, False
+    CITY_WALL = 370, 31, 143, 16201, False
+    COLOSSEUM = 263, 58, 1520, 16505, False
+    DOCK = 45, 13, -1, 16144, False
+    DORMITION_CATHEDRAL = 1369, 37, 1493, 16182, False
+    FARM = 50, 35, 357, 16149, False
+    FEITORIA = 1021, 53, 1446, 16159, False
+    FENCE = 1062, 30, 1065, 16797, False
+    FIRE_TOWER = 190, 26, 1438, 16158, False
+    FISH_TRAP = 199, 41, 278, 16495, False
+    FORTIFIED_PALISADE_WALL = 119, 30, 143, 16202, False
+    FORTIFIED_TOWER = 1102, 45, 1444, 16231, False
+    FORTIFIED_WALL = 155, 31, 1509, 16204, False
+    FORTRESS = 33, 8, 1486, 16142, False
+    GATE_NORTHWEST_TO_SOUTHEAST = 88, 36, 1501, 16185, False
+    GATE_WEST_TO_EAST = 659, 36, 1502, 16185, False
+    GATE_SOUTHWEST_TO_NORTHEAST = 64, 36, 1500, 16185, False
+    GATE_NORTH_TO_SOUTH = 667, 36, 1503, 16185, False
+    GOL_GUMBAZ = 1217, 37, 1487, 16578, False
+    GUARD_TOWER = 234, 25, 1437, 16154, False
+    HARBOR = 1189, 56, -1, 16144, False
+    HOUSE = 70, 34, 1403, 16344, False
+    HUT_A = 1082, 75, 1455, 16221, False
+    HUT_B = 1083, 75, 1456, 16221, False
+    HUT_C = 1084, 74, 1457, 16221, False
+    HUT_D = 1085, 75, 1458, 16221, False
+    HUT_E = 1086, 75, 1459, 16221, False
+    HUT_F = 1087, 75, 1460, 16221, False
+    HUT_G = 1088, 75, 1461, 16221, False
+    KEEP = 235, 26, 1438, 16155, False
+    KREPOST = 1251, 55, 1479, 16349, False
+    LUMBER_CAMP = 562, 40, 1409, 16464, False
+    MARKET = 84, 16, 1422, 16161, False
+    MILL = 68, 19, 1404, 16157, False
+    MINING_CAMP = 584, 39, 1410, 16487, False
+    MONASTERY = 104, 10, 1421, 16138, False
+    MONUMENT = 826, 37, -1, 16726, False
+    OUTPOST = 598, 38, 1405, 16504, False
+    PALISADE_GATE_SOUTHWEST_TO_NORTHEAST = 793, 44, 1441, 16186, False
+    PALISADE_GATE_WEST_TO_EAST = 797, 44, 1442, 16186, False
+    PALISADE_GATE_NORTHWEST_TO_SOUTHEAST = 789, 44, 1440, 16186, False
+    PALISADE_GATE_NORTH_TO_SOUTH = 801, 44, 1443, 16186, False
+    PALISADE_WALL = 72, 30, 1407, 16202, False
+    PYRAMID = 689, 57, 1515, 16571, False
+    QUIMPER_CATHEDRAL = 872, 37, 1489, 16572, False
+    RICE_FARM = 1187, 35, 1188, 16149, False
+    ROCK_CHURCH = 1378, 341, -1, 16182, False
+    SANCHI_STUPA = 1216, 37, 1490, 16578, False
+    SANKORE_MADRASAH = 1367, 37, 1491, 16182, False
+    SEA_GATE_SOUTHWEST_TO_NORTHEAST = 1379, 71, -1, 16186, False
+    SEA_GATE_NORTH_TO_SOUTH = 1391, 71, -1, 16186, False
+    SEA_GATE_WEST_TO_EAST = 1387, 71, -1, 16186, False
+    SEA_GATE_NORTHWEST_TO_SOUTHEAST = 1383, 71, -1, 16186, False
+    SEA_TOWER = 785, 25, -1, 16704, False
+    SEA_WALL = 788, 30, -1, 16707, False
+    SHRINE = 1264, 12, 1483, 16138, False
+    SIEGE_WORKSHOP = 49, 22, 1425, 16169, False
+    STABLE = 101, 23, 1417, 16171, False
+    STONE_WALL = 117, 31, 1508, 16203, False
+    STORAGE = 1081, 59, 1484, 16219, False
+    TEMPLE_OF_HEAVEN = 637, 11, 1481, 16505, False
+    TENT_A = 1097, 78, 1462, 16230, False
+    TENT_B = 1098, 83, 1463, 16230, False
+    TENT_C = 1099, 83, 1464, 16230, False
+    TENT_D = 1100, 83, 1465, 16230, False
+    TENT_E = 1101, 83, 1466, 16230, False
+    TOWER_OF_LONDON = 1368, 37, 1492, 16182, False
+    TOWN_CENTER = 109, 28, 1408, 16164, False
+    TRADE_WORKSHOP = 110, 17, 1429, 16174, False
+    UNIVERSITY = 209, 32, 1427, 16176, False
+    WATCH_TOWER = 79, 25, 1436, 16178, False
+    WONDER = 276, 37, 1445, 16182, False
+    WOODEN_BRIDGE_A_BOTTOM = 1311, -1, 144, 16513, False
+    WOODEN_BRIDGE_A_MIDDLE = 1310, -1, 144, 16512, False
+    WOODEN_BRIDGE_A_TOP = 1309, -1, 144, 16511, False
+    WOODEN_BRIDGE_B_BOTTOM = 1314, -1, 144, 16516, False
+    WOODEN_BRIDGE_B_MIDDLE = 1313, -1, 144, 16515, False
+    WOODEN_BRIDGE_B_TOP = 1312, -1, 144, 16514, False
+    YURT_A = 712, 81, 1447, 16594, False
+    YURT_B = 713, 82, 1448, 16595, False
+    YURT_C = 714, 82, 1449, 16596, False
+    YURT_D = 715, 82, 1450, 16597, False
+    YURT_E = 716, 80, 1451, 16598, False
+    YURT_F = 717, 80, 1452, 16599, False
+    YURT_G = 718, 80, 1453, 16600, False
+    YURT_H = 719, 79, 1454, 16601, False
+    DONJON = 1665, 84, 1524, 16350, False
+    TRADE_WORKSHOP_BR = 1647, 17, 1429, 16174, False
+    TRADE_WORKSHOP_TG = 179, 17, 1429, 16174, False
+    TOWN_CENTER_PACKED = 444, 264, 1274, 16311, False
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/conditions.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/conditions.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Attributes for the **none**  condition are:\n
     ... It's called none... What parameters do **you** think it has?! ❤ 
     """
     BRING_OBJECT_TO_AREA = 1
     """
     Attributes for the **bring_object_to_area** condition are:\n
     - unit_object  
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - inverted
     """
     BRING_OBJECT_TO_OBJECT = 2
     """
     Attributes for the **bring_object_to_object** condition are:\n
     - unit_object
     - next_object
@@ -37,31 +37,31 @@
     """
     OWN_FEWER_OBJECTS = 4
     """
     Attributes for the **own_fewer_objects** condition are:\n
     - quantity
     - object_list
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     """
     OBJECTS_IN_AREA = 5
     """
     Attributes for the **object_in_area** condition are:\n
     - quantity
     - object_list
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - inverted
     """
     DESTROY_OBJECT = 6
     """
     Attributes for the **destroy_object** condition are:\n
@@ -255,18 +255,18 @@
     "attribute": -1,
     "unit_object": -1,
     "next_object": -1,
     "object_list": -1,
     "source_player": -1,
     "technology": -1,
     "timer": -1,
-    "area_1_x": -1,
-    "area_1_y": -1,
-    "area_2_x": -1,
-    "area_2_y": -1,
+    "area_x1": -1,
+    "area_y1": -1,
+    "area_x2": -1,
+    "area_y2": -1,
     "object_group": -1,
     "object_type": -1,
     "ai_signal": -1,
     "inverted": -1,
     "variable": -1,
     "comparison": -1,
     "target_player": -1,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/effects.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/effects.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,92 +62,91 @@
     TASK_OBJECT = 12
     """Attributes for the **task_object** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y
     - location_object_reference
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     DECLARE_VICTORY = 13
     """Attributes for the **declare_victory** effect are: \n
     - source_player
     - enabled"""
     KILL_OBJECT = 14
     """Attributes for the **kill_object** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     REMOVE_OBJECT = 15
     """Attributes for the **remove_object** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     CHANGE_VIEW = 16
     """Attributes for the **change_view** effect are: \n
     - source_player
     - location_x
     - location_y
-    - location_object_reference
     - scroll"""
     UNLOAD = 17
     """Attributes for the **unload** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y
     - location_object_reference
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     CHANGE_OWNERSHIP = 18
     """Attributes for the **change_ownership** effect are: \n
     - object_list_unit_id
     - source_player
     - target_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - flash_object
     - selected_object_ids"""
     PATROL = 19
     """Attributes for the **patrol** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y
     - location_object_reference
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     DISPLAY_INSTRUCTIONS = 20
     """Attributes for the **display_instructions** effect are: \n
     - object_list_unit_id
     - source_player
@@ -160,178 +159,178 @@
     CLEAR_INSTRUCTIONS = 21
     """Attributes for the **clear_instructions** effect are: \n
     - instruction_panel_position"""
     FREEZE_OBJECT = 22
     """Attributes for the **freeze_object** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     USE_ADVANCED_BUTTONS = 23
     """Attributes for the **use_advanced_buttons** effect are: \n
     None. \n
     Please don't use this effect. Please."""
     DAMAGE_OBJECT = 24
     """Attributes for the **damage_object** effect are: \n
     - quantity
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     PLACE_FOUNDATION = 25
     """Attributes for the **place_foundation** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y"""
     CHANGE_OBJECT_NAME = 26
     """Attributes for the **change_object_name** effect are: \n
     - object_list_unit_id
     - source_player
     - string_id
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - message
     - selected_object_ids"""
     CHANGE_OBJECT_HP = 27
     """Attributes for the **change_object_hp** effect are: \n
     - quantity
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - operation
     - selected_object_ids"""
     CHANGE_OBJECT_ATTACK = 28
     """Attributes for the **change_object_attack** effect are: \n
     - armour_attack_quantity
     - armour_attack_class
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - operation
     - selected_object_ids"""
     STOP_OBJECT = 29
     """Attributes for the **stop_object** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     ATTACK_MOVE = 30
     """Attributes for the **attack_move** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y
     - location_object_reference
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     CHANGE_OBJECT_ARMOR = 31
     """Attributes for the **change_object_armor** effect are: \n
     - armour_attack_quantity
     - armour_attack_class
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - operation
     - selected_object_ids"""
     CHANGE_OBJECT_RANGE = 32
     """Attributes for the **change_object_range** effect are: \n
     - quantity
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - operation
     - selected_object_ids"""
     CHANGE_OBJECT_SPEED = 33
     """Attributes for the **change_object_speed** effect are: \n
     - quantity
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     HEAL_OBJECT = 34
     """Attributes for the **heal_object** effect are: \n
     - quantity
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     TELEPORT_OBJECT = 35
     """Attributes for the **teleport_object** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - selected_object_ids"""
     CHANGE_OBJECT_STANCE = 36
     """Attributes for the **change_object_stance** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - attack_stance
     - selected_object_ids"""
     DISPLAY_TIMER = 37
     """Attributes for the **display_timer** effect are: \n
     - string_id
@@ -364,31 +363,31 @@
     - source_player
     - target_player
     - visibility_state"""
     CHANGE_OBJECT_ICON = 42
     """Attributes for the **change_object_icon** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - object_list_unit_id_2
     - selected_object_ids"""
     REPLACE_OBJECT = 43
     """Attributes for the **replace_object** effect are: \n
     - object_list_unit_id
     - source_player
     - target_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_group
     - object_type
     - object_list_unit_id_2
     - selected_object_ids"""
     CHANGE_OBJECT_DESCRIPTION = 44
     """Attributes for the **change_object_description** effect are: \n
     - object_list_unit_id
@@ -417,18 +416,18 @@
     - source_player
     - string_id
     - message"""
     CREATE_GARRISONED_OBJECT = 49
     """Attributes for the **create_garrisoned_object** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - object_list_unit_id_2
     - selected_object_ids"""
     ACKNOWLEDGE_AI_SIGNAL = 50
     """Attributes for the **acknowledge_ai_signal** effect are: \n
     - ai_signal_value"""
     MODIFY_ATTRIBUTE = 51
     """Attributes for the **modify_attribute** effect are: \n
@@ -454,18 +453,18 @@
     - variable"""
     SET_BUILDING_GATHER_POINT = 54
     """Attributes for the **set_building_gather_point** effect are: \n
     - object_list_unit_id
     - source_player
     - location_x
     - location_y
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     SCRIPT_CALL = 55
     """Attributes for the **script_call** effect are: \n
     - string_id
     - message"""
     CHANGE_VARIABLE = 56
     """Attributes for the **change_variable** effect are: \n
@@ -476,55 +475,55 @@
     CLEAR_TIMER = 57
     """Attributes for the **clear_timer** effect are: \n
     - timer"""
     CHANGE_OBJECT_PLAYER_COLOR = 58
     """Attributes for the **change_object_player_color** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - player_color
     - selected_object_ids"""
     CHANGE_OBJECT_CIVILIZATION_NAME = 59
     """Attributes for the **change_object_civilization_name** effect are: \n
     - string_id
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     CHANGE_OBJECT_PLAYER_NAME = 60
     """Attributes for the **change_object_player_name** effect are: \n
     - object_list_unit_id
     - source_player
     - string_id
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     DISABLE_UNIT_TARGETING = 61
     """Attributes for the **disable_unit_targeting** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     ENABLE_UNIT_TARGETING = 62
     """Attributes for the **enable_unit_targeting** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     CHANGE_TECHNOLOGY_COST = 63
     """Attributes for the **change_technology_cost** effect are: \n
     - source_player
     - technology
     - food
     - wood
@@ -559,27 +558,27 @@
     """Attributes for the **acknowledge_multiplayer_ai_signal** effect are: \n
     - ai_signal_value
     """
     DISABLE_OBJECT_SELECTION = 70
     """Attributes for the **disable_object_selection** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     ENABLE_OBJECT_SELECTION = 71
     """Attributes for the **enable_object_selection** effect are: \n
     - object_list_unit_id
     - source_player
-    - area_1_x
-    - area_1_y
-    - area_2_x
-    - area_2_y
+    - area_x1
+    - area_y1
+    - area_x2
+    - area_y2
     - selected_object_ids"""
     # Possibly used for marking when achievements should be achieved. Doesn't seem to work in scenario's. F
     # UNKNOWN_0 = 58  # Was 58... Not anymore (?)
 
 
 empty_attributes = {
     "effect_type": -1,
@@ -595,18 +594,18 @@
     "technology": -1,
     "string_id": -1,
     "display_time": -1,
     "trigger_id": -1,
     "location_x": -1,
     "location_y": -1,
     "location_object_reference": -1,
-    "area_1_x": -1,
-    "area_1_y": -1,
-    "area_2_x": -1,
-    "area_2_y": -1,
+    "area_x1": -1,
+    "area_y1": -1,
+    "area_x2": -1,
+    "area_y2": -1,
     "object_group": -1,
     "object_type": -1,
     "instruction_panel_position": -1,
     "attack_stance": -1,
     "time_unit": -1,
     "enabled": -1,
     "food": -1,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/scripts/get_icon_ids.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/scripts/get_icon_ids.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/scripts/object_parser.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/scripts/object_parser.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/techs.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/techs.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,22 +34,22 @@
             TechInfo.YEOMEN, TechInfo.EL_DORADO, TechInfo.FUROR_CELTICA, TechInfo.DRILL, TechInfo.MAHOUTS,
             TechInfo.ZEALOTRY, TechInfo.ARTILLERY, TechInfo.CRENELLATIONS, TechInfo.ANARCHY, TechInfo.ATHEISM,
             TechInfo.GARLAND_WARS, TechInfo.BERSERKERGANG, TechInfo.ROCKETRY, TechInfo.KATAPARUTO, TechInfo.LOGISTICA,
             TechInfo.BEARDED_AXE, TechInfo.SUPREMACY, TechInfo.SHINKICHON, TechInfo.PERFUSION, TechInfo.ATLATL,
             TechInfo.WARWOLF, TechInfo.GREAT_WALL, TechInfo.CHIEFTAINS, TechInfo.GREEK_FIRE, TechInfo.STRONGHOLD,
             TechInfo.MARAUDERS, TechInfo.YASAMA, TechInfo.OBSIDIAN_ARROWS, TechInfo.PANOKSEON, TechInfo.NOMADS,
             TechInfo.KAMANDARAN, TechInfo.IRONCLAD, TechInfo.MADRASAH, TechInfo.SIPAHI, TechInfo.INQUISITION,
-            TechInfo.CHIVALRY, TechInfo.PAVISE, TechInfo.SILK_ROAD, TechInfo.SULTANS, TechInfo.SHATAGNI,
-            TechInfo.ORTHODOXY, TechInfo.DRUZHINA, TechInfo.CORVINIAN_ARMY, TechInfo.RECURVE_BOW, TechInfo.ANDEAN_SLING,
-            TechInfo.COURIERS, TechInfo.CARRACK, TechInfo.ARQUEBUS, TechInfo.ROYAL_HEIRS, TechInfo.TORSION_ENGINES,
-            TechInfo.TIGUI, TechInfo.FARIMBA, TechInfo.KASBAH, TechInfo.MAGHRABI_CAMELS, TechInfo.TUSK_SWORDS,
-            TechInfo.DOUBLE_CROSSBOW, TechInfo.THALASSOCRACY, TechInfo.FORCED_LEVY, TechInfo.HOWDAH,
-            TechInfo.MANIPUR_CAVALRY, TechInfo.CHATRAS, TechInfo.PAPER_MONEY, TechInfo.STIRRUPS, TechInfo.BAGAINS,
-            TechInfo.SILK_ARMOR, TechInfo.TIMURID_SIEGECRAFT, TechInfo.STEPPE_HUSBANDRY, TechInfo.CUMAN_MERCENARIES,
-            TechInfo.HILL_FORTS, TechInfo.TOWER_SHIELDS, TechInfo.BURGUNDIAN_VINEYARDS, TechInfo.FELMISH_REVOLUTION,
+            TechInfo.CHIVALRY, TechInfo.PAVISE, TechInfo.SILK_ROAD, TechInfo.SULTANS, TechInfo.SHATAGNI, 
+            TechInfo.ORTHODOXY, TechInfo.DRUZHINA, TechInfo.CORVINIAN_ARMY, TechInfo.RECURVE_BOW, TechInfo.ANDEAN_SLING, 
+            TechInfo.COURIERS, TechInfo.CARRACK, TechInfo.ARQUEBUS, TechInfo.ROYAL_HEIRS, TechInfo.TORSION_ENGINES, 
+            TechInfo.TIGUI, TechInfo.FARIMBA, TechInfo.KASBAH, TechInfo.MAGHRABI_CAMELS, TechInfo.TUSK_SWORDS, 
+            TechInfo.DOUBLE_CROSSBOW, TechInfo.THALASSOCRACY, TechInfo.FORCED_LEVY, TechInfo.HOWDAH, 
+            TechInfo.MANIPUR_CAVALRY, TechInfo.CHATRAS, TechInfo.PAPER_MONEY, TechInfo.STIRRUPS, TechInfo.BAGAINS, 
+            TechInfo.SILK_ARMOR, TechInfo.TIMURID_SIEGECRAFT, TechInfo.STEPPE_HUSBANDRY, TechInfo.CUMAN_MERCENARIES, 
+            TechInfo.HILL_FORTS, TechInfo.TOWER_SHIELDS, TechInfo.BURGUNDIAN_VINEYARDS, TechInfo.FLEMISH_REVOLUTION,
             TechInfo.FIRST_CRUSADE, TechInfo.SCUTAGE,
         ]
 
     ANARCHY = 16, 33
     ANDEAN_SLING = 516, 33
     ARBALESTER = 237, 54
     ARCHITECTURE = 51, 14
@@ -319,10 +319,11 @@
     WHEELBARROW = 213, 79
     YASAMA = 484, 33
     YEOMEN = 3, 33
     ZEALOTRY = 9, 107
     SICILIANS = 749, -1
     BURGUNDIANS = 748, -1
     BURGUNDIAN_VINEYARDS = 754, 33
-    FELMISH_REVOLUTION = 755, 107
+    FLEMISH_REVOLUTION = 755, 107
     FIRST_CRUSADE = 756, 33
     SCUTAGE = 757, 107
+    CONVERSION_ENABLER = 243, -1
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/terrains.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/terrains.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/trigger_lists.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/trigger_lists.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     AGGRESSIVE_STANCE = 0
     DEFENSIVE_STANCE = 1
     STAND_GROUND = 2
     NO_ATTACK_STANCE = 3
 
 
 class UnitAIAction(IntEnum):
+    """Detailed introduction: [https://airef.github.io/parameters/parameters-details.html#ActionId]"""
     ANY = 0
     ATTACK = 1
     BUILD = 3
     CONVERT = 5
     DEFEND = 2
     ENTER = 18
     EVADE = 17
@@ -61,14 +62,15 @@
     r2c3 = 8
     r2c4 = 9
     r2c5 = 10
     r3c1 = 11
     r3c2 = 12
     r3c3 = 13
     r3c4 = 14
+
     # r3c5 = 15  # Doesn't actually work in-game. Probably to make space for the arrow key.
 
     @classmethod
     def row_col(cls, row, col):
         return cls((row - 1) * 5 + col)
 
 
@@ -135,36 +137,38 @@
     ATTACK_RELOAD_TIME = 10
     ACCURACY_PERCENT = 11
     MAX_RANGE = 12
     WORK_RATE = 13
     CARRY_CAPACITY = 14
     BASE_ARMOR = 15
     PROJECTILE_UNIT = 16
-    ICON_GRAPHICS_ANGLE = 17
+    GRAPHICS_ANGLE = 17
     TERRAIN_DEFENSE_BONUS = 18
     ENABLE_SMART_PROJECTILES = 19
     MINIMUM_RANGE = 20
     AMOUNT_OF_1ST_RESOURCES = 21
     BLAST_WIDTH = 22
     SEARCH_RADIUS = 23
     BONUS_DAMAGE_RESIST = 24
     ICON_ID = 25
     HERO_STATUS = 40
     FRAME_DELAY = 41
     TRAIN_LOCATION = 42
     TRAIN_BUTTON = 43
-    BLAST_LEVEL = 44
+    BLAST_ATTACK_LEVEL = 44
+    BLAST_DEFENSE_LEVEL = 45
     SHOWN_ATTACK = 46
     SHOWN_RANGE = 47
     SHOWN_MELEE_ARMOR = 48
     SHOWN_PIERCE_ARMOR = 49
     OBJECT_NAME_ID = 50
     SHORT_DESCRIPTION_ID = 51
     TERRAIN_RESTRICTION_ID = 53
     DEAD_UNIT_ID = 57
+    HOTKEY_ID = 58
     RESOURCE_COSTS = 100
     TRAIN_TIME = 101
     TOTAL_MISSILES = 102
     FOOD_COSTS = 103
     WOOD_COSTS = 104
     GOLD_COSTS = 105
     STONE_COSTS = 106
@@ -763,15 +767,15 @@
     """Stone Given per Minute to the Source Player"""
     GOLD_TRICKLE = 233
     """Gold Given per Minute to the Source Player"""
     SPAWN_LIMIT = 234
     """Number of buildings from which a tech with command type 7 (spawn) will spawn units"""
     FLEMISH_MILITIA_POPULATION = 235
     """Number of Flemish Militia of the Source Player"""
-    FARMING_GOLD_TRICKLE = 235
+    FARMING_GOLD_TRICKLE = 236
     """
     Farming Gold Generation Rate*0.01 of the Source Player:
 
     - Burgundian Vineyards set this to 1.5 => 0.015g/s for One Farmer Continuously Farming.
     - in Practise, Its Closer to 0.01g/s Factoring in Walking Times
     """
 
@@ -846,37 +850,215 @@
     KING = 59
     MISC_BUILDING = 60
     CONTROLLED_ANIMAL = 61
 
 
 class TerrainRestrictions(IntEnum):
     ALL = 0
+    """Used by terrain eyecandy and sundries."""
     LAND_AND_SHALLOWS = 1
+    """Used by part of animals."""
     BEACH = 2
     WATER_SMALL_TRAIL = 3
+    """Used by most ships and sea gate."""
     LAND = 4
+    """Used by most land buildings."""
     NOTHING = 5
     WATER_NO_TRAIL = 6
+    """Used by docks."""
     ALL_EXCEPT_WATER = 7
+    """Used by land troops."""
     LAND_EXCEPT_FARM = 8
+    """Used by land resources."""
     NOTHING_2 = 9
     LAND_AND_BEACH = 10
+    """Used by land walls and gates."""
     LAND_EXCEPT_FARM_2 = 11
+    """Used by trees and mountains."""
     ALL_EXCEPT_WATER_BRIDGE_CANNON = 12
     WATER_MEDIUM_TRAIL = 13
-    ALL_EXCEPT_WATER_BRIDGE = 14
+    """Used by big fish and fishing ship."""
+    ALL_EXCEPT_WATER_BRIDGE_ARROW = 14
     WATER_LARGE_TRAIL = 15
+    """Only used by transport ship."""
     GRASS_AND_BEACH = 16
     WATER_AND_BRIDGE_EXCEPT_BEACH = 17
     ALL_EXCEPT_WATER_BRIDGE_SPEAR = 18
     ONLY_WATER_AND_ICE = 19
-    ALL_EXCEPT_WATER2 = 20
+    """Used by fish."""
+    ALL_EXCEPT_WATER_WHEEL = 20
+    """Used by units with wheels, such as Rams and Scorpions."""
     SHALLOW_WATER = 21
     ALL_DART = 22
-    ALL_ARROW = 23
-    ALL_CANNON = 24
-    ALL_SPEAR = 25
-    ALL_DART2 = 26
-    ALL_EXPLOSION = 27
-    UNKNOWN = 28
-    UNKNOWN_2 = 29
+    ALL_ARROW_FIRE = 23
+    """Only used by Arrows with fire (After chemistry)."""
+    ALL_CANNON_FIRE = 24
+    """Only used by Cannon balls (After chemistry)."""
+    ALL_SPEAR_FIRE = 25
+    """Only used by Spears with fire (After chemistry)."""
+    ALL_DART_FIRE = 26
+    """Only used by Darts with fire (After chemistry)."""
+    ALL_LASER = 27
+    """Only used by Projectile Laser with id 1595"""
+    ALL_EXCEPT_WATER_CAVALRY = 28
+    """Such as Cavalry Archer, Cavalry, Conquistador, Missionary and Flaming Camel."""
+    ALL_EXCEPT_WATER_PACKET_TREBUCHET = 29
+    """All types of Trebuchet(Packed)."""
     WATER_SMALLEST_TRAIL = 30
+    """Used by medium ships, such as Trade Cog, Fire Galley and Longboat."""
+
+
+class HeroStatusFlag(IntEnum):
+    @staticmethod
+    def combine(
+            hero_regeneration=False,
+            cannot_be_converted=False,
+            defensive_stance_by_default=False,
+            protected_formation=False,
+            delete_confirmation=False):
+
+        total = 2 if cannot_be_converted else 0
+        total += 4 if hero_regeneration else 0
+        total += 8 if defensive_stance_by_default else 0
+        total += 16 if protected_formation else 0
+        total += 32 if delete_confirmation else 0
+        return total
+
+    FULL_HERO_STATUS = 1
+    CANNOT_BE_CONVERTED = 2
+    HERO_REGENERATION = 4
+    DEFENSIVE_STANCE_BY_DEFAULT = 8
+    PROTECTED_FORMATION = 16
+    DELETE_CONFIRMATION = 32
+
+
+class BlastLevel(IntEnum):
+    RESOURCES = 0
+    TREES = 1
+    NEARBY_UNITS = 2
+    TARGET_ONLY = 3
+
+
+class DamageClass(IntEnum):
+    WONDER = 0
+    """Since HD. Only wonders has this armour class. However there is no unit having this damage class."""
+    INFANTRY = 1
+    TURTLE_SHIPS = 2
+    BASE_PIERCE = 3
+    BASE_MELEE = 4
+    WAR_ELEPHANTS = 5
+    UNUSED_ID6 = 6
+    UNUSED_ID7 = 7
+    CAVALRY = 8
+    UNUSED_ID9 = 9
+    UNUSED_ID10 = 10
+    ALL_BUILDINGS_EXCEPT_PORT = 11
+    """Port is the building with id 446"""
+    UNUSED_ID12 = 12
+    STONE_DEFENSE = 13
+    PREDATOR_ANIMALS_FE = 14
+    """Wolf, Bear, Jaguar, Tiger, etc. have this armour class"""
+    ARCHERS = 15
+    BATTLE_SHIPS_AND_SABOTEUR = 16
+    """Camels also had this armour class before AK"""
+    RAMS = 17
+    TREES = 18
+    UNIQUE_UNITS = 19
+    SIEGE_WEAPONS = 20
+    STANDARD_BUILDINGS = 21
+    WALLS_AND_GATES = 22
+    GUNPOWDER_UNITS = 23
+    BOARS = 24
+    MONKS = 25
+    CASTLE = 26
+    SPEARMEN = 27
+    CAVALRY_ARCHERS = 28
+    EAGLE_WARRIORS = 29
+    CAMELS = 30
+    """Camels use this armour class since and after AK"""
+    LEITIS = 31
+    CONDOTTIERO = 32
+    ORGAN_GUN_BULLET = 33
+    """Only Projectile Gunpowder (Secondary) with id 1119 has this damage class. No unit has this armour class."""
+    FISHING_SHIP = 34
+    MAMELUKES = 35
+    HEROES_AND_KING = 36
+    UNUSED_ID37 = 37
+    UNUSED_ID38 = 38
+    UNUSED_ID39 = 39
+    UNUSED_ID40 = 40
+    UNUSED_ID41 = 41
+    UNUSED_ID42 = 42
+    UNUSED_ID43 = 43
+    UNUSED_ID44 = 44
+    UNUSED_ID45 = 45
+    UNUSED_ID46 = 46
+    UNUSED_ID47 = 47
+    UNUSED_ID48 = 48
+    UNUSED_ID49 = 49
+
+
+class Hotkey(IntEnum):
+    """
+    Enum for all possible static keys
+
+    Many hotkeys will be missing from this file (Like arrow up). The reason for this is explained in the UGC guide:
+    https://divy1211.github.io/AoE2DE_UGC_Guide/general/hotkeys/hotkeys/
+    We'll try to update this list every update (when new strings are added to the game).
+    """
+
+    SPACE = 10101
+    PAGE_UP = 15000
+    LEFT_ARROW = 2312
+    RIGHT_ARROW = 19707
+    DOWN_ARROW = 19731
+    INSERT = 9025
+    DELETE = 19602
+    ZERO = 99
+    ONE = 98
+    TWO = 10360
+    THREE = 9786
+    FOUR = 10362
+    FIVE = 9785
+    SIX = 213
+    SEVEN = 8828
+    EIGHT = 9448
+    NINE = 9783
+    A = 1001
+    B = 1005
+    C = 1201
+    D = 1151
+    E = 1007
+    F = 4137
+    G = 2012
+    H = 2407
+    I = 1212
+    J = 1222
+    K = 4141
+    L = 1101
+    M = 1006
+    N = 3001
+    O = 214
+    P = 1210
+    Q = 4169
+    R = 1200
+    S = 1102
+    T = 2016
+    U = 1205
+    V = 1150
+    W = 1008
+    X = 1002
+    Y = 2008
+    Z = 4174
+    APPLICATION = 19704
+    NUM_ZERO = 19721
+    NUM_ONE = 4563
+    NUM_FOUR = 19499
+    NUM_FIVE = 5558
+    NUM_SEVEN = 10069
+    NUM_EIGHT = 1011
+    NUM_DELETE = 20123
+    F3 = 9798
+    F4 = 22019
+    F7 = 9840
+    F8 = 1152
+    F15 = 10661
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/datasets/units.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/datasets/units.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,11 @@
-from enum import Enum
+from AoE2ScenarioParser.datasets.support.info_dataset_base import InfoDatasetBase
 
 
-class UnitInfo(Enum):
-    @property
-    def ID(self):
-        return self.value[0]
-
-    @classmethod
-    def from_id(cls, value: int):
-        if type(value) is not int:
-            raise TypeError(f"from_id expected int, got {type(value)}")
-        if value == -1:
-            raise ValueError("-1 is not a valid id value")
-        for x in cls._member_map_.values():
-            if x.value[0] == value:
-                return x
-        raise ValueError(f"{value} is not a valid id value")
-
-    @property
-    def ICON_ID(self):
-        return self.value[1]
-
-    @classmethod
-    def from_icon_id(cls, value: int):
-        if type(value) is not int:
-            raise TypeError(f"from_icon_id expected int, got {type(value)}")
-        if value == -1:
-            raise ValueError("-1 is not a valid icon_id value")
-        for x in cls._member_map_.values():
-            if x.value[1] == value:
-                return x
-        raise ValueError(f"{value} is not a valid icon_id value")
-
-    @property
-    def DEAD_ID(self):
-        return self.value[2]
-
-    @classmethod
-    def from_dead_id(cls, value: int):
-        if type(value) is not int:
-            raise TypeError(f"from_dead_id expected int, got {type(value)}")
-        if value == -1:
-            raise ValueError("-1 is not a valid dead_id value")
-        for x in cls._member_map_.values():
-            if x.value[2] == value:
-                return x
-        raise ValueError(f"{value} is not a valid dead_id value")
-
-    @property
-    def IS_GAIA_ONLY(self):
-        return self.value[3]
-
-    @staticmethod
-    def gaia_only():
-        result = []
-        for x in UnitInfo:
-            if x.IS_GAIA:
-                result.append(x)
-        return result
-
-    @staticmethod
-    def non_gaia():
-        result = []
-        for x in UnitInfo:
-            if not x.IS_GAIA:
-                result.append(x)
-        return result
+class UnitInfo(InfoDatasetBase):
 
     @staticmethod
     def vils():
         return [
             UnitInfo.VILLAGER_MALE, UnitInfo.VILLAGER_FEMALE, UnitInfo.VILLAGER_MALE_BUILDER,
             UnitInfo.VILLAGER_FEMALE_BUILDER, UnitInfo.VILLAGER_MALE_FARMER, UnitInfo.VILLAGER_FEMALE_FARMER,
             UnitInfo.VILLAGER_MALE_FISHERMAN, UnitInfo.VILLAGER_FEMALE_FISHERMAN, UnitInfo.VILLAGER_MALE_FORAGER,
@@ -108,290 +44,292 @@
             UnitInfo.KONNIK_DISMOUNTED, UnitInfo.ELITE_KONNIK_DISMOUNTED, UnitInfo.KONNIK_KREPOST,
             UnitInfo.ELITE_KONNIK_KREPOST, UnitInfo.ELITE_KIPCHAK_CUMAN_MERCENARIES, UnitInfo.FLAMING_CAMEL,
             UnitInfo.COUSTILLIER, UnitInfo.ELITE_COUSTILLIER, UnitInfo.SERJEANT, UnitInfo.ELITE_SERJEANT,
             UnitInfo.SERJEANT_DONJON, UnitInfo.ELITE_SERJEANT_DONJON, UnitInfo.FLEMISH_MILITIA_MALE,
             UnitInfo.FLEMISH_MILITIA_FEMALE, UnitInfo.FLEMISH_MILITIA,
         ]
 
-    BEAR = 486, 151, 489, True
-    BUTTERFLY1 = 1608, -1, -1, True
-    BUTTERFLY2 = 1609, -1, -1, True
-    BUTTERFLY3 = 1610, -1, -1, True
-    CROCODILE = 1031, 193, 1032, True
-    DEER = 65, 3, 43, True
-    DIRE_WOLF = 89, 7, 237, True
-    ELEPHANT = 1301, 179, 1332, True
-    FALCON = 1056, 5, -1, True
-    HAWK = 96, 283, -1, True
-    IBEX = 1239, 267, 1240, True
-    IRON_BOAR = 810, 98, 356, True
-    JAGUAR = 812, 111, 813, True
-    JAVELINA = 822, 98, 356, True
-    KOMODO_DRAGON = 1135, 226, 1136, True
-    LION = 1029, 194, 1030, True
-    MACAW = 816, 284, -1, True
-    OSTRICH = 1026, 196, 1027, True
-    RABID_WOLF = 202, 7, 237, True
-    RHINOCEROS = 1139, 225, 1140, True
-    SEAGULLS = 303, -1, -1, True
-    SNOW_LEOPARD = 1241, 268, 1242, True
-    STORK = 1028, 285, -1, True
-    STORMY_DOG = 862, 159, -1, True
-    TIGER = 1137, 227, 1138, True
-    VULTURE = 1305, 286, -1, True
-    WILD_BACTRIAN_CAMEL = 1247, 266, 1238, True
-    WILD_BOAR = 48, 98, 356, True
-    WILD_CAMEL = 884, 135, 898, True
-    WILD_HORSE = 835, 112, 815, True
-    WOLF = 126, 7, 237, True
-    ZEBRA = 1019, 192, 1020, True
-    MOVEABLE_MAP_REVEALER = 0, -1, -1, False
-    ALFRED_THE_ALPACA = 1300, 177, 1331, False
-    AMAZON_ARCHER = 850, 165, 1325, False
-    AMAZON_WARRIOR = 825, 166, 1324, False
-    ARAMBAI = 1126, 230, 1127, False
-    ARBALESTER = 492, 90, 496, False
-    ARCHER = 4, 17, 3, False
-    BACTRIAN_CAMEL = 1237, 266, 1238, False
-    BALLISTA_ELEPHANT = 1120, 231, 1121, False
-    BANDIT = 299, 8, 152, False
-    BATTERING_RAM = 1258, 74, 23, False
-    BATTLE_ELEPHANT = 1132, 228, 1133, False
-    BERSERK = 692, 38, 693, False
-    BOMBARD_CANNON = 36, 30, 16, False
-    BOYAR = 876, 114, 877, False
-    CAMEL = 897, 135, 898, False
-    CAMEL_ARCHER = 1007, 191, 1008, False
-    CAMEL_RIDER = 329, 78, 113, False
-    CANNON_GALLEON = 420, 55, -1, False
-    CANOE = 778, 164, -1, False
-    CAPPED_RAM = 422, 63, 423, False
-    CARAVEL = 1004, 198, -1, False
-    CART = 1338, 34, 205, False
-    CATAPHRACT = 40, 35, 27, False
-    CAVALIER = 283, 49, 139, False
-    CAVALRY_ARCHER = 39, 19, 34, False
-    CENTURION = 275, 138, 277, False
-    CHAMPION = 567, 72, 568, False
-    CHU_KO_NU = 73, 36, 28, False
-    COBRA_CAR = 748, 142, -1, False
-    CONDOTTIERO = 882, 134, 883, False
-    CONQUISTADOR = 771, 106, 772, False
-    COW_A = 705, 150, 843, False
-    COW_B = 1596, 150, 1597, False
-    COW_C = 1598, 150, 1599, False
-    COW_D = 1600, 150, 1601, False
-    CROSSBOWMAN = 24, 18, 26, False
-    DEMOLITION_RAFT = 1104, 202, -1, False
-    DEMOLITION_SHIP = 527, 84, -1, False
-    DONKEY = 846, 158, 848, False
-    DRAGON_SHIP = 1302, 178, -1, False
-    EAGLE_SCOUT = 751, 109, 754, False
-    EAGLE_WARRIOR = 753, 148, 1116, False
-    EASTERN_SWORDSMAN = 894, 186, 895, False
-    ELEPHANT_ARCHER = 873, 93, 874, False
-    ELITE_ARAMBAI = 1128, 230, 1127, False
-    ELITE_BALLISTA_ELEPHANT = 1122, 231, 1121, False
-    ELITE_BATTLE_ELEPHANT = 1134, 246, 1154, False
-    ELITE_BERSERK = 694, 38, 695, False
-    ELITE_BOYAR = 878, 114, 877, False
-    ELITE_CAMEL_ARCHER = 1009, 191, 1008, False
-    ELITE_CANNON_GALLEON = 691, 298, -1, False
-    ELITE_CARAVEL = 1006, 198, -1, False
-    ELITE_CATAPHRACT = 553, 35, 27, False
-    ELITE_CHU_KO_NU = 559, 36, 28, False
-    ELITE_CONQUISTADOR = 773, 106, 772, False
-    ELITE_EAGLE_WARRIOR = 752, 149, 1117, False
-    ELITE_ELEPHANT_ARCHER = 875, 93, 874, False
-    ELITE_GBETO = 1015, 197, 1014, False
-    ELITE_GENITOUR = 1012, 201, 1011, False
-    ELITE_GENOESE_CROSSBOWMAN = 868, 133, 867, False
-    ELITE_HUSKARL = 555, 50, 62, False
-    ELITE_JAGUAR_WARRIOR = 726, 110, 750, False
-    ELITE_JANISSARY = 557, 39, 107, False
-    ELITE_KAMAYUK = 881, 97, 880, False
-    ELITE_KARAMBIT_WARRIOR = 1125, 233, 1124, False
-    ELITE_KESHIK = 1230, 251, 1229, False
-    ELITE_KIPCHAK = 1233, 252, 1232, False
-    ELITE_KONNIK = 1227, 249, 1253, False
-    ELITE_KONNIK_DISMOUNTED = 1253, 250, 1257, False
-    ELITE_LEITIS = 1236, 253, 1235, False
-    ELITE_LONGBOAT = 533, 40, -1, False
-    ELITE_LONGBOWMAN = 530, 41, 115, False
-    ELITE_MAGYAR_HUSZAR = 871, 99, 870, False
-    ELITE_MAMELUKE = 556, 37, 44, False
-    ELITE_MANGUDAI = 561, 42, 135, False
-    ELITE_ORGAN_GUN = 1003, 190, 1002, False
-    ELITE_PLUMED_ARCHER = 765, 108, 764, False
-    ELITE_RATTAN_ARCHER = 1131, 232, 1130, False
-    ELITE_SAMURAI = 560, 44, 151, False
-    ELITE_SHOTEL_WARRIOR = 1018, 195, 1017, False
-    ELITE_SKIRMISHER = 6, 21, 100, False
-    ELITE_STEPPE_LANCER = 1372, 274, 1373, False
-    ELITE_TARKAN = 757, 105, 756, False
-    ELITE_TEUTONIC_KNIGHT = 554, 45, 181, False
-    ELITE_THROWING_AXEMAN = 531, 46, 157, False
-    ELITE_TURTLE_SHIP = 832, 116, -1, False
-    ELITE_WAR_ELEPHANT = 558, 43, 136, False
-    ELITE_WAR_WAGON = 829, 117, 828, False
-    ELITE_WOAD_RAIDER = 534, 47, 233, False
-    FAST_FIRE_SHIP = 532, 85, -1, False
-    FIRE_GALLEY = 1103, 203, -1, False
-    FIRE_SHIP = 529, 86, -1, False
-    FISHING_SHIP = 13, 24, -1, False
-    FLAMETHROWER = 188, 144, 189, False
-    FLAMING_CAMEL = 1263, 270, -1, False
-    FURIOUS_THE_MONKEY_BOY = 860, 132, 861, False
-    GALLEON = 442, 60, -1, False
-    GALLEY = 539, 87, -1, False
-    GBETO = 1013, 197, 1014, False
-    GENITOUR = 1010, 201, 1011, False
-    GENOESE_CROSSBOWMAN = 866, 133, 867, False
-    GOAT = 1060, 200, 1061, False
-    GOOSE = 1243, 265, 1244, False
-    HALBERDIER = 359, 104, 502, False
-    HAND_CANNONEER = 5, 22, 98, False
-    HEAVY_CAMEL_RIDER = 330, 79, 495, False
-    HEAVY_CAVALRY_ARCHER = 474, 71, 631, False
-    HEAVY_CROSSBOWMAN = 493, 133, 867, False
-    HEAVY_DEMOLITION_SHIP = 528, 83, -1, False
-    HEAVY_PIKEMAN = 892, 136, 893, False
-    HEAVY_SCORPION = 542, 89, 543, False
-    HEAVY_SWORDSMAN = 76, 184, 99, False
-    HORSE_A = 814, 112, 815, False
-    HORSE_B = 1356, 112, 1357, False
-    HORSE_C = 1602, 112, 1603, False
-    HORSE_D = 1604, 112, 1605, False
-    HORSE_E = 1606, 112, 1607, False
-    HUSKARL = 41, 50, 62, False
-    HUSSAR = 441, 103, 480, False
-    IMPERIAL_CAMEL_RIDER = 207, 185, 300, False
-    IMPERIAL_SKIRMISHER = 1155, 229, 1156, False
-    INVISIBLE_OBJECT = 1291, -1, -1, False
-    IROQUOIS_WARRIOR = 1374, 297, 1375, False
-    JAGUAR_WARRIOR = 725, 110, 750, False
-    JANISSARY = 46, 39, 107, False
-    JUNK = 15, 211, -1, False
-    KAMAYUK = 879, 97, 880, False
-    KARAMBIT_WARRIOR = 1123, 233, 1124, False
-    KESHIK = 1228, 251, 1229, False
-    KHAN = 1275, 258, 1277, False
-    KING = 434, 48, 435, False
-    KIPCHAK = 1231, 252, 1232, False
-    KNIGHT = 38, 1, 111, False
-    KONNIK = 1225, 249, 1252, False
-    KONNIK_DISMOUNTED = 1252, 250, 1257, False
-    LEGIONARY = 1, 139, 2, False
-    LEITIS = 1234, 253, 1235, False
-    LIGHT_CAVALRY = 546, 91, 547, False
-    LLAMA = 305, 156, 780, False
-    LONG_SWORDSMAN = 77, 13, 180, False
-    LONGBOAT = 250, 40, -1, False
-    LONGBOWMAN = 8, 41, 115, False
-    MAGYAR_HUSZAR = 869, 99, 870, False
-    MAMELUKE = 282, 37, 44, False
-    MAN_AT_ARMS = 75, 10, 154, False
-    MANGONEL = 280, 27, 121, False
-    MANGUDAI = 11, 42, 135, False
-    MERCHANT = 1572, 346, 1573, False
-    MILITIA = 74, 8, 152, False
-    MISSIONARY = 775, 107, 776, False
-    MONK = 125, 33, 134, False
-    MONK_WITH_RELIC = 286, 33, 134, False
-    NINJA = 1145, 299, 1147, False
-    NORSE_WARRIOR = 361, 140, 362, False
-    ONAGER = 550, 101, 675, False
-    ORGAN_GUN = 1001, 190, 1002, False
-    OX_CART = 1271, 263, 1272, False
-    OX_WAGON = 1273, 264, 1274, False
-    PALADIN = 569, 2, 570, False
-    PENGUIN = 639, 157, 641, False
-    PETARD = 440, 113, -1, False
-    PHOTONMAN = 1577, 300, 1578, False
-    PIG = 1245, 269, 1246, False
-    PIKEMAN = 358, 11, 501, False
-    PLUMED_ARCHER = 763, 108, 764, False
-    PRIEST = 1023, 294, 1024, False
-    PRIEST_WITH_RELIC = 1400, 33, 1024, False
-    QUEEN = 1292, 168, 1328, False
-    RATTAN_ARCHER = 1129, 232, 1130, False
-    RELIC_CART = 1304, 295, 285, False
-    ROYAL_JANISSARY = 52, 296, 1576, False
-    SAMURAI = 291, 44, 151, False
-    SCORPION = 279, 80, 149, False
-    SCOUT_CAVALRY = 448, 64, 449, False
-    SHARKATZOR = 1222, 352, -1, False
-    SHEEP = 594, 96, 595, False
-    SHOTEL_WARRIOR = 1016, 195, 1017, False
-    SIEGE_ONAGER = 588, 102, 589, False
-    SIEGE_RAM = 548, 73, 549, False
-    SIEGE_TOWER = 1105, 212, 1107, False
-    SKIRMISHER = 7, 20, 238, False
-    SLINGER = 185, 143, 186, False
-    SPEARMAN = 93, 31, 140, False
-    STEPPE_LANCER = 1370, 273, 1371, False
-    TARKAN = 755, 105, 756, False
-    TEUTONIC_KNIGHT = 25, 45, 181, False
-    THROWING_AXEMAN = 281, 46, 157, False
-    TORCH_A_CONVERTABLE = 854, -1, -1, False
-    TORCH_B_CONVERTABLE = 1377, -1, -1, False
-    TRADE_CART_EMPTY = 128, 34, 178, False
-    TRADE_CART_FULL = 204, 34, 205, False
-    TRADE_COG = 17, 23, -1, False
-    TRANSPORT_SHIP = 545, 95, -1, False
-    TREBUCHET = 42, 28, 194, False
-    TREBUCHET_PACKED = 331, 29, 735, False
-    TURKEY = 833, 115, 834, False
-    TURTLE_SHIP = 831, 116, -1, False
-    TWO_HANDED_SWORDSMAN = 473, 12, 500, False
-    VILLAGER_MALE = 83, 15, 224, False
-    VILLAGER_FEMALE = 293, 16, 211, False
-    VILLAGER_MALE_BUILDER = 118, 330, 225, False
-    VILLAGER_FEMALE_BUILDER = 212, 329, 213, False
-    VILLAGER_MALE_FARMER = 259, 332, 226, False
-    VILLAGER_FEMALE_FARMER = 214, 331, 215, False
-    VILLAGER_MALE_FISHERMAN = 56, 332, 58, False
-    VILLAGER_FEMALE_FISHERMAN = 57, 331, 60, False
-    VILLAGER_MALE_FORAGER = 120, 332, 353, False
-    VILLAGER_FEMALE_FORAGER = 354, 331, 355, False
-    VILLAGER_MALE_GOLD_MINER = 579, 334, 229, False
-    VILLAGER_FEMALE_GOLD_MINER = 581, 333, 221, False
-    VILLAGER_MALE_HUNTER = 122, 332, 227, False
-    VILLAGER_FEMALE_HUNTER = 216, 331, 217, False
-    VILLAGER_MALE_LUMBERJACK = 123, 339, 228, False
-    VILLAGER_FEMALE_LUMBERJACK = 218, 338, 219, False
-    VILLAGER_MALE_REPAIRER = 156, 330, 225, False
-    VILLAGER_FEMALE_REPAIRER = 222, 329, 213, False
-    VILLAGER_MALE_SHEPHERD = 592, 332, 593, False
-    VILLAGER_FEMALE_SHEPHERD = 590, 331, 591, False
-    VILLAGER_MALE_STONE_MINER = 124, 336, 229, False
-    VILLAGER_FEMALE_STONE_MINER = 220, 335, 221, False
-    VMDL = 206, 337, -1, False
-    WAR_ELEPHANT = 239, 43, 136, False
-    WAR_GALLEY = 21, 25, -1, False
-    WAR_WAGON = 827, 117, 828, False
-    WATER_BUFFALO = 1142, 224, 1143, False
-    WOAD_RAIDER = 232, 47, 233, False
-    XOLOTL_WARRIOR = 1570, 351, 1571, False
-    SMALL_TEMP_MAP_REVEAL = 112, -1, -1, False
-    LARGE_TEMP_MAP_REVEAL = 332, -1, -1, False
-    BOARDER_GALLEY = 536, 82, -1, False
-    HUSKARL_BARRACKS = 759, 50, 62, False
-    ELITE_HUSKARL_BARRACKS = 761, 50, 62, False
-    TARKAN_STABLE = 886, 105, 756, False
-    ELITE_TARKAN_STABLE = 887, 105, 756, False
-    GENITOUR_ORIGINAL = 583, 19, 152, False
-    ELITE_GENITOUR_ORIGINAL = 596, 19, 152, False
-    COUSTILLIER = 1655, 355, 1656, False
-    ELITE_COUSTILLIER = 1657, 355, 1656, False
-    FLEMISH_MILITIA = 1699, 354, 1664, False
-    FLEMISH_MILITIA_MALE = 1663, 354, 1664, False
-    FLEMISH_MILITIA_FEMALE = 1697, 354, 1698, False
-    SERJEANT = 1658, 356, 1662, False
-    ELITE_SERJEANT = 1659, 356, 1662, False
-    SERJEANT_DONJON = 1660, 356, 1662, False
-    ELITE_SERJEANT_DONJON = 1661, 356, 1662, False
-    CONDOTTIERO_PLACEHOLDER = 184, 134, 883, False
-    KONNIK_KREPOST = 1254, 249, 1252, False
-    ELITE_KONNIK_KREPOST = 1255, 249, 1253, False
-    ELITE_KIPCHAK_CUMAN_MERCENARIES = 1260, 252, 1232, False
-    FOOD_WOOD_GOLD_TRICKLE = 1654, -1, -1, False
+    BEAR = 486, 151, 489, 16712, True
+    BUTTERFLY1 = 1608, -1, -1, 16716, True
+    BUTTERFLY2 = 1609, -1, -1, 16716, True
+    BUTTERFLY3 = 1610, -1, -1, 16716, True
+    CROCODILE = 1031, 193, 1032, 16060, True
+    DEER = 65, 3, 43, 16071, True
+    DIRE_WOLF = 89, 7, 237, 16553, True
+    ELEPHANT = 1301, 179, 1332, 16722, True
+    FALCON = 1056, 5, -1, 16058, True
+    HAWK = 96, 283, -1, 16073, True
+    IBEX = 1239, 267, 1240, 16071, True
+    IRON_BOAR = 810, 98, 356, 16710, True
+    JAGUAR = 812, 111, 813, 16712, True
+    JAVELINA = 822, 98, 356, 16722, True
+    KOMODO_DRAGON = 1135, 226, 1136, 16163, True
+    LION = 1029, 194, 1030, 16059, True
+    MACAW = 816, 284, -1, 16716, True
+    OSTRICH = 1026, 196, 1027, 16071, True
+    RABID_WOLF = 202, 7, 237, 16652, True
+    RHINOCEROS = 1139, 225, 1140, 16172, True
+    SEAGULLS = 303, -1, -1, 16716, True
+    SNOW_LEOPARD = 1241, 268, 1242, 16060, True
+    STORK = 1028, 285, -1, 16058, True
+    STORMY_DOG = 862, 159, -1, 16764, True
+    TIGER = 1137, 227, 1138, 16170, True
+    VULTURE = 1305, 286, -1, 16716, True
+    WILD_BACTRIAN_CAMEL = 1247, 266, 1238, 16735, True
+    WILD_BOAR = 48, 98, 356, 16406, True
+    WILD_CAMEL = 884, 135, 898, 16735, True
+    WILD_HORSE = 835, 112, 815, 16735, True
+    WOLF = 126, 7, 237, 16075, True
+    ZEBRA = 1019, 192, 1020, 16071, True
+    MOVEABLE_MAP_REVEALER = 0, -1, -1, 16000, False
+    ALFRED_THE_ALPACA = 1300, 177, 1331, 16469, False
+    AMAZON_ARCHER = 850, 165, 1325, 16683, False
+    AMAZON_WARRIOR = 825, 166, 1324, 16667, False
+    ARAMBAI = 1126, 230, 1127, 16101, False
+    ARBALESTER = 492, 90, 496, 16418, False
+    ARCHER = 4, 17, 3, 16083, False
+    BACTRIAN_CAMEL = 1237, 266, 1238, 16714, False
+    BALLISTA_ELEPHANT = 1120, 231, 1121, 16101, False
+    BANDIT = 299, 8, 152, 16098, False
+    BATTERING_RAM = 1258, 74, 23, 16094, False
+    BATTLE_ELEPHANT = 1132, 228, 1133, 16733, False
+    BERSERK = 692, 38, 693, 16574, False
+    BOMBARD_CANNON = 36, 30, 16, 16093, False
+    BOYAR = 876, 114, 877, 16101, False
+    CAMEL = 897, 135, 898, 16714, False
+    CAMEL_ARCHER = 1007, 191, 1008, 16101, False
+    CAMEL_RIDER = 329, 78, 113, 16416, False
+    CANNON_GALLEON = 420, 55, -1, 16287, False
+    CANOE = 778, 164, -1, 16106, False
+    CAPPED_RAM = 422, 63, 423, 16289, False
+    CARAVEL = 1004, 198, -1, 16106, False
+    CART = 1338, 34, 205, 16100, False
+    CATAPHRACT = 40, 35, 27, 16101, False
+    CAVALIER = 283, 49, 139, 16070, False
+    CAVALRY_ARCHER = 39, 19, 34, 16085, False
+    CENTURION = 275, 138, 277, 16451, False
+    CHAMPION = 567, 72, 568, 16469, False
+    CHU_KO_NU = 73, 36, 28, 16102, False
+    COBRA_CAR = 748, 142, -1, 16658, False
+    CONDOTTIERO = 882, 134, 883, 16679, False
+    CONQUISTADOR = 771, 106, 772, 16687, False
+    COW_A = 705, 150, 843, 16498, False
+    COW_B = 1596, 150, 1597, 16498, False
+    COW_C = 1598, 150, 1599, 16498, False
+    COW_D = 1600, 150, 1601, 16498, False
+    CROSSBOWMAN = 24, 18, 26, 16084, False
+    DEMOLITION_RAFT = 1104, 202, -1, 16424, False
+    DEMOLITION_SHIP = 527, 84, -1, 16424, False
+    DONKEY = 846, 158, 848, 16100, False
+    DRAGON_SHIP = 1302, 178, -1, 16739, False
+    EAGLE_SCOUT = 751, 109, 754, 16671, False
+    EAGLE_WARRIOR = 753, 148, 1116, 16671, False
+    EASTERN_SWORDSMAN = 894, 186, 895, 16081, False
+    ELEPHANT_ARCHER = 873, 93, 874, 16101, False
+    ELITE_ARAMBAI = 1128, 230, 1127, 16101, False
+    ELITE_BALLISTA_ELEPHANT = 1122, 231, 1121, 16101, False
+    ELITE_BATTLE_ELEPHANT = 1134, 246, 1154, 16733, False
+    ELITE_BERSERK = 694, 38, 695, 16576, False
+    ELITE_BOYAR = 878, 114, 877, 16101, False
+    ELITE_CAMEL_ARCHER = 1009, 191, 1008, 16101, False
+    ELITE_CANNON_GALLEON = 691, 298, -1, 16573, False
+    ELITE_CARAVEL = 1006, 198, -1, 16106, False
+    ELITE_CATAPHRACT = 553, 35, 27, 16451, False
+    ELITE_CHU_KO_NU = 559, 36, 28, 16452, False
+    ELITE_CONQUISTADOR = 773, 106, 772, 16689, False
+    ELITE_EAGLE_WARRIOR = 752, 149, 1117, 16673, False
+    ELITE_ELEPHANT_ARCHER = 875, 93, 874, 16101, False
+    ELITE_GBETO = 1015, 197, 1014, 16101, False
+    ELITE_GENITOUR = 1012, 201, 1011, 16417, False
+    ELITE_GENOESE_CROSSBOWMAN = 868, 133, 867, 16101, False
+    ELITE_HUSKARL = 555, 50, 62, 16454, False
+    ELITE_JAGUAR_WARRIOR = 726, 110, 750, 16669, False
+    ELITE_JANISSARY = 557, 39, 107, 16455, False
+    ELITE_KAMAYUK = 881, 97, 880, 16460, False
+    ELITE_KARAMBIT_WARRIOR = 1125, 233, 1124, 16101, False
+    ELITE_KESHIK = 1230, 251, 1229, 16101, False
+    ELITE_KIPCHAK = 1233, 252, 1232, 16108, False
+    ELITE_KONNIK = 1227, 249, 1253, 16101, False
+    ELITE_KONNIK_DISMOUNTED = 1253, 250, 1257, 16411, False
+    ELITE_LEITIS = 1236, 253, 1235, 16101, False
+    ELITE_LONGBOAT = 533, 40, -1, 16457, False
+    ELITE_LONGBOWMAN = 530, 41, 115, 16456, False
+    ELITE_MAGYAR_HUSZAR = 871, 99, 870, 16101, False
+    ELITE_MAMELUKE = 556, 37, 44, 16453, False
+    ELITE_MANGUDAI = 561, 42, 135, 16458, False
+    ELITE_ORGAN_GUN = 1003, 190, 1002, 16101, False
+    ELITE_PLUMED_ARCHER = 765, 108, 764, 16685, False
+    ELITE_RATTAN_ARCHER = 1131, 232, 1130, 16101, False
+    ELITE_SAMURAI = 560, 44, 151, 16460, False
+    ELITE_SHOTEL_WARRIOR = 1018, 195, 1017, 16101, False
+    ELITE_SKIRMISHER = 6, 21, 100, 16087, False
+    ELITE_STEPPE_LANCER = 1372, 274, 1373, 16746, False
+    ELITE_TARKAN = 757, 105, 756, 16677, False
+    ELITE_TEUTONIC_KNIGHT = 554, 45, 181, 16462, False
+    ELITE_THROWING_AXEMAN = 531, 46, 157, 16461, False
+    ELITE_TURTLE_SHIP = 832, 116, -1, 16106, False
+    ELITE_WAR_ELEPHANT = 558, 43, 136, 16459, False
+    ELITE_WAR_WAGON = 829, 117, 828, 16729, False
+    ELITE_WOAD_RAIDER = 534, 47, 233, 16463, False
+    FAST_FIRE_SHIP = 532, 85, -1, 16429, False
+    FIRE_GALLEY = 1103, 203, -1, 16426, False
+    FIRE_SHIP = 529, 86, -1, 16426, False
+    FISHING_SHIP = 13, 24, -1, 16090, False
+    FLAMETHROWER = 188, 144, 189, 16109, False
+    FLAMING_CAMEL = 1263, 270, -1, 16734, False
+    FURIOUS_THE_MONKEY_BOY = 860, 132, 861, 16763, False
+    GALLEON = 442, 60, -1, 16309, False
+    GALLEY = 539, 87, -1, 16436, False
+    GBETO = 1013, 197, 1014, 16101, False
+    GENITOUR = 1010, 201, 1011, 16417, False
+    GENOESE_CROSSBOWMAN = 866, 133, 867, 16101, False
+    GOAT = 1060, 200, 1061, 16061, False
+    GOOSE = 1243, 265, 1244, 16061, False
+    HALBERDIER = 359, 104, 502, 16409, False
+    HAND_CANNONEER = 5, 22, 98, 16086, False
+    HEAVY_CAMEL_RIDER = 330, 79, 495, 16417, False
+    HEAVY_CAVALRY_ARCHER = 474, 71, 631, 16412, False
+    HEAVY_CROSSBOWMAN = 493, 133, 867, 16101, False
+    HEAVY_DEMOLITION_SHIP = 528, 83, -1, 16425, False
+    HEAVY_PIKEMAN = 892, 136, 893, 16410, False
+    HEAVY_SCORPION = 542, 89, 543, 16439, False
+    HEAVY_SWORDSMAN = 76, 184, 99, 16077, False
+    HORSE_A = 814, 112, 815, 16714, False
+    HORSE_B = 1356, 112, 1357, 16714, False
+    HORSE_C = 1602, 112, 1603, 16714, False
+    HORSE_D = 1604, 112, 1605, 16714, False
+    HORSE_E = 1606, 112, 1607, 16714, False
+    HUSKARL = 41, 50, 62, 16104, False
+    HUSSAR = 441, 103, 480, 16661, False
+    IMPERIAL_CAMEL_RIDER = 207, 185, 300, 16417, False
+    IMPERIAL_SKIRMISHER = 1155, 229, 1156, 16087, False
+    INVISIBLE_OBJECT = 1291, -1, -1, 16000, False
+    IROQUOIS_WARRIOR = 1374, 297, 1375, 16113, False
+    JAGUAR_WARRIOR = 725, 110, 750, 16667, False
+    JANISSARY = 46, 39, 107, 16105, False
+    JUNK = 15, 211, -1, 16092, False
+    KAMAYUK = 879, 97, 880, 16110, False
+    KARAMBIT_WARRIOR = 1123, 233, 1124, 16101, False
+    KESHIK = 1228, 251, 1229, 16101, False
+    KHAN = 1275, 258, 1277, 16458, False
+    KING = 434, 48, 435, 16301, False
+    KIPCHAK = 1231, 252, 1232, 16108, False
+    KNIGHT = 38, 1, 111, 16068, False
+    KONNIK = 1225, 249, 1252, 16101, False
+    KONNIK_DISMOUNTED = 1252, 250, 1257, 16411, False
+    LEGIONARY = 1, 139, 2, 16669, False
+    LEITIS = 1234, 253, 1235, 16101, False
+    LIGHT_CAVALRY = 546, 91, 547, 16444, False
+    LLAMA = 305, 156, 780, 16498, False
+    LONG_SWORDSMAN = 77, 13, 180, 16081, False
+    LONGBOAT = 250, 40, -1, 16106, False
+    LONGBOWMAN = 8, 41, 115, 16107, False
+    MAGYAR_HUSZAR = 869, 99, 870, 16101, False
+    MAMELUKE = 282, 37, 44, 16103, False
+    MAN_AT_ARMS = 75, 10, 154, 16080, False
+    MANGONEL = 280, 27, 121, 16095, False
+    MANGUDAI = 11, 42, 135, 16108, False
+    MERCHANT = 1572, 346, 1573, 16301, False
+    MILITIA = 74, 8, 152, 16079, False
+    MISSIONARY = 775, 107, 776, 16691, False
+    MONK = 125, 33, 134, 16099, False
+    MONK_WITH_RELIC = 286, 33, 134, 16380, False
+    NINJA = 1145, 299, 1147, 16110, False
+    NORSE_WARRIOR = 361, 140, 362, 16081, False
+    ONAGER = 550, 101, 675, 16448, False
+    ORGAN_GUN = 1001, 190, 1002, 16101, False
+    OX_CART = 1271, 263, 1272, 16100, False
+    OX_WAGON = 1273, 264, 1274, 16100, False
+    PALADIN = 569, 2, 570, 16471, False
+    PENGUIN = 639, 157, 641, 16469, False
+    PETARD = 440, 113, -1, 16660, False
+    PHOTONMAN = 1577, 300, 1578, 16043, False
+    PIG = 1245, 269, 1246, 16061, False
+    PIKEMAN = 358, 11, 501, 16408, False
+    PLUMED_ARCHER = 763, 108, 764, 16683, False
+    PRIEST = 1023, 294, 1024, 16120, False
+    PRIEST_WITH_RELIC = 1400, 33, 1024, 16380, False
+    QUEEN = 1292, 168, 1328, 16302, False
+    RATTAN_ARCHER = 1129, 232, 1130, 16101, False
+    RELIC_CART = 1304, 295, 285, 16082, False
+    ROYAL_JANISSARY = 52, 296, 1576, 16455, False
+    SAMURAI = 291, 44, 151, 16110, False
+    SCORPION = 279, 80, 149, 16096, False
+    SCOUT_CAVALRY = 448, 64, 449, 16326, False
+    SHARKATZOR = 1222, 352, -1, 16458, False
+    SHEEP = 594, 96, 595, 16498, False
+    SHOTEL_WARRIOR = 1016, 195, 1017, 16101, False
+    SIEGE_ONAGER = 588, 102, 589, 16493, False
+    SIEGE_RAM = 548, 73, 549, 16446, False
+    SIEGE_TOWER = 1105, 212, 1107, 16445, False
+    SKIRMISHER = 7, 20, 238, 16088, False
+    SLINGER = 185, 143, 186, 16743, False
+    SPEARMAN = 93, 31, 140, 16078, False
+    STEPPE_LANCER = 1370, 273, 1371, 16746, False
+    TARKAN = 755, 105, 756, 16675, False
+    TEUTONIC_KNIGHT = 25, 45, 181, 16112, False
+    THROWING_AXEMAN = 281, 46, 157, 16111, False
+    TORCH_A_CONVERTABLE = 854, -1, -1, 16753, False
+    TORCH_B_CONVERTABLE = 1377, -1, -1, 16753, False
+    TRADE_CART_EMPTY = 128, 34, 178, 16100, False
+    TRADE_CART_FULL = 204, 34, 205, 16100, False
+    TRADE_COG = 17, 23, -1, 16089, False
+    TRANSPORT_SHIP = 545, 95, -1, 16443, False
+    TREBUCHET = 42, 28, 194, 16097, False
+    TREBUCHET_PACKED = 331, 29, 735, 16381, False
+    TURKEY = 833, 115, 834, 16733, False
+    TURTLE_SHIP = 831, 116, -1, 16106, False
+    TWO_HANDED_SWORDSMAN = 473, 12, 500, 16411, False
+    VILLAGER_MALE = 83, 15, 224, 16121, False
+    VILLAGER_FEMALE = 293, 16, 211, 16121, False
+    VILLAGER_MALE_BUILDER = 118, 330, 225, 16122, False
+    VILLAGER_FEMALE_BUILDER = 212, 329, 213, 16122, False
+    VILLAGER_MALE_FARMER = 259, 332, 226, 16123, False
+    VILLAGER_FEMALE_FARMER = 214, 331, 215, 16123, False
+    VILLAGER_MALE_FISHERMAN = 56, 332, 58, 16499, False
+    VILLAGER_FEMALE_FISHERMAN = 57, 331, 60, 16499, False
+    VILLAGER_MALE_FORAGER = 120, 332, 353, 16402, False
+    VILLAGER_FEMALE_FORAGER = 354, 331, 355, 16402, False
+    VILLAGER_MALE_GOLD_MINER = 579, 334, 229, 16482, False
+    VILLAGER_FEMALE_GOLD_MINER = 581, 333, 221, 16482, False
+    VILLAGER_MALE_HUNTER = 122, 332, 227, 16124, False
+    VILLAGER_FEMALE_HUNTER = 216, 331, 217, 16124, False
+    VILLAGER_MALE_LUMBERJACK = 123, 339, 228, 16125, False
+    VILLAGER_FEMALE_LUMBERJACK = 218, 338, 219, 16125, False
+    VILLAGER_MALE_REPAIRER = 156, 330, 225, 16127, False
+    VILLAGER_FEMALE_REPAIRER = 222, 329, 213, 16127, False
+    VILLAGER_MALE_SHEPHERD = 592, 332, 593, 16496, False
+    VILLAGER_FEMALE_SHEPHERD = 590, 331, 591, 16496, False
+    VILLAGER_MALE_STONE_MINER = 124, 336, 229, 16126, False
+    VILLAGER_FEMALE_STONE_MINER = 220, 335, 221, 16126, False
+    VMDL = 206, 337, -1, 16656, False
+    WAR_ELEPHANT = 239, 43, 136, 16109, False
+    WAR_GALLEY = 21, 25, -1, 16091, False
+    WAR_WAGON = 827, 117, 828, 16727, False
+    WATER_BUFFALO = 1142, 224, 1143, 16175, False
+    WOAD_RAIDER = 232, 47, 233, 16113, False
+    XOLOTL_WARRIOR = 1570, 351, 1571, 16326, False
+    BOARDER_GALLEY = 536, 82, -1, 16703, False
+    HUSKARL_BARRACKS = 759, 50, 62, 16748, False
+    ELITE_HUSKARL_BARRACKS = 761, 50, 62, 16748, False
+    TARKAN_STABLE = 886, 105, 756, 16741, False
+    ELITE_TARKAN_STABLE = 887, 105, 756, 16741, False
+    GENITOUR_ORIGINAL = 583, 19, 152, 16663, False
+    ELITE_GENITOUR_ORIGINAL = 596, 19, 152, 16665, False
+    COUSTILLIER = 1655, 355, 1656, 16101, False
+    ELITE_COUSTILLIER = 1657, 355, 1656, 16101, False
+    FLEMISH_MILITIA = 1699, 354, 1664, 16735, False
+    FLEMISH_MILITIA_MALE = 1663, 354, 1664, 16469, False
+    FLEMISH_MILITIA_FEMALE = 1697, 354, 1698, 16469, False
+    SERJEANT = 1658, 356, 1662, 16104, False
+    ELITE_SERJEANT = 1659, 356, 1662, 16454, False
+    SERJEANT_DONJON = 1660, 356, 1662, 16101, False
+    ELITE_SERJEANT_DONJON = 1661, 356, 1662, 16101, False
+    CONDOTTIERO_PLACEHOLDER = 184, 134, 883, 16679, False
+    KONNIK_KREPOST = 1254, 249, 1252, 16101, False
+    ELITE_KONNIK_KREPOST = 1255, 249, 1253, 16101, False
+    ELITE_KIPCHAK_CUMAN_MERCENARIES = 1260, 252, 1232, 16730, False
+    FOOD_WOOD_GOLD_TRICKLE = 1654, -1, -1, 16737, False
+    CUMAN_DISABLED = 1261, 114, 1232, 16108, False
+    OUTLW = 158, 17, 3, 16074, True
+    RFARC = 571, 17, 572, 16474, False
+    MONUMENT_RESOURCE_ENABLER = 1639, 17, 572, 16464, False
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/bytes_conversions.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/bytes_conversions.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/bytes_parser.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/bytes_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         retriever (Retriever): The retriever
         value (List[Any]): A value to be put in the retriever
 
     Returns:
         The given list or the value inside it
     """
     if retriever.datatype.repeat != 1:
-        return listify(value)
+        return value
 
     if retriever.is_list is not None:
-        return listify(value) if retriever.is_list else value[0]
+        return value if retriever.is_list else value[0]
 
     # Fallback to length check
     if len(value) == 1:
         return value[0]
 
     return value
 
@@ -51,24 +51,24 @@
     try:
         for i in range(retriever.datatype.repeat):
             if var_type != "str":  # (Signed) ints, floats, chars, plain bytes etc.
                 retrieved_bytes.append(igenerator.get_bytes(var_len))
             else:  # String, Stored as: (signed int (n), string (string_length = n))
                 int_bytes = igenerator.get_bytes(var_len)
                 string_length = bytes_to_int(int_bytes, signed=True)
-                string_bytes = b'' if string_length == 0 else igenerator.get_bytes(string_length)
+                string_bytes = igenerator.get_bytes(string_length)
                 retrieved_bytes.append(int_bytes + string_bytes)
     except EndOfFileError:
         if is_end_of_file_mark(retriever):
             retriever.datatype.repeat = 0
             return []
     except TypeError:
         print(retriever)
         print(retriever.datatype.repeat)
-        exit()
+        exit()  # Todo: Should not exit (?)
 
     # If more bytes present in the file after END_OF_FILE_MARK
     handle_end_of_file_mark(igenerator, retriever)
 
     return retrieved_bytes
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/helper.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/helper.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/incremental_generator.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/incremental_generator.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/pretty_format.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/pretty_format.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/printers.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/printers.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/helper/string_manipulations.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/helper/string_manipulations.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/aoe2_object.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/aoe2_object.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/aoe2_object_manager.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/aoe2_object_manager.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/condition.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/condition.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         RetrieverObjectLink("object_list", "Triggers",
                             "trigger_data[__index__].condition_data[__index__].object_list"),
         RetrieverObjectLink("source_player", "Triggers",
                             "trigger_data[__index__].condition_data[__index__].source_player"),
         RetrieverObjectLink("technology", "Triggers",
                             "trigger_data[__index__].condition_data[__index__].technology"),
         RetrieverObjectLink("timer", "Triggers", "trigger_data[__index__].condition_data[__index__].timer"),
-        RetrieverObjectLink("area_1_x", "Triggers", "trigger_data[__index__].condition_data[__index__].area_1_x"),
-        RetrieverObjectLink("area_1_y", "Triggers", "trigger_data[__index__].condition_data[__index__].area_1_y"),
-        RetrieverObjectLink("area_2_x", "Triggers", "trigger_data[__index__].condition_data[__index__].area_2_x"),
-        RetrieverObjectLink("area_2_y", "Triggers", "trigger_data[__index__].condition_data[__index__].area_2_y"),
+        RetrieverObjectLink("area_x1", "Triggers", "trigger_data[__index__].condition_data[__index__].area_x1"),
+        RetrieverObjectLink("area_y1", "Triggers", "trigger_data[__index__].condition_data[__index__].area_y1"),
+        RetrieverObjectLink("area_x2", "Triggers", "trigger_data[__index__].condition_data[__index__].area_x2"),
+        RetrieverObjectLink("area_y2", "Triggers", "trigger_data[__index__].condition_data[__index__].area_y2"),
         RetrieverObjectLink("object_group", "Triggers",
                             "trigger_data[__index__].condition_data[__index__].object_group"),
         RetrieverObjectLink("object_type", "Triggers",
                             "trigger_data[__index__].condition_data[__index__].object_type"),
         RetrieverObjectLink("ai_signal", "Triggers", "trigger_data[__index__].condition_data[__index__].ai_signal"),
         RetrieverObjectLink("inverted", "Triggers", "trigger_data[__index__].condition_data[__index__].inverted"),
         RetrieverObjectLink("variable", "Triggers", "trigger_data[__index__].condition_data[__index__].variable"),
@@ -57,18 +57,18 @@
                  attribute: int = None,
                  unit_object: int = None,
                  next_object: int = None,
                  object_list: int = None,
                  source_player: IntEnum = None,
                  technology: IntEnum = None,
                  timer: int = None,
-                 area_1_x: int = None,
-                 area_1_y: int = None,
-                 area_2_x: int = None,
-                 area_2_y: int = None,
+                 area_x1: int = None,
+                 area_y1: int = None,
+                 area_x2: int = None,
+                 area_y2: int = None,
                  object_group: int = None,
                  object_type: int = None,
                  ai_signal: int = None,
                  inverted: int = None,
                  variable: int = None,
                  comparison: int = None,
                  target_player: IntEnum = None,
@@ -82,18 +82,18 @@
         self.attribute: int = attribute
         self.unit_object: int = unit_object
         self.next_object: int = next_object
         self.object_list: int = object_list
         self.source_player: int = source_player
         self.technology: int = technology
         self.timer: int = timer
-        self.area_1_x: int = area_1_x
-        self.area_1_y: int = area_1_y
-        self.area_2_x: int = area_2_x
-        self.area_2_y: int = area_2_y
+        self.area_x1: int = area_x1
+        self.area_y1: int = area_y1
+        self.area_x2: int = area_x2
+        self.area_y2: int = area_y2
         self.object_group: int = object_group
         self.object_type: int = object_type
         self.ai_signal: int = ai_signal
         self.inverted: int = inverted
         self.variable: int = variable
         self.comparison: int = comparison
         self.target_player: int = target_player
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/effect.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/effect.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
         RetrieverObjectLink("string_id", "Triggers", "trigger_data[__index__].effect_data[__index__].string_id"),
         RetrieverObjectLink("display_time", "Triggers", "trigger_data[__index__].effect_data[__index__].display_time"),
         RetrieverObjectLink("trigger_id", "Triggers", "trigger_data[__index__].effect_data[__index__].trigger_id"),
         RetrieverObjectLink("location_x", "Triggers", "trigger_data[__index__].effect_data[__index__].location_x"),
         RetrieverObjectLink("location_y", "Triggers", "trigger_data[__index__].effect_data[__index__].location_y"),
         RetrieverObjectLink("location_object_reference", "Triggers",
                             "trigger_data[__index__].effect_data[__index__].location_object_reference"),
-        RetrieverObjectLink("area_1_x", "Triggers", "trigger_data[__index__].effect_data[__index__].area_1_x"),
-        RetrieverObjectLink("area_1_y", "Triggers", "trigger_data[__index__].effect_data[__index__].area_1_y"),
-        RetrieverObjectLink("area_2_x", "Triggers", "trigger_data[__index__].effect_data[__index__].area_2_x"),
-        RetrieverObjectLink("area_2_y", "Triggers", "trigger_data[__index__].effect_data[__index__].area_2_y"),
+        RetrieverObjectLink("area_x1", "Triggers", "trigger_data[__index__].effect_data[__index__].area_x1"),
+        RetrieverObjectLink("area_y1", "Triggers", "trigger_data[__index__].effect_data[__index__].area_y1"),
+        RetrieverObjectLink("area_x2", "Triggers", "trigger_data[__index__].effect_data[__index__].area_x2"),
+        RetrieverObjectLink("area_y2", "Triggers", "trigger_data[__index__].effect_data[__index__].area_y2"),
         RetrieverObjectLink("object_group", "Triggers", "trigger_data[__index__].effect_data[__index__].object_group"),
         RetrieverObjectLink("object_type", "Triggers", "trigger_data[__index__].effect_data[__index__].object_type"),
         RetrieverObjectLink("instruction_panel_position", "Triggers",
                             "trigger_data[__index__].effect_data[__index__].instruction_panel_position"),
         RetrieverObjectLink("attack_stance", "Triggers",
                             "trigger_data[__index__].effect_data[__index__].attack_stance"),
         RetrieverObjectLink("time_unit", "Triggers", "trigger_data[__index__].effect_data[__index__].time_unit"),
@@ -100,18 +100,18 @@
                  technology: int = None,
                  string_id: int = None,
                  display_time: int = None,
                  trigger_id: int = None,
                  location_x: int = None,
                  location_y: int = None,
                  location_object_reference: int = None,
-                 area_1_x: int = None,
-                 area_1_y: int = None,
-                 area_2_x: int = None,
-                 area_2_y: int = None,
+                 area_x1: int = None,
+                 area_y1: int = None,
+                 area_x2: int = None,
+                 area_y2: int = None,
                  object_group: int = None,
                  object_type: int = None,
                  instruction_panel_position: int = None,
                  attack_stance: int = None,
                  time_unit: int = None,
                  enabled: int = None,
                  food: int = None,
@@ -155,18 +155,18 @@
         self.technology: int = technology
         self.string_id: int = string_id
         self.display_time: int = display_time
         self.trigger_id: int = trigger_id
         self.location_x: int = location_x
         self.location_y: int = location_y
         self.location_object_reference: int = location_object_reference
-        self.area_1_x: int = area_1_x
-        self.area_1_y: int = area_1_y
-        self.area_2_x: int = area_2_x
-        self.area_2_y: int = area_2_y
+        self.area_x1: int = area_x1
+        self.area_y1: int = area_y1
+        self.area_x2: int = area_x2
+        self.area_y2: int = area_y2
         self.object_group: int = object_group
         self.object_type: int = object_type
         self.instruction_panel_position: int = instruction_panel_position
         self.attack_stance: int = attack_stance
         self.time_unit: int = time_unit
         self.enabled: int = enabled
         self.food: int = food
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/terrain_tile.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/terrain_tile.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/trigger.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         self._effects = val
         self.effect_order = list(range(0, len(val)))
 
     def _add_effect(self, effect_type: EffectId, ai_script_goal=None, armour_attack_quantity=None,
                     armour_attack_class=None, quantity=None, tribute_list=None, diplomacy=None,
                     object_list_unit_id=None, source_player=None, target_player=None, technology=None, string_id=None,
                     display_time=None, trigger_id=None, location_x=None, location_y=None,
-                    location_object_reference=None, area_1_x=None, area_1_y=None, area_2_x=None, area_2_y=None,
+                    location_object_reference=None, area_x1=None, area_y1=None, area_x2=None, area_y2=None,
                     object_group=None, object_type=None, instruction_panel_position=None, attack_stance=None,
                     time_unit=None, enabled=None, food=None, wood=None, stone=None, gold=None, item_id=None,
                     flash_object=None, force_research_technology=None, visibility_state=None, scroll=None,
                     operation=None, object_list_unit_id_2=None, button_location=None, ai_signal_value=None,
                     object_attributes=None, variable=None, timer=None, facet=None, play_sound=None, message=None,
                     player_color=None, sound_name=None, selected_object_ids=None) -> Effect:
         """Used to add new effect to trigger. Please use trigger.new_effect.<effect_name> instead"""
@@ -174,16 +174,16 @@
             effect_attr[key] = (locals()[key] if locals()[key] is not None else value)
         new_effect = Effect(**effect_attr)
         self.effects.append(new_effect)
         return new_effect
 
     def _add_condition(self, condition_type: ConditionId, quantity=None,
                        attribute=None, unit_object=None, next_object=None, object_list=None,
-                       source_player=None, technology=None, timer=None, area_1_x=None, area_1_y=None, area_2_x=None,
-                       area_2_y=None, object_group=None, object_type=None, ai_signal=None, inverted=None, variable=None,
+                       source_player=None, technology=None, timer=None, area_x1=None, area_y1=None, area_x2=None,
+                       area_y2=None, object_group=None, object_type=None, ai_signal=None, inverted=None, variable=None,
                        comparison=None, target_player=None, unit_ai_action=None, xs_function=None) -> Condition:
         """Used to add new condition to trigger. Please use trigger.new_condition.<condition_name> instead"""
 
         def get_default_condition_attributes(cond_type):
             """Gets the default condition attributes based on a certain condition type, with exception handling"""
             try:
                 return condition_dataset.default_attributes[cond_type]
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/unit.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -79,8 +79,12 @@
     @tile.setter
     def tile(self, tile: Tile) -> None:
         self.x = tile.x
         self.y = tile.y
 
     @property
     def name(self) -> str:
-        return pretty_format_name(helper.get_enum_from_unit_const(self.unit_const).name)
+        unit_enum = helper.get_enum_from_unit_const(self.unit_const)
+        if unit_enum:
+            return pretty_format_name(unit_enum.name)
+        else:
+            return f"Unknown{self.unit_const}"  # e.g."Unknown411"
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/data_objects/variable.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/data_objects/variable.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/de/map_manager_de.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/de/map_manager_de.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/de/trigger_manager_de.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/de/trigger_manager_de.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/map_manager.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/map_manager.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/trigger_manager.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/managers/unit_manager.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/managers/unit_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,20 +180,30 @@
         highest_id = 0  # If no units, default to 0
         for player in range(0, 9):
             for unit in self.units[player]:
                 if highest_id < unit.reference_id:
                     highest_id = unit.reference_id
         return highest_id + 1
 
-    def remove_unit(self, reference_id: int = None, unit: Unit = None):
+    def remove_unit(self, reference_id: int = None, unit: Unit = None) -> None:
+        """
+        Removes a unit. Please note that `unit=...` is a lot faster than `reference_id=...` due to reference_id having
+        to search through all units on the map. And unit has an ownership (player) attribute which is used for knowing
+        which list to remove the unit from.
+
+        Args:
+            reference_id (int): The id of the unit. Note that this is NOT a unit constant (So NOT: UnitInfo.ARCHER)
+            unit (Unit): The Unit object to be removed.
+        """
         if reference_id is not None and unit is not None:
             raise ValueError("Cannot use both unit_ref_id and unit arguments. Use one or the other.")
         if reference_id is None and unit is None:
             raise ValueError("Both unit_ref_id and unit arguments were unused. Use one.")
 
         if reference_id is not None:
             for player in range(0, 9):
                 for i, unit in enumerate(self.units[player]):
                     if unit.reference_id == reference_id:
                         del self.units[player][i]
+                        return
         elif unit is not None:
             self.units[unit.player.value].remove(unit)
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/enums/group_by.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/enums/group_by.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/tile.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/tile.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/trigger_ce_lock.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/trigger_ce_lock.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/objects/support/trigger_select.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/objects/support/trigger_select.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/scenarios/aoe2_de_scenario.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/scenarios/aoe2_de_scenario.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/scenarios/aoe2_scenario.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/scenarios/aoe2_scenario.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,26 @@
 import json
 import zlib
 from pathlib import Path
 from typing import Union, Dict
 
 import AoE2ScenarioParser.datasets.conditions as conditions
 import AoE2ScenarioParser.datasets.effects as effects
-from  AoE2ScenarioParser.helper.printers import s_print
+from AoE2ScenarioParser.helper.printers import s_print
 from AoE2ScenarioParser.helper.exceptions import InvalidScenarioStructureError, UnknownScenarioStructureError, \
     UnknownStructureError
 from AoE2ScenarioParser.helper.string_manipulations import create_textual_hex
 from AoE2ScenarioParser.helper.incremental_generator import IncrementalGenerator
 from AoE2ScenarioParser.objects.aoe2_object_manager import AoE2ObjectManager
 from AoE2ScenarioParser.objects.managers.map_manager import MapManager
 from AoE2ScenarioParser.objects.managers.trigger_manager import TriggerManager
 from AoE2ScenarioParser.objects.managers.unit_manager import UnitManager
 from AoE2ScenarioParser.sections.aoe2_file_section import AoE2FileSection
 
 
-def initialise_version_dependencies(game_version, scenario_version):
-    condition_json = get_version_dependant_structure_file(game_version, scenario_version, "conditions")
-
-    for condition_id, structure in condition_json.items():
-        condition_id = int(condition_id)
-
-        conditions.condition_names[condition_id] = structure['name']
-        conditions.default_attributes[condition_id] = structure['default_attributes']
-        conditions.attributes[condition_id] = structure['attributes']
-
-    effect_json = get_version_dependant_structure_file(game_version, scenario_version, "effects")
-
-    for effect_id, structure in effect_json.items():
-        effect_id = int(effect_id)
-
-        effects.effect_names[effect_id] = structure['name']
-        effects.default_attributes[effect_id] = structure['default_attributes']
-        effects.attributes[effect_id] = structure['attributes']
-
-
 class AoE2Scenario:
     @property
     def trigger_manager(self) -> TriggerManager:
         return self._object_manager.managers['Trigger']
 
     @property
     def unit_manager(self) -> UnitManager:
@@ -138,19 +118,28 @@
     def _add_to_sections(self, section):
         self.sections[section.name] = section
 
     """ ##########################################################################################
     ####################################### Write functions ######################################
     ########################################################################################## """
 
-    def write_to_file(self, filename):
-        self._write_from_structure(filename)
+    def write_to_file(self, filename, skip_reconstruction=False):
+        """
+        Write the scenario to a new file
+
+        Args:
+            filename (str): The location to write the file to
+            skip_reconstruction (bool): If reconstruction should be skipped. If true, this will ignore all changes made
+                using the managers (For example all changes made using trigger_manager).
+        """
+        self._write_from_structure(filename, skip_reconstruction)
 
-    def _write_from_structure(self, filename):
-        self._object_manager.reconstruct()
+    def _write_from_structure(self, filename, skip_reconstruction=False):
+        if not skip_reconstruction:
+            self._object_manager.reconstruct()
 
         s_print("\nFile writing from structure started...", final=True)
         binary = self._get_file_section_data(self.sections.get('FileHeader'))
 
         binary_list_to_be_compressed = []
         for file_part in self.sections.values():
             if file_part.name == "FileHeader":
@@ -224,14 +213,34 @@
                 result.append(create_textual_hex(trail.hex(), space_distance=2, enter_distance=24))
                 s_print("\tWriting trail finished successfully.", final=True)
 
             f.write(''.join(result))
         s_print("Writing structure to file finished successfully.", final=True)
 
 
+def initialise_version_dependencies(game_version, scenario_version):
+    condition_json = get_version_dependant_structure_file(game_version, scenario_version, "conditions")
+
+    for condition_id, structure in condition_json.items():
+        condition_id = int(condition_id)
+
+        conditions.condition_names[condition_id] = structure['name']
+        conditions.default_attributes[condition_id] = structure['default_attributes']
+        conditions.attributes[condition_id] = structure['attributes']
+
+    effect_json = get_version_dependant_structure_file(game_version, scenario_version, "effects")
+
+    for effect_id, structure in effect_json.items():
+        effect_id = int(effect_id)
+
+        effects.effect_names[effect_id] = structure['name']
+        effects.default_attributes[effect_id] = structure['default_attributes']
+        effects.attributes[effect_id] = structure['attributes']
+
+
 def get_file_version(generator: IncrementalGenerator):
     """Get first 4 bytes of a file, which contains the version of the scenario"""
     return generator.get_bytes(4, update_progress=False).decode('ASCII')
 
 
 def decompress_bytes(file_content):
     return zlib.decompress(file_content, -zlib.MAX_WBITS)
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/aoe2_file_section.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/aoe2_file_section.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,119 +1,100 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Dict, List
+from typing import Dict
 
 from AoE2ScenarioParser.helper import bytes_parser, string_manipulations
 from AoE2ScenarioParser.helper.incremental_generator import IncrementalGenerator
 from AoE2ScenarioParser.helper.list_functions import listify
 from AoE2ScenarioParser.helper.pretty_format import pretty_format_list
 from AoE2ScenarioParser.helper.string_manipulations import create_textual_hex, insert_char
 from AoE2ScenarioParser.sections.aoe2_struct_model import AoE2StructModel, model_dict_from_structure
 from AoE2ScenarioParser.sections.dependencies.dependency import handle_retriever_dependency
-from AoE2ScenarioParser.sections.retrievers.retriever import Retriever, duplicate_retriever_list
+from AoE2ScenarioParser.sections.retrievers.retriever import Retriever, duplicate_retriever_map, reset_retriever_map
 
 
 class SectionLevel(Enum):
     TOP_LEVEL = 0
     STRUCT = 1
 
 
 class AoE2FileSection:
-    dependencies = {}
-
-    def __init__(self, name, retrievers, struct_models=None, level=SectionLevel.TOP_LEVEL):
+    def __init__(self, name, retriever_map, struct_models=None, level=SectionLevel.TOP_LEVEL):
         if struct_models is None:
             struct_models = {}
 
         self.name: str = name
-        self.retrievers: List[Retriever] = retrievers
+        self.retriever_map = retriever_map
         self.byte_length: int = -1
         self.struct_models: Dict[str, AoE2StructModel] = struct_models
         self.level: SectionLevel = level
 
-        self.retriever_map = {}
-        for retriever in retrievers:
-            self.retriever_map[retriever.name] = retriever
-
-            if retriever.name in self.__class__.dependencies.keys():
-                for key, value in self.__class__.dependencies[retriever.name].items():
-                    setattr(retriever, key, value)
-
     @classmethod
     def from_model(cls, model, set_defaults=False) -> AoE2FileSection:
         """
         Create a copy (what was called struct before) from a model.
 
         Args:
             model (AoE2StructModel): The model to copy from
             set_defaults (bool): If retrievers need to be set to the default values
 
         Returns:
             An AoE2FileSection instance based on the model
         """
-        # Using pickle.loads(pickle.dumps(...)) instead of copy.deepcopy()
-        # Reason for this is the huge speed difference. Details can be found at:
-        # https://stackoverflow.com/a/29385667/7230293
-        duplicate_list = duplicate_retriever_list(model.retrievers)
+        duplicate_rmap = duplicate_retriever_map(model.retriever_map)
         if set_defaults:
-            for retriever in duplicate_list:
-                retriever.set_data_to_default()
+            reset_retriever_map(duplicate_rmap)
 
         return cls(
             name=model.name,
-            retrievers=duplicate_list,
+            retriever_map=duplicate_rmap,
             struct_models=model.structs,
             level=SectionLevel.STRUCT
         )
 
     @classmethod
     def from_structure(cls, section_name, structure):
-        retrievers = []
+        retriever_map = {}
         for name, attr in structure.get('retrievers').items():
-            retrievers.append(Retriever.from_structure(name, attr))
+            retriever_map[name] = Retriever.from_structure(name, attr)
 
         structs = model_dict_from_structure(structure)
-        return cls(section_name, retrievers, structs)
-
-    @classmethod
-    def from_data(cls, name, retrievers, data, sections):
-        part = cls(name, retrievers)
-        part.set_data(data, sections)
-        return part
+        return cls(section_name, retriever_map, structs)
 
     def get_data_as_bytes(self):
         result = []
-        for retriever in self.retrievers:
+        retriever: Retriever
+        for retriever in self.retriever_map.values():
             result.append(retriever.get_data_as_bytes())
         return b''.join(result)
 
-    def set_data_from_generator(self, igenerator: IncrementalGenerator, sections: Dict[str, AoE2FileSection]) \
-            -> None:
+    def set_data_from_generator(self, igenerator: IncrementalGenerator, sections: Dict[str, AoE2FileSection]) -> None:
         """
         Fill data from all retrievers with data from the given generator. Generator is expected to return bytes.
         Bytes will be parsed based on the retrievers. The total length of bytes read to fill this section is also stored
         in this section as `byte_length`.
 
         Args:
             igenerator: A generator from a binary scenario file
             sections: A list of sections to reference when the retrievers have
-                dependencies to orf rom them.
+                dependencies to or from them.
         """
         total_length = 0
-        for retriever in self.retrievers:
+        for retriever in self.retriever_map.values():
             try:
                 handle_retriever_dependency(retriever, "construct", self, sections)
                 if retriever.datatype.type == "struct":
                     retriever.data = []
-                    struct_name = retriever.datatype.var[7:]  # 7 == len("struct:") | Remove struct naming prefix
+                    struct_name = retriever.datatype.var[7:]  # 7 == len("struct:") >> Removing struct naming prefix
                     for _ in range(retriever.datatype.repeat):
                         model = self.struct_models.get(struct_name)
                         if model is None:
                             raise ValueError(f"Model '{struct_name}' not found. Likely not defined in structure.")
+
                         struct = AoE2FileSection.from_model(model)
                         struct.set_data_from_generator(igenerator, sections)
                         retriever.data.append(struct)
 
                         total_length += struct.byte_length
                 else:
                     retrieved_bytes = bytes_parser.retrieve_bytes(igenerator, retriever)
@@ -125,26 +106,28 @@
                     print(struct.get_byte_structure_as_string(sections))
                 print(f"\n\n[{e.__class__.__name__}] Occurred while setting data in:\n\t{retriever}")
                 raise e
 
         self.byte_length = total_length
 
     def set_data(self, data, sections):
-        if len(data) == len(self.retrievers):
+        retrievers = self.retriever_map.values()
+
+        if len(data) == len(retrievers):
             for i in range(len(data)):
-                self.retrievers[i].data = data[i]
+                retrievers[i].data = data[i]
 
-                if hasattr(self.retrievers[i], 'on_construct'):
-                    handle_retriever_dependency(self.retrievers[i], "construct", self, sections)
+                if hasattr(retrievers[i], 'on_construct'):
+                    handle_retriever_dependency(retrievers[i], "construct", self, sections)
         else:
             print(f"\nError in: {self.__class__.__name__}")
             print(f"Data: (len: {len(data)}) "
                   f"{pretty_format_list([f'{i}: {str(x)}' for i, x in enumerate(data)])}")
-            print(f"Retrievers: (len: {len(self.retrievers)}) "
-                  f"{pretty_format_list([f'{i}: {str(x)}' for i, x in enumerate(self.retrievers)])}")
+            print(f"Retrievers: (len: {len(retrievers)}) "
+                  f"{pretty_format_list([f'{i}: {str(x)}' for i, x in enumerate(self.retriever_map.values())])}")
             raise ValueError("Data list isn't the same size as the DataType list")
 
     def __getattr__(self, item):
         """Providing a default way to access retriever data labeled 'name'"""
         if 'retriever_map' not in self.__dict__:
             return super().__getattribute__(item)
         else:
@@ -180,30 +163,30 @@
 
     def get_byte_structure_as_string(self, sections, skip_retrievers=None):
         if skip_retrievers is None:
             skip_retrievers = []
 
         byte_structure = "\n" + self.get_header_string()
 
-        for retriever in self.retrievers:
-            if retriever.name in skip_retrievers:
+        for key, retriever in self.retriever_map.items():
+            if key in skip_retrievers:
                 continue
             byte_structure += "\n"
 
             listed_retriever_data = listify(retriever.data)
             struct_header_set = False
             for struct in listed_retriever_data:
                 if isinstance(struct, AoE2FileSection):
                     if not struct_header_set:
-                        byte_structure += f"\n{'#' * 27} {retriever.name} ({retriever.datatype.to_simple_string()})"
+                        byte_structure += f"\n{'#' * 27} {key} ({retriever.datatype.to_simple_string()})"
                         struct_header_set = True
                     byte_structure += struct.get_byte_structure_as_string(sections)
             # Struct Header was set. Retriever was struct, data retrieved using recursion. Next retriever.
             if struct_header_set:
-                byte_structure += f"{'#' * 27} End of: {retriever.name} ({retriever.datatype.to_simple_string()})\n"
+                byte_structure += f"{'#' * 27} End of: {key} ({retriever.datatype.to_simple_string()})\n"
                 continue
 
             retriever_data_bytes = retriever.get_data_as_bytes()
             if retriever_data_bytes is None:
                 return byte_structure
             else:
                 retriever_data_bytes = retriever_data_bytes.hex()
@@ -235,31 +218,30 @@
             byte_structure += "\n".join(combined_strings)
 
         return byte_structure + "\n"
 
     def __str__(self):
         represent = self.name + ": \n"
 
-        for i, val in enumerate(self.retrievers):
-            if type(self.retrievers[i].data) is list and len(self.retrievers[i].data) > 0:
-                if isinstance(self.retrievers[i].data[0], AoE2FileSection):
-                    represent += "\t" + val.name + ": [\n"
-                    for x in self.retrievers[i].data:
+        for retriever in self.retriever_map.values():
+            if type(retriever.data) is list and len(retriever.data) > 0:
+                if isinstance(retriever.data[0], AoE2FileSection):
+                    represent += "\t" + retriever.name + ": [\n"
+                    for x in retriever.data:
                         represent += "\t\t" + str(x)
                     represent += "\t]\n"
                 else:
                     represent += self._entry_to_string(
-                        val.name,
-                        str(self.retrievers[i].data),
-                        str(val.datatype.to_simple_string())
+                        retriever.name,
+                        str(retriever.data),
+                        str(retriever.datatype.to_simple_string())
                     )
             else:
-                if self.retrievers[i].data is not None:
-                    data = self.retrievers[i].data
-                else:
-                    data = "None"
-                represent += self._entry_to_string(val.name, str(data), str(val.datatype.to_simple_string()))
+                data = retriever.data or "None"
+                represent += self._entry_to_string(
+                    retriever.name, str(data), str(retriever.datatype.to_simple_string())
+                )
 
         return represent
 
     def __repr__(self):
         return f"<AoE2FileSection> {self.name}"
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/aoe2_struct_model.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/aoe2_struct_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import annotations
 
-from typing import List, Dict
+from typing import Dict
 
-from AoE2ScenarioParser.helper.pretty_format import pretty_format_list
+from AoE2ScenarioParser.helper.pretty_format import pretty_format_dict
 from AoE2ScenarioParser.sections.retrievers.retriever import Retriever
 
 
 class AoE2StructModel:
-    def __init__(self, name: str, retrievers: List[Retriever], structs: Dict[AoE2StructModel]):
+    def __init__(self, name: str, retriever_map: Dict[str, Retriever], structs: Dict[AoE2StructModel]):
         self.name = name
-        self.retrievers = retrievers
+        self.retriever_map = retriever_map
         self.structs = structs
 
     @classmethod
     def from_structure(cls, name, structure) -> AoE2StructModel:
-        retrievers = []
+        retriever_map = {}
         for retriever_name, attr in structure.get('retrievers').items():
-            retrievers.append(Retriever.from_structure(retriever_name, attr))
+            retriever_map[retriever_name] = Retriever.from_structure(retriever_name, attr)
         structs = model_dict_from_structure(structure)
 
-        return cls(name, retrievers, structs)
+        return cls(name, retriever_map, structs)
 
     def __str__(self):
-        return_string = f"[AoE2StructModel] {self.name} -> retrievers: " + pretty_format_list(self.retrievers)
-        return return_string
+        return f"[AoE2StructModel] {self.name} -> retrievers: " + pretty_format_dict(self.retriever_map)
 
 
 def model_dict_from_structure(structure) -> Dict[AoE2StructModel]:
     models = {}
     for name, attr in structure.get('structs', {}).items():
         # Create struct model
         models[name] = AoE2StructModel.from_structure(name, attr)
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import math
-from typing import List
 
 from AoE2ScenarioParser.sections.dependencies.dependency_action import DependencyAction
 from AoE2ScenarioParser.sections.retrievers.retriever import Retriever
 
 
 def refresh_targets(retriever_event, section, sections):
     for target in retriever_event.dependency_target.targets:
@@ -17,15 +16,15 @@
     handle_retriever_dependency(retriever, "refresh", section, sections)
 
 
 def handle_retriever_dependency(retriever: Retriever, state, section, sections):
     on_x = f'on_{state}'
     if not hasattr(retriever, on_x):
         return
-    self_list: List[Retriever] = section.retrievers
+
     retriever_event = getattr(retriever, on_x)  # construct, commit or refresh
 
     action = retriever_event.dependency_action
 
     if action == DependencyAction.REFRESH_SELF:
         execute_refresh_action(retriever, section, sections)
     elif action == DependencyAction.REFRESH:
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency_eval.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency_eval.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/dependency_target.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/dependency_target.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/dependencies/retriever_dependency.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/dependencies/retriever_dependency.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/datatype.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/datatype.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/retriever.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/retriever.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from __future__ import annotations
 
+import pickle
+from typing import Dict
+
 from AoE2ScenarioParser.helper import bytes_parser, string_manipulations
 from AoE2ScenarioParser.helper.bytes_conversions import parse_bytes_to_val, parse_val_to_bytes
 from AoE2ScenarioParser.helper.list_functions import listify
 from AoE2ScenarioParser.helper.pretty_format import pretty_format_list
 from AoE2ScenarioParser.sections.dependencies.dependency_action import DependencyAction
 from AoE2ScenarioParser.sections.dependencies.retriever_dependency import RetrieverDependency
 from AoE2ScenarioParser.sections.retrievers.datatype import DataType
@@ -73,15 +76,14 @@
         if self.log_value:
             print(f"{self.to_simple_string()} (Data: {self.data}) retrieved: {joined_result}")
 
         return joined_result
 
     def set_data_from_bytes(self, bytes_list):
         if self.datatype.repeat > 0 and len(bytes_list) == 0:
-            print(type(bytes_list), bytes_list)
             raise ValueError("Unable to set bytes when no bytes are given")
         if self.datatype.repeat > 0 and self.datatype.repeat != len(bytes_list):
             raise ValueError("Unable to set bytes when bytes list isn't equal to repeat")
 
         result = [parse_bytes_to_val(self, entry_bytes) for entry_bytes in bytes_list]
         self.data = bytes_parser.vorl(self, result)
 
@@ -178,16 +180,21 @@
         if type(self.data) is list:
             data = str(pretty_format_list(self.data))
         else:
             data = string_manipulations.q_str(self.data)
         return f"{self.to_simple_string()} >>> {data}"
 
 
-def duplicate_retriever_list(retriever_list):
-    return [r.duplicate() for r in retriever_list]
+def duplicate_retriever_map(retriever_map: Dict[str, Retriever]) -> Dict[str, Retriever]:
+    return pickle.loads(pickle.dumps(retriever_map))
+
+
+def reset_retriever_map(retriever_map: Dict[str, Retriever]) -> None:
+    for retriever in retriever_map.values():
+        retriever.set_data_to_default()
 
 
 def _evaluate_is_list_attribute(retriever, dependency):
     if dependency.dependency_action == DependencyAction.SET_REPEAT and retriever.is_list is None:
         retriever.is_list = True
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/retriever_object_link.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/retriever_object_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,14 @@
         retriever = None
         file_section = section
         for index, item in enumerate(self.splitted_link):
             if "[" in item:
                 file_section = getattr(file_section, item[:-11])[number_hist[index]]
             else:
                 retriever = file_section.retriever_map[item]
-                # retriever = get_retriever_by_name(file_section.retrievers, item)
-        retriever_list = file_section.retrievers
 
         if retriever is None:
             raise ValueError("RetrieverObjectLink is unable to find retriever")
 
         if self.process_as_object:
             struct_datatype = retriever.datatype.var
 
@@ -168,15 +166,15 @@
                     player_units = getattr(player_units_section, item)
                     units.append(self.process_object_list(player_units, [player], sections, scenario_version))
         return units
 
     def _commit_special_unit_case(self, sections, value):
         for player, player_unit in enumerate(value):
             player_unit_retriever = sections["Units"].players_units[player]
-            retriever_list = player_unit_retriever.retrievers
+            retriever_list = player_unit_retriever.retriever_map.values()
             units = player_unit_retriever.retriever_map["units"]
             # units = get_retriever_by_name(retriever_list, "units")
             struct_model = player_unit_retriever.struct_models["UnitStruct"]
 
             RetrieverObjectLink.update_retriever_length(units, struct_model, len(value[player]))
             RetrieverObjectLink.commit_object_list(player_unit, sections, [player])
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/sections/retrievers/support.py` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/sections/retrievers/support.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/changelog.md` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/changelog.md`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/conditions.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/conditions.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9661154401154397%*

 * *Differences: {"'0'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'1'": "{'attributes': {insert: [(2, 'area_x1'), (3, 'area_y1'), (4, 'area_x2'), (5, 'area_y2')], "*

 * *        "delete: [5, 4, 3, 2]}, 'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': "*

 * *        "-1, 'area_y2': -1, delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'10'": "{'default_attributes': {'area_x1': -1, 'area_y1': […]*

```diff
@@ -1,18 +1,18 @@
 {
     "0": {
         "attributes": [
             "condition_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 0,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -27,26 +27,26 @@
         },
         "name": "none"
     },
     "1": {
         "attributes": [
             "condition_type",
             "unit_object",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 1,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -65,18 +65,18 @@
         "attributes": [
             "condition_type",
             "timer",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 10,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -95,18 +95,18 @@
         "attributes": [
             "condition_type",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 11,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -125,18 +125,18 @@
         "attributes": [
             "condition_type",
             "ai_signal",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 12,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -155,18 +155,18 @@
         "attributes": [
             "condition_type",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 13,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -189,18 +189,18 @@
             "object_list",
             "object_group",
             "object_type",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 14,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -218,18 +218,18 @@
     "15": {
         "attributes": [
             "condition_type",
             "unit_object"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 15,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -247,18 +247,18 @@
     "16": {
         "attributes": [
             "condition_type",
             "unit_object"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 16,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -278,18 +278,18 @@
             "condition_type",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 17,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -309,18 +309,18 @@
             "condition_type",
             "quantity",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 18,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -339,18 +339,18 @@
         "attributes": [
             "condition_type",
             "quantity",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 19,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -370,18 +370,18 @@
             "condition_type",
             "unit_object",
             "next_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 2,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -399,18 +399,18 @@
     "20": {
         "attributes": [
             "condition_type",
             "quantity"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 20,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -431,18 +431,18 @@
             "quantity",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 21,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -463,18 +463,18 @@
             "quantity",
             "inverted",
             "variable",
             "comparison"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 22,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -495,18 +495,18 @@
             "quantity",
             "unit_object",
             "inverted",
             "comparison"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 23,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -527,18 +527,18 @@
             "quantity",
             "source_player",
             "inverted",
             "target_player"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 24,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -560,18 +560,18 @@
             "object_list",
             "source_player",
             "object_group",
             "object_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 3,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -588,27 +588,27 @@
     },
     "4": {
         "attributes": [
             "condition_type",
             "quantity",
             "object_list",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 4,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -625,28 +625,28 @@
     },
     "5": {
         "attributes": [
             "condition_type",
             "quantity",
             "object_list",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 5,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -665,18 +665,18 @@
         "attributes": [
             "condition_type",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 6,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -696,18 +696,18 @@
             "condition_type",
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 7,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -728,18 +728,18 @@
             "quantity",
             "attribute",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": 0,
             "comparison": -1,
             "condition_type": 8,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -759,18 +759,18 @@
             "condition_type",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 9,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/effects.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/effects.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9698738469746877%*

 * *Differences: {"'0'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'1'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'10'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *         "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'11'": "{'def […]*

```diff
@@ -2,18 +2,18 @@
     "0": {
         "attributes": [
             "effect_type"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 0,
@@ -61,18 +61,18 @@
             "diplomacy",
             "source_player",
             "target_player"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": 0,
             "display_time": -1,
             "effect_type": 1,
@@ -118,18 +118,18 @@
         "attributes": [
             "effect_type",
             "ai_script_goal"
         ],
         "default_attributes": {
             "ai_script_goal": 1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 10,
@@ -180,18 +180,18 @@
             "location_y",
             "item_id",
             "facet"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 11,
@@ -237,29 +237,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 12,
@@ -306,18 +306,18 @@
             "effect_type",
             "source_player",
             "enabled"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 13,
@@ -360,29 +360,29 @@
         "name": "declare_victory"
     },
     "14": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 14,
@@ -425,29 +425,29 @@
         "name": "kill_object"
     },
     "15": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 15,
@@ -491,24 +491,23 @@
     },
     "16": {
         "attributes": [
             "effect_type",
             "source_player",
             "location_x",
             "location_y",
-            "location_object_reference",
             "scroll"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 16,
@@ -554,29 +553,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 17,
@@ -620,30 +619,30 @@
     },
     "18": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "target_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "flash_object",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 18,
@@ -689,29 +688,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 19,
@@ -759,18 +758,18 @@
             "source_player",
             "technology",
             "force_research_technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 2,
@@ -823,18 +822,18 @@
             "play_sound",
             "message",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": 10,
             "effect_type": 20,
@@ -880,18 +879,18 @@
         "attributes": [
             "effect_type",
             "instruction_panel_position"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 21,
@@ -934,29 +933,29 @@
         "name": "clear_instructions"
     },
     "22": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 22,
@@ -1001,18 +1000,18 @@
     "23": {
         "attributes": [
             "effect_type"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 23,
@@ -1056,29 +1055,29 @@
     },
     "24": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 24,
@@ -1127,18 +1126,18 @@
             "source_player",
             "location_x",
             "location_y"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 25,
@@ -1182,28 +1181,28 @@
     },
     "26": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "message",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 26,
@@ -1247,30 +1246,30 @@
     },
     "27": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 27,
@@ -1315,30 +1314,30 @@
     "28": {
         "attributes": [
             "effect_type",
             "armour_attack_quantity",
             "armour_attack_class",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": 0,
             "armour_attack_quantity": 1,
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 28,
@@ -1381,29 +1380,29 @@
         "name": "change_object_attack"
     },
     "29": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 29,
@@ -1452,18 +1451,18 @@
             "string_id",
             "message",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 3,
@@ -1509,29 +1508,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 30,
@@ -1576,30 +1575,30 @@
     "31": {
         "attributes": [
             "effect_type",
             "armour_attack_quantity",
             "armour_attack_class",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": 0,
             "armour_attack_quantity": 1,
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 31,
@@ -1643,30 +1642,30 @@
     },
     "32": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 32,
@@ -1710,29 +1709,29 @@
     },
     "33": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 33,
@@ -1776,29 +1775,29 @@
     },
     "34": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 34,
@@ -1843,29 +1842,29 @@
     "35": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 35,
@@ -1908,30 +1907,30 @@
         "name": "teleport_object"
     },
     "36": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "attack_stance",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": 0,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 36,
@@ -1981,18 +1980,18 @@
             "time_unit",
             "timer",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": 10,
             "effect_type": 37,
@@ -2041,18 +2040,18 @@
             "source_player",
             "enabled",
             "item_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 38,
@@ -2101,18 +2100,18 @@
             "technology",
             "enabled",
             "item_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 39,
@@ -2162,18 +2161,18 @@
             "location_y",
             "location_object_reference",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 4,
@@ -2224,18 +2223,18 @@
             "wood",
             "stone",
             "gold"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 40,
@@ -2283,18 +2282,18 @@
             "source_player",
             "target_player",
             "visibility_state"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 41,
@@ -2337,30 +2336,30 @@
         "name": "set_player_visibility"
     },
     "42": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 42,
@@ -2404,30 +2403,30 @@
     },
     "43": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "target_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 43,
@@ -2476,18 +2475,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 44,
@@ -2535,18 +2534,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 45,
@@ -2595,18 +2594,18 @@
             "source_player",
             "object_list_unit_id_2",
             "button_location"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": 0,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 46,
@@ -2655,18 +2654,18 @@
             "technology",
             "object_list_unit_id_2",
             "button_location"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": 7,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 47,
@@ -2714,18 +2713,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 48,
@@ -2768,28 +2767,28 @@
         "name": "change_civilization_name"
     },
     "49": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 49,
@@ -2838,18 +2837,18 @@
             "tribute_list",
             "source_player",
             "target_player"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 5,
@@ -2895,18 +2894,18 @@
         "attributes": [
             "effect_type",
             "ai_signal_value"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 50,
@@ -2957,18 +2956,18 @@
             "item_id",
             "operation",
             "object_attributes"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 51,
@@ -3018,18 +3017,18 @@
             "source_player",
             "item_id",
             "operation"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 52,
@@ -3079,18 +3078,18 @@
             "item_id",
             "operation",
             "variable"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 53,
@@ -3139,18 +3138,18 @@
             "operation",
             "variable",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 56,
@@ -3196,18 +3195,18 @@
         "attributes": [
             "effect_type",
             "timer"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 57,
@@ -3253,18 +3252,18 @@
         "attributes": [
             "effect_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 6,
@@ -3310,18 +3309,18 @@
         "attributes": [
             "effect_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 7,
@@ -3367,18 +3366,18 @@
         "attributes": [
             "effect_type",
             "trigger_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 8,
@@ -3424,18 +3423,18 @@
         "attributes": [
             "effect_type",
             "trigger_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 9,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.37/structure.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.37/structure.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999646624893571%*

 * *Differences: {"'Triggers'": "{'structs': {'TriggerStruct': {'structs': {'EffectStruct': {'retrievers': "*

 * *               "{'area_x1': OrderedDict([('type', 's32'), ('default', -1)]), 'area_y1': "*

 * *               "OrderedDict([('type', 's32'), ('default', -1)]), 'area_x2': OrderedDict([('type', "*

 * *               "'s32'), ('default', -1)]), 'area_y2': OrderedDict([('type', 's32'), ('default', "*

 * *               "-1)]), delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}, "*

 * *               "'ConditionStruct': {'retrievers […]*

```diff
@@ -1613,27 +1613,27 @@
                 "structs": {
                     "ConditionStruct": {
                         "retrievers": {
                             "ai_signal": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_x": {
+                            "area_x1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_y": {
+                            "area_x2": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_x": {
+                            "area_y1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_y": {
+                            "area_y2": {
                                 "default": -1,
                                 "type": "s32"
                             },
                             "attribute": {
                                 "default": -1,
                                 "type": "s32"
                             },
@@ -1713,27 +1713,27 @@
                                 "default": -1,
                                 "type": "s32"
                             },
                             "ai_signal_value": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_x": {
+                            "area_x1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_y": {
+                            "area_x2": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_x": {
+                            "area_y1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_y": {
+                            "area_y2": {
                                 "default": -1,
                                 "type": "s32"
                             },
                             "armour_attack_class": {
                                 "default": -1,
                                 "dependencies": {
                                     "on_construct": {
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/conditions.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/conditions.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9694341500793114%*

 * *Differences: {"'0'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'1'": "{'attributes': {insert: [(2, 'area_x1'), (3, 'area_y1'), (4, 'area_x2'), (5, 'area_y2')], "*

 * *        "delete: [5, 4, 3, 2]}, 'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': "*

 * *        "-1, 'area_y2': -1, delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'10'": "{'default_attributes': {'area_x1': -1, 'area_y1': […]*

```diff
@@ -1,18 +1,18 @@
 {
     "0": {
         "attributes": [
             "condition_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 0,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -29,26 +29,26 @@
         },
         "name": "none"
     },
     "1": {
         "attributes": [
             "condition_type",
             "unit_object",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 1,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -69,18 +69,18 @@
         "attributes": [
             "condition_type",
             "timer",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 10,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -101,18 +101,18 @@
         "attributes": [
             "condition_type",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 11,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -133,18 +133,18 @@
         "attributes": [
             "condition_type",
             "ai_signal",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 12,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -165,18 +165,18 @@
         "attributes": [
             "condition_type",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 13,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -201,18 +201,18 @@
             "object_list",
             "object_group",
             "object_type",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 14,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -232,18 +232,18 @@
     "15": {
         "attributes": [
             "condition_type",
             "unit_object"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 15,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -263,18 +263,18 @@
     "16": {
         "attributes": [
             "condition_type",
             "unit_object"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 16,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -296,18 +296,18 @@
             "condition_type",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 17,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -329,18 +329,18 @@
             "condition_type",
             "quantity",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 18,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -361,18 +361,18 @@
         "attributes": [
             "condition_type",
             "quantity",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 19,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -394,18 +394,18 @@
             "condition_type",
             "unit_object",
             "next_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 2,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -425,18 +425,18 @@
     "20": {
         "attributes": [
             "condition_type",
             "quantity"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 20,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -459,18 +459,18 @@
             "quantity",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 21,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -493,18 +493,18 @@
             "quantity",
             "inverted",
             "variable",
             "comparison"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 22,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -527,18 +527,18 @@
             "quantity",
             "unit_object",
             "inverted",
             "comparison"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 23,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -561,18 +561,18 @@
             "quantity",
             "source_player",
             "inverted",
             "target_player"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 24,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -591,18 +591,18 @@
     },
     "25": {
         "attributes": [
             "xs_function"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 25,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -623,18 +623,18 @@
         "attributes": [
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 26,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -655,18 +655,18 @@
         "attributes": [
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 27,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -688,18 +688,18 @@
             "unit_object",
             "next_object",
             "inverted",
             "unit_ai_action"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 28,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -716,18 +716,18 @@
         },
         "name": "object_has_action"
     },
     "29": {
         "attributes": [],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 29,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -751,18 +751,18 @@
             "object_list",
             "source_player",
             "object_group",
             "object_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 3,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -782,18 +782,18 @@
     "30": {
         "attributes": [
             "ai_signal",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 30,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -812,27 +812,27 @@
     },
     "4": {
         "attributes": [
             "condition_type",
             "quantity",
             "object_list",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 4,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -851,28 +851,28 @@
     },
     "5": {
         "attributes": [
             "condition_type",
             "quantity",
             "object_list",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 5,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -893,18 +893,18 @@
         "attributes": [
             "condition_type",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 6,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -926,18 +926,18 @@
             "condition_type",
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 7,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -960,18 +960,18 @@
             "quantity",
             "attribute",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": 0,
             "comparison": -1,
             "condition_type": 8,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -993,18 +993,18 @@
             "condition_type",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 9,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/effects.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/effects.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9673429054810855%*

 * *Differences: {"'0'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'1'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'10'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *         "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'11'": "{'def […]*

```diff
@@ -2,18 +2,18 @@
     "0": {
         "attributes": [
             "effect_type"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 0,
@@ -62,18 +62,18 @@
             "diplomacy",
             "source_player",
             "target_player"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": 0,
             "display_time": -1,
             "effect_type": 1,
@@ -120,18 +120,18 @@
         "attributes": [
             "effect_type",
             "ai_script_goal"
         ],
         "default_attributes": {
             "ai_script_goal": 1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 10,
@@ -183,18 +183,18 @@
             "location_y",
             "item_id",
             "facet"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 11,
@@ -241,29 +241,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 12,
@@ -311,18 +311,18 @@
             "effect_type",
             "source_player",
             "enabled"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 13,
@@ -366,29 +366,29 @@
         "name": "declare_victory"
     },
     "14": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 14,
@@ -432,29 +432,29 @@
         "name": "kill_object"
     },
     "15": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 15,
@@ -499,24 +499,23 @@
     },
     "16": {
         "attributes": [
             "effect_type",
             "source_player",
             "location_x",
             "location_y",
-            "location_object_reference",
             "scroll"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 16,
@@ -563,29 +562,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 17,
@@ -630,30 +629,30 @@
     },
     "18": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "target_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "flash_object",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 18,
@@ -700,29 +699,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 19,
@@ -771,18 +770,18 @@
             "source_player",
             "technology",
             "force_research_technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 2,
@@ -836,18 +835,18 @@
             "play_sound",
             "message",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": 10,
             "effect_type": 20,
@@ -894,18 +893,18 @@
         "attributes": [
             "effect_type",
             "instruction_panel_position"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 21,
@@ -949,29 +948,29 @@
         "name": "clear_instructions"
     },
     "22": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 22,
@@ -1017,18 +1016,18 @@
     "23": {
         "attributes": [
             "effect_type"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 23,
@@ -1073,29 +1072,29 @@
     },
     "24": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 24,
@@ -1145,18 +1144,18 @@
             "source_player",
             "location_x",
             "location_y"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 25,
@@ -1201,28 +1200,28 @@
     },
     "26": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "message",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 26,
@@ -1267,30 +1266,30 @@
     },
     "27": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 27,
@@ -1336,30 +1335,30 @@
     "28": {
         "attributes": [
             "effect_type",
             "armour_attack_quantity",
             "armour_attack_class",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": 0,
             "armour_attack_quantity": 1,
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 28,
@@ -1403,29 +1402,29 @@
         "name": "change_object_attack"
     },
     "29": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 29,
@@ -1475,18 +1474,18 @@
             "string_id",
             "message",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 3,
@@ -1533,29 +1532,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 30,
@@ -1601,30 +1600,30 @@
     "31": {
         "attributes": [
             "effect_type",
             "armour_attack_quantity",
             "armour_attack_class",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": 0,
             "armour_attack_quantity": 1,
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 31,
@@ -1669,30 +1668,30 @@
     },
     "32": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 32,
@@ -1737,29 +1736,29 @@
     },
     "33": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 33,
@@ -1804,29 +1803,29 @@
     },
     "34": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 34,
@@ -1872,29 +1871,29 @@
     "35": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 35,
@@ -1938,30 +1937,30 @@
         "name": "teleport_object"
     },
     "36": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "attack_stance",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": 0,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 36,
@@ -2012,18 +2011,18 @@
             "time_unit",
             "timer",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": 10,
             "effect_type": 37,
@@ -2073,18 +2072,18 @@
             "source_player",
             "enabled",
             "item_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 38,
@@ -2134,18 +2133,18 @@
             "technology",
             "enabled",
             "item_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 39,
@@ -2196,18 +2195,18 @@
             "location_y",
             "location_object_reference",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 4,
@@ -2259,18 +2258,18 @@
             "wood",
             "stone",
             "gold"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 40,
@@ -2319,18 +2318,18 @@
             "source_player",
             "target_player",
             "visibility_state"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 41,
@@ -2374,30 +2373,30 @@
         "name": "set_player_visibility"
     },
     "42": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 42,
@@ -2442,30 +2441,30 @@
     },
     "43": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "target_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 43,
@@ -2515,18 +2514,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 44,
@@ -2575,18 +2574,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 45,
@@ -2636,18 +2635,18 @@
             "source_player",
             "object_list_unit_id_2",
             "button_location"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": 0,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 46,
@@ -2697,18 +2696,18 @@
             "technology",
             "object_list_unit_id_2",
             "button_location"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": 7,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 47,
@@ -2757,18 +2756,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 48,
@@ -2812,28 +2811,28 @@
         "name": "change_civilization_name"
     },
     "49": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 49,
@@ -2883,18 +2882,18 @@
             "tribute_list",
             "source_player",
             "target_player"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 5,
@@ -2941,18 +2940,18 @@
         "attributes": [
             "effect_type",
             "ai_signal_value"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 50,
@@ -3004,18 +3003,18 @@
             "item_id",
             "operation",
             "object_attributes"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 51,
@@ -3066,18 +3065,18 @@
             "source_player",
             "item_id",
             "operation"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 52,
@@ -3128,18 +3127,18 @@
             "item_id",
             "operation",
             "variable"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 53,
@@ -3184,27 +3183,27 @@
     },
     "54": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 54,
@@ -3251,18 +3250,18 @@
         "attributes": [
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 55,
@@ -3312,18 +3311,18 @@
             "operation",
             "variable",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 56,
@@ -3370,18 +3369,18 @@
         "attributes": [
             "effect_type",
             "timer"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 57,
@@ -3424,27 +3423,27 @@
         },
         "name": "clear_timer"
     },
     "58": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 58,
@@ -3486,27 +3485,27 @@
             "wood": -1
         },
         "name": "change_object_player_color"
     },
     "59": {
         "attributes": [
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 59,
@@ -3553,18 +3552,18 @@
         "attributes": [
             "effect_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 6,
@@ -3608,27 +3607,27 @@
         "name": "unlock_gate"
     },
     "60": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 60,
@@ -3671,27 +3670,27 @@
         },
         "name": "change_object_player_name"
     },
     "61": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 61,
@@ -3734,27 +3733,27 @@
         },
         "name": "disable_unit_targeting"
     },
     "62": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 62,
@@ -3805,18 +3804,18 @@
             "wood",
             "stone",
             "gold"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 63,
@@ -3864,18 +3863,18 @@
             "quantity",
             "source_player",
             "technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 64,
@@ -3924,18 +3923,18 @@
             "technology",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 65,
@@ -3984,18 +3983,18 @@
             "technology",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 66,
@@ -4042,18 +4041,18 @@
         "attributes": [
             "source_player",
             "technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 67,
@@ -4100,18 +4099,18 @@
         "attributes": [
             "source_player",
             "technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 68,
@@ -4157,18 +4156,18 @@
     "69": {
         "attributes": [
             "ai_signal_value"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 69,
@@ -4215,18 +4214,18 @@
         "attributes": [
             "effect_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 7,
@@ -4269,27 +4268,27 @@
         },
         "name": "lock_gate"
     },
     "70": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 70,
@@ -4332,27 +4331,27 @@
         },
         "name": "disable_object_selection"
     },
     "71": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 71,
@@ -4399,18 +4398,18 @@
         "attributes": [
             "effect_type",
             "trigger_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 8,
@@ -4457,18 +4456,18 @@
         "attributes": [
             "effect_type",
             "trigger_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 9,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.40/structure.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.40/structure.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999699519230769%*

 * *Differences: {"'Triggers'": "{'structs': {'TriggerStruct': {'structs': {'EffectStruct': {'retrievers': "*

 * *               "{'area_x1': OrderedDict([('type', 's32'), ('default', -1)]), 'area_y1': "*

 * *               "OrderedDict([('type', 's32'), ('default', -1)]), 'area_x2': OrderedDict([('type', "*

 * *               "'s32'), ('default', -1)]), 'area_y2': OrderedDict([('type', 's32'), ('default', "*

 * *               "-1)]), delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}, "*

 * *               "'ConditionStruct': {'retrievers […]*

```diff
@@ -1728,27 +1728,27 @@
                 "structs": {
                     "ConditionStruct": {
                         "retrievers": {
                             "ai_signal": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_x": {
+                            "area_x1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_y": {
+                            "area_x2": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_x": {
+                            "area_y1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_y": {
+                            "area_y2": {
                                 "default": -1,
                                 "type": "s32"
                             },
                             "attribute": {
                                 "default": -1,
                                 "type": "s32"
                             },
@@ -1840,27 +1840,27 @@
                                 "default": -1,
                                 "type": "s32"
                             },
                             "ai_signal_value": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_x": {
+                            "area_x1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_y": {
+                            "area_x2": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_x": {
+                            "area_y1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_y": {
+                            "area_y2": {
                                 "default": -1,
                                 "type": "s32"
                             },
                             "armour_attack_class": {
                                 "default": -1,
                                 "dependencies": {
                                     "on_construct": {
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/conditions.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/conditions.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9694341500793114%*

 * *Differences: {"'0'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'1'": "{'attributes': {insert: [(2, 'area_x1'), (3, 'area_y1'), (4, 'area_x2'), (5, 'area_y2')], "*

 * *        "delete: [5, 4, 3, 2]}, 'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': "*

 * *        "-1, 'area_y2': -1, delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'10'": "{'default_attributes': {'area_x1': -1, 'area_y1': […]*

```diff
@@ -1,18 +1,18 @@
 {
     "0": {
         "attributes": [
             "condition_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 0,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -29,26 +29,26 @@
         },
         "name": "none"
     },
     "1": {
         "attributes": [
             "condition_type",
             "unit_object",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 1,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -69,18 +69,18 @@
         "attributes": [
             "condition_type",
             "timer",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 10,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -101,18 +101,18 @@
         "attributes": [
             "condition_type",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 11,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -133,18 +133,18 @@
         "attributes": [
             "condition_type",
             "ai_signal",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 12,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -165,18 +165,18 @@
         "attributes": [
             "condition_type",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 13,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -201,18 +201,18 @@
             "object_list",
             "object_group",
             "object_type",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 14,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -232,18 +232,18 @@
     "15": {
         "attributes": [
             "condition_type",
             "unit_object"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 15,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -263,18 +263,18 @@
     "16": {
         "attributes": [
             "condition_type",
             "unit_object"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 16,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -296,18 +296,18 @@
             "condition_type",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 17,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -329,18 +329,18 @@
             "condition_type",
             "quantity",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 18,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -361,18 +361,18 @@
         "attributes": [
             "condition_type",
             "quantity",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 19,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -394,18 +394,18 @@
             "condition_type",
             "unit_object",
             "next_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 2,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -425,18 +425,18 @@
     "20": {
         "attributes": [
             "condition_type",
             "quantity"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 20,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -459,18 +459,18 @@
             "quantity",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 21,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -493,18 +493,18 @@
             "quantity",
             "inverted",
             "variable",
             "comparison"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 22,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -527,18 +527,18 @@
             "quantity",
             "unit_object",
             "inverted",
             "comparison"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 23,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -561,18 +561,18 @@
             "quantity",
             "source_player",
             "inverted",
             "target_player"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 24,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -591,18 +591,18 @@
     },
     "25": {
         "attributes": [
             "xs_function"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 25,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -623,18 +623,18 @@
         "attributes": [
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 26,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -655,18 +655,18 @@
         "attributes": [
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 27,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -688,18 +688,18 @@
             "unit_object",
             "next_object",
             "inverted",
             "unit_ai_action"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 28,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -716,18 +716,18 @@
         },
         "name": "object_has_action"
     },
     "29": {
         "attributes": [],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 29,
             "inverted": -1,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -751,18 +751,18 @@
             "object_list",
             "source_player",
             "object_group",
             "object_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 3,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -782,18 +782,18 @@
     "30": {
         "attributes": [
             "ai_signal",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 30,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -812,27 +812,27 @@
     },
     "4": {
         "attributes": [
             "condition_type",
             "quantity",
             "object_list",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 4,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -851,28 +851,28 @@
     },
     "5": {
         "attributes": [
             "condition_type",
             "quantity",
             "object_list",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": 0,
             "condition_type": 5,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -893,18 +893,18 @@
         "attributes": [
             "condition_type",
             "unit_object",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 6,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -926,18 +926,18 @@
             "condition_type",
             "unit_object",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 7,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -960,18 +960,18 @@
             "quantity",
             "attribute",
             "source_player",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": 0,
             "comparison": -1,
             "condition_type": 8,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
@@ -993,18 +993,18 @@
             "condition_type",
             "source_player",
             "technology",
             "inverted"
         ],
         "default_attributes": {
             "ai_signal": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "attribute": -1,
             "comparison": -1,
             "condition_type": 9,
             "inverted": 0,
             "next_object": -1,
             "object_group": -1,
             "object_list": -1,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/effects.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/effects.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9673429054810855%*

 * *Differences: {"'0'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'1'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *        "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'10'": "{'default_attributes': {'area_x1': -1, 'area_y1': -1, 'area_x2': -1, 'area_y2': -1, "*

 * *         "delete: ['area_1_x', 'area_1_y', 'area_2_x', 'area_2_y']}}",*

 * * "'11'": "{'def […]*

```diff
@@ -2,18 +2,18 @@
     "0": {
         "attributes": [
             "effect_type"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 0,
@@ -62,18 +62,18 @@
             "diplomacy",
             "source_player",
             "target_player"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": 0,
             "display_time": -1,
             "effect_type": 1,
@@ -120,18 +120,18 @@
         "attributes": [
             "effect_type",
             "ai_script_goal"
         ],
         "default_attributes": {
             "ai_script_goal": 1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 10,
@@ -183,18 +183,18 @@
             "location_y",
             "item_id",
             "facet"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 11,
@@ -241,29 +241,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 12,
@@ -311,18 +311,18 @@
             "effect_type",
             "source_player",
             "enabled"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 13,
@@ -366,29 +366,29 @@
         "name": "declare_victory"
     },
     "14": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 14,
@@ -432,29 +432,29 @@
         "name": "kill_object"
     },
     "15": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 15,
@@ -499,24 +499,23 @@
     },
     "16": {
         "attributes": [
             "effect_type",
             "source_player",
             "location_x",
             "location_y",
-            "location_object_reference",
             "scroll"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 16,
@@ -563,29 +562,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 17,
@@ -630,30 +629,30 @@
     },
     "18": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "target_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "flash_object",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 18,
@@ -700,29 +699,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 19,
@@ -771,18 +770,18 @@
             "source_player",
             "technology",
             "force_research_technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 2,
@@ -836,18 +835,18 @@
             "play_sound",
             "message",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": 10,
             "effect_type": 20,
@@ -894,18 +893,18 @@
         "attributes": [
             "effect_type",
             "instruction_panel_position"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 21,
@@ -949,29 +948,29 @@
         "name": "clear_instructions"
     },
     "22": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 22,
@@ -1017,18 +1016,18 @@
     "23": {
         "attributes": [
             "effect_type"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 23,
@@ -1073,29 +1072,29 @@
     },
     "24": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 24,
@@ -1145,18 +1144,18 @@
             "source_player",
             "location_x",
             "location_y"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 25,
@@ -1201,28 +1200,28 @@
     },
     "26": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "message",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 26,
@@ -1267,30 +1266,30 @@
     },
     "27": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 27,
@@ -1336,30 +1335,30 @@
     "28": {
         "attributes": [
             "effect_type",
             "armour_attack_quantity",
             "armour_attack_class",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": 0,
             "armour_attack_quantity": 1,
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 28,
@@ -1403,29 +1402,29 @@
         "name": "change_object_attack"
     },
     "29": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 29,
@@ -1475,18 +1474,18 @@
             "string_id",
             "message",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 3,
@@ -1533,29 +1532,29 @@
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
             "location_object_reference",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 30,
@@ -1601,30 +1600,30 @@
     "31": {
         "attributes": [
             "effect_type",
             "armour_attack_quantity",
             "armour_attack_class",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": 0,
             "armour_attack_quantity": 1,
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 31,
@@ -1669,30 +1668,30 @@
     },
     "32": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "operation",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 32,
@@ -1737,29 +1736,29 @@
     },
     "33": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 33,
@@ -1804,29 +1803,29 @@
     },
     "34": {
         "attributes": [
             "effect_type",
             "quantity",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 34,
@@ -1872,29 +1871,29 @@
     "35": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 35,
@@ -1938,30 +1937,30 @@
         "name": "teleport_object"
     },
     "36": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "attack_stance",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": 0,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 36,
@@ -2012,18 +2011,18 @@
             "time_unit",
             "timer",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": 10,
             "effect_type": 37,
@@ -2073,18 +2072,18 @@
             "source_player",
             "enabled",
             "item_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 38,
@@ -2134,18 +2133,18 @@
             "technology",
             "enabled",
             "item_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 39,
@@ -2196,18 +2195,18 @@
             "location_y",
             "location_object_reference",
             "sound_name"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 4,
@@ -2259,18 +2258,18 @@
             "wood",
             "stone",
             "gold"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 40,
@@ -2319,18 +2318,18 @@
             "source_player",
             "target_player",
             "visibility_state"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 41,
@@ -2374,30 +2373,30 @@
         "name": "set_player_visibility"
     },
     "42": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 42,
@@ -2442,30 +2441,30 @@
     },
     "43": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
             "target_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_group",
             "object_type",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 43,
@@ -2515,18 +2514,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 44,
@@ -2575,18 +2574,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 45,
@@ -2636,18 +2635,18 @@
             "source_player",
             "object_list_unit_id_2",
             "button_location"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": 0,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 46,
@@ -2697,18 +2696,18 @@
             "technology",
             "object_list_unit_id_2",
             "button_location"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": 7,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 47,
@@ -2757,18 +2756,18 @@
             "source_player",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 48,
@@ -2812,28 +2811,28 @@
         "name": "change_civilization_name"
     },
     "49": {
         "attributes": [
             "effect_type",
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "object_list_unit_id_2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 49,
@@ -2883,18 +2882,18 @@
             "tribute_list",
             "source_player",
             "target_player"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 5,
@@ -2941,18 +2940,18 @@
         "attributes": [
             "effect_type",
             "ai_signal_value"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 50,
@@ -3004,18 +3003,18 @@
             "item_id",
             "operation",
             "object_attributes"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 51,
@@ -3066,18 +3065,18 @@
             "source_player",
             "item_id",
             "operation"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 52,
@@ -3128,18 +3127,18 @@
             "item_id",
             "operation",
             "variable"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 53,
@@ -3184,27 +3183,27 @@
     },
     "54": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
             "location_x",
             "location_y",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 54,
@@ -3251,18 +3250,18 @@
         "attributes": [
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 55,
@@ -3312,18 +3311,18 @@
             "operation",
             "variable",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 56,
@@ -3370,18 +3369,18 @@
         "attributes": [
             "effect_type",
             "timer"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 57,
@@ -3424,27 +3423,27 @@
         },
         "name": "clear_timer"
     },
     "58": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 58,
@@ -3486,27 +3485,27 @@
             "wood": -1
         },
         "name": "change_object_player_color"
     },
     "59": {
         "attributes": [
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 59,
@@ -3553,18 +3552,18 @@
         "attributes": [
             "effect_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 6,
@@ -3608,27 +3607,27 @@
         "name": "unlock_gate"
     },
     "60": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
             "string_id",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 60,
@@ -3671,27 +3670,27 @@
         },
         "name": "change_object_player_name"
     },
     "61": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 61,
@@ -3734,27 +3733,27 @@
         },
         "name": "disable_unit_targeting"
     },
     "62": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 62,
@@ -3805,18 +3804,18 @@
             "wood",
             "stone",
             "gold"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 63,
@@ -3864,18 +3863,18 @@
             "quantity",
             "source_player",
             "technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 64,
@@ -3924,18 +3923,18 @@
             "technology",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 65,
@@ -3984,18 +3983,18 @@
             "technology",
             "string_id",
             "message"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 66,
@@ -4042,18 +4041,18 @@
         "attributes": [
             "source_player",
             "technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 67,
@@ -4100,18 +4099,18 @@
         "attributes": [
             "source_player",
             "technology"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 68,
@@ -4157,18 +4156,18 @@
     "69": {
         "attributes": [
             "ai_signal_value"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": 0,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 69,
@@ -4215,18 +4214,18 @@
         "attributes": [
             "effect_type",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 7,
@@ -4269,27 +4268,27 @@
         },
         "name": "lock_gate"
     },
     "70": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 70,
@@ -4332,27 +4331,27 @@
         },
         "name": "disable_object_selection"
     },
     "71": {
         "attributes": [
             "object_list_unit_id",
             "source_player",
-            "area_1_x",
-            "area_1_y",
-            "area_2_x",
-            "area_2_y",
+            "area_x1",
+            "area_y1",
+            "area_x2",
+            "area_y2",
             "selected_object_ids"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 71,
@@ -4399,18 +4398,18 @@
         "attributes": [
             "effect_type",
             "trigger_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 8,
@@ -4457,18 +4456,18 @@
         "attributes": [
             "effect_type",
             "trigger_id"
         ],
         "default_attributes": {
             "ai_script_goal": -1,
             "ai_signal_value": -1,
-            "area_1_x": -1,
-            "area_1_y": -1,
-            "area_2_x": -1,
-            "area_2_y": -1,
+            "area_x1": -1,
+            "area_x2": -1,
+            "area_y1": -1,
+            "area_y2": -1,
             "armour_attack_class": [],
             "armour_attack_quantity": [],
             "attack_stance": -1,
             "button_location": -1,
             "diplomacy": -1,
             "display_time": -1,
             "effect_type": 9,
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser/versions/DE/v1.41/structure.json` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser/versions/DE/v1.41/structure.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997696314102564%*

 * *Differences: {"'FileHeader'": "{'retrievers': {'version': {'default': '1.41'}}}",*

 * * "'Triggers'": "{'structs': {'TriggerStruct': {'structs': {'EffectStruct': {'retrievers': "*

 * *               "{'area_x1': OrderedDict([('type', 's32'), ('default', -1)]), 'area_y1': "*

 * *               "OrderedDict([('type', 's32'), ('default', -1)]), 'area_x2': OrderedDict([('type', "*

 * *               "'s32'), ('default', -1)]), 'area_y2': OrderedDict([('type', 's32'), ('default', "*

 * *               "-1)]), delete: ['area_1_x', 'area_1_y', 'area_2 […]*

```diff
@@ -603,15 +603,15 @@
             },
             "unknown_value_2": {
                 "comment": "Always (?) 1",
                 "default": 1,
                 "type": "u32"
             },
             "version": {
-                "default": "1.40",
+                "default": "1.41",
                 "type": "c4"
             }
         }
     },
     "Files": {
         "retrievers": {
             "__END_OF_FILE_MARK__": {
@@ -1736,27 +1736,27 @@
                 "structs": {
                     "ConditionStruct": {
                         "retrievers": {
                             "ai_signal": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_x": {
+                            "area_x1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_y": {
+                            "area_x2": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_x": {
+                            "area_y1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_y": {
+                            "area_y2": {
                                 "default": -1,
                                 "type": "s32"
                             },
                             "attribute": {
                                 "default": -1,
                                 "type": "s32"
                             },
@@ -1848,27 +1848,27 @@
                                 "default": -1,
                                 "type": "s32"
                             },
                             "ai_signal_value": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_x": {
+                            "area_x1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_1_y": {
+                            "area_x2": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_x": {
+                            "area_y1": {
                                 "default": -1,
                                 "type": "s32"
                             },
-                            "area_2_y": {
+                            "area_y2": {
                                 "default": -1,
                                 "type": "s32"
                             },
                             "armour_attack_class": {
                                 "default": 0,
                                 "dependencies": {
                                     "on_construct": {
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/PKG-INFO` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 Metadata-Version: 2.1
 Name: AoE2ScenarioParser
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a project for editing parts of an 'aoe2scenario' file from Age of Empires 2 Definitive Edition
 Home-page: https://github.com/KSneijders/AoE2ScenarioParser
 Author: Kerwin Sneijders
 Author-email: ksneijders@hotmail.com
 License: UNKNOWN
 Description: # AoE2ScenarioParser
         
-        This is a project for editing parts of an `aoe2scenario` file from **Age of Empires 2
-        Definitive Edition** outside of the in-game editor.
+        This is a project for editing parts of an `aoe2scenario` file from **Age of Empires 2 Definitive Edition** outside of
+        the in-game editor.
         
-        Documentation can be found on the [readthedocs] page.  
-        Examples can be found in the cheatsheets.
+        Documentation can be found on the [readthedocs] page.
         
-        - [Triggers Cheatsheet] (More up-to-date information can be found on: [readthedocs])
-        - [Units Cheatsheet] (More up-to-date information can be found on: [readthedocs])
-        - [Datasets Cheatsheet] (More up-to-date information can be found on: [readthedocs])
+        **For now**, some of the documentation can also be found here on github:
+        
+        - [Triggers Cheatsheet]
+        - [Units Cheatsheet]
+        - [Datasets Cheatsheet]
         
         [readthedocs]: https://aoe2scenarioparser.readthedocs.io/en/master/
+        
         [triggers cheatsheet]: ./cheatsheets/TRIGGERS.md
+        
         [units cheatsheet]: ./cheatsheets/UNITS.md
+        
         [datasets cheatsheet]: ./cheatsheets/DATASETS.md
         
         # Progress
         
-        Current up-to-date progress can be found on the [changelog.md] page. (Dev branch for non-released progress).
+        Current up-to-date progress can be found on the [changelog.md] page. (Check the `dev` branch for non-released progress).
         
         [changelog.md]: ./changelog.md
         
         ## Features:
         
         |            | View               | Add                | Edit               | Remove             |
         | ---------- | ------------------ | ------------------ | ------------------ | ------------------ |
         | Triggers   | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Conditions | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Effects    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Units      | n/a                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Map*       | n/a                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         
-        The map can be edited in size. Every tile can be changed in terrain, layer and elevation.
-        
-        ## Bugs:
-        
-        - None that I know of
-        
-        If you find a bug, please check if it's already been reported or maybe even fixed ([changelog.md]). Please report any bugs you find to the [github issue board].
-        
-        [github issue board]: https://github.com/KSneijders/AoE2ScenarioParser/issues
+        &nbsp;
         
         ## Support:
         
-        | ScenarioFiles | Read               | Write              | Reference                                                                                                                                                                                                                                                                                                                                                                                             |
-        | ------------- | ------------------ | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | 1.36          | :x:                | :x:                | ?                                                                                                                                                                                                                                                                                                                                                                                                     |
-        | 1.37          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [35584] (February 27th) <br> **Unchanged in**: <br> - Update [36202] (March 30th) <br> - Update [36906] (April 29th) <br> - Update [37650] (May 27th) <br> - Hotfix [37906] (June 2nd) <br> - Update [39284] (July 20th) <br> - Hotfix [39515] (July 27th) <br> - Update [40220] (August 24th) <br> - Update [40874] (September 22nd) <br> - Update [41855] (October 20th) |
-        | 1.40          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [42848] (November 17th) <br> **Unchanged in**: <br> - Hotfix [43210] (November 24th)                                                                                                                                                                                                                                                                                       |
-        | 1.41          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [44725] (January 25th) <br> **Unchanged in**: <br> - Hotfix [44834] (January 28th)<br> - Hotfix [45185] (February 11th)<br> - Update [46265] (March 24th)                                                                                                                                                                                                                                                                                         |
+        | Scenario file version | Read               | Write              | Reference                                                                                                                                                                                                                                                                                                                                                                                             |
+        | ------------- | ------------------ | ------------------ | -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------                                                                                                                                                   |
+        | 1.37          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [35584] (February 27th, 2020) <br> **Unchanged in**: <br> - Update [36202] (March 30th, 2020) <br> - Update [36906] (April 29th, 2020) <br> - Update [37650] (May 27th, 2020) <br> - Hotfix [37906] (June 2nd, 2020) <br> - Update [39284] (July 20th, 2020) <br> - Hotfix [39515] (July 27th, 2020) <br> - Update [40220] (August 24th, 2020) <br> - Update [40874] (September 22nd, 2020) <br> - Update [41855] (October 20th, 2020) |
+        | 1.40          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [42848] (November 17th, 2020) <br> **Unchanged in**: <br> - Hotfix [43210] (November 24th, 2020)                                                                                                                                                                                                                                                                                       |
+        | 1.41          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [44725] (January 25th, 2021) <br> **Unchanged in**: <br> - Hotfix [44834] (January 28th, 2021)<br> - Hotfix [45185] (February 11th, 2021)<br> - Update [46265] (March 24th, 2021)<br> - Update [47820] (May 3rd, 2021)                                                                                                                                                                                                                                                                                             |
         
         [35584]: https://www.ageofempires.com/news/aoe2de-update-35584/
         [36202]: https://www.ageofempires.com/news/aoe2de-update-36202/
         [36906]: https://www.ageofempires.com/news/aoe2de-update-36906/
         [37650]: https://www.ageofempires.com/news/aoe2de-update-37650/
         [37906]: https://www.ageofempires.com/news/aoe2de-hotfix-37906/
         [39284]: https://www.ageofempires.com/news/aoe2de-update-39284/
@@ -70,14 +65,15 @@
         [41855]: https://www.ageofempires.com/news/aoe2de-update-41855/
         [42848]: https://www.ageofempires.com/news/aoe2de-update-42848/
         [43210]: https://www.ageofempires.com/news/aoe2de-hotfix-43210/
         [44725]: https://www.ageofempires.com/news/aoeiide-update-44725/
         [44834]: https://www.ageofempires.com/news/aoeiide-update-44725#hotfix-44834
         [45185]: https://www.ageofempires.com/news/aoe2de-hotfix-45185/
         [46265]: https://www.ageofempires.com/news/aoe2de-update-46295/
+        [47820]: https://www.ageofempires.com/news/aoe2de-update-47820/
         
         # Authors
         
         - Kerwin Sneijders (Main Author)
         
         # License
```

### Comparing `AoE2ScenarioParser-0.1.8/AoE2ScenarioParser.egg-info/SOURCES.txt` & `AoE2ScenarioParser-0.1.9/AoE2ScenarioParser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 AoE2ScenarioParser.egg-info/top_level.txt
 AoE2ScenarioParser/datasets/buildings.py
 AoE2ScenarioParser/datasets/conditions.py
 AoE2ScenarioParser/datasets/effects.py
 AoE2ScenarioParser/datasets/heroes.py
 AoE2ScenarioParser/datasets/other.py
 AoE2ScenarioParser/datasets/players.py
+AoE2ScenarioParser/datasets/projectiles.py
 AoE2ScenarioParser/datasets/techs.py
 AoE2ScenarioParser/datasets/terrains.py
 AoE2ScenarioParser/datasets/trigger_lists.py
 AoE2ScenarioParser/datasets/units.py
 AoE2ScenarioParser/datasets/scripts/get_icon_ids.py
 AoE2ScenarioParser/datasets/scripts/object_parser.py
+AoE2ScenarioParser/datasets/support/info_dataset_base.py
 AoE2ScenarioParser/helper/bytes_conversions.py
 AoE2ScenarioParser/helper/bytes_parser.py
 AoE2ScenarioParser/helper/exceptions.py
 AoE2ScenarioParser/helper/helper.py
 AoE2ScenarioParser/helper/incremental_generator.py
 AoE2ScenarioParser/helper/list_functions.py
 AoE2ScenarioParser/helper/pretty_format.py
```

### Comparing `AoE2ScenarioParser-0.1.8/PKG-INFO` & `AoE2ScenarioParser-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 Metadata-Version: 2.1
 Name: AoE2ScenarioParser
-Version: 0.1.8
+Version: 0.1.9
 Summary: This is a project for editing parts of an 'aoe2scenario' file from Age of Empires 2 Definitive Edition
 Home-page: https://github.com/KSneijders/AoE2ScenarioParser
 Author: Kerwin Sneijders
 Author-email: ksneijders@hotmail.com
 License: UNKNOWN
 Description: # AoE2ScenarioParser
         
-        This is a project for editing parts of an `aoe2scenario` file from **Age of Empires 2
-        Definitive Edition** outside of the in-game editor.
+        This is a project for editing parts of an `aoe2scenario` file from **Age of Empires 2 Definitive Edition** outside of
+        the in-game editor.
         
-        Documentation can be found on the [readthedocs] page.  
-        Examples can be found in the cheatsheets.
+        Documentation can be found on the [readthedocs] page.
         
-        - [Triggers Cheatsheet] (More up-to-date information can be found on: [readthedocs])
-        - [Units Cheatsheet] (More up-to-date information can be found on: [readthedocs])
-        - [Datasets Cheatsheet] (More up-to-date information can be found on: [readthedocs])
+        **For now**, some of the documentation can also be found here on github:
+        
+        - [Triggers Cheatsheet]
+        - [Units Cheatsheet]
+        - [Datasets Cheatsheet]
         
         [readthedocs]: https://aoe2scenarioparser.readthedocs.io/en/master/
+        
         [triggers cheatsheet]: ./cheatsheets/TRIGGERS.md
+        
         [units cheatsheet]: ./cheatsheets/UNITS.md
+        
         [datasets cheatsheet]: ./cheatsheets/DATASETS.md
         
         # Progress
         
-        Current up-to-date progress can be found on the [changelog.md] page. (Dev branch for non-released progress).
+        Current up-to-date progress can be found on the [changelog.md] page. (Check the `dev` branch for non-released progress).
         
         [changelog.md]: ./changelog.md
         
         ## Features:
         
         |            | View               | Add                | Edit               | Remove             |
         | ---------- | ------------------ | ------------------ | ------------------ | ------------------ |
         | Triggers   | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Conditions | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Effects    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Units      | n/a                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         | Map*       | n/a                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
         
-        The map can be edited in size. Every tile can be changed in terrain, layer and elevation.
-        
-        ## Bugs:
-        
-        - None that I know of
-        
-        If you find a bug, please check if it's already been reported or maybe even fixed ([changelog.md]). Please report any bugs you find to the [github issue board].
-        
-        [github issue board]: https://github.com/KSneijders/AoE2ScenarioParser/issues
+        &nbsp;
         
         ## Support:
         
-        | ScenarioFiles | Read               | Write              | Reference                                                                                                                                                                                                                                                                                                                                                                                             |
-        | ------------- | ------------------ | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | 1.36          | :x:                | :x:                | ?                                                                                                                                                                                                                                                                                                                                                                                                     |
-        | 1.37          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [35584] (February 27th) <br> **Unchanged in**: <br> - Update [36202] (March 30th) <br> - Update [36906] (April 29th) <br> - Update [37650] (May 27th) <br> - Hotfix [37906] (June 2nd) <br> - Update [39284] (July 20th) <br> - Hotfix [39515] (July 27th) <br> - Update [40220] (August 24th) <br> - Update [40874] (September 22nd) <br> - Update [41855] (October 20th) |
-        | 1.40          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [42848] (November 17th) <br> **Unchanged in**: <br> - Hotfix [43210] (November 24th)                                                                                                                                                                                                                                                                                       |
-        | 1.41          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [44725] (January 25th) <br> **Unchanged in**: <br> - Hotfix [44834] (January 28th)<br> - Hotfix [45185] (February 11th)<br> - Update [46265] (March 24th)                                                                                                                                                                                                                                                                                         |
+        | Scenario file version | Read               | Write              | Reference                                                                                                                                                                                                                                                                                                                                                                                             |
+        | ------------- | ------------------ | ------------------ | -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------                                                                                                                                                   |
+        | 1.37          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [35584] (February 27th, 2020) <br> **Unchanged in**: <br> - Update [36202] (March 30th, 2020) <br> - Update [36906] (April 29th, 2020) <br> - Update [37650] (May 27th, 2020) <br> - Hotfix [37906] (June 2nd, 2020) <br> - Update [39284] (July 20th, 2020) <br> - Hotfix [39515] (July 27th, 2020) <br> - Update [40220] (August 24th, 2020) <br> - Update [40874] (September 22nd, 2020) <br> - Update [41855] (October 20th, 2020) |
+        | 1.40          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [42848] (November 17th, 2020) <br> **Unchanged in**: <br> - Hotfix [43210] (November 24th, 2020)                                                                                                                                                                                                                                                                                       |
+        | 1.41          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [44725] (January 25th, 2021) <br> **Unchanged in**: <br> - Hotfix [44834] (January 28th, 2021)<br> - Hotfix [45185] (February 11th, 2021)<br> - Update [46265] (March 24th, 2021)<br> - Update [47820] (May 3rd, 2021)                                                                                                                                                                                                                                                                                             |
         
         [35584]: https://www.ageofempires.com/news/aoe2de-update-35584/
         [36202]: https://www.ageofempires.com/news/aoe2de-update-36202/
         [36906]: https://www.ageofempires.com/news/aoe2de-update-36906/
         [37650]: https://www.ageofempires.com/news/aoe2de-update-37650/
         [37906]: https://www.ageofempires.com/news/aoe2de-hotfix-37906/
         [39284]: https://www.ageofempires.com/news/aoe2de-update-39284/
@@ -70,14 +65,15 @@
         [41855]: https://www.ageofempires.com/news/aoe2de-update-41855/
         [42848]: https://www.ageofempires.com/news/aoe2de-update-42848/
         [43210]: https://www.ageofempires.com/news/aoe2de-hotfix-43210/
         [44725]: https://www.ageofempires.com/news/aoeiide-update-44725/
         [44834]: https://www.ageofempires.com/news/aoeiide-update-44725#hotfix-44834
         [45185]: https://www.ageofempires.com/news/aoe2de-hotfix-45185/
         [46265]: https://www.ageofempires.com/news/aoe2de-update-46295/
+        [47820]: https://www.ageofempires.com/news/aoe2de-update-47820/
         
         # Authors
         
         - Kerwin Sneijders (Main Author)
         
         # License
```

### Comparing `AoE2ScenarioParser-0.1.8/README.md` & `AoE2ScenarioParser-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 # AoE2ScenarioParser
 
-This is a project for editing parts of an `aoe2scenario` file from **Age of Empires 2
-Definitive Edition** outside of the in-game editor.
+This is a project for editing parts of an `aoe2scenario` file from **Age of Empires 2 Definitive Edition** outside of
+the in-game editor.
 
-Documentation can be found on the [readthedocs] page.  
-Examples can be found in the cheatsheets.
+Documentation can be found on the [readthedocs] page.
 
-- [Triggers Cheatsheet] (More up-to-date information can be found on: [readthedocs])
-- [Units Cheatsheet] (More up-to-date information can be found on: [readthedocs])
-- [Datasets Cheatsheet] (More up-to-date information can be found on: [readthedocs])
+**For now**, some of the documentation can also be found here on github:
+
+- [Triggers Cheatsheet]
+- [Units Cheatsheet]
+- [Datasets Cheatsheet]
 
 [readthedocs]: https://aoe2scenarioparser.readthedocs.io/en/master/
+
 [triggers cheatsheet]: ./cheatsheets/TRIGGERS.md
+
 [units cheatsheet]: ./cheatsheets/UNITS.md
+
 [datasets cheatsheet]: ./cheatsheets/DATASETS.md
 
 # Progress
 
-Current up-to-date progress can be found on the [changelog.md] page. (Dev branch for non-released progress).
+Current up-to-date progress can be found on the [changelog.md] page. (Check the `dev` branch for non-released progress).
 
 [changelog.md]: ./changelog.md
 
 ## Features:
 
 |            | View               | Add                | Edit               | Remove             |
 | ---------- | ------------------ | ------------------ | ------------------ | ------------------ |
 | Triggers   | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Conditions | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Effects    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Units      | n/a                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 | Map*       | n/a                | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
 
-The map can be edited in size. Every tile can be changed in terrain, layer and elevation.
-
-## Bugs:
-
-- None that I know of
-
-If you find a bug, please check if it's already been reported or maybe even fixed ([changelog.md]). Please report any bugs you find to the [github issue board].
-
-[github issue board]: https://github.com/KSneijders/AoE2ScenarioParser/issues
+&nbsp;
 
 ## Support:
 
-| ScenarioFiles | Read               | Write              | Reference                                                                                                                                                                                                                                                                                                                                                                                             |
-| ------------- | ------------------ | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| 1.36          | :x:                | :x:                | ?                                                                                                                                                                                                                                                                                                                                                                                                     |
-| 1.37          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [35584] (February 27th) <br> **Unchanged in**: <br> - Update [36202] (March 30th) <br> - Update [36906] (April 29th) <br> - Update [37650] (May 27th) <br> - Hotfix [37906] (June 2nd) <br> - Update [39284] (July 20th) <br> - Hotfix [39515] (July 27th) <br> - Update [40220] (August 24th) <br> - Update [40874] (September 22nd) <br> - Update [41855] (October 20th) |
-| 1.40          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [42848] (November 17th) <br> **Unchanged in**: <br> - Hotfix [43210] (November 24th)                                                                                                                                                                                                                                                                                       |
-| 1.41          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [44725] (January 25th) <br> **Unchanged in**: <br> - Hotfix [44834] (January 28th)<br> - Hotfix [45185] (February 11th)<br> - Update [46265] (March 24th)                                                                                                                                                                                                                                                                                         |
+| Scenario file version | Read               | Write              | Reference                                                                                                                                                                                                                                                                                                                                                                                             |
+| ------------- | ------------------ | ------------------ | -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------                                                                                                                                                   |
+| 1.37          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [35584] (February 27th, 2020) <br> **Unchanged in**: <br> - Update [36202] (March 30th, 2020) <br> - Update [36906] (April 29th, 2020) <br> - Update [37650] (May 27th, 2020) <br> - Hotfix [37906] (June 2nd, 2020) <br> - Update [39284] (July 20th, 2020) <br> - Hotfix [39515] (July 27th, 2020) <br> - Update [40220] (August 24th, 2020) <br> - Update [40874] (September 22nd, 2020) <br> - Update [41855] (October 20th, 2020) |
+| 1.40          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [42848] (November 17th, 2020) <br> **Unchanged in**: <br> - Hotfix [43210] (November 24th, 2020)                                                                                                                                                                                                                                                                                       |
+| 1.41          | :heavy_check_mark: | :heavy_check_mark: | Version since game update: [44725] (January 25th, 2021) <br> **Unchanged in**: <br> - Hotfix [44834] (January 28th, 2021)<br> - Hotfix [45185] (February 11th, 2021)<br> - Update [46265] (March 24th, 2021)<br> - Update [47820] (May 3rd, 2021)                                                                                                                                                                                                                                                                                             |
 
 [35584]: https://www.ageofempires.com/news/aoe2de-update-35584/
 [36202]: https://www.ageofempires.com/news/aoe2de-update-36202/
 [36906]: https://www.ageofempires.com/news/aoe2de-update-36906/
 [37650]: https://www.ageofempires.com/news/aoe2de-update-37650/
 [37906]: https://www.ageofempires.com/news/aoe2de-hotfix-37906/
 [39284]: https://www.ageofempires.com/news/aoe2de-update-39284/
@@ -62,14 +57,15 @@
 [41855]: https://www.ageofempires.com/news/aoe2de-update-41855/
 [42848]: https://www.ageofempires.com/news/aoe2de-update-42848/
 [43210]: https://www.ageofempires.com/news/aoe2de-hotfix-43210/
 [44725]: https://www.ageofempires.com/news/aoeiide-update-44725/
 [44834]: https://www.ageofempires.com/news/aoeiide-update-44725#hotfix-44834
 [45185]: https://www.ageofempires.com/news/aoe2de-hotfix-45185/
 [46265]: https://www.ageofempires.com/news/aoe2de-update-46295/
+[47820]: https://www.ageofempires.com/news/aoe2de-update-47820/
 
 # Authors
 
 - Kerwin Sneijders (Main Author)
 
 # License
```

### Comparing `AoE2ScenarioParser-0.1.8/setup.py` & `AoE2ScenarioParser-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AoE2ScenarioParser",
-    version="0.1.8",
+    version="0.1.9",
     author="Kerwin Sneijders",
     author_email="ksneijders@hotmail.com",
     description="This is a project for editing parts of an 'aoe2scenario' file from Age of Empires 2 Definitive Edition",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KSneijders/AoE2ScenarioParser",
```

