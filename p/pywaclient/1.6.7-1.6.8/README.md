# Comparing `tmp/pywaclient-1.6.7.tar.gz` & `tmp/pywaclient-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pywaclient-1.6.7.tar", last modified: Wed May  1 13:58:39 2024, max compression
+gzip compressed data, was "dist/pywaclient-1.6.8.tar", last modified: Sat May 25 16:10:54 2024, max compression
```

## Comparing `pywaclient-1.6.7.tar` & `pywaclient-1.6.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-01 13:58:29.000000 pywaclient-1.6.7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-01 13:58:29.000000 pywaclient-1.6.7/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-01 13:58:29.000000 pywaclient-1.6.7/LICENCE
--rw-r--r--   0 root         (0) root         (0)     7468 2024-05-01 13:58:39.000000 pywaclient-1.6.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7076 2024-05-01 13:58:29.000000 pywaclient-1.6.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient/
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient/endpoints/
--rw-rw-rw-   0 root         (0) root         (0)     7038 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/articles.py
--rw-rw-rw-   0 root         (0) root         (0)     2242 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/block_templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/categories.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/chronicles.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/eras.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/histories.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/images.py
--rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/manuscripts.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/map_marker_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2900 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/maps.py
--rw-rw-rw-   0 root         (0) root         (0)     3076 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/notebooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/rpg_system.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/secrets.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/subscriber_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/timelines.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/users.py
--rw-rw-rw-   0 root         (0) root         (0)     2268 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/variables.py
--rw-rw-rw-   0 root         (0) root         (0)    15951 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/endpoints/worlds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)     3488 2024-05-01 13:58:29.000000 pywaclient-1.6.7/pywaclient/exceptions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7468 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1855 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-01 13:58:39.000000 pywaclient-1.6.7/pywaclient.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-01 13:58:29.000000 pywaclient-1.6.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 13:58:39.000000 pywaclient-1.6.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-01 13:58:29.000000 pywaclient-1.6.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 13:58:39.000000 pywaclient-1.6.7/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/data/block.json
--rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/data/form_schema.json
--rw-rw-rw-   0 root         (0) root         (0)     1015 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/init_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_article_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_block_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_block_template_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_block_template_part_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_canvas_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_category_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_character_relationships.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_chronicle_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2092 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_history_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_image_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_manuscript_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_map_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_notebook_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_organization_diplomacy.py
--rw-rw-rw-   0 root         (0) root         (0)     2986 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_parse_response.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_rpg_system_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_secret_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_subscriber_group_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3542 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_timeline_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_user_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_variable_collection_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_variable_endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     5133 2024-05-01 13:58:29.000000 pywaclient-1.6.7/tests/test_world_endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-05-25 16:10:43.000000 pywaclient-1.6.8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-05-25 16:10:43.000000 pywaclient-1.6.8/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-25 16:10:43.000000 pywaclient-1.6.8/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     7468 2024-05-25 16:10:54.000000 pywaclient-1.6.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7076 2024-05-25 16:10:43.000000 pywaclient-1.6.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient/
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient/endpoints/
+-rw-rw-rw-   0 root         (0) root         (0)     7038 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/articles.py
+-rw-rw-rw-   0 root         (0) root         (0)     2242 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/block_templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/categories.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/chronicles.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/eras.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/histories.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/images.py
+-rw-rw-rw-   0 root         (0) root         (0)     6023 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/manuscripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/map_marker_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2900 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3076 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/notebooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/rpg_system.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/subscriber_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/timelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     2268 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/variables.py
+-rw-rw-rw-   0 root         (0) root         (0)    15501 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/endpoints/worlds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     3488 2024-05-25 16:10:43.000000 pywaclient-1.6.8/pywaclient/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7468 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1855 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-25 16:10:54.000000 pywaclient-1.6.8/pywaclient.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-25 16:10:43.000000 pywaclient-1.6.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 16:10:54.000000 pywaclient-1.6.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-25 16:10:43.000000 pywaclient-1.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 16:10:54.000000 pywaclient-1.6.8/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/data/block.json
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/data/form_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/init_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_article_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_block_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_block_template_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_block_template_part_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_canvas_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_category_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_character_relationships.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_chronicle_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_history_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_image_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_manuscript_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_map_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_notebook_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_organization_diplomacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_parse_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_rpg_system_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_secret_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_subscriber_group_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3542 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_timeline_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_user_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_variable_collection_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_variable_endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     5133 2024-05-25 16:10:43.000000 pywaclient-1.6.8/tests/test_world_endpoint.py
```

### Comparing `pywaclient-1.6.7/LICENCE` & `pywaclient-1.6.8/LICENCE`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/PKG-INFO` & `pywaclient-1.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.6.7
+Version: 1.6.8
 Summary: A simple wrapper client library for the World Anvil API.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.6.7/README.md` & `pywaclient-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/__init__.py` & `pywaclient-1.6.8/pywaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/api.py` & `pywaclient-1.6.8/pywaclient/api.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/__init__.py` & `pywaclient-1.6.8/pywaclient/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/articles.py` & `pywaclient-1.6.8/pywaclient/endpoints/articles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/block_templates.py` & `pywaclient-1.6.8/pywaclient/endpoints/block_templates.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/blocks.py` & `pywaclient-1.6.8/pywaclient/endpoints/blocks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/canvas.py` & `pywaclient-1.6.8/pywaclient/endpoints/canvas.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/categories.py` & `pywaclient-1.6.8/pywaclient/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/chronicles.py` & `pywaclient-1.6.8/pywaclient/endpoints/chronicles.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/eras.py` & `pywaclient-1.6.8/pywaclient/endpoints/eras.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/histories.py` & `pywaclient-1.6.8/pywaclient/endpoints/histories.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/images.py` & `pywaclient-1.6.8/pywaclient/endpoints/images.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/manuscripts.py` & `pywaclient-1.6.8/pywaclient/endpoints/manuscripts.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/map_marker_types.py` & `pywaclient-1.6.8/pywaclient/endpoints/map_marker_types.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/maps.py` & `pywaclient-1.6.8/pywaclient/endpoints/maps.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/notebooks.py` & `pywaclient-1.6.8/pywaclient/endpoints/notebooks.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/rpg_system.py` & `pywaclient-1.6.8/pywaclient/endpoints/rpg_system.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/secrets.py` & `pywaclient-1.6.8/pywaclient/endpoints/secrets.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/subscriber_groups.py` & `pywaclient-1.6.8/pywaclient/endpoints/subscriber_groups.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/timelines.py` & `pywaclient-1.6.8/pywaclient/endpoints/timelines.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/users.py` & `pywaclient-1.6.8/pywaclient/endpoints/users.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 class UserCrudEndpoint(BasicEndpoint):
 
     def __init__(self, client: 'BoromirApiClient'):
         super().__init__(client, 'user')
         self.identity_path = 'identity'
         self.path_blocktemplates = f'{self.path}/blocktemplates'
         self.path_worlds = f'{self.path}/worlds'
+        self.path_notebooks = f'{self.path}/notebooks'
 
     def identity(self):
         """Get the user that is associated with the authentication token provided."""
         return self._get_request(self.identity_path, {})
 
     def patch(self, identifier: str, content: Dict[str, Any]) -> Dict[str, str]:
         """Update (patch) the content of a user.
@@ -48,7 +49,15 @@
     def worlds(self, identifier: str) -> Iterable[Dict[str, Any]]:
         """Returns a list of all worlds owned by this user.
 
         :param identifier:  The identifier of the user that the worlds should be returned from.
         :return:            An iterable of the world entities.
         """
         return self._scroll_collection(self.path_worlds, {'id': identifier}, 'entities')
+
+    def notebooks(self, identifier: str) -> Iterable[Dict[str, Any]]:
+        """Returns a list of all worlds owned by this user.
+
+        :param identifier:  The identifier of the user that the worlds should be returned from.
+        :return:            An iterable of the world entities.
+        """
+        return self._scroll_collection(self.path_notebooks, {'id': identifier}, 'entities')
```

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/variables.py` & `pywaclient-1.6.8/pywaclient/endpoints/variables.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient/endpoints/worlds.py` & `pywaclient-1.6.8/pywaclient/endpoints/worlds.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         self.path_maps = f'{self.path}/maps'
         self.path_images = f'{self.path}/images'
         self.path_histories = f'{self.path}/histories'
         self.path_timelines = f'{self.path}/timelines'
         self.path_chronicles = f'{self.path}/chronicles'
         self.path_canvases = f'{self.path}/canvases'
         self.path_blocks = f'{self.path}/blocks'
