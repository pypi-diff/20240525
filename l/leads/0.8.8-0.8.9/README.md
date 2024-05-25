# Comparing `tmp/leads-0.8.8.tar.gz` & `tmp/leads-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leads-0.8.8.tar", last modified: Sat Mar 30 18:33:30 2024, max compression
+gzip compressed data, was "leads-0.8.9.tar", last modified: Sat Apr  6 02:49:17 2024, max compression
```

## Comparing `leads-0.8.8.tar` & `leads-0.8.9.tar`

### file list

```diff
@@ -1,129 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-30 18:33:26.000000 leads-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-03-30 18:33:30.196691 leads-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10755 2024-03-30 18:33:26.000000 leads-0.8.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.184691 leads-0.8.8/leads/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-30 18:33:26.000000 leads-0.8.8/leads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-30 18:33:26.000000 leads-0.8.8/leads/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.184691 leads-0.8.8/leads/comm/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-30 18:33:26.000000 leads-0.8.8/leads/comm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.184691 leads-0.8.8/leads/comm/client/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-30 18:33:26.000000 leads-0.8.8/leads/comm/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-30 18:33:26.000000 leads-0.8.8/leads/comm/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-03-30 18:33:26.000000 leads-0.8.8/leads/comm/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.184691 leads-0.8.8/leads/comm/server/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-30 18:33:26.000000 leads-0.8.8/leads/comm/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-30 18:33:26.000000 leads-0.8.8/leads/comm/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.184691 leads-0.8.8/leads/config/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-30 18:33:26.000000 leads-0.8.8/leads/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-30 18:33:26.000000 leads-0.8.8/leads/config/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-30 18:33:26.000000 leads-0.8.8/leads/config/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-30 18:33:26.000000 leads-0.8.8/leads/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-30 18:33:26.000000 leads-0.8.8/leads/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-30 18:33:26.000000 leads-0.8.8/leads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-30 18:33:26.000000 leads-0.8.8/leads/data_persistence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.184691 leads-0.8.8/leads/dt/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-30 18:33:26.000000 leads-0.8.8/leads/dt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-30 18:33:26.000000 leads-0.8.8/leads/dt/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-30 18:33:26.000000 leads-0.8.8/leads/dt/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-30 18:33:26.000000 leads-0.8.8/leads/dt/odometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-03-30 18:33:26.000000 leads-0.8.8/leads/dt/predefined_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-30 18:33:26.000000 leads-0.8.8/leads/dt/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-30 18:33:26.000000 leads-0.8.8/leads/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-03-30 18:33:26.000000 leads-0.8.8/leads/leads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-30 18:33:26.000000 leads-0.8.8/leads/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-30 18:33:26.000000 leads-0.8.8/leads/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.188691 leads-0.8.8/leads/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/atbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/dtcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/ebi.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/gps_speed_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-30 18:33:26.000000 leads-0.8.8/leads/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-30 18:33:26.000000 leads-0.8.8/leads/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-30 18:33:26.000000 leads-0.8.8/leads/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-30 18:33:26.000000 leads-0.8.8/leads/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/leads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11103 2024-03-30 18:33:30.000000 leads-0.8.8/leads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-30 18:33:30.000000 leads-0.8.8/leads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 18:33:30.000000 leads-0.8.8/leads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-30 18:33:30.000000 leads-0.8.8/leads.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-30 18:33:30.000000 leads-0.8.8/leads.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.188691 leads-0.8.8/leads_arduino/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-30 18:33:26.000000 leads-0.8.8/leads_arduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-30 18:33:26.000000 leads-0.8.8/leads_arduino/arduino_micro.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-30 18:33:26.000000 leads-0.8.8/leads_arduino/arduino_nano.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-30 18:33:26.000000 leads-0.8.8/leads_arduino/arduino_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-30 18:33:26.000000 leads-0.8.8/leads_arduino/voltage_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-30 18:33:26.000000 leads-0.8.8/leads_arduino/wheel_speed_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.188691 leads-0.8.8/leads_comm_serial/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-30 18:33:26.000000 leads-0.8.8/leads_comm_serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-30 18:33:26.000000 leads-0.8.8/leads_comm_serial/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.188691 leads-0.8.8/leads_emulation/
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-03-30 18:33:26.000000 leads-0.8.8/leads_emulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.188691 leads-0.8.8/leads_gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.188691 leads-0.8.8/leads_gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/leads_gui/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/battery-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/battery-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/battery-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    33139 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/brake-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    53997 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/brake-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    54591 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/brake-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/ecs-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    16263 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/ecs-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/ecs-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/engine-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    16525 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/engine-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/engine-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/hazard-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/hazard-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    23259 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/hazard-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/high-beam-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    21010 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/high-beam-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/high-beam-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/light-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    25902 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/light-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    26382 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/light-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/motor-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/motor-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    19372 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/motor-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    17264 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/satellite-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/satellite-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    23587 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/satellite-white.png
--rw-r--r--   0 runner    (1001) docker     (127)    25026 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/speed-black.png
--rw-r--r--   0 runner    (1001) docker     (127)    26142 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/speed-red.png
--rw-r--r--   0 runner    (1001) docker     (127)    26727 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/icons/speed-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/leads-theme.json
--rw-r--r--   0 runner    (1001) docker     (127)    56625 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/prototype.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/speedometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-30 18:33:26.000000 leads-0.8.8/leads_gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/leads_raspberry_pi/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-30 18:33:26.000000 leads-0.8.8/leads_raspberry_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-30 18:33:26.000000 leads-0.8.8/leads_raspberry_pi/gps_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-30 18:33:26.000000 leads-0.8.8/leads_raspberry_pi/led.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-30 18:33:26.000000 leads-0.8.8/leads_raspberry_pi/led_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-30 18:33:26.000000 leads-0.8.8/leads_raspberry_pi/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/leads_vec/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/leads_vec/_bootloader/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/_bootloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/_bootloader/leads_vec.service.sh
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/_bootloader/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 18:33:30.196691 leads-0.8.8/leads_vec_rc/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec_rc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec_rc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-30 18:33:26.000000 leads-0.8.8/leads_vec_rc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 18:33:30.196691 leads-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-30 18:33:26.000000 leads-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.404859 leads-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-06 02:49:13.000000 leads-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-06 02:49:17.404859 leads-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10752 2024-04-06 02:49:13.000000 leads-0.8.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.388858 leads-0.8.9/leads/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-06 02:49:13.000000 leads-0.8.9/leads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-06 02:49:13.000000 leads-0.8.9/leads/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.388858 leads-0.8.9/leads/comm/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-06 02:49:13.000000 leads-0.8.9/leads/comm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.388858 leads-0.8.9/leads/comm/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-06 02:49:13.000000 leads-0.8.9/leads/comm/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-06 02:49:13.000000 leads-0.8.9/leads/comm/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-04-06 02:49:13.000000 leads-0.8.9/leads/comm/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.388858 leads-0.8.9/leads/comm/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-06 02:49:13.000000 leads-0.8.9/leads/comm/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-06 02:49:13.000000 leads-0.8.9/leads/comm/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.388858 leads-0.8.9/leads/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 02:49:13.000000 leads-0.8.9/leads/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-06 02:49:13.000000 leads-0.8.9/leads/config/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-06 02:49:13.000000 leads-0.8.9/leads/config/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-06 02:49:13.000000 leads-0.8.9/leads/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-06 02:49:13.000000 leads-0.8.9/leads/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-06 02:49:13.000000 leads-0.8.9/leads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-06 02:49:13.000000 leads-0.8.9/leads/data_persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.388858 leads-0.8.9/leads/dt/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-06 02:49:13.000000 leads-0.8.9/leads/dt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-06 02:49:13.000000 leads-0.8.9/leads/dt/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-06 02:49:13.000000 leads-0.8.9/leads/dt/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-06 02:49:13.000000 leads-0.8.9/leads/dt/odometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-06 02:49:13.000000 leads-0.8.9/leads/dt/predefined_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 02:49:13.000000 leads-0.8.9/leads/dt/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-06 02:49:13.000000 leads-0.8.9/leads/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-06 02:49:13.000000 leads-0.8.9/leads/leads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-06 02:49:13.000000 leads-0.8.9/leads/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-06 02:49:13.000000 leads-0.8.9/leads/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.392859 leads-0.8.9/leads/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/atbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/dtcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/ebi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/gps_speed_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-06 02:49:13.000000 leads-0.8.9/leads/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-06 02:49:13.000000 leads-0.8.9/leads/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-06 02:49:13.000000 leads-0.8.9/leads/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-06 02:49:13.000000 leads-0.8.9/leads/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.404859 leads-0.8.9/leads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-06 02:49:17.000000 leads-0.8.9/leads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-06 02:49:17.000000 leads-0.8.9/leads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:49:17.000000 leads-0.8.9/leads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 02:49:17.000000 leads-0.8.9/leads.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-06 02:49:17.000000 leads-0.8.9/leads.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.392859 leads-0.8.9/leads_arduino/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 02:49:13.000000 leads-0.8.9/leads_arduino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-06 02:49:13.000000 leads-0.8.9/leads_arduino/arduino_micro.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-06 02:49:13.000000 leads-0.8.9/leads_arduino/arduino_nano.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-06 02:49:13.000000 leads-0.8.9/leads_arduino/arduino_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-06 02:49:13.000000 leads-0.8.9/leads_arduino/voltage_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-06 02:49:13.000000 leads-0.8.9/leads_arduino/wheel_speed_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.392859 leads-0.8.9/leads_comm_serial/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-06 02:49:13.000000 leads-0.8.9/leads_comm_serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-06 02:49:13.000000 leads-0.8.9/leads_comm_serial/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.392859 leads-0.8.9/leads_emulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-06 02:49:13.000000 leads-0.8.9/leads_emulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.392859 leads-0.8.9/leads_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/accelerometer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.392859 leads-0.8.9/leads_gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.400858 leads-0.8.9/leads_gui/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/battery-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15962 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/battery-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16218 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/battery-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33139 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/brake-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53997 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/brake-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54591 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/brake-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    59262 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/car-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60600 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/car-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60639 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/car-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/engine-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16525 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/engine-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16813 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/engine-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/esc-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16263 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/esc-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/esc-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/hazard-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22803 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/hazard-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23259 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/hazard-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/high-beam-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21010 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/high-beam-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/high-beam-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/light-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25902 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/light-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26382 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/light-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/motor-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/motor-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19372 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/motor-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17264 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/satellite-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/satellite-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23587 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/satellite-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25026 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/speed-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26142 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/speed-red.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26727 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/icons/speed-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/leads-theme.json
+-rw-r--r--   0 runner    (1001) docker     (127)    56625 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/performance_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11845 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/speedometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-06 02:49:13.000000 leads-0.8.9/leads_gui/typography.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.400858 leads-0.8.9/leads_raspberry_pi/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 02:49:13.000000 leads-0.8.9/leads_raspberry_pi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-06 02:49:13.000000 leads-0.8.9/leads_raspberry_pi/gps_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-06 02:49:13.000000 leads-0.8.9/leads_raspberry_pi/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-06 02:49:13.000000 leads-0.8.9/leads_raspberry_pi/led_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-06 02:49:13.000000 leads-0.8.9/leads_raspberry_pi/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.400858 leads-0.8.9/leads_vec/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.400858 leads-0.8.9/leads_vec/_bootloader/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/_bootloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/_bootloader/leads_vec.service.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/_bootloader/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:49:17.404859 leads-0.8.9/leads_vec_rc/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec_rc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec_rc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-06 02:49:13.000000 leads-0.8.9/leads_vec_rc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:49:17.404859 leads-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-06 02:49:13.000000 leads-0.8.9/setup.py
```

### Comparing `leads-0.8.8/LICENSE` & `leads-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/PKG-INFO` & `leads-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leads
-Version: 0.8.8
+Version: 0.8.9
 Summary: Lightweight Embedded Assisted Driving System
 Home-page: https://github.com/ProjectNeura/LEADS
 Author: ProjectNeura
 Author-email: central@projectneura.org
 License: Apache License 2.0
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
@@ -247,15 +247,15 @@
 
 ### Main
 
 #### Pin Configuration
 
 ![pin-config](docs/assets/pin-config.png)
 
