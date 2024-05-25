# Comparing `tmp/bttc-0.0.79.tar.gz` & `tmp/bttc-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.79.tar", last modified: Sun May 19 04:06:50 2024, max compression
+gzip compressed data, was "bttc-0.0.80.tar", last modified: Sat May 25 14:30:25 2024, max compression
```

## Comparing `bttc-0.0.79.tar` & `bttc-0.0.80.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.79/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2765 2024-05-19 04:06:50.516775 bttc-0.0.79/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2037 2024-05-19 04:05:38.000000 bttc-0.0.79/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-05-19 04:06:38.000000 bttc-0.0.79/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    10830 2024-05-19 04:05:38.000000 bttc-0.0.79/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.79/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.79/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.79/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    36248 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.508775 bttc-0.0.79/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9163 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7155 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.79/bttc/utils/device_factory.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/utils/dialer_simulator.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.79/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.79/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.79/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    17165 2024-05-19 04:05:38.000000 bttc-0.0.79/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2765 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-19 04:06:50.516775 bttc-0.0.79/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.79/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.463412 bttc-0.0.80/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.80/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2751 2024-05-25 14:30:25.463412 bttc-0.0.80/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2023 2024-05-25 14:30:11.000000 bttc-0.0.80/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-05-25 14:29:31.000000 bttc-0.0.80/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    10830 2024-05-19 04:05:38.000000 bttc-0.0.80/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.80/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-05-20 14:07:40.000000 bttc-0.0.80/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.80/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.80/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    40032 2024-05-25 14:27:31.000000 bttc-0.0.80/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.451412 bttc-0.0.80/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9163 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7155 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.80/bttc/utils/device_factory.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/utils/dialer_simulator.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.80/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-11 11:42:51.000000 bttc-0.0.80/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.80/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.459412 bttc-0.0.80/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.80/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    17165 2024-05-19 04:05:38.000000 bttc-0.0.80/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.80/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.80/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-25 14:30:25.455412 bttc-0.0.80/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2751 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-25 14:30:25.000000 bttc-0.0.80/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-25 14:30:25.463412 bttc-0.0.80/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.80/setup.py
```

### Comparing `bttc-0.0.79/LICENSE` & `bttc-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/PKG-INFO` & `bttc-0.0.80/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.79
+Version: 0.0.80
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -75,19 +75,19 @@
 
 
 ### `dut.mc`: Utility to support common Media control operations/methods.
 The `dut.mc` utility, loaded automatically when you access your device, lets you control music playback and get its current state.
 
 
 ## Release info
+* Release v0.0.80: #230
+* Release v0.0.79: #211, #222
 * Release v0.0.78: #207, #209, #212, #213, #215, #217
 * Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
-* Release v0.0.68: #99, #101, #103
-* Release v0.0.67: #90, #91, #95
```

### Comparing `bttc-0.0.79/README.md` & `bttc-0.0.80/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,19 +56,19 @@
 
 
 ### `dut.mc`: Utility to support common Media control operations/methods.
 The `dut.mc` utility, loaded automatically when you access your device, lets you control music playback and get its current state.
 
 
 ## Release info
+* Release v0.0.80: #230
+* Release v0.0.79: #211, #222
 * Release v0.0.78: #207, #209, #212, #213, #215, #217
 * Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
-* Release v0.0.68: #99, #101, #103
-* Release v0.0.67: #90, #91, #95
```

### Comparing `bttc-0.0.79/bttc/__init__.py` & `bttc-0.0.80/bttc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.79'
+__version__ = '0.0.80'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.79/bttc/apk_utils.py` & `bttc-0.0.80/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/ble_data.py` & `bttc-0.0.80/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/ble_utils.py` & `bttc-0.0.80/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/bt_data.py` & `bttc-0.0.80/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/bt_utils.py` & `bttc-0.0.80/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/cli/__init__.py` & `bttc-0.0.80/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/cli/constants.py` & `bttc-0.0.80/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/cli/main.py` & `bttc-0.0.80/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/common_data.py` & `bttc-0.0.80/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/constants.py` & `bttc-0.0.80/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/core.py` & `bttc-0.0.80/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/errors.py` & `bttc-0.0.80/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/general_data.py` & `bttc-0.0.80/bttc/general_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/general_utils.py` & `bttc-0.0.80/bttc/general_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,14 +262,97 @@
       return [
           prop for prop in self if prop.key and re_pattern_obj.search(prop.key)]
 
     return [
         prop for prop in self if prop.key == pattern]
 
 