-        self.path_notebooks = f'{self.path}/notebooks'
 
     def articles(self, world_id: str, category_id: str = None, complete: bool = True, limit: int = 50, offset: int = 0) -> Iterable[Dict[str, Any]]:
         """
         List all articles by a world, filtered with a limit of entities shown at an offset and optionally by a category.
 
         :param world_id:    The id of the world the articles should be returned from.
         :param category_id: (optional) The id of the category to return the articles from. To get articles without a category set
@@ -294,16 +293,8 @@
         """
         assert 1 <= limit <= 50
         assert offset >= 0
         if complete:
             return self._scroll_collection(self.path_canvases, {'id': world_id}, 'entities')
         return self._post_request(self.path_canvases,
                                   {'id': world_id},
-                                  {'limit': limit, 'offset': offset})['entities']
-
-    def notebooks(self, identifier: str) -> Iterable[Dict[str, Any]]:
-        """Returns a list of all worlds owned by this user.
-
-        :param identifier:  The identifier of the user that the worlds should be returned from.
-        :return:            An iterable of the world entities.
-        """
-        return self._scroll_collection(self.path_notebooks, {'id': identifier}, 'entities')
+                                  {'limit': limit, 'offset': offset})['entities']
```

### Comparing `pywaclient-1.6.7/pywaclient/exceptions/__init__.py` & `pywaclient-1.6.8/pywaclient/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/pywaclient.egg-info/PKG-INFO` & `pywaclient-1.6.8/pywaclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaclient
-Version: 1.6.7
+Version: 1.6.8
 Summary: A simple wrapper client library for the World Anvil API.
 Home-page: https://gitlab.com/SoulLink/world-anvil-api-client
 Author: Jonas Waeber
 Author-email: jonaswaeber@gmail.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pywaclient-1.6.7/pywaclient.egg-info/SOURCES.txt` & `pywaclient-1.6.8/pywaclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/setup.py` & `pywaclient-1.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/data/block.json` & `pywaclient-1.6.8/tests/data/block.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/data/form_schema.json` & `pywaclient-1.6.8/tests/data/form_schema.json`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/init_client.py` & `pywaclient-1.6.8/tests/init_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 import os
 from pywaclient.api import BoromirApiClient
 
 world_id = 'daae0a12-f3c3-4978-b571-b5313e3c1741'
 client = BoromirApiClient(
     name='TEST APPLICATION',
     url='https://gitlab.com/SoulLink/world-anvil-api-client',
-    application_key=os.environ.get('WA_APPLICATION_KEY'),
-    authentication_token=os.environ.get('WA_AUTH_TOKEN'),
+    application_key=os.environ.get('APPLICATION_KEY'),
+    authentication_token=os.environ.get('AUTHENTICATION_TOKEN'),
     version='0.1.0'
 )
 user_id = client.user.identity()['id']
```