-### Remote Controller
+### Remote Analyst
 
 ![comm-flowchart](docs/assets/comm-flowchart.png)
 
 ## Collaborations
 
 ### Community
```

### Comparing `leads-0.8.8/README.md` & `leads-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
 
 ### Main
 
 #### Pin Configuration
 
 ![pin-config](docs/assets/pin-config.png)
 
-### Remote Controller
+### Remote Analyst
 
 ![comm-flowchart](docs/assets/comm-flowchart.png)
 
 ## Collaborations
 
 ### Community
```

### Comparing `leads-0.8.8/leads/callback.py` & `leads-0.8.9/leads/callback.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/comm/client/client.py` & `leads-0.8.9/leads/comm/client/client.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/comm/prototype.py` & `leads-0.8.9/leads/comm/prototype.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/comm/server/server.py` & `leads-0.8.9/leads/comm/server/server.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/config/registry.py` & `leads-0.8.9/leads/config/registry.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/config/template.py` & `leads-0.8.9/leads/config/template.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/context.py` & `leads-0.8.9/leads/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABCMeta as _ABCMeta, abstractmethod as _abstractmethod
 from collections import deque as _deque
 from time import time as _time
 from typing import TypeVar as _TypeVar, Generic as _Generic
 
 from numpy import diff as _diff, average as _average, array as _array
 