+class Settings:
+  """Utility class to handle settings of DUT."""
+
+  SettingPattern = re.compile(
+      r'^(?P<setting_name>[:/ ,._a-zA-Z0-9]+)='
+      r'(?P<setting_value>.*)$')
+
+  def __init__(self, ad: typing_utils.AdbDevice):
+    self._ad = ad
+
+  @property
+  def g(self):
+    return Settings.Namespace(self._ad, 'global')
+
+  @property
+  def secure(self):
+    return Settings.Namespace(self._ad, 'secure')
+
+  @property
+  def system(self):
+    return Settings.Namespace(self._ad, 'system')
+
+  class Namespace:
+    """Namespace of settings.
+
+    Namespace is one of {system, secure, global}, case-insensitive
+    """
+    @dataclasses.dataclass
+    class Setting:
+      name: str
+      value: str
+      err: str = ""
+
+    class SettingIter:
+      def __init__(self, setting_info: list[str]):
+        self._setting_info = setting_info
+
+      def __iter__(self) -> Iterator:
+        return self
+
+      def __next__(self):
+        if self._setting_info:
+          next_setting_str = self._setting_info.pop(0).strip()
+          if next_setting_str:
+            mth = Settings.SettingPattern.match(next_setting_str)
+            if not mth:
+              return Settings.Namespace.Setting(
+                  name=None,
+                  value=None,
+                  err=f'Unexpected setting: {next_setting_str}')
+            return Settings.Namespace.Setting(
+                name=mth['setting_name'], value=mth['setting_value'])
+
+          raise StopIteration
+
+    def __init__(self, ad: typing_utils.AdbDevice, namespace: str):
+      self._ad = ad
+      self._namespace = namespace
+
+    def __getitem__(
+      self, setting_or_slice: str | slice
+    ) -> str | list["Settings.Namespace.Setting"]:
+      """Accesses setting value of current namespace."""
+      if isinstance(setting_or_slice, slice):
+        return list(self)[setting_or_slice]
+
+      setting_value = settings_get(
+          self._ad, self._namespace, setting_or_slice)
+      return Settings.Namespace.Setting(
+          name=setting_or_slice, value=setting_value)
+
+    def __setitem__(self, setting: str, value: str):
+      """Put setting value of current namespace."""
+      settings_put(self._ad, self._namespace, setting, value)
+
+    def __iter__(self) -> Iterator:
+      """Iterates the settings of current namespace."""
+      return Settings.Namespace.SettingIter(
+          self._ad.adb.shell(f"settings list {self._namespace}")
+              .decode()
+              .split("\n"))
+
+
 class LogcatSearchStrategy:
   """Logcat searching strategy."""
 
   def __init__(self, interested_ts: str, log_pattern: str):
     try:
       self._start_time_conv = datetime.datetime.strptime(
           interested_ts, _DATETIME_FMT)
@@ -365,15 +448,18 @@
     self._bind(get_all_volume)
     self._bind(get_volume)
     self._bind(is_apk_installed)
     self._bind(logcat_filter)
     self.props = Props(self._ad)
     self._bind(push_file)
     self._bind(push_non_persistent_property)
+    self._bind(settings_get)
+    self._bind(settings_put)
     self._bind(set_volume)