### Comparing `pywaclient-1.6.7/tests/test_article_endpoint.py` & `pywaclient-1.6.8/tests/test_article_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_block_endpoint.py` & `pywaclient-1.6.8/tests/test_block_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_block_template_endpoint.py` & `pywaclient-1.6.8/tests/test_block_template_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_block_template_part_endpoint.py` & `pywaclient-1.6.8/tests/test_block_template_part_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_canvas_endpoint.py` & `pywaclient-1.6.8/tests/test_canvas_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_category_endpoint.py` & `pywaclient-1.6.8/tests/test_category_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_character_relationships.py` & `pywaclient-1.6.8/tests/test_character_relationships.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_chronicle_endpoint.py` & `pywaclient-1.6.8/tests/test_chronicle_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_history_endpoint.py` & `pywaclient-1.6.8/tests/test_history_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_image_endpoint.py` & `pywaclient-1.6.8/tests/test_image_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_manuscript_endpoint.py` & `pywaclient-1.6.8/tests/test_manuscript_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_map_endpoint.py` & `pywaclient-1.6.8/tests/test_map_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_notebook_endpoint.py` & `pywaclient-1.6.8/tests/test_notebook_endpoint.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,28 +12,17 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from init_client import client, world_id, user_id
 
 if __name__ == '__main__':
 
-    for notebook in client.world.notebooks(user_id):
-        notebook = client.notebook.get(notebook['id'], 1)
-        print(notebook)
-        if 'notesections' in notebook:
-            for note_section in notebook['notesections']:
-                note_section = client.notebook.note_section.get(note_section['id'], 1)
-                print(note_section)
-                if 'notes' in note_section:
-                    for note in note_section['notes']:
-                        note = client.notebook.note_section.note.get(note['id'], 1)
-                        print(note)
+    for n in client.user.notebooks(user_id):
+        print(n)
 
-
-    print("extracted")
     notebook = client.notebook.put(
         {
             'title': 'A New Notebook',
             'world': {
                 'id': world_id
             }
         }
```

### Comparing `pywaclient-1.6.7/tests/test_organization_diplomacy.py` & `pywaclient-1.6.8/tests/test_organization_diplomacy.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_parse_response.py` & `pywaclient-1.6.8/tests/test_parse_response.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_rpg_system_endpoint.py` & `pywaclient-1.6.8/tests/test_rpg_system_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_secret_endpoint.py` & `pywaclient-1.6.8/tests/test_secret_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_subscriber_group_endpoint.py` & `pywaclient-1.6.8/tests/test_subscriber_group_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_timeline_endpoint.py` & `pywaclient-1.6.8/tests/test_timeline_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_user_endpoint.py` & `pywaclient-1.6.8/tests/test_user_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_variable_collection_endpoint.py` & `pywaclient-1.6.8/tests/test_variable_collection_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_variable_endpoint.py` & `pywaclient-1.6.8/tests/test_variable_endpoint.py`

 * *Files identical despite different names*

### Comparing `pywaclient-1.6.7/tests/test_world_endpoint.py` & `pywaclient-1.6.8/tests/test_world_endpoint.py`

 * *Files identical despite different names*