-from leads.constant import ECSMode
+from leads.constant import ESCMode
 from leads.data import DataContainer, SRWDataContainer, DRWDataContainer
 
 T = _TypeVar("T", bound=DataContainer)
 
 
 def _check_data_type(data: T, superclass: type[DataContainer] = DataContainer) -> None:
     if not isinstance(data, superclass):
@@ -36,15 +36,15 @@
         self._initial_data_type: type[DataContainer] = type(initial_data)
         if data_seq_size < 1:
             raise ValueError("`data_seq_size` must be greater or equal to 1")
         self._data_seq: _deque[dct] = _deque((initial_data,), maxlen=data_seq_size)
         self._speed_seq: _deque[float] = _deque(maxlen=data_seq_size)
         self._lap_time_seq: _deque[int] = _deque((int(_time() * 1000),), maxlen=num_laps_timed + 1)
         self._torque_mapping: list[float] = [1] if srw_mode else [1, 1]
-        self._ecs_mode: ECSMode = ECSMode.STANDARD
+        self._esc_mode: ESCMode = ESCMode.STANDARD
         self._hazard: bool = False
 
     def data(self) -> T:
         """
         :return: a copy of the current data container
         """
         return self._data_seq[-1]
@@ -57,18 +57,18 @@
         _check_data_type(data, self._initial_data_type)
         self._data_seq.append(data)
         self._speed_seq.append(data.speed)
 
     def srw_mode(self) -> bool:
         return self._srw_mode
 
-    def ecs_mode(self, ecs_mode: ECSMode | None = None) -> ECSMode | None:
-        if ecs_mode is None:
-            return self._ecs_mode
-        self._ecs_mode = ecs_mode
+    def esc_mode(self, esc_mode: ESCMode | None = None) -> ESCMode | None:
+        if esc_mode is None:
+            return self._esc_mode
+        self._esc_mode = esc_mode
 
     @_abstractmethod
     def update(self) -> None:
         raise NotImplementedError
 
     @_abstractmethod
     def intervene(self, *args, **kwargs) -> None:  # real signature unknown
```

### Comparing `leads-0.8.8/leads/data_persistence.py` & `leads-0.8.9/leads/data_persistence.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/dt/controller.py` & `leads-0.8.9/leads/dt/controller.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/dt/device.py` & `leads-0.8.9/leads/dt/device.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/dt/odometer.py` & `leads-0.8.9/leads/dt/odometer.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/dt/registry.py` & `leads-0.8.9/leads/dt/registry.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/event.py` & `leads-0.8.9/leads/event.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/leads.py` & `leads-0.8.9/leads/leads.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/logger.py` & `leads-0.8.9/leads/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from leads.config import set_on_register_config, ConfigTemplate
 from leads.os import _currentframe
 from leads.types import OnRegister as _OnRegister
 
 
 class Level(_IntEnum):
-    DEBUG: int = 0x00
-    INFO: int = 0x01
-    WARN: int = 0x02
-    ERROR: int = 0x03
+    DEBUG: int = 0
+    INFO: int = 1
+    WARN: int = 2
+    ERROR: int = 3
 
 
 class Logger(object):
     REGULAR: int = 0
     BOLD: int = 1
     ITALIC: int = 3
     UNDERLINED: int = 4
```

### Comparing `leads-0.8.8/leads/os.py` & `leads-0.8.9/leads/os.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/plugin/abs.py` & `leads-0.8.9/leads/plugin/abs.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/plugin/dtcs.py` & `leads-0.8.9/leads/plugin/dtcs.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/plugin/gps_speed_correction.py` & `leads-0.8.9/leads/plugin/gps_speed_correction.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/plugin/plugin.py` & `leads-0.8.9/leads/plugin/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any as _Any
 
-from leads.constant import ECSMode
+from leads.constant import ESCMode
 from leads.context import Context
 from leads.registry import require_context
 from leads.types import RequiredData as _RequiredData
 
 
 class Plugin(object):
     def __init__(self, required_data: _RequiredData) -> None:
@@ -20,15 +20,15 @@
         return self.state[key]
 
     def __setitem__(self, key: str, value: _Any) -> None:
         self.state[key] = value
 
     def enabled(self, enabled: bool | None = None) -> bool | None:
         if enabled is None:
-            return require_context().ecs_mode() != ECSMode.OFF and self._enabled
+            return require_context().esc_mode() != ESCMode.OFF and self._enabled
         self._enabled = enabled
 
     def required_data(self) -> list[str]:
         return (self._required_data if isinstance(self._required_data, list) else
                 self._required_data[0] if require_context().srw_mode() else self._required_data[1])
 
     def on_load(self, context: Context) -> None: ...
```

### Comparing `leads-0.8.8/leads/registry.py` & `leads-0.8.9/leads/registry.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads/sft.py` & `leads-0.8.9/leads/sft.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads.egg-info/PKG-INFO` & `leads-0.8.9/leads.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leads
-Version: 0.8.8
+Version: 0.8.9
 Summary: Lightweight Embedded Assisted Driving System
 Home-page: https://github.com/ProjectNeura/LEADS
 Author: ProjectNeura
 Author-email: central@projectneura.org
 License: Apache License 2.0
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
@@ -247,15 +247,15 @@
 
 ### Main
 
 #### Pin Configuration
 
 ![pin-config](docs/assets/pin-config.png)
 