+    self.settings = Settings(self._ad)
     self.shell = bt_utils.safe_adb_shell(ad)
     self._bind(take_screenshot)
 
   @property
   def airplane_mode(self) -> bool:
     """Gets the current airplane mode status of the device.
 
@@ -1203,14 +1289,62 @@
     ad.adb.shell("'chmod 644 /data/local.prop'", shell=True)
   except adb.AdbError as ex:
     ad.log.error(
         f'Failed to push persistent property="{property_name}": {ex}')
     raise ex
 
 
+def settings_get(
+    ad: typing_utils.AdbDevice, namespace: str, setting: str) -> str:
+  """Gets setting from a given namespace in device's settings.
+
+  Args:
+    ad: Adb like device.
+    namespace: Namespace to query for.
+    setting: The setting name.
+
+  Returns:
+    The corresponding setting value.
+
+  Raises:
+    adb.Error: Fail to get setting from given namespace.
+  """
+  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+      f"settings get {namespace} {setting}"
+  )
+  if ret_code != 0:
+    raise adb.Error(
+        f"Failed to retrieve setting={setting} (rt={ret_code}): "
+        f'{stdout or "?"}')
+
+  return stdout.strip()
+
+
+def settings_put(
+    ad: typing_utils.AdbDevice, namespace: str, setting: str, value: str
+):
+  """Put setting into a given namespace in device's settings.
+
+  Args:
+    ad: Adb like device.
+    namespace: Namespace to process.
+    setting: The setting name.
+
+  Raises:
+    adb.Error: Fail to put device_config setting.
+  """
+  stdout, _, ret_code = bt_utils.safe_adb_shell(ad)(
+      f"settings put {namespace} {setting} {value}")
+  if ret_code != 0:
+    raise adb.Error(
+        f'Failed to put "{setting}={value}" in namespace={namespace}'
+        f'(rt={ret_code}): {stdout or "?"}'
+    )
+
+
 def set_volume(
     ad: typing_utils.AdbDevice,
     volume_type: general_data.VolumeType,
     level: int,
     sync_wait_sec: int = 2) -> str:
   """Sets the level of a certain volume type.
```

### Comparing `bttc-0.0.79/bttc/mc_data.py` & `bttc-0.0.80/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/mc_utils.py` & `bttc-0.0.80/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.80/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.80/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.80/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.80/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.80/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.80/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/avrcp/errors.py` & `bttc-0.0.80/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/__init__.py` & `bttc-0.0.80/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/constants.py` & `bttc-0.0.80/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/errors.py` & `bttc-0.0.80/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.80/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.80/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.80/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.80/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/strategy.py` & `bttc-0.0.80/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/ad_checker.py` & `bttc-0.0.80/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/device_factory.py` & `bttc-0.0.80/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/dialer_simulator.py` & `bttc-0.0.80/bttc/utils/dialer_simulator.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/iperf/__init__.py` & `bttc-0.0.80/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/iperf/errors.py` & `bttc-0.0.80/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/key_events_handler.py` & `bttc-0.0.80/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/log_parser.py` & `bttc-0.0.80/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/logcat.py` & `bttc-0.0.80/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.80/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.80/bttc/utils/media_player/yt_player_agent.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/retry.py` & `bttc-0.0.80/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/typing_utils.py` & `bttc-0.0.80/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.80/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/ui_pages/errors.py` & `bttc-0.0.80/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.80/bttc/utils/ui_pages/ui_core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.80/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils/ui_pages/utils.py` & `bttc-0.0.80/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/utils_loader.py` & `bttc-0.0.80/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc/wifi_utils.py` & `bttc-0.0.80/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/bttc.egg-info/PKG-INFO` & `bttc-0.0.80/bttc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.79
+Version: 0.0.80
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -75,19 +75,19 @@
 
 
 ### `dut.mc`: Utility to support common Media control operations/methods.
 The `dut.mc` utility, loaded automatically when you access your device, lets you control music playback and get its current state.
 
 
 ## Release info
+* Release v0.0.80: #230
+* Release v0.0.79: #211, #222
 * Release v0.0.78: #207, #209, #212, #213, #215, #217
 * Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
-* Release v0.0.68: #99, #101, #103
-* Release v0.0.67: #90, #91, #95
```

### Comparing `bttc-0.0.79/bttc.egg-info/SOURCES.txt` & `bttc-0.0.80/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.79/setup.py` & `bttc-0.0.80/setup.py`

 * *Files identical despite different names*

