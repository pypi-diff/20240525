# Comparing `tmp/velbus-aio-2024.4.1.tar.gz` & `tmp/velbus_aio-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velbus-aio-2024.4.1.tar", last modified: Sun Apr  7 12:20:10 2024, max compression
+gzip compressed data, was "velbus_aio-2024.5.1.tar", last modified: Sat May 25 06:14:48 2024, max compression
```

## Comparing `velbus-aio-2024.4.1.tar` & `velbus_aio-2024.5.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7664 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/velbus_aio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 12:20:10.000000 velbus-aio-2024.4.1/velbus_aio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.689069 velbus-aio-2024.4.1/velbusaio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22799 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/command_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:10.705069 velbus-aio-2024.4.1/velbusaio/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/blind_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/bus_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_part3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/channel_name_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/clear_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/counter_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/counter_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/cover_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dali_dim_value_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dimmer_channel_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/dimmer_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/edge_set_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/edge_set_custom_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/forced_off.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/forced_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/interface_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/ir_receiver_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/kwh_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/light_value_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memo_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memory_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memory_data_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/memory_dump_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_subtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/module_type_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/push_button_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/read_data_block_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/read_data_from_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/realtime_clock_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/receive_buffer_full.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/receive_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/relay_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/restore_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/select_program.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/sensor_temp_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/sensor_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_daylight_saving.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_realtime_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/set_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/slider_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/slow_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/start_relay_blinking_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/start_relay_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_relay_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_relay_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_comfort.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_night.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/switch_to_safe.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part3.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part4.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_set_cooling.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/temp_set_heating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/update_led_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/very_fast_blinking_led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/write_data_to_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/write_memory_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/messages/write_module_address_and_serial_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    35467 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/module.py
--rw-r--r--   0 runner    (1001) docker     (127)   250396 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/protocol.json
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/raw_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-07 12:20:06.000000 velbus-aio-2024.4.1/velbusaio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:14:48.237371 velbus_aio-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-25 06:14:48.237371 velbus_aio-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 06:14:48.237371 velbus_aio-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:14:48.233371 velbus_aio-2024.5.1/velbus_aio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-25 06:14:48.000000 velbus_aio-2024.5.1/velbus_aio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-25 06:14:48.000000 velbus_aio-2024.5.1/velbus_aio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:14:48.000000 velbus_aio-2024.5.1/velbus_aio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:14:47.000000 velbus_aio-2024.5.1/velbus_aio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 06:14:48.000000 velbus_aio-2024.5.1/velbus_aio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 06:14:48.000000 velbus_aio-2024.5.1/velbus_aio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:14:48.221371 velbus_aio-2024.5.1/velbusaio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22889 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/command_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:14:48.233371 velbus_aio-2024.5.1/velbusaio/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/blind_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/bus_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/bus_error_counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/bus_error_counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/bus_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/channel_name_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/channel_name_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/channel_name_part3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/channel_name_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/clear_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/counter_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/counter_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/cover_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/cover_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/cover_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/cover_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/dali_device_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/dali_device_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/dali_dim_value_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/dimmer_channel_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/dimmer_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/edge_set_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/edge_set_custom_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/forced_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/forced_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/interface_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/ir_receiver_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/kwh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/light_value_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/memo_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/memory_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/memory_data_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/memory_dump_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/module_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/module_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/module_subtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/module_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/module_type_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/push_button_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/read_data_block_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/read_data_from_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/realtime_clock_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/receive_buffer_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/receive_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/relay_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/restore_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/select_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/sensor_temp_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/sensor_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/set_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/set_daylight_saving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/set_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/set_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/set_realtime_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/set_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/slider_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/slow_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/start_relay_blinking_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/start_relay_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/switch_relay_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/switch_relay_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/switch_to_comfort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/switch_to_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/switch_to_night.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/switch_to_safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_set_cooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/temp_set_heating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/update_led_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/very_fast_blinking_led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/write_data_to_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/write_memory_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/messages/write_module_address_and_serial_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35458 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250396 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/protocol.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/raw_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-25 06:14:38.000000 velbus_aio-2024.5.1/velbusaio/util.py
```

### Comparing `velbus-aio-2024.4.1/LICENSE` & `velbus_aio-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/PKG-INFO` & `velbus_aio-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
@@ -22,15 +22,15 @@
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.5.0
-Requires-Dist: pyserial-asyncio>=0.5
+Requires-Dist: pyserial-asyncio_fast>=0.11
 Requires-Dist: backoff>=1.10.0
 
 ![CI](https://github.com/Cereal2nd/velbus-aio/actions/workflows/main.yml/badge.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Cereal2nd/velbus-aio/master.svg)](https://results.pre-commit.ci/latest/github/Cereal2nd/velbus-aio/master)
 
 # velbus-aio
```

### Comparing `velbus-aio-2024.4.1/README.md` & `velbus_aio-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/pyproject.toml` & `velbus_aio-2024.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "velbus-aio"
 license = {text = "MIT"}
-version = "2024.4.1"
+version = "2024.5.1"
 description = "Open-source home automation platform running on Python 3."
 readme = "README.md"
 authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords = ["home", "velbus", "automation"]
 classifiers = [
@@ -26,15 +26,15 @@
     "Topic :: Home Automation",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8.0"
 dependencies = [
     "pyserial>=3.5.0",
-    "pyserial-asyncio>=0.5",
+    "pyserial-asyncio_fast>=0.11",
     "backoff>=1.10.0",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/Cereal2nd/velbus-aio"
 "Bug Reports" = "https://github.com/Cereal2nd/velbus-aio/issues"
 
@@ -47,15 +47,15 @@
 exclude = ["tests", "tests.*", "examples"]
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 skips = ["B301", "B403", "B323", "B104", "B110"]
 
 [tool.bumpver]
-current_version = "2024.4.1"
+current_version = "2024.5.1"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `velbus-aio-2024.4.1/velbus_aio.egg-info/PKG-INFO` & `velbus_aio-2024.5.1/velbus_aio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velbus-aio
-Version: 2024.4.1
+Version: 2024.5.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: MIT
 Project-URL: Source Code, https://github.com/Cereal2nd/velbus-aio
 Project-URL: Bug Reports, https://github.com/Cereal2nd/velbus-aio/issues
 Keywords: home,velbus,automation
 Platform: any
@@ -22,15 +22,15 @@
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial>=3.5.0
-Requires-Dist: pyserial-asyncio>=0.5
+Requires-Dist: pyserial-asyncio_fast>=0.11
 Requires-Dist: backoff>=1.10.0
 
 ![CI](https://github.com/Cereal2nd/velbus-aio/actions/workflows/main.yml/badge.svg)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/Cereal2nd/velbus-aio/master.svg)](https://results.pre-commit.ci/latest/github/Cereal2nd/velbus-aio/master)
 
 # velbus-aio
```

### Comparing `velbus-aio-2024.4.1/velbus_aio.egg-info/SOURCES.txt` & `velbus_aio-2024.5.1/velbus_aio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/channels.py` & `velbus_aio-2024.5.1/velbusaio/channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,18 @@
         return {
             k: d[k]
             for k in d
             if k != "_writer" and k != "_on_status_update" and k != "_name_parts"
         }
 
     def to_cache(self) -> dict:
-        return {"name": self._name, "type": type(self).__name__}
+        dst = {"name": self._name, "type": type(self).__name__}
+        if hasattr(self, "_Unit"):
+            dst["Unit"] = self._Unit
+        return dst
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self._on_status_update = []
         self._name_parts = {}
 
     def __repr__(self) -> str:
```

### Comparing `velbus-aio-2024.4.1/velbusaio/command_registry.py` & `velbus_aio-2024.5.1/velbusaio/command_registry.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/const.py` & `velbus_aio-2024.5.1/velbusaio/const.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/controller.py` & `velbus_aio-2024.5.1/velbusaio/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pathlib
 import re
 import ssl
 import time
 from urllib.parse import urlparse
 
 import serial
-import serial_asyncio
+import serial_asyncio_fast
 
 from velbusaio.channels import Channel
 from velbusaio.const import LOAD_TIMEOUT
 from velbusaio.exceptions import VelbusConnectionFailed
 from velbusaio.handler import PacketHandler
 from velbusaio.helpers import get_cache_dir
 from velbusaio.message import Message
@@ -155,24 +155,26 @@
                 )
 
             except (ConnectionRefusedError, OSError) as err:
                 raise VelbusConnectionFailed from err
         else:
             # serial port
             try:
-                _transport, _protocol = await serial_asyncio.create_serial_connection(
-                    asyncio.get_event_loop(),
-                    lambda: self._protocol,
-                    url=self._dsn,
-                    baudrate=38400,
-                    bytesize=serial.EIGHTBITS,
-                    parity=serial.PARITY_NONE,
-                    stopbits=serial.STOPBITS_ONE,
-                    xonxoff=0,
-                    rtscts=1,
+                _transport, _protocol = (
+                    await serial_asyncio_fast.create_serial_connection(
+                        asyncio.get_event_loop(),
+                        lambda: self._protocol,
+                        url=self._dsn,
+                        baudrate=38400,
+                        bytesize=serial.EIGHTBITS,
+                        parity=serial.PARITY_NONE,
+                        stopbits=serial.STOPBITS_ONE,
+                        xonxoff=0,
+                        rtscts=1,
+                    )
                 )
             except (FileNotFoundError, serial.SerialException) as err:
                 raise VelbusConnectionFailed from err
         if test_connect:
             return
         # if auth is required send the auth key
         if auth:
```

### Comparing `velbus-aio-2024.4.1/velbusaio/discovery.py` & `velbus_aio-2024.5.1/velbusaio/discovery.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/exceptions.py` & `velbus_aio-2024.5.1/velbusaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/handler.py` & `velbus_aio-2024.5.1/velbusaio/handler.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/helpers.py` & `velbus_aio-2024.5.1/velbusaio/helpers.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/message.py` & `velbus_aio-2024.5.1/velbusaio/message.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/__init__.py` & `velbus_aio-2024.5.1/velbusaio/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/blind_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/blind_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/bus_active.py` & `velbus_aio-2024.5.1/velbusaio/messages/bus_active.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/bus_error_counter_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/bus_error_counter_status_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/bus_error_counter_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/bus_off.py` & `velbus_aio-2024.5.1/velbusaio/messages/bus_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/channel_name_part1.py` & `velbus_aio-2024.5.1/velbusaio/messages/channel_name_part1.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/channel_name_part2.py` & `velbus_aio-2024.5.1/velbusaio/messages/channel_name_part2.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/channel_name_part3.py` & `velbus_aio-2024.5.1/velbusaio/messages/channel_name_part3.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/channel_name_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/channel_name_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/clear_led.py` & `velbus_aio-2024.5.1/velbusaio/messages/clear_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/counter_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/counter_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/counter_status_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/counter_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/cover_down.py` & `velbus_aio-2024.5.1/velbusaio/messages/cover_down.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/cover_off.py` & `velbus_aio-2024.5.1/velbusaio/messages/cover_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/cover_position.py` & `velbus_aio-2024.5.1/velbusaio/messages/cover_position.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/cover_up.py` & `velbus_aio-2024.5.1/velbusaio/messages/cover_up.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings.py` & `velbus_aio-2024.5.1/velbusaio/messages/dali_device_settings.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/dali_device_settings_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/dali_device_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/dali_dim_value_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/dali_dim_value_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/dimmer_channel_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/dimmer_channel_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/dimmer_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/dimmer_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/edge_set_color.py` & `velbus_aio-2024.5.1/velbusaio/messages/edge_set_color.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/edge_set_custom_color.py` & `velbus_aio-2024.5.1/velbusaio/messages/edge_set_custom_color.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/fast_blinking_led.py` & `velbus_aio-2024.5.1/velbusaio/messages/fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/forced_off.py` & `velbus_aio-2024.5.1/velbusaio/messages/forced_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/forced_on.py` & `velbus_aio-2024.5.1/velbusaio/messages/forced_on.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/interface_status_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/interface_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/kwh_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/kwh_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/light_value_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/light_value_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/memo_text.py` & `velbus_aio-2024.5.1/velbusaio/messages/memo_text.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/memory_data.py` & `velbus_aio-2024.5.1/velbusaio/messages/memory_data.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/memory_data_block.py` & `velbus_aio-2024.5.1/velbusaio/messages/memory_data_block.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/memory_dump_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/memory_dump_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/module_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/module_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/module_status_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/module_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/module_subtype.py` & `velbus_aio-2024.5.1/velbusaio/messages/module_subtype.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/module_type.py` & `velbus_aio-2024.5.1/velbusaio/messages/module_type.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/module_type_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/module_type_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/push_button_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/push_button_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/raw.py` & `velbus_aio-2024.5.1/velbusaio/messages/raw.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/read_data_block_from_memory.py` & `velbus_aio-2024.5.1/velbusaio/messages/read_data_block_from_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/read_data_from_memory.py` & `velbus_aio-2024.5.1/velbusaio/messages/read_data_from_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/realtime_clock_status_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/realtime_clock_status_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/receive_buffer_full.py` & `velbus_aio-2024.5.1/velbusaio/messages/receive_buffer_full.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/receive_ready.py` & `velbus_aio-2024.5.1/velbusaio/messages/receive_ready.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/relay_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/relay_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/restore_dimmer.py` & `velbus_aio-2024.5.1/velbusaio/messages/restore_dimmer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/select_program.py` & `velbus_aio-2024.5.1/velbusaio/messages/select_program.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/sensor_settings_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/sensor_temp_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/sensor_temp_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/sensor_temperature.py` & `velbus_aio-2024.5.1/velbusaio/messages/sensor_temperature.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/set_date.py` & `velbus_aio-2024.5.1/velbusaio/messages/set_date.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/set_daylight_saving.py` & `velbus_aio-2024.5.1/velbusaio/messages/set_daylight_saving.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/set_dimmer.py` & `velbus_aio-2024.5.1/velbusaio/messages/set_dimmer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-"""
-:author: Frank van Breugel
+""":author: Frank van Breugel
 """
 
 from __future__ import annotations
 
 from velbusaio.command_registry import register
 from velbusaio.message import Message
 
 COMMAND_CODE = 0x07
 
 
 @register(
     COMMAND_CODE,
-    ["VMB1DM", "VMBDME", "VMB4DC", "VMBDMI", "VMBDMI-R", "VMB1LED", "VMB8DC-20"],
+    ["VMB1DM", "VMBDME", "VMB4DC", "VMB1LED"],
 )
 class SetDimmerMessage(Message):
-    """
+    """with this message the channel numbering is a bitnumber
     send by:
     received by: VMBDME, VMB4DC
     """
 
     def __init__(self, address=None):
         Message.__init__(self)
         self.dimmer_channels = []
@@ -30,43 +29,39 @@
     def set_defaults(self, address):
         if address is not None:
             self.set_address(address)
         self.set_high_priority()
         self.set_no_rtr()
 
     def populate(self, priority, address, rtr, data):
-        """
-        :return: None
-        """
+        """:return: None"""
         self.needs_high_priority(priority)
         self.needs_no_rtr(rtr)
         self.needs_data(data, 4)
         self.set_attributes(priority, address, rtr)
         self.dimmer_channels = self.byte_to_channels(data[0])
         self.dimmer_state = data[1]
         self.dimmer_transitiontime = int.from_bytes(
             data[2:3], byteorder="big", signed=False
         )
 
     def data_to_binary(self):
-        """
-        :return: bytes
-        """
+        """:return: bytes"""
         return bytes(
             [
                 COMMAND_CODE,
                 self.channels_to_byte(self.dimmer_channels),
                 self.dimmer_state,
             ]
         ) + self.dimmer_transitiontime.to_bytes(2, byteorder="big", signed=False)
 
 
-@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20"])
+@register(COMMAND_CODE, ["VMBDALI", "VMBDALI-20", "VMBDMI", "VMBDMI-R", "VMB8DC-20"])
 class SetDimmerMessage2(SetDimmerMessage):
-    """
+    """This with this message the channel numbering is an integer
     send by:
     received by: VMBDALI
     """
 
     def byte_to_channels(self, byte: int) -> list[int]:
         return [byte]
```

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/set_led.py` & `velbus_aio-2024.5.1/velbusaio/messages/set_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/set_realtime_clock.py` & `velbus_aio-2024.5.1/velbusaio/messages/set_realtime_clock.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/set_temperature.py` & `velbus_aio-2024.5.1/velbusaio/messages/set_temperature.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/slider_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/slider_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/slow_blinking_led.py` & `velbus_aio-2024.5.1/velbusaio/messages/slow_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/start_relay_blinking_timer.py` & `velbus_aio-2024.5.1/velbusaio/messages/start_relay_blinking_timer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/start_relay_timer.py` & `velbus_aio-2024.5.1/velbusaio/messages/start_relay_timer.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/switch_relay_off.py` & `velbus_aio-2024.5.1/velbusaio/messages/switch_relay_off.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/switch_relay_on.py` & `velbus_aio-2024.5.1/velbusaio/messages/switch_relay_on.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/switch_to_comfort.py` & `velbus_aio-2024.5.1/velbusaio/messages/switch_to_comfort.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/switch_to_day.py` & `velbus_aio-2024.5.1/velbusaio/messages/switch_to_day.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/switch_to_night.py` & `velbus_aio-2024.5.1/velbusaio/messages/switch_to_night.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/switch_to_safe.py` & `velbus_aio-2024.5.1/velbusaio/messages/switch_to_safe.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part1.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part1.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part2.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part2.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part3.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part3.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_part4.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_part4.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_settings_request.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_sensor_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_sensor_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_set_cooling.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_set_cooling.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/temp_set_heating.py` & `velbus_aio-2024.5.1/velbusaio/messages/temp_set_heating.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/update_led_status.py` & `velbus_aio-2024.5.1/velbusaio/messages/update_led_status.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/very_fast_blinking_led.py` & `velbus_aio-2024.5.1/velbusaio/messages/very_fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/write_data_to_memory.py` & `velbus_aio-2024.5.1/velbusaio/messages/write_data_to_memory.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/write_memory_block.py` & `velbus_aio-2024.5.1/velbusaio/messages/write_memory_block.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/messages/write_module_address_and_serial_number.py` & `velbus_aio-2024.5.1/velbusaio/messages/write_module_address_and_serial_number.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/module.py` & `velbus_aio-2024.5.1/velbusaio/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,26 +544,28 @@
         try:
             cfile = pathlib.Path(f"{self._cache_dir}/{self._address}.json")
             with cfile.open("r") as fl:
                 cache = json.load(fl)
         except OSError:
             cache = {}
         # load default channels
-        await self.__load_default_channels()
+        await self._load_default_channels()
         # load the data from memory ( the stuff that we need)
         if "name" in cache and cache["name"] != "":
             self._name = cache["name"]
         else:
             await self.__load_memory()
         # load the module status
         await self._request_module_status()
         # load the channel names
         if "channels" in cache:
             for num, chan in cache["channels"].items():
                 self._channels[int(num)]._name = chan["name"]
+                if "Unit" in chan:
+                    self._channels[int(num)]._Unit = chan["Unit"]
                 self._channels[int(num)]._is_loaded = True
         else:
             await self._request_channel_name()
         # load the module specific stuff
         self._load()
         # stop the loading
         self._is_loading = False
@@ -722,15 +724,15 @@
                     )
                     msg = ReadDataFromMemoryMessage(self._address)
                     msg.priority = PRIORITY_LOW
                     msg.high_address = addr[0]
                     msg.low_address = addr[1]
                     await self._writer(msg)
 
-    async def __load_default_channels(self) -> None:
+    async def _load_default_channels(self) -> None:
         if "Channels" not in self._data:
             return
 
         for chan, chan_data in self._data["Channels"].items():
             edit = True
             if "Editable" not in chan_data or chan_data["Editable"] != "yes":
                 edit = False
@@ -770,27 +772,23 @@
             memorymap,
             build_year,
             build_week,
             cache_dir,
         )
         self.group_members: dict[int, set[int]] = {}
 
-    async def load(self, from_cache: bool = False) -> None:
-        await super().load(from_cache)
-
-        if not from_cache:
-            for chan in range(1, 64 + 1):
-                self._channels[chan] = Channel(
-                    self, chan, "placeholder", True, self._writer, self._address
-                )
-                # Placeholders will keep this module loading
-                # Until the DaliDeviceSettings messages either delete or replace these placeholder's
-                # with actual channels
-
-            await self._request_dali_channels()
+    async def _load_default_channels(self) -> None:
+        for chan in range(1, 64 + 1):
+            self._channels[chan] = Channel(
+                self, chan, "placeholder", True, self._writer, self._address
+            )
+            # Placeholders will keep this module loading
+            # Until the DaliDeviceSettings messages either delete or replace these placeholder's
+            # with actual channels
+        await self._request_dali_channels()
 
     async def _request_dali_channels(self):
         msg_type = commandRegistry.get_command(
             DALI_DEVICE_SETTINGS_REQUEST_COMMAND_CODE, self.get_type()
         )
         msg: DaliDeviceSettingsRequest = msg_type(self._address)
         msg.priority = PRIORITY_LOW
```

### Comparing `velbus-aio-2024.4.1/velbusaio/protocol.json` & `velbus_aio-2024.5.1/velbusaio/protocol.json`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/protocol.py` & `velbus_aio-2024.5.1/velbusaio/protocol.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/raw_message.py` & `velbus_aio-2024.5.1/velbusaio/raw_message.py`

 * *Files identical despite different names*

### Comparing `velbus-aio-2024.4.1/velbusaio/util.py` & `velbus_aio-2024.5.1/velbusaio/util.py`

 * *Files identical despite different names*