-### Remote Controller
+### Remote Analyst
 
 ![comm-flowchart](docs/assets/comm-flowchart.png)
 
 ## Collaborations
 
 ### Community
```

### Comparing `leads-0.8.8/leads.egg-info/SOURCES.txt` & `leads-0.8.9/leads.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -47,35 +47,42 @@
 leads_arduino/arduino_proto.py
 leads_arduino/voltage_sensor.py
 leads_arduino/wheel_speed_sensor.py
 leads_comm_serial/__init__.py
 leads_comm_serial/connection.py
 leads_emulation/__init__.py
 leads_gui/__init__.py
+leads_gui/accelerometer.py
 leads_gui/config.py
 leads_gui/icons.py
+leads_gui/performance_checker.py
 leads_gui/prototype.py
+leads_gui/proxy.py
 leads_gui/runtime.py
 leads_gui/speedometer.py
 leads_gui/system.py
 leads_gui/types.py
+leads_gui/typography.py
 leads_gui/assets/leads-theme.json
 leads_gui/assets/logo.png
 leads_gui/assets/icons/battery-black.png
 leads_gui/assets/icons/battery-red.png
 leads_gui/assets/icons/battery-white.png
 leads_gui/assets/icons/brake-black.png
 leads_gui/assets/icons/brake-red.png
 leads_gui/assets/icons/brake-white.png
-leads_gui/assets/icons/ecs-black.png
-leads_gui/assets/icons/ecs-red.png
-leads_gui/assets/icons/ecs-white.png
+leads_gui/assets/icons/car-black.png
+leads_gui/assets/icons/car-red.png
+leads_gui/assets/icons/car-white.png
 leads_gui/assets/icons/engine-black.png
 leads_gui/assets/icons/engine-red.png
 leads_gui/assets/icons/engine-white.png
+leads_gui/assets/icons/esc-black.png
+leads_gui/assets/icons/esc-red.png
+leads_gui/assets/icons/esc-white.png
 leads_gui/assets/icons/hazard-black.png
 leads_gui/assets/icons/hazard-red.png
 leads_gui/assets/icons/hazard-white.png
 leads_gui/assets/icons/high-beam-black.png
 leads_gui/assets/icons/high-beam-red.png
 leads_gui/assets/icons/high-beam-white.png
 leads_gui/assets/icons/light-black.png
```

### Comparing `leads-0.8.8/leads_arduino/arduino_proto.py` & `leads-0.8.9/leads_arduino/arduino_proto.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_arduino/wheel_speed_sensor.py` & `leads-0.8.9/leads_arduino/wheel_speed_sensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from math import pi as _pi
 from time import time as _time
 from typing import override as _override
 
+from numpy import pi as _pi
+
 from leads import Device as _Device, get_device as _get_device, Odometer as _Odometer
 
 
 def rpm2kmh(rpm: float, wheel_circumference: float) -> float:
     """
     :param rpm: revolutions per minute
     :param wheel_circumference: wheel circumference in centimeters
```

### Comparing `leads-0.8.8/leads_comm_serial/connection.py` & `leads-0.8.9/leads_comm_serial/connection.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_emulation/__init__.py` & `leads-0.8.9/leads_emulation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from random import randint as _randint
 from typing import override as _override
 
 from numpy import sin as _sin, pi as _pi
 
 from leads import Controller as _Controller, SRWDataContainer as _SRWDataContainer, \
-    DRWDataContainer as _DRWDataContainer
+    DRWDataContainer as _DRWDataContainer, Device as _Device
 
 
 class _EmulatedController(_Controller):
     def __init__(self,
                  minimum: int = 30,
                  maximum: int = 40,
                  skid_possibility: float = .1) -> None:
@@ -72,7 +72,13 @@
             return _DRWDataContainer(voltage=48.0,
                                      min_speed=(fws := (_sin(self.counter) + .5) * self.magnitude + self.offset),
                                      front_wheel_speed=fws,
                                      left_rear_wheel_speed=(rws := self.generate_rear_wheel_speed(fws)),
                                      right_rear_wheel_speed=rws)
         finally:
             self.counter = (self.counter + self.acceleration) % _pi
+
+
+class GPSReceiver(_Device):
+    @_override
+    def read(self) -> [bool, float, float, float, int, int]:
+        return False, 0, 0, 0, 0, 0
```

### Comparing `leads-0.8.8/leads_gui/assets/icons/battery-black.png` & `leads-0.8.9/leads_gui/assets/icons/battery-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/battery-red.png` & `leads-0.8.9/leads_gui/assets/icons/battery-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/battery-white.png` & `leads-0.8.9/leads_gui/assets/icons/battery-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/brake-black.png` & `leads-0.8.9/leads_gui/assets/icons/brake-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/brake-red.png` & `leads-0.8.9/leads_gui/assets/icons/brake-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/brake-white.png` & `leads-0.8.9/leads_gui/assets/icons/brake-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/ecs-black.png` & `leads-0.8.9/leads_gui/assets/icons/esc-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/ecs-red.png` & `leads-0.8.9/leads_gui/assets/icons/esc-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/ecs-white.png` & `leads-0.8.9/leads_gui/assets/icons/esc-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/engine-black.png` & `leads-0.8.9/leads_gui/assets/icons/engine-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/engine-red.png` & `leads-0.8.9/leads_gui/assets/icons/engine-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/engine-white.png` & `leads-0.8.9/leads_gui/assets/icons/engine-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/hazard-black.png` & `leads-0.8.9/leads_gui/assets/icons/hazard-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/hazard-red.png` & `leads-0.8.9/leads_gui/assets/icons/hazard-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/hazard-white.png` & `leads-0.8.9/leads_gui/assets/icons/hazard-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/high-beam-black.png` & `leads-0.8.9/leads_gui/assets/icons/high-beam-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/high-beam-red.png` & `leads-0.8.9/leads_gui/assets/icons/high-beam-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/high-beam-white.png` & `leads-0.8.9/leads_gui/assets/icons/high-beam-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/light-black.png` & `leads-0.8.9/leads_gui/assets/icons/light-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/light-red.png` & `leads-0.8.9/leads_gui/assets/icons/light-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/light-white.png` & `leads-0.8.9/leads_gui/assets/icons/light-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/motor-black.png` & `leads-0.8.9/leads_gui/assets/icons/motor-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/motor-red.png` & `leads-0.8.9/leads_gui/assets/icons/motor-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/motor-white.png` & `leads-0.8.9/leads_gui/assets/icons/motor-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/satellite-black.png` & `leads-0.8.9/leads_gui/assets/icons/satellite-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/satellite-red.png` & `leads-0.8.9/leads_gui/assets/icons/satellite-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/satellite-white.png` & `leads-0.8.9/leads_gui/assets/icons/satellite-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/speed-black.png` & `leads-0.8.9/leads_gui/assets/icons/speed-black.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/speed-red.png` & `leads-0.8.9/leads_gui/assets/icons/speed-red.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/icons/speed-white.png` & `leads-0.8.9/leads_gui/assets/icons/speed-white.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/assets/leads-theme.json` & `leads-0.8.9/leads_gui/assets/leads-theme.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'CTkFont'": "{'macOS': {'family': 'Arial', 'size': 14}, 'Windows': {'family': 'Arial', 'size': "*

 * *              "14}, 'Linux': {'family': 'Arial', 'size': 14}}"}*

```diff
@@ -24,26 +24,26 @@
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
     "CTkFont": {
         "Linux": {
-            "family": "Roboto",
-            "size": 13,
+            "family": "Arial",
+            "size": 14,
             "weight": "normal"
         },
         "Windows": {
-            "family": "Roboto",
-            "size": 13,
+            "family": "Arial",
+            "size": 14,
             "weight": "normal"
         },
         "macOS": {
-            "family": "SF Display",
-            "size": 13,
+            "family": "Arial",
+            "size": 14,
             "weight": "normal"
         }
     },
     "CTkFrame": {
         "border_color": "gray50",
         "border_width": 0,
         "corner_radius": 4,
```

### Comparing `leads-0.8.8/leads_gui/assets/logo.png` & `leads-0.8.9/leads_gui/assets/logo.png`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/config.py` & `leads-0.8.9/leads_gui/config.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_gui/icons.py` & `leads-0.8.9/leads_gui/icons.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         return _CTkImage(self.load_source(color if color else Color.BLACK),
                          None if color else self.load_source(Color.WHITE),
                          size=(size, size))
 
 
 Battery: _Icon = _Icon("battery")
 Brake: _Icon = _Icon("brake")
-ECS: _Icon = _Icon("ecs")
+Car: _Icon = _Icon("car")
+ESC: _Icon = _Icon("esc")
 Engine: _Icon = _Icon("engine")
 Hazard: _Icon = _Icon("hazard")
 HighBeam: _Icon = _Icon("high-beam")
 Light: _Icon = _Icon("light")
 Motor: _Icon = _Icon("motor")
 Satellite: _Icon = _Icon("satellite")
 Speed: _Icon = _Icon("speed")
```

### Comparing `leads-0.8.8/leads_raspberry_pi/__init__.py` & `leads-0.8.9/leads_raspberry_pi/__init__.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_raspberry_pi/gps_receiver.py` & `leads-0.8.9/leads_raspberry_pi/gps_receiver.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             self._ground_speed = float(ground_speed) * 1.852 if (ground_speed := data.data[6]) else 0
         if NMEAGPSReceiver._has_field(data.fields, "gps_qual", 5):
             self._quality = int(data.data[5])
         if NMEAGPSReceiver._has_field(data.fields, "num_sats", 6):
             self._num_satellites = int(data.data[6])
 
     @_override
-    def read(self) -> [bool, float, float, float, int]:
+    def read(self) -> [bool, float, float, float, int, int]:
         """
         :return: [validity, ground speed, latitude, longitude, quality, num of satellites]
         """
         return self._valid, self._ground_speed, self._latitude, self._longitude, self._quality, self._num_satellites
 
     @_override
     def run(self) -> None:
```

### Comparing `leads-0.8.8/leads_raspberry_pi/led.py` & `leads-0.8.9/leads_raspberry_pi/led.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from gpiozero import LED as _LED
 
 from leads import Device as _Device
 
 
 class LEDCommand(_IntEnum):
-    OFF: int = 0x00
-    ON: int = 0x01
-    BLINK: int = 0x02
+    OFF: int = 0
+    ON: int = 1
+    BLINK: int = 2
 
 
 class LED(_Device):
     """
     Control a LED digitally.
     Supports:
     - Any 2-pin LED
```

### Comparing `leads-0.8.8/leads_raspberry_pi/led_group.py` & `leads-0.8.9/leads_raspberry_pi/led_group.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_vec/__main__.py` & `leads-0.8.9/leads_vec/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from argparse import ArgumentParser as _ArgumentParser, BooleanOptionalAction as _BooleanOptionalAction
 from os import mkdir as _mkdir, chmod as _chmod
 from os.path import exists as _exists
 from subprocess import run as _run
 from sys import exit as _exit, version as _version
 
 from leads import register_controller as _register_controller, MAIN_CONTROLLER as _MAIN_CONTROLLER, \
-    L as _L, load_config as _load_config, register_config as _register_config
-from leads_gui import get_system_platform as _get_system_platform, Config as _Config
+    L as _L, load_config as _load_config, register_config as _register_config, device as _device, \
+    GPS_RECEIVER as _GPS_RECEIVER
+from leads_gui import Config as _Config
+from leads_gui.system import get_system_platform as _get_system_platform
 
 if __name__ == "__main__":
     parser = _ArgumentParser(prog="LEADS VeC",
                              description="Lightweight Embedded Assisted Driving System VeC",
                              epilog="ProjectNeura: https://projectneura.org"
                                     "GitHub: https://github.com/ProjectNeura/LEADS")
     parser.add_argument("action", choices=("info", "run"))
     parser.add_argument("-r", "--register", choices=("systemd", "config"), default=None, help="service to register")
     parser.add_argument("-c", "--config", default=None, help="specified configuration file")
+    parser.add_argument("--emu", action=_BooleanOptionalAction, default=False, help="use emulator")
     parser.add_argument("--xws", action=_BooleanOptionalAction, default=False, help="use X Window System")
     args = parser.parse_args()
     if args.action == "info":
         from leads_vec.__version__ import __version__
 
         _L.info("LEADS Version: " + __version__,
                 "System Platform: " + _get_system_platform(),
@@ -53,20 +56,32 @@
     if args.xws:
         from os import getuid as _getuid
         from pwd import getpwuid as _getpwuid
 
         _L.info("Configuring X Window System...")
         _run(("/usr/bin/xhost", "+SI:localuser:" + _getpwuid(_getuid()).pw_name))
     try:
+        if args.emu:
+            raise AttributeError("User specifies to use emulator")
         from leads_vec.controller import _
-    except ImportError as e:
+    except (ImportError, AttributeError) as e:
         _L.debug(repr(e))
-        _L.warn("`leads_vec.controller` is not available, using emulation module instead...")
+        if isinstance(e, ImportError):
+            _L.warn("`leads_vec.controller` is not available, using emulation module instead...")
         try:
-            from leads_emulation import SRWRandom as _Controller
+            if config.srw_mode:
+                from leads_emulation import SRWSin as _Controller
+            else:
+                from leads_emulation import DRWSin as _Controller
 
             _register_controller(_MAIN_CONTROLLER, _Controller())
+            from leads_emulation import GPSReceiver as _GPSReceiver
+
+
+            @_device(_GPS_RECEIVER, _MAIN_CONTROLLER)
+            class GPS(_GPSReceiver):
+                pass
         except ImportError:
             raise ImportError("At least one adapter has to be installed")
     from leads_vec.cli import main
 
     _exit(main())
```

### Comparing `leads-0.8.8/leads_vec/_bootloader/systemd.py` & `leads-0.8.9/leads_vec/_bootloader/systemd.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_vec/cli.py` & `leads-0.8.9/leads_vec/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from leads.comm import *
 from leads_gui import *
 from leads_vec.__version__ import __version__
 
 
 class CustomRuntimeData(RuntimeData):
     m1_mode: int = 0
-    m2_mode: int = 0
-    m3_mode: int = 0
     control_system_switch_changed: bool = False
 
 
 def make_system_switch(ctx: LEADS, system: SystemLiteral, runtime_data: RuntimeData) -> Callable[[], None]:
     def switch() -> None:
         ctx.plugin(system).enabled(not ctx.plugin(system).enabled())
         runtime_data.control_system_switch_changed = True
@@ -37,62 +35,68 @@
     ctx.plugin("GPS_SPEED_CORRECTION", GPSSpeedCorrection())
     window = Window(cfg.width,
                     cfg.height,
                     cfg.refresh_rate,
                     CustomRuntimeData(),
                     fullscreen=cfg.fullscreen,
                     no_title_bar=cfg.no_title_bar)
-    m1 = StringVar(window.root(), "")
-    m2 = DoubleVar(window.root(), 0)
-    m3 = StringVar(window.root(), "")
-    ecs = StringVar(window.root(), "STANDARD")
+    root = window.root()
+    root.configure(cursor="dot")
+    m1 = StringVar(root, "")
+    speed = DoubleVar(root, 0)
+    voltage = StringVar(root, "")
+    speed_trend = DoubleVar(root, 0)
+    g_force = GForceVar(root, 0, 0)
+    esc = StringVar(root, "STANDARD")
 
     def render(manager: ContextManager):
-        def switch_m1_mode():
+        def switch_m1_mode(_):
             manager.rd().m1_mode = (manager.rd().m1_mode + 1) % 3
 
-        def switch_m3_mode():
-            manager.rd().m3_mode = (manager.rd().m3_mode + 1) % 3
+        manager["m1"] = Typography(root, theme_key="CTkButton", variable=m1, clickable=True,
+                                   command=switch_m1_mode, font=("Arial", cfg.font_size_small - 4)).lock_ratio(.7)
+        manager["m2"] = Speedometer(root, variable=speed).lock_ratio(.7)
+        manager["m3"] = ProxyCanvas(root, "CTkButton",
+                                    Typography(root, theme_key="CTkButton", variable=voltage,
+                                               font=("Arial", cfg.font_size_medium - 4)),
+                                    SpeedTrendMeter(root, theme_key="CTkButton", variable=speed_trend,
+                                                    font=("Arial", cfg.font_size_medium - 4)),
+                                    GForceMeter(root, theme_key="CTkButton", variable=g_force,
+                                                font=("Arial", cfg.font_size_medium - 4))).lock_ratio(.7)
 
-        manager["m1"] = CTkButton(manager.root(), textvariable=m1, command=switch_m1_mode,
-                                  font=("Arial", cfg.font_size_small))
-        manager["m2"] = Speedometer(manager.root(), variable=m2)
-        manager["m3"] = CTkButton(manager.root(), textvariable=m3, command=switch_m3_mode,
-                                  font=("Arial", cfg.font_size_medium))
-
-        manager["comm_status"] = CTkLabel(manager.root(), text="COMM OFFLINE", text_color="gray",
+        manager["comm_status"] = CTkLabel(root, text="COMM OFFLINE", text_color="gray",
                                           font=("Arial", cfg.font_size_small))
 
         i = 0
         for system in SystemLiteral:
             i += 1
             system_lower = system.lower()
-            manager[system_lower + "_status"] = CTkLabel(manager.root(), text=system + " READY", text_color="green",
+            manager[system_lower + "_status"] = CTkLabel(root, text=system + " READY", text_color="green",
                                                          font=("Arial", cfg.font_size_small))
             add_hotkey(str(i), switch := make_system_switch(ctx, SystemLiteral(system), manager.rd()))
-            manager[system_lower] = CTkButton(manager.root(), text=system + " ON", command=switch,
+            manager[system_lower] = CTkButton(root, text=system + " ON", command=switch,
                                               font=("Arial", cfg.font_size_small))
 
-        manager["time_lap"] = CTkButton(manager.root(), text="Time Lap", command=ctx.time_lap,
+        manager["time_lap"] = CTkButton(root, text="Time Lap", command=ctx.time_lap,
                                         font=("Arial", cfg.font_size_small))
 
         def hazard():
             ctx.hazard(not ctx.hazard())
             manager["hazard"].configure(image=Hazard(color=Color.RED if ctx.hazard() else None))
 
-        manager["hazard"] = CTkButton(manager.root(), text="", image=Hazard(), command=hazard)
+        manager["hazard"] = CTkButton(root, text="", image=Hazard(), command=hazard)
 
-        def switch_ecs_mode(mode):
-            manager["ecs"].configure(selected_color=(c := "green" if (ecs_mode := ECSMode[mode]) < 2 else "red"),
+        def switch_esc_mode(mode):
+            manager["esc"].configure(selected_color=(c := "green" if (esc_mode := ESCMode[mode]) < 2 else "red"),
                                      selected_hover_color=c)
-            ctx.ecs_mode(ecs_mode)
+            ctx.esc_mode(esc_mode)
             manager.rd().control_system_switch_changed = True
 
-        manager["ecs"] = CTkSegmentedButton(manager.root(), values=["STANDARD", "AGGRESSIVE", "SPORT", "OFF"],
-                                            variable=ecs, command=switch_ecs_mode, font=("Arial", cfg.font_size_small))
+        manager["esc"] = CTkSegmentedButton(root, values=["STANDARD", "AGGRESSIVE", "SPORT", "OFF"], variable=esc,
+                                            command=switch_esc_mode, font=("Arial", cfg.font_size_small))
 
     uim = initialize(window, render, ctx, get_controller(MAIN_CONTROLLER))
 
     class CommCallback(Callback):
         def on_fail(self, service: Service, error: Exception) -> None:
             self.super(service=service, error=error)
             L.error("Comm server error: " + repr(error))
@@ -120,33 +124,30 @@
             d = e.context.data()
             if uim.rd().m1_mode == 0:
                 lap_time_list = ctx.get_lap_time_list()
                 m1.set("LAP TIMES\n\n" + ("No Lap Timed" if len(lap_time_list) < 1 else "\n".join(map(format_lap_time,
                                                                                                       lap_time_list))))
             elif uim.rd().m1_mode == 1:
                 gps = get_device(GPS_RECEIVER).read()
-                m1.set(f"GPS {"VALID" if d.gps_valid else "NO FIX"} - {gps[4]} {gps[5]}\n"
+                m1.set(f"GPS {"VALID" if d.gps_valid else "NO FIX"} - {gps[4]} {gps[5]}\n\n"
                        f"{d.gps_ground_speed:.1f} KM / H\n"
                        f"LAT {d.latitude:.5f}\nLON {d.longitude:.5f}")
             elif uim.rd().m1_mode == 2:
                 m1.set(f"VeC {__version__.upper()}\n\n"
                        f"{datetime.now().strftime("%Y-%m-%d %H:%M:%S")}\n"
                        f"{(duration := int(time()) - uim.rd().start_time) // 60} MIN {duration % 60} SEC\n"
                        f"{(m := d.mileage):.1f} KM - {m * 3600 / duration:.1f} KM / H\n\n"
                        f"{"SRW MODE" if cfg.srw_mode else "DRW MODE"}\n"
-                       f"{cfg.refresh_rate} FPS\n"
+                       f"{cfg.refresh_rate} - {uim.fps():.2f} FPS\n"
                        f"{ip[-1] if len(ip := my_ip_addresses()) > 0 else "NOT FOUND"}:{uim.rd().comm.port()}")
-            m2.set(d.speed)
-            if uim.rd().m3_mode == 0:
-                m3.set(f"{d.voltage:.1f} V")
-            elif uim.rd().m3_mode == 1:
-                m3.set("G Force")
-            elif uim.rd().m3_mode == 2:
-                m3.set("STrend\n"
-                       f"{(st := ctx.get_speed_trend() * 10):.1f} {"↑" if st > 0 else "↓"}")
+            speed.set(d.speed)
+            voltage.set(f"{d.voltage:.1f} V")
+            st = ctx.get_speed_trend()
+            speed_trend.set(st)
+            g_force.set((d.lateral_acceleration, d.forward_acceleration))
             if uim.rd().comm.num_connections() < 1:
                 uim["comm_status"].configure(text="COMM OFFLINE", text_color="gray")
             else:
                 uim["comm_status"].configure(text="COMM ONLINE", text_color=["black", "white"])
             if uim.rd().control_system_switch_changed:
                 for system in SystemLiteral:
                     system_lowercase = system.lower()
@@ -174,66 +175,62 @@
 
         def post_suspend(self, e: SuspensionEvent) -> None:
             self.super(e)
             if e.system in SystemLiteral:
                 uim[e.system.lower() + "_status"].configure(text=e.system + " READY", text_color="green")
 
     ctx.set_event_listener(CustomListener())
-    uim["battery_fault"] = CTkLabel(uim.root(), text="")
-    uim["ecs_fault"] = CTkLabel(uim.root(), text="")
-    uim["gps_fault"] = CTkLabel(uim.root(), text="")
-    uim["motor_fault"] = CTkLabel(uim.root(), text="")
-    uim["wheel_speed_fault"] = CTkLabel(uim.root(), text="")
+    uim["battery_fault"] = CTkLabel(root, text="")
+    uim["esc_fault"] = CTkLabel(root, text="")
+    uim["gps_fault"] = CTkLabel(root, text="")
+    uim["motor_fault"] = CTkLabel(root, text="")
+    uim["wheel_speed_fault"] = CTkLabel(root, text="")
 
     def on_fail(_, e: SuspensionEvent) -> None:
-        if e.system == "ECS":
-            uim["ecs_fault"].configure(image=ECS(color=Color.RED))
+        if e.system == "ESC":
+            uim["esc_fault"].configure(image=ESC(color=Color.RED))
         elif e.system == "BATT":
             uim["battery_fault"].configure(image=Battery(color=Color.RED))
         elif e.system == "MOTOR":
             uim["motor_fault"].configure(image=Motor(color=Color.RED))
         elif e.system == "WSC":
             uim["wheel_speed_fault"].configure(image=Speed(color=Color.RED))
         elif e.system == "GPS":
             uim["gps_fault"].configure(image=Satellite(color=Color.RED))
 
     SFT.on_fail = on_fail
 
     def on_recover(_, e: SuspensionEvent) -> None:
-        if e.system == "ECS":
-            uim["ecs_fault"].configure(image=None)
+        if e.system == "ESC":
+            uim["esc_fault"].configure(image=None)
         elif e.system == "BATT":
             uim["battery_fault"].configure(image=None)
         elif e.system == "MOTOR":
             uim["motor_fault"].configure(image=None)
         elif e.system == "WSC":
             uim["wheel_speed_fault"].configure(image=None)
         elif e.system == "GPS":
             uim["gps_fault"].configure(image=None)
 
     SFT.on_recover = on_recover
     if cfg.manual_mode:
         layout = [
             ["m1", "m2", "m3"],
-            [*map(lambda s: s.lower() + "_status", SystemLiteral), "comm_status"],
+            [CTkLabel(root, text="MANUAL MODE"), CTkLabel(root, text="ASSISTANCE DISABLED"), "comm_status"],
             ["time_lap", "hazard"],
-            ["battery_fault", "ecs_fault", "gps_fault", "motor_fault", "wheel_speed_fault"]
+            ["battery_fault", "esc_fault", "gps_fault", "motor_fault", "wheel_speed_fault"]
         ]
-        ctx.ecs_mode(ECSMode.OFF)
+        ctx.esc_mode(ESCMode.OFF)
         uim.rd().control_system_switch_changed = True
     else:
         layout = [
             ["m1", "m2", "m3"],
             [*map(lambda s: s.lower() + "_status", SystemLiteral), "comm_status"],
             list(map(lambda s: s.lower(), SystemLiteral)),
-            ["ecs"],
+            ["esc"],
             ["time_lap", "hazard"],
-            ["battery_fault", "ecs_fault", "gps_fault", "motor_fault", "wheel_speed_fault"]
+            ["battery_fault", "esc_fault", "gps_fault", "motor_fault", "wheel_speed_fault"]
         ]
     uim.layout(layout)
-    placeholder_row = len(layout)
-    CTkLabel(uim.root(), text="").grid(row=placeholder_row, column=0)
-    uim.root().grid_rowconfigure(0, weight=1)
-    uim.root().grid_rowconfigure(placeholder_row, weight=2)
     initialize_main()
     uim.show()
     return 0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `leads-0.8.8/leads_vec/controller.py` & `leads-0.8.9/leads_vec/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from leads import device, controller, MAIN_CONTROLLER, get_controller, WHEEL_SPEED_CONTROLLER, SRWDataContainer, \
     DRWDataContainer, LEFT_FRONT_WHEEL_SPEED_SENSOR, RIGHT_FRONT_WHEEL_SPEED_SENSOR, Controller, \
     CENTER_REAR_WHEEL_SPEED_SENSOR, LEFT_REAR_WHEEL_SPEED_SENSOR, RIGHT_REAR_WHEEL_SPEED_SENSOR, require_config, \
     mark_system, POWER_CONTROLLER, ODOMETER, GPS_RECEIVER, ConcurrentOdometer
 from leads_arduino import ArduinoMicro, WheelSpeedSensor, VoltageSensor
-from leads_raspberry_pi import NMEAGPSReceiver
+from leads_raspberry_pi import NMEAGPSReceiver, LEDGroup, LED, LEDGroupCommand, LEDCommand, Transition
 
 config = require_config()
 BAUD_RATE: int = config.get("baud_rate", 9600)
 POWER_CONTROLLER_PORT: str = config.get("power_controller_port", "COM4")
 WHEEL_SPEED_CONTROLLER_PORT: str = config.get("wheel_speed_controller_port", "COM3")
 GPS_RECEIVER_PORT: str = config.get("gps_receiver_port", "COM5")
 FRONT_WHEEL_DIAMETER: float = config.get("front_wheel_diameter", 20)  # 20 inches
@@ -50,15 +50,15 @@
     def initialize(self, *parent_tags: str) -> None:
         mark_system(self, "POWER", "BATT")
 
 
 @controller(WHEEL_SPEED_CONTROLLER, MAIN_CONTROLLER, (WHEEL_SPEED_CONTROLLER_PORT, BAUD_RATE))
 class WheelSpeedController(ArduinoMicro):
     def initialize(self, *parent_tags: str) -> None:
-        mark_system(self, "WSC", "ECS")
+        mark_system(self, "WSC", "ESC")
         super().initialize(*parent_tags)
 
     def read(self) -> dict[str, float]:
         lfws = self.device(LEFT_FRONT_WHEEL_SPEED_SENSOR).read()
         rfws = self.device(RIGHT_FRONT_WHEEL_SPEED_SENSOR).read()
         front_wheel_speed = (lfws + rfws) * .5
         return {
@@ -97,19 +97,31 @@
         [(FRONT_WHEEL_DIAMETER, ODOMETER),
          (FRONT_WHEEL_DIAMETER, ODOMETER),
          (REAR_WHEEL_DIAMETER, ODOMETER),
          (REAR_WHEEL_DIAMETER, ODOMETER)]
 )))
 class WheelSpeedSensors(WheelSpeedSensor):
     def initialize(self, *parent_tags: str) -> None:
-        mark_system(self, "WSC", "ECS")
+        mark_system(self, "WSC", "ESC")
         super().initialize(*parent_tags)
 
 
 @device(GPS_RECEIVER, MAIN_CONTROLLER, (GPS_RECEIVER_PORT,))
 class GPS(NMEAGPSReceiver):
     def initialize(self, *parent_tags: str) -> None:
         mark_system(self, "GPS")
         super().initialize(*parent_tags)
 
 
+@device("left_turning_light", MAIN_CONTROLLER, (LED(5), LED(6)))
+class LeftTurningLight(LEDGroup):
+    def initialize(self, *parent_tags: str) -> None:
+        self.write(LEDGroupCommand(LEDCommand.BLINK, Transition("left2right")))
+
+
+@device("right_turning_light", MAIN_CONTROLLER, (LED(17), LED(18)))
+class RightTurningLight(LEDGroup):
+    def initialize(self, *parent_tags: str) -> None:
+        self.write(LEDGroupCommand(LEDCommand.BLINK, Transition("right2left")))
+
+
 _ = None  # null export
```

### Comparing `leads-0.8.8/leads_vec_rc/__main__.py` & `leads-0.8.9/leads_vec_rc/__main__.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/leads_vec_rc/cli.py` & `leads-0.8.9/leads_vec_rc/cli.py`

 * *Files identical despite different names*

### Comparing `leads-0.8.8/setup.py` & `leads-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="leads",
-    version="0.8.8",
+    version="0.8.9",
     python_requires=">=3.12",
     author="ProjectNeura",
     author_email="central@projectneura.org",
     description="Lightweight Embedded Assisted Driving System",
     license="Apache License 2.0",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
```

