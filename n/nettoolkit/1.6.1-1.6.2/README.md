# Comparing `tmp/nettoolkit-1.6.1.tar.gz` & `tmp/nettoolkit-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettoolkit-1.6.1.tar", last modified: Thu Mar 21 06:31:34 2024, max compression
+gzip compressed data, was "nettoolkit-1.6.2.tar", last modified: Sat May 25 02:50:32 2024, max compression
```

## Comparing `nettoolkit-1.6.1.tar` & `nettoolkit-1.6.2.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.435946 nettoolkit-1.6.1/
--rw-rw-rw-   0        0        0     1091 2023-03-27 08:31:48.000000 nettoolkit-1.6.1/LICENSE
--rw-rw-rw-   0        0        0      713 2024-03-21 06:31:34.435946 nettoolkit-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-10-18 01:47:58.000000 nettoolkit-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.255980 nettoolkit-1.6.1/nettoolkit/
--rw-rw-rw-   0        0        0     2907 2024-03-21 06:29:04.000000 nettoolkit-1.6.1/nettoolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.266255 nettoolkit-1.6.1/nettoolkit/addressing/
--rw-rw-rw-   0        0        0       78 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/addressing/__init__.py
--rw-rw-rw-   0        0        0    51053 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/addressing.py
--rw-rw-rw-   0        0        0     3400 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/batch.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.275824 nettoolkit-1.6.1/nettoolkit/addressing/forms/
--rw-rw-rw-   0        0        0        0 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/forms/__init__.py
--rw-rw-rw-   0        0        0     1476 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/forms/compare_scanner_outputs.py
--rw-rw-rw-   0        0        0     2760 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/forms/create_batch.py
--rw-rw-rw-   0        0        0     4566 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/forms/prefixes_oper.py
--rw-rw-rw-   0        0        0     3092 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/forms/subnet_scanner.py
--rw-rw-rw-   0        0        0     4951 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/addressing/subnetscan.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.285981 nettoolkit-1.6.1/nettoolkit/capture_it/
--rw-rw-rw-   0        0        0      290 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/__init__.py
--rw-rw-rw-   0        0        0     2200 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/_detection.py
--rw-rw-rw-   0        0        0     9542 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/cap_summary.py
--rw-rw-rw-   0        0        0     3242 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/captures.py
--rw-rw-rw-   0        0        0     3758 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/clp.py
--rw-rw-rw-   0        0        0     4104 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/command.py
--rw-rw-rw-   0        0        0      667 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/common.py
--rw-rw-rw-   0        0        0     9080 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/configure.py
--rw-rw-rw-   0        0        0     5494 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/conn.py
--rw-rw-rw-   0        0        0     9686 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/exec_device.py
--rw-rw-rw-   0        0        0    17079 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/executions.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.285981 nettoolkit-1.6.1/nettoolkit/capture_it/forms/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/capture_it/forms/__init__.py
--rw-rw-rw-   0        0        0     5532 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/forms/common_to_all.py
--rw-rw-rw-   0        0        0     1589 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/forms/cred.py
--rw-rw-rw-   0        0        0     2548 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/forms/custom.py
--rw-rw-rw-   0        0        0     1855 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/forms/options.py
--rw-rw-rw-   0        0        0     1939 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/capture_it/forms/quick_show.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.295915 nettoolkit-1.6.1/nettoolkit/compare_it/
--rw-rw-rw-   0        0        0      200 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/compare_it/__init__.py
--rw-rw-rw-   0        0        0    12342 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/compare_it/diff.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.295915 nettoolkit-1.6.1/nettoolkit/compare_it/forms/
--rw-rw-rw-   0        0        0        0 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/compare_it/forms/__init__.py
--rw-rw-rw-   0        0        0     5204 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/compare_it/forms/compare_configs.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.295915 nettoolkit-1.6.1/nettoolkit/detect/
--rw-rw-rw-   0        0        0       81 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     2630 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/detect/detection.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.305820 nettoolkit-1.6.1/nettoolkit/facts_finder/
--rw-rw-rw-   0        0        0      530 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/__init__.py
--rw-rw-rw-   0        0        0     6182 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/clean.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.305820 nettoolkit-1.6.1/nettoolkit/facts_finder/commons/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/commons/__init__.py
--rw-rw-rw-   0        0        0     1151 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/commons/common.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.305820 nettoolkit-1.6.1/nettoolkit/facts_finder/forms/
--rw-rw-rw-   0        0        0        0 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/forms/__init__.py
--rw-rw-rw-   0        0        0     3809 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/forms/ff_custom.py
--rw-rw-rw-   0        0        0     4048 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/forms/ff_custom_cit.py
--rw-rw-rw-   0        0        0     3238 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/forms/ff_generate.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.315914 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/
--rw-rw-rw-   0        0        0      324 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.328666 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/
--rw-rw-rw-   0        0        0      888 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_arp_table.py
--rw-rw-rw-   0        0        0     6452 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_bgp.py
--rw-rw-rw-   0        0        0     2302 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_cdp.py
--rw-rw-rw-   0        0        0     1697 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_description.py
--rw-rw-rw-   0        0        0     2018 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_status.py
--rw-rw-rw-   0        0        0     1976 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_lldp.py
--rw-rw-rw-   0        0        0     1500 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_mac_table.py
--rw-rw-rw-   0        0        0     5143 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_ospf.py
--rw-rw-rw-   0        0        0    10147 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py
--rw-rw-rw-   0        0        0     3024 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_prefix_list.py
--rw-rw-rw-   0        0        0     5591 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_routes.py
--rw-rw-rw-   0        0        0     5332 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_system.py
--rw-rw-rw-   0        0        0     4386 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py
--rw-rw-rw-   0        0        0     1374 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_version.py
--rw-rw-rw-   0        0        0     4746 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/common.py
--rw-rw-rw-   0        0        0     7509 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco_parser.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.336174 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/commons/
--rw-rw-rw-   0        0        0      125 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/commons/__init__.py
--rw-rw-rw-   0        0        0     2061 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/commons/generator_commons.py
--rw-rw-rw-   0        0        0      250 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/device.py
--rw-rw-rw-   0        0        0     4506 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/facts_gen.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.345936 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/
--rw-rw-rw-   0        0        0      845 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/__init__.py
--rw-rw-rw-   0        0        0     2277 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_arp_table.py
--rw-rw-rw-   0        0        0     2924 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py
--rw-rw-rw-   0        0        0     1467 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_int_description.py
--rw-rw-rw-   0        0        0     2030 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_lldp.py
--rw-rw-rw-   0        0        0      890 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running.py
--rw-rw-rw-   0        0        0     7219 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_bgp.py
--rw-rw-rw-   0        0        0    16908 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py
--rw-rw-rw-   0        0        0     5898 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_ospf.py
--rw-rw-rw-   0        0        0     3195 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_prefix_lists.py
--rw-rw-rw-   0        0        0     4318 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routes.py
--rw-rw-rw-   0        0        0     3447 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py
--rw-rw-rw-   0        0        0     8424 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_system.py
--rw-rw-rw-   0        0        0     1101 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_version.py
--rw-rw-rw-   0        0        0     1482 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/common.py
--rw-rw-rw-   0        0        0     6363 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper_parser.py
--rw-rw-rw-   0        0        0     3534 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/generators/merger.py
--rw-rw-rw-   0        0        0     6888 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/inputlog.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.355858 nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/
--rw-rw-rw-   0        0        0      199 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/__init__.py
--rw-rw-rw-   0        0        0     1684 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/cisco.py
--rw-rw-rw-   0        0        0     6025 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/common.py
--rw-rw-rw-   0        0        0     2558 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/juniper.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.359885 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/
--rw-rw-rw-   0        0        0      139 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.365969 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/
--rw-rw-rw-   0        0        0      345 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/__init__.py
--rw-rw-rw-   0        0        0     7992 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/cisco_tables.py
--rw-rw-rw-   0        0        0     1734 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/cisco_var.py
--rw-rw-rw-   0        0        0     1465 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/cisco_vrfs.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.365969 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/commands/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/commands/__init__.py
--rw-rw-rw-   0        0        0     3407 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/commands/cmd_dict.py
--rw-rw-rw-   0        0        0     3019 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/merger.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.365969 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/commons/
--rw-rw-rw-   0        0        0      303 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/commons/__init__.py
--rw-rw-rw-   0        0        0     8515 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/commons/modifier_commons.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.365969 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/
--rw-rw-rw-   0        0        0      303 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.365969 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/commands/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/commands/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/commands/cmd_dict.py
--rw-rw-rw-   0        0        0     2345 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/juniper_tables.py
--rw-rw-rw-   0        0        0     1068 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/juniper_var.py
--rw-rw-rw-   0        0        0     2197 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/merger.py
--rw-rw-rw-   0        0        0     5164 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/facts_finder/rearrange.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.376156 nettoolkit-1.6.1/nettoolkit/j2config/
--rw-rw-rw-   0        0        0      314 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.376156 nettoolkit-1.6.1/nettoolkit/j2config/cmn/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/cmn/__init__.py
--rw-rw-rw-   0        0        0     6648 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/j2config/cmn/common_fn.py
--rw-rw-rw-   0        0        0     5140 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/data_collect.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.376156 nettoolkit-1.6.1/nettoolkit/j2config/forms/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/forms/__init__.py
--rw-rw-rw-   0        0        0     6421 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/j2config/forms/input_data.py
--rw-rw-rw-   0        0        0     9427 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/j2config/func.py
--rw-rw-rw-   0        0        0      617 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/general.py
--rw-rw-rw-   0        0        0     4235 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/j2.py
--rw-rw-rw-   0        0        0     1518 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/j2config/read_conditions.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.385902 nettoolkit-1.6.1/nettoolkit/log/
--rw-rw-rw-   0        0        0        4 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/log/__init__.py
--rw-rw-rw-   0        0        0      907 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/log/log_executions.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.385902 nettoolkit-1.6.1/nettoolkit/nettoolkit/
--rw-rw-rw-   0        0        0       40 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.396089 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/
--rw-rw-rw-   0        0        0        0 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/__init__.py
--rw-rw-rw-   0        0        0     7515 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/cable_n_connectors.xlsx
--rw-rw-rw-   0        0        0     5963 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/formitems.py
--rw-rw-rw-   0        0        0     3905 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/gui_template.py
--rw-rw-rw-   0        0        0     3978 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/tab_event_funcs.py
--rw-rw-rw-   0        0        0     4667 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_event_funcs.py
--rw-rw-rw-   0        0        0     1077 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_event_updators.py
--rw-rw-rw-   0        0        0     2666 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_frames.py
--rw-rw-rw-   0        0        0     1819 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_retractables.py
--rw-rw-rw-   0        0        0     4408 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit/gui.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.396089 nettoolkit-1.6.1/nettoolkit/nettoolkit_common/
--rw-rw-rw-   0        0        0     1219 2024-03-21 05:10:21.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit_common/__init__.py
--rw-rw-rw-   0        0        0     7448 2024-03-21 05:13:13.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit_common/common.py
--rw-rw-rw-   0        0        0    49599 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit_common/gpl.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.396089 nettoolkit-1.6.1/nettoolkit/nettoolkit_db/
--rw-rw-rw-   0        0        0      443 2024-03-21 06:29:10.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit_db/__init__.py
--rw-rw-rw-   0        0        0     7754 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit_db/convertdict.py
--rw-rw-rw-   0        0        0     7044 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/nettoolkit_db/database.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.407966 nettoolkit-1.6.1/nettoolkit/pyJuniper/
--rw-rw-rw-   0        0        0      257 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.407966 nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/
--rw-rw-rw-   0        0        0        0 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/__init__.py
--rw-rw-rw-   0        0        0     2466 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/juniper_oper.py
--rw-rw-rw-   0        0        0     1582 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/md5_calculator.py
--rw-rw-rw-   0        0        0     5108 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/pw_enc_dec.py
--rw-rw-rw-   0        0        0    17243 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/hierarchy.py
--rw-rw-rw-   0        0        0     3917 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/hierarchy_rules.py
--rw-rw-rw-   0        0        0     4426 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/jset.py
--rw-rw-rw-   0        0        0     3219 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyJuniper/juniper.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.415970 nettoolkit-1.6.1/nettoolkit/pyNetCrypt/
--rw-rw-rw-   0        0        0      596 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/pyNetCrypt/__init__.py
--rw-rw-rw-   0        0        0     2664 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyNetCrypt/cpw_cracker.py
--rw-rw-rw-   0        0        0      428 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/pyNetCrypt/generate.py
--rw-rw-rw-   0        0        0     4708 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyNetCrypt/jpw_cracker.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.426079 nettoolkit-1.6.1/nettoolkit/pyVig/
--rw-rw-rw-   0        0        0     1071 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/__init__.py
--rw-rw-rw-   0        0        0     2957 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/cablings.py
--rw-rw-rw-   0        0        0      488 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/common.py
--rw-rw-rw-   0        0        0     7228 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/database.py
--rw-rw-rw-   0        0        0     4032 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/devices.py
--rw-rw-rw-   0        0        0     6687 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/entities.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.426079 nettoolkit-1.6.1/nettoolkit/pyVig/forms/
--rw-rw-rw-   0        0        0        0 2024-01-15 11:31:59.000000 nettoolkit-1.6.1/nettoolkit/pyVig/forms/__init__.py
--rw-rw-rw-   0        0        0     2170 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/forms/custom.py
--rw-rw-rw-   0        0        0     8515 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/forms/input_data.py
--rw-rw-rw-   0        0        0    10036 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/general.py
--rw-rw-rw-   0        0        0    10727 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/maths.py
--rw-rw-rw-   0        0        0    21584 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/oper.py
--rw-rw-rw-   0        0        0     5301 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/pyVig.py
--rw-rw-rw-   0        0        0     1685 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/static.py
--rw-rw-rw-   0        0        0     2072 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/stencils.py
--rw-rw-rw-   0        0        0    20566 2024-03-21 04:49:46.000000 nettoolkit-1.6.1/nettoolkit/pyVig/visio.py
-drwxrwxrwx   0        0        0        0 2024-03-21 06:31:34.426079 nettoolkit-1.6.1/nettoolkit.egg-info/
--rw-rw-rw-   0        0        0      713 2024-03-21 06:31:34.000000 nettoolkit-1.6.1/nettoolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7402 2024-03-21 06:31:34.000000 nettoolkit-1.6.1/nettoolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 06:31:34.000000 nettoolkit-1.6.1/nettoolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-03-21 06:31:34.000000 nettoolkit-1.6.1/nettoolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-21 06:31:34.000000 nettoolkit-1.6.1/nettoolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 06:31:34.435946 nettoolkit-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0      926 2024-03-21 06:28:48.000000 nettoolkit-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.461722 nettoolkit-1.6.2/
+-rw-rw-rw-   0        0        0     1091 2023-03-27 08:31:48.000000 nettoolkit-1.6.2/LICENSE
+-rw-rw-rw-   0        0        0      713 2024-05-25 02:50:32.461722 nettoolkit-1.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-10-18 01:47:58.000000 nettoolkit-1.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.308214 nettoolkit-1.6.2/nettoolkit/
+-rw-rw-rw-   0        0        0     2907 2024-05-25 02:45:19.000000 nettoolkit-1.6.2/nettoolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.320716 nettoolkit-1.6.2/nettoolkit/addressing/
+-rw-rw-rw-   0        0        0       78 2024-05-08 10:36:40.000000 nettoolkit-1.6.2/nettoolkit/addressing/__init__.py
+-rw-rw-rw-   0        0        0    51806 2024-05-25 02:45:08.000000 nettoolkit-1.6.2/nettoolkit/addressing/addressing.py
+-rw-rw-rw-   0        0        0     3400 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/batch.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.320716 nettoolkit-1.6.2/nettoolkit/addressing/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/forms/__init__.py
+-rw-rw-rw-   0        0        0     1476 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/forms/compare_scanner_outputs.py
+-rw-rw-rw-   0        0        0     2760 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/forms/create_batch.py
+-rw-rw-rw-   0        0        0     4566 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/forms/prefixes_oper.py
+-rw-rw-rw-   0        0        0     3092 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/forms/subnet_scanner.py
+-rw-rw-rw-   0        0        0     4951 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/addressing/subnetscan.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.336343 nettoolkit-1.6.2/nettoolkit/capture_it/
+-rw-rw-rw-   0        0        0      290 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/__init__.py
+-rw-rw-rw-   0        0        0     2200 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/_detection.py
+-rw-rw-rw-   0        0        0     9542 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/cap_summary.py
+-rw-rw-rw-   0        0        0     3242 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/captures.py
+-rw-rw-rw-   0        0        0     3758 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/clp.py
+-rw-rw-rw-   0        0        0     4104 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/command.py
+-rw-rw-rw-   0        0        0      667 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/common.py
+-rw-rw-rw-   0        0        0     9080 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/configure.py
+-rw-rw-rw-   0        0        0     5494 2024-05-24 04:02:29.000000 nettoolkit-1.6.2/nettoolkit/capture_it/conn.py
+-rw-rw-rw-   0        0        0     9686 2024-05-24 04:07:15.000000 nettoolkit-1.6.2/nettoolkit/capture_it/exec_device.py
+-rw-rw-rw-   0        0        0    17079 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/executions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.336343 nettoolkit-1.6.2/nettoolkit/capture_it/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/forms/__init__.py
+-rw-rw-rw-   0        0        0     5532 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/forms/common_to_all.py
+-rw-rw-rw-   0        0        0     1589 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/forms/cred.py
+-rw-rw-rw-   0        0        0     2548 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/forms/custom.py
+-rw-rw-rw-   0        0        0     1855 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/forms/options.py
+-rw-rw-rw-   0        0        0     1939 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/capture_it/forms/quick_show.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.336343 nettoolkit-1.6.2/nettoolkit/compare_it/
+-rw-rw-rw-   0        0        0      200 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/compare_it/__init__.py
+-rw-rw-rw-   0        0        0    12342 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/compare_it/diff.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.336343 nettoolkit-1.6.2/nettoolkit/compare_it/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/compare_it/forms/__init__.py
+-rw-rw-rw-   0        0        0     5204 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/compare_it/forms/compare_configs.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.336343 nettoolkit-1.6.2/nettoolkit/detect/
+-rw-rw-rw-   0        0        0       81 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     2630 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/detect/detection.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.351966 nettoolkit-1.6.2/nettoolkit/facts_finder/
+-rw-rw-rw-   0        0        0      530 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/__init__.py
+-rw-rw-rw-   0        0        0     6182 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/clean.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.351966 nettoolkit-1.6.2/nettoolkit/facts_finder/commons/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/commons/__init__.py
+-rw-rw-rw-   0        0        0     1151 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/commons/common.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.351966 nettoolkit-1.6.2/nettoolkit/facts_finder/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/forms/__init__.py
+-rw-rw-rw-   0        0        0     3809 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/forms/ff_custom.py
+-rw-rw-rw-   0        0        0     4048 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/forms/ff_custom_cit.py
+-rw-rw-rw-   0        0        0     3238 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/forms/ff_generate.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.351966 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/
+-rw-rw-rw-   0        0        0      324 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.367591 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/
+-rw-rw-rw-   0        0        0      888 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_arp_table.py
+-rw-rw-rw-   0        0        0     6452 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_bgp.py
+-rw-rw-rw-   0        0        0     2302 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_cdp.py
+-rw-rw-rw-   0        0        0     1697 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_description.py
+-rw-rw-rw-   0        0        0     2018 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_status.py
+-rw-rw-rw-   0        0        0     1976 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_lldp.py
+-rw-rw-rw-   0        0        0     1500 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_mac_table.py
+-rw-rw-rw-   0        0        0     5143 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_ospf.py
+-rw-rw-rw-   0        0        0    10147 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py
+-rw-rw-rw-   0        0        0     3024 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_prefix_list.py
+-rw-rw-rw-   0        0        0     5591 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_routes.py
+-rw-rw-rw-   0        0        0     5332 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_system.py
+-rw-rw-rw-   0        0        0     4386 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py
+-rw-rw-rw-   0        0        0     1374 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_version.py
+-rw-rw-rw-   0        0        0     4746 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/common.py
+-rw-rw-rw-   0        0        0     7509 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.367591 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/commons/
+-rw-rw-rw-   0        0        0      125 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/commons/__init__.py
+-rw-rw-rw-   0        0        0     2061 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/commons/generator_commons.py
+-rw-rw-rw-   0        0        0      250 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/device.py
+-rw-rw-rw-   0        0        0     4506 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/facts_gen.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.383214 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/
+-rw-rw-rw-   0        0        0      845 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/__init__.py
+-rw-rw-rw-   0        0        0     2277 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_arp_table.py
+-rw-rw-rw-   0        0        0     2924 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py
+-rw-rw-rw-   0        0        0     1467 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_int_description.py
+-rw-rw-rw-   0        0        0     2030 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_lldp.py
+-rw-rw-rw-   0        0        0      890 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running.py
+-rw-rw-rw-   0        0        0     7219 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_bgp.py
+-rw-rw-rw-   0        0        0    16908 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py
+-rw-rw-rw-   0        0        0     5898 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_ospf.py
+-rw-rw-rw-   0        0        0     3195 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_prefix_lists.py
+-rw-rw-rw-   0        0        0     4318 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routes.py
+-rw-rw-rw-   0        0        0     3447 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py
+-rw-rw-rw-   0        0        0     8424 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_system.py
+-rw-rw-rw-   0        0        0     1101 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_version.py
+-rw-rw-rw-   0        0        0     1482 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/common.py
+-rw-rw-rw-   0        0        0     6363 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper_parser.py
+-rw-rw-rw-   0        0        0     3534 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/generators/merger.py
+-rw-rw-rw-   0        0        0     6888 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/inputlog.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.398216 nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/
+-rw-rw-rw-   0        0        0      199 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/__init__.py
+-rw-rw-rw-   0        0        0     1684 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/cisco.py
+-rw-rw-rw-   0        0        0     6025 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/common.py
+-rw-rw-rw-   0        0        0     2558 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/juniper.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.399224 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/
+-rw-rw-rw-   0        0        0      139 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.399224 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/
+-rw-rw-rw-   0        0        0      345 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/__init__.py
+-rw-rw-rw-   0        0        0     7992 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/cisco_tables.py
+-rw-rw-rw-   0        0        0     1734 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/cisco_var.py
+-rw-rw-rw-   0        0        0     1465 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/cisco_vrfs.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.399224 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/commands/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/commands/__init__.py
+-rw-rw-rw-   0        0        0     3407 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/commands/cmd_dict.py
+-rw-rw-rw-   0        0        0     3019 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/merger.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.399224 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/commons/
+-rw-rw-rw-   0        0        0      303 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/commons/__init__.py
+-rw-rw-rw-   0        0        0     8515 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/commons/modifier_commons.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.399224 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/
+-rw-rw-rw-   0        0        0      303 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.399224 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/commands/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/commands/__init__.py
+-rw-rw-rw-   0        0        0     1334 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/commands/cmd_dict.py
+-rw-rw-rw-   0        0        0     2345 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/juniper_tables.py
+-rw-rw-rw-   0        0        0     1068 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/juniper_var.py
+-rw-rw-rw-   0        0        0     2197 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/merger.py
+-rw-rw-rw-   0        0        0     5164 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/facts_finder/rearrange.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.414850 nettoolkit-1.6.2/nettoolkit/j2config/
+-rw-rw-rw-   0        0        0      314 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.414850 nettoolkit-1.6.2/nettoolkit/j2config/cmn/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/cmn/__init__.py
+-rw-rw-rw-   0        0        0     6726 2024-05-22 02:39:47.000000 nettoolkit-1.6.2/nettoolkit/j2config/cmn/common_fn.py
+-rw-rw-rw-   0        0        0     5140 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/data_collect.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.414850 nettoolkit-1.6.2/nettoolkit/j2config/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/forms/__init__.py
+-rw-rw-rw-   0        0        0     6421 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/forms/input_data.py
+-rw-rw-rw-   0        0        0     9427 2024-05-16 06:37:57.000000 nettoolkit-1.6.2/nettoolkit/j2config/func.py
+-rw-rw-rw-   0        0        0      617 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/general.py
+-rw-rw-rw-   0        0        0     4235 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/j2.py
+-rw-rw-rw-   0        0        0     1518 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/j2config/read_conditions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.414850 nettoolkit-1.6.2/nettoolkit/log/
+-rw-rw-rw-   0        0        0        4 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/log/__init__.py
+-rw-rw-rw-   0        0        0      907 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/log/log_executions.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.414850 nettoolkit-1.6.2/nettoolkit/nettoolkit/
+-rw-rw-rw-   0        0        0       40 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.430473 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/__init__.py
+-rw-rw-rw-   0        0        0     7514 2024-04-30 04:07:40.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/cable_n_connectors.xlsx
+-rw-rw-rw-   0        0        0     5963 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/formitems.py
+-rw-rw-rw-   0        0        0     3905 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/gui_template.py
+-rw-rw-rw-   0        0        0     3978 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/tab_event_funcs.py
+-rw-rw-rw-   0        0        0     4667 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_event_funcs.py
+-rw-rw-rw-   0        0        0     1077 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_event_updators.py
+-rw-rw-rw-   0        0        0     2666 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_frames.py
+-rw-rw-rw-   0        0        0     1819 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_retractables.py
+-rw-rw-rw-   0        0        0     4408 2024-03-21 04:56:55.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit/gui.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.430473 nettoolkit-1.6.2/nettoolkit/nettoolkit_common/
+-rw-rw-rw-   0        0        0     1219 2024-03-21 05:10:36.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit_common/__init__.py
+-rw-rw-rw-   0        0        0     7448 2024-03-21 05:10:52.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit_common/common.py
+-rw-rw-rw-   0        0        0    49599 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit_common/gpl.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.430473 nettoolkit-1.6.2/nettoolkit/nettoolkit_db/
+-rw-rw-rw-   0        0        0      443 2024-05-25 02:40:23.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit_db/__init__.py
+-rw-rw-rw-   0        0        0     7754 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit_db/convertdict.py
+-rw-rw-rw-   0        0        0     7044 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/nettoolkit_db/database.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.430473 nettoolkit-1.6.2/nettoolkit/pyJuniper/
+-rw-rw-rw-   0        0        0      257 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.430473 nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/__init__.py
+-rw-rw-rw-   0        0        0     2466 2024-04-25 06:18:02.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/juniper_oper.py
+-rw-rw-rw-   0        0        0     1582 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/md5_calculator.py
+-rw-rw-rw-   0        0        0     5108 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/pw_enc_dec.py
+-rw-rw-rw-   0        0        0    17243 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/hierarchy.py
+-rw-rw-rw-   0        0        0     3917 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/hierarchy_rules.py
+-rw-rw-rw-   0        0        0     4426 2024-04-25 06:18:13.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/jset.py
+-rw-rw-rw-   0        0        0     3219 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyJuniper/juniper.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.446103 nettoolkit-1.6.2/nettoolkit/pyNetCrypt/
+-rw-rw-rw-   0        0        0      596 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyNetCrypt/__init__.py
+-rw-rw-rw-   0        0        0     2664 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyNetCrypt/cpw_cracker.py
+-rw-rw-rw-   0        0        0      428 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyNetCrypt/generate.py
+-rw-rw-rw-   0        0        0     4708 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyNetCrypt/jpw_cracker.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.446103 nettoolkit-1.6.2/nettoolkit/pyVig/
+-rw-rw-rw-   0        0        0     1084 2024-03-24 04:35:44.000000 nettoolkit-1.6.2/nettoolkit/pyVig/__init__.py
+-rw-rw-rw-   0        0        0     2957 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/cablings.py
+-rw-rw-rw-   0        0        0      488 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/common.py
+-rw-rw-rw-   0        0        0     7228 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/database.py
+-rw-rw-rw-   0        0        0     4032 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/devices.py
+-rw-rw-rw-   0        0        0     6687 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/entities.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.446103 nettoolkit-1.6.2/nettoolkit/pyVig/forms/
+-rw-rw-rw-   0        0        0        0 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/forms/__init__.py
+-rw-rw-rw-   0        0        0     2170 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/forms/custom.py
+-rw-rw-rw-   0        0        0     8515 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/forms/input_data.py
+-rw-rw-rw-   0        0        0    10036 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/general.py
+-rw-rw-rw-   0        0        0    10727 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/maths.py
+-rw-rw-rw-   0        0        0    21626 2024-03-24 05:04:41.000000 nettoolkit-1.6.2/nettoolkit/pyVig/oper.py
+-rw-rw-rw-   0        0        0     5301 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/pyVig.py
+-rw-rw-rw-   0        0        0     1685 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/static.py
+-rw-rw-rw-   0        0        0     2072 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/stencils.py
+-rw-rw-rw-   0        0        0    20566 2024-03-21 04:56:56.000000 nettoolkit-1.6.2/nettoolkit/pyVig/visio.py
+drwxrwxrwx   0        0        0        0 2024-05-25 02:50:32.461722 nettoolkit-1.6.2/nettoolkit.egg-info/
+-rw-rw-rw-   0        0        0      713 2024-05-25 02:50:32.000000 nettoolkit-1.6.2/nettoolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7402 2024-05-25 02:50:32.000000 nettoolkit-1.6.2/nettoolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 02:50:32.000000 nettoolkit-1.6.2/nettoolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-25 02:50:32.000000 nettoolkit-1.6.2/nettoolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 02:50:32.000000 nettoolkit-1.6.2/nettoolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 02:50:32.461722 nettoolkit-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      926 2024-03-25 07:00:04.000000 nettoolkit-1.6.2/setup.py
```

### Comparing `nettoolkit-1.6.1/LICENSE` & `nettoolkit-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/PKG-INFO` & `nettoolkit-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettoolkit
-Version: 1.6.1
+Version: 1.6.2
 Summary: Tool Set for Networking Geeks
 Home-page: https://github.com/alias1978/nettoolkit
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nettoolkit-1.6.1/nettoolkit/__init__.py` & `nettoolkit-1.6.2/nettoolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __doc__ = '''Networking Tool Set'''
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 
 def version():
 	return __version__
 
 ## --- IMPORTS --- ##
```

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/addressing.py` & `nettoolkit-1.6.2/nettoolkit/addressing/addressing.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,14 +395,39 @@
 			nset.add(subnet.expand(min_subnet_size))
 		elif isinstance(subnet, str) and int(subnet.split("/")[-1]) > min_subnet_size:
 			nset.add(IPv4(subnet).expand(min_subnet_size))
 	summaries.extend(nset)
 	nSummaries = get_summaries(*set(summaries))
 	return nSummaries
 
+def break_prefix(pfx, mask_size):
+	"""downsize larger prefix size to smaller size
+
+	Args:
+		pfx (str): prefix/subnet
+		mask_size (int): required mask size numeric
+
+	Raises:
+		Exception: InputError: Invalid Prefix
+		Exception: InputError: Invalid mask_size
+
+	Returns:
+		str: broken prefix
+	"""    	
+	try:
+		s = IPv4(pfx)
+	except:
+		raise Exception(f"InputError: Invalid Prefix {pfx}")
+	try:
+		bit_length = 2**(32-mask_size)
+	except:
+		raise Exception(f"InputError: Invalid mask_size {mask_size}")
+	d = s.size/bit_length
+	return s/d
+
 def recapsulate(subnet, size):
 	"""capsulate provided subnet (str, IPv4) with given sizing.
 
 	Args:
 		subnet (str, IPv4): string or IPv4 Object
 		size (int): subnet mask, for sizing
 
@@ -1148,14 +1173,25 @@
 		Returns:
 			int: ip number
 		"""		
 		if isinstance(ip, str):
 			child = addressing(ip)
 		return child.to_decimal() - self.to_decimal()
 
+	def get_octet(self, o):
+		"""get the desired octet for subnet
+
+		Args:
+			o (int): octet number
+
+		Returns:
+			str: octet number
+		"""    		
+		return ipv4_octets(self)['octets'][o-1]
+
 
 # ------------------------------------------------------------------------------
 # Routes Class
 # ------------------------------------------------------------------------------
 class Routes(object):
 	"""Routes Object
 	Either one input is require (route_list, route_file)
```

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/batch.py` & `nettoolkit-1.6.2/nettoolkit/addressing/batch.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/forms/compare_scanner_outputs.py` & `nettoolkit-1.6.2/nettoolkit/addressing/forms/compare_scanner_outputs.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/forms/create_batch.py` & `nettoolkit-1.6.2/nettoolkit/addressing/forms/create_batch.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/forms/prefixes_oper.py` & `nettoolkit-1.6.2/nettoolkit/addressing/forms/prefixes_oper.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/forms/subnet_scanner.py` & `nettoolkit-1.6.2/nettoolkit/addressing/forms/subnet_scanner.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/addressing/subnetscan.py` & `nettoolkit-1.6.2/nettoolkit/addressing/subnetscan.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/_detection.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/_detection.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/cap_summary.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/cap_summary.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/captures.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/captures.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/clp.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/clp.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/command.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/command.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/common.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/common.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/configure.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/configure.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/conn.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/conn.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/exec_device.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/exec_device.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/executions.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/executions.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/forms/common_to_all.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/forms/common_to_all.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/forms/cred.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/forms/cred.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/forms/custom.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/forms/custom.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/forms/options.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/forms/options.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/capture_it/forms/quick_show.py` & `nettoolkit-1.6.2/nettoolkit/capture_it/forms/quick_show.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/compare_it/diff.py` & `nettoolkit-1.6.2/nettoolkit/compare_it/diff.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/compare_it/forms/compare_configs.py` & `nettoolkit-1.6.2/nettoolkit/compare_it/forms/compare_configs.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/detect/detection.py` & `nettoolkit-1.6.2/nettoolkit/detect/detection.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/__init__.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/__init__.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/clean.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/clean.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/commons/common.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/commons/common.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/forms/ff_custom.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/forms/ff_custom.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/forms/ff_custom_cit.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/forms/ff_custom_cit.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/forms/ff_generate.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/forms/ff_generate.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/__init__.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/__init__.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_arp_table.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_arp_table.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_bgp.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_bgp.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_cdp.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_cdp.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_description.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_description.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_status.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_int_status.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_lldp.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_lldp.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_mac_table.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_mac_table.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_ospf.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_ospf.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_interfaces.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_prefix_list.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_prefix_list.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_routes.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_routes.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_system.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_system.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_running_vrfs.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/_cmd_parse_version.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/_cmd_parse_version.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco/common.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco/common.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/cisco_parser.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/cisco_parser.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/commons/generator_commons.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/commons/generator_commons.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/facts_gen.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/facts_gen.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/__init__.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/__init__.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_arp_table.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_arp_table.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_chassis_hardware.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_int_description.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_int_description.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_lldp.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_lldp.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_bgp.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_bgp.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_interfaces.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_ospf.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_ospf.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_prefix_lists.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_prefix_lists.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routes.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routes.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_routing_instances.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_system.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_running_system.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/_cmd_parse_version.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/_cmd_parse_version.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper/common.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper/common.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/juniper_parser.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/juniper_parser.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/generators/merger.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/generators/merger.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/inputlog.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/inputlog.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/cisco.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/cisco.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/common.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/common.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/mergers/juniper.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/mergers/juniper.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/cisco_tables.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/cisco_tables.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/cisco_var.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/cisco_var.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/cisco_vrfs.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/cisco_vrfs.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/commands/cmd_dict.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/commands/cmd_dict.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/cisco/merger.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/cisco/merger.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/commons/modifier_commons.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/commons/modifier_commons.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/commands/cmd_dict.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/commands/cmd_dict.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/juniper_tables.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/juniper_tables.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/juniper_var.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/juniper_var.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/modifiers/juniper/merger.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/modifiers/juniper/merger.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/facts_finder/rearrange.py` & `nettoolkit-1.6.2/nettoolkit/facts_finder/rearrange.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/cmn/common_fn.py` & `nettoolkit-1.6.2/nettoolkit/j2config/cmn/common_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,8 +409,13 @@
 00001980: 0922 2222 090d 0a09 6966 206e 6f74 2061  ."""....if not a
 00001990: 736e 3a20 7265 7475 726e 2022 220d 0a09  sn: return ""...
 000019a0: 6173 6e20 3d20 6173 6e2e 7374 7269 7028  asn = asn.strip(
 000019b0: 2920 2b20 2220 220d 0a09 6173 705f 7072  ) + " "...asp_pr
 000019c0: 6570 5f73 7472 696e 6720 3d20 6173 6e2a  ep_string = asn*
 000019d0: 7469 6d65 730d 0a09 7265 7475 726e 2061  times...return a
 000019e0: 7370 5f70 7265 705f 7374 7269 6e67 2e73  sp_prep_string.s
-000019f0: 7472 6970 2829 0d0a                      trip()..
+000019f0: 7472 6970 2829 0d0a 0d0a 6465 6620 7374  trip()....def st
+00001a00: 7269 6e67 2873 293a 0d0a 0972 6574 7572  ring(s):...retur
+00001a10: 6e20 7374 7228 7329 202b 2022 2022 0d0a  n str(s) + " "..
+00001a20: 0d0a 6465 6620 7374 7269 6e67 5f61 735f  ..def string_as_
+00001a30: 6973 2873 293a 0d0a 0972 6574 7572 6e20  is(s):...return 
+00001a40: 7374 7228 7329                           str(s)
```

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/data_collect.py` & `nettoolkit-1.6.2/nettoolkit/j2config/data_collect.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/forms/input_data.py` & `nettoolkit-1.6.2/nettoolkit/j2config/forms/input_data.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/func.py` & `nettoolkit-1.6.2/nettoolkit/j2config/func.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/general.py` & `nettoolkit-1.6.2/nettoolkit/j2config/general.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/j2.py` & `nettoolkit-1.6.2/nettoolkit/j2config/j2.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/j2config/read_conditions.py` & `nettoolkit-1.6.2/nettoolkit/j2config/read_conditions.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/log/log_executions.py` & `nettoolkit-1.6.2/nettoolkit/log/log_executions.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/cable_n_connectors.xlsx` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/cable_n_connectors.xlsx`

 * *Files 6% similar despite different names*

```diff
@@ -375,96 +375,96 @@
 00001760: e917 346e 2a7c b69c 6f07 7c1f a28f 1613  ..4n*|..o.|.....
 00001770: 2582 44bc d02a ca6f b139 049d 5b9a 7129  %.D..*.o.9..[.q)
 00001780: ab7f 778c 5a86 a055 11ef f31c 3e35 6737  ..w.Z..U....>5g7
 00001790: 2a9c 7dba b8d7 77b6 67f0 b577 baab edd5  *.}...w.g..w....
 000017a0: 12b5 b583 4cb6 5af9 e389 0fef 81ec 1d38  ....L.Z........8
 000017b0: 284d 9992 f9db a4fb 70d4 ecce ff32 003e  (M......p....2.>
 000017c0: f692 74eb 1f50 4b03 0414 0000 0008 0000  ..t..PK.........
-000017d0: 003f 001f 4943 a028 0100 0051 0200 0011  .?..IC.(...Q....
+000017d0: 003f 0052 a5df e527 0100 0051 0200 0011  .?.R...'...Q....
 000017e0: 0000 0064 6f63 5072 6f70 732f 636f 7265  ...docProps/core
 000017f0: 2e78 6d6c 9d92 5f4b c330 14c5 df05 bf43  .xml.._K.0.....C
-00001800: c97b 9bb4 9b53 42db 81ca 9e1c 084e 14df  .{...SB......N..
-00001810: 4272 b705 9b3f 24d1 6edf deb4 ddba 0df6  Br...?$.n.......
-00001820: e4e3 cd39 f777 cfbd a49c ef54 93fc 82f3  ...9.w.....T....
-00001830: d2e8 0ae5 1941 0968 6e84 d49b 0abd af16  .....A.hn.......
-00001840: e903 4a7c 605a b0c6 68a8 d01e 3c9a d7b7  ..J|`Z..h...<...
-00001850: 3725 b794 1b07 afce 5870 4182 4f22 497b  7%......XpA.O"I{
-00001860: ca6d 85b6 2158 8ab1 e75b 50cc 67d1 a1a3  .m..!X...[P.g...
-00001870: b836 4eb1 104b b7c1 96f1 6fb6 015c 1032  .6N..K....o..\.2
-00001880: c30a 0213 2c30 dc01 533b 12d1 0129 f888  ....,0..S;...)..
-00001890: b43f aee9 0182 6368 4081 0e1e e759 8e4f  .?....ch@....Y.O
-000018a0: de00 4ef9 ab0d bd72 e654 32ec 2d5c b51e  ..N....r.T2.-\..
-000018b0: c5d1 bdf3 7234 b66d 9bb5 93de 1af3 e7f8  ....r4.m........
-000018c0: 73f9 f2d6 af9a 4add dd8a 03aa 4bc1 2977  s.....J.....K.)w
-000018d0: c082 7175 89cf 8b78 b886 f9b0 8c37 5e4b  ..qu...x.....7^K
-000018e0: 108f fba8 5f79 3b2c 32f4 8148 6200 3ac4  ...._y;,2..Hb.:.
-000018f0: 3d2a 1f93 a7e7 d502 d505 29a6 29c9 d3fc  =*........).)...
-00001900: 7e45 6674 3aa3 77e4 ab1b 79d1 7f02 aac3  ~Eft:.w...y.....
-00001910: 907f 138f 8021 f7e5 27a8 ff00 504b 0304  .....!..'...PK..
-00001920: 1400 0000 0800 0000 3f00 2738 8bc4 7b01  ........?.'8..{.
-00001930: 0000 1103 0000 1000 0000 646f 6350 726f  ..........docPro
-00001940: 7073 2f61 7070 2e78 6d6c 9d92 416b e330  ps/app.xml..Ak.0
-00001950: 1085 ef85 fd0f 46f7 4476 5896 1264 9592  ......F.DvX..d..
-00001960: ecd2 c396 0692 b667 551e c7a2 b224 3453  .......gU....$4S
-00001970: 93f4 d757 7688 ebb4 7b5a 9fde cc3c 9e3e  ...Wv...{Z...<.>
-00001980: 8f24 6e0e adcd 3a88 68bc 2b59 31cf 5906  .$n...:.h.+Y1.Y.
-00001990: 4efb cab8 7dc9 1e77 7f66 d72c 4352 ae52  N...}..w.f.,CR.R
-000019a0: d63b 28d9 1190 ddc8 1f57 6213 7d80 4806  .;(......Wb.}.H.
-000019b0: 304b 110e 4bd6 1085 25e7 a81b 6815 ced3  0K..K...%...h...
-000019c0: d8a5 49ed 63ab 2895 71cf 7d5d 1b0d 6baf  ..I.c.(.q.}]..k.
-000019d0: df5a 70c4 1779 fe8b c381 c055 50cd c218  .Zp..y.....UP...
-000019e0: c84e 89cb 8efe 37b4 f2ba e7c3 a7dd 31a4  .N....7.......1.
-000019f0: 3c29 6e43 b046 2b4a 7f29 ef8d 8e1e 7d4d  <)nC.F+J.)....}M
-00001a00: d9ef 8306 2bf8 7428 52d0 16f4 5b34 7494  ....+.t(R...[4t.
-00001a10: b9e0 d352 6cb5 b2b0 4ac1 b256 1641 f0cf  ...Rl...J..V.A..
-00001a20: 86b8 03d5 2f6d a34c 4429 3a5a 76a0 c9c7  ..../m.LD):Zv...
-00001a30: 0ccd 7b5a db82 652f 0aa1 c729 59a7 a251  ..{Z..e/...)Y..Q
-00001a40: 8ed8 c976 2a06 6d03 5294 cf3e be62 0340  ...v*.m.R..>.b.@
-00001a50: 28f8 d81c e4d4 3bd5 e6a7 2c06 4312 9746  (.....;...,.C..F
-00001a60: 3e82 247d 89b8 3364 011f ea8d 8af4 0fe2  >.$}..3d........
-00001a70: 624a 3c30 b009 e3b6 e72b bef1 9d4f fa92  bJ<0.....+...O..
-00001a80: bdf2 6d50 2e2d 908f eaaf 71af f818 767e  ..mP.-....q...v~
-00001a90: ad08 ceeb bc6c 8a6d a322 54e9 06c6 758f  .....l.m."T...u.
-00001aa0: 0d71 97b8 a2ed fdab 46b9 3d54 67cf f741  .q......F.=Tg..A
-00001ab0: 7ff9 4fa7 172e 8bc5 3c4f df70 e7e7 9ee0  ..O.....<O.p....
-00001ac0: 9f6f 597e 0050 4b01 0214 0014 0000 0008  .oY~.PK.........
-00001ad0: 0000 003f 00f8 4aa7 2151 0100 0090 0400  ...?..J.!Q......
-00001ae0: 0013 0000 0000 0000 0000 0000 00b6 8100  ................
-00001af0: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
-00001b00: 735d 2e78 6d6c 504b 0102 1400 1400 0000  s].xmlPK........
-00001b10: 0800 0000 3f00 507c 4ec1 ea00 0000 4c02  ....?.P|N.....L.
-00001b20: 0000 0b00 0000 0000 0000 0000 0000 b681  ................
-00001b30: 8201 0000 5f72 656c 732f 2e72 656c 7350  ...._rels/.relsP
-00001b40: 4b01 0214 0014 0000 0008 0000 003f 0087  K............?..
-00001b50: e085 69ea 0000 00ba 0200 001a 0000 0000  ..i.............
-00001b60: 0000 0000 0000 00b6 8195 0200 0078 6c2f  .............xl/
-00001b70: 5f72 656c 732f 776f 726b 626f 6f6b 2e78  _rels/workbook.x
-00001b80: 6d6c 2e72 656c 7350 4b01 0214 0014 0000  ml.relsPK.......
-00001b90: 0008 0000 003f 005b c982 8b67 0700 0034  .....?.[...g...4
-00001ba0: 3800 0018 0000 0000 0000 0000 0000 00b6  8...............
-00001bb0: 81b7 0300 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00001bc0: 7473 2f73 6865 6574 312e 786d 6c50 4b01  ts/sheet1.xmlPK.
-00001bd0: 0214 0014 0000 0008 0000 003f 0052 cce8  ...........?.R..
-00001be0: ef4b 0100 0027 0200 000f 0000 0000 0000  .K...'..........
-00001bf0: 0000 0000 00b6 8154 0b00 0078 6c2f 776f  .......T...xl/wo
-00001c00: 726b 626f 6f6b 2e78 6d6c 504b 0102 1400  rkbook.xmlPK....
-00001c10: 1400 0000 0800 0000 3f00 aaf1 c163 bc02  ........?....c..
-00001c20: 0000 100e 0000 1400 0000 0000 0000 0000  ................
-00001c30: 0000 b681 cc0c 0000 786c 2f73 6861 7265  ........xl/share
-00001c40: 6453 7472 696e 6773 2e78 6d6c 504b 0102  dStrings.xmlPK..
-00001c50: 1400 1400 0000 0800 0000 3f00 7118 15ad  ..........?.q...
-00001c60: fd01 0000 3e05 0000 0d00 0000 0000 0000  ....>...........
-00001c70: 0000 0000 b681 ba0f 0000 786c 2f73 7479  ..........xl/sty
-00001c80: 6c65 732e 786d 6c50 4b01 0214 0014 0000  les.xmlPK.......
-00001c90: 0008 0000 003f 00e9 a625 b8b2 0500 0053  .....?...%.....S
-00001ca0: 1b00 0013 0000 0000 0000 0000 0000 00b6  ................
-00001cb0: 81e2 1100 0078 6c2f 7468 656d 652f 7468  .....xl/theme/th
-00001cc0: 656d 6531 2e78 6d6c 504b 0102 1400 1400  eme1.xmlPK......
-00001cd0: 0000 0800 0000 3f00 1f49 43a0 2801 0000  ......?..IC.(...
-00001ce0: 5102 0000 1100 0000 0000 0000 0000 0000  Q...............
-00001cf0: b681 c517 0000 646f 6350 726f 7073 2f63  ......docProps/c
-00001d00: 6f72 652e 786d 6c50 4b01 0214 0014 0000  ore.xmlPK.......
-00001d10: 0008 0000 003f 0027 388b c47b 0100 0011  .....?.'8..{....
-00001d20: 0300 0010 0000 0000 0000 0000 0000 00b6  ................
-00001d30: 811c 1900 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
-00001d40: 702e 786d 6c50 4b05 0600 0000 000a 000a  p.xmlPK.........
-00001d50: 0080 0200 00c5 1a00 0000 00              ...........
+00001800: c97b 9b74 2d2a a1ed 4065 4f0e 0427 8a6f  .{.t-*..@eO..'.o
+00001810: 21b9 db82 cd1f 9268 b76f 6fda 6edd 067b  !......h.oo.n..{
+00001820: f2f1 e69c fbbb e75e 52cd 77aa 4d7e c179  .......^R.w.M~.y
+00001830: 6974 8df2 8ca0 0434 3742 ea4d 8dde 578b  it.....47B.M..W.
+00001840: f401 253e 302d 586b 34d4 680f 1ecd 9bdb  ..%>0-Xk4.h.....
+00001850: 9b8a 5bca 8d83 5767 2cb8 20c1 2791 a43d  ..[...Wg,. .'..=
+00001860: e5b6 46db 102c c5d8 f32d 28e6 b3e8 d051  ..F..,...-(....Q
+00001870: 5c1b a758 88a5 db60 cbf8 37db 009e 1172  \..X...`..7....r
+00001880: 8715 0426 5860 b807 a676 22a2 0352 f009  ...&X`...v"..R..
+00001890: 697f 5c3b 0004 c7d0 8202 1d3c ceb3 1c9f  i.\;.......<....
+000018a0: bc01 9cf2 571b 06e5 cca9 64d8 5bb8 6a3d  ....W.....d.[.j=
+000018b0: 8a93 7be7 e564 ecba 2eeb 8ac1 1af3 e7f8  ..{..d..........
+000018c0: 73f9 f236 ac9a 4add df8a 036a 2ac1 2977  s..6..J....j*.)w
+000018d0: c082 714d 85cf 8b78 b896 f9b0 8c37 5e4b  ..qM...x.....7^K
+000018e0: 108f fba8 5f79 3b2c 32f6 8148 6200 3ac6  ...._y;,2..Hb.:.
+000018f0: 3d2a 1fc5 d3f3 6a81 9a19 9995 2929 d382  =*....j.....))..
+00001900: ac48 49c9 3d2d c957 3ff2 a2ff 0454 8721  .HI.=-.W?....T.!
+00001910: ff26 1e01 63ee cb4f d0fc 0150 4b03 0414  .&..c..O...PK...
+00001920: 0000 0008 0000 003f 0027 388b c47b 0100  .......?.'8..{..
+00001930: 0011 0300 0010 0000 0064 6f63 5072 6f70  .........docProp
+00001940: 732f 6170 702e 786d 6c9d 9241 6be3 3010  s/app.xml..Ak.0.
+00001950: 85ef 85fd 0f46 f744 7658 9612 6495 92ec  .....F.DvX..d...
+00001960: d2c3 9606 92b6 6755 1ec7 a2b2 2434 5393  ......gU....$4S.
+00001970: f4d7 5776 88eb b47b 5a9f decc 3c9e 3e8f  ..Wv...{Z...<.>.
+00001980: 246e 0ead cd3a 8868 bc2b 5931 cf59 064e  $n...:.h.+Y1.Y.N
+00001990: fbca b87d c91e 777f 66d7 2c43 52ae 52d6  ...}..w.f.,CR.R.
+000019a0: 3b28 d911 90dd c81f 5762 137d 8048 0630  ;(......Wb.}.H.0
+000019b0: 4b11 0e4b d610 8525 e7a8 1b68 15ce d3d8  K..K...%...h....
+000019c0: a549 ed63 ab28 9571 cf7d 5d1b 0d6b afdf  .I.c.(.q.}]..k..
+000019d0: 5a70 c417 79fe 8bc3 81c0 5550 cdc2 18c8  Zp..y.....UP....
+000019e0: 4e89 cb8e fe37 b4f2 bae7 c3a7 dd31 a43c  N....7.......1.<
+000019f0: 296e 43b0 462b 4a7f 29ef 8d8e 1e7d 4dd9  )nC.F+J.)....}M.
+00001a00: ef83 062b f874 2852 d016 f45b 3474 94b9  ...+.t(R...[4t..
+00001a10: e0d3 526c b5b2 b04a c1b2 5616 41f0 cf86  ..Rl...J..V.A...
+00001a20: b803 d52f 6da3 4c44 293a 5a76 a0c9 c70c  .../m.LD):Zv....
+00001a30: cd7b 5adb 8265 2f0a a1c7 2959 a7a2 518e  .{Z..e/...)Y..Q.
+00001a40: d8c9 762a 066d 0352 94cf 3ebe 6203 4028  ..v*.m.R..>.b.@(
+00001a50: f8d8 1ce4 d43b d5e6 a72c 0643 1297 463e  .....;...,.C..F>
+00001a60: 8224 7d89 b833 6401 1fea 8d8a f40f e262  .$}..3d........b
+00001a70: 4a3c 30b0 09e3 b6e7 2bbe f19d 4ffa 92bd  J<0.....+...O...
+00001a80: f26d 502e 2d90 8fea af71 aff8 1876 7ead  .mP.-....q...v~.
+00001a90: 08ce ebbc 6c8a 6da3 2254 e906 c675 8f0d  ....l.m."T...u..
+00001aa0: 7197 b8a2 edfd ab46 b93d 5467 cff7 417f  q......F.=Tg..A.
+00001ab0: f94f a717 2e8b c53c 4fdf 70e7 e79e e09f  .O.....<O.p.....
+00001ac0: 6f59 7e00 504b 0102 1400 1400 0000 0800  oY~.PK..........
+00001ad0: 0000 3f00 f84a a721 5101 0000 9004 0000  ..?..J.!Q.......
+00001ae0: 1300 0000 0000 0000 0000 0000 b681 0000  ................
+00001af0: 0000 5b43 6f6e 7465 6e74 5f54 7970 6573  ..[Content_Types
+00001b00: 5d2e 786d 6c50 4b01 0214 0014 0000 0008  ].xmlPK.........
+00001b10: 0000 003f 0050 7c4e c1ea 0000 004c 0200  ...?.P|N.....L..
+00001b20: 000b 0000 0000 0000 0000 0000 00b6 8182  ................
+00001b30: 0100 005f 7265 6c73 2f2e 7265 6c73 504b  ..._rels/.relsPK
+00001b40: 0102 1400 1400 0000 0800 0000 3f00 87e0  ............?...
+00001b50: 8569 ea00 0000 ba02 0000 1a00 0000 0000  .i..............
+00001b60: 0000 0000 0000 b681 9502 0000 786c 2f5f  ............xl/_
+00001b70: 7265 6c73 2f77 6f72 6b62 6f6f 6b2e 786d  rels/workbook.xm
+00001b80: 6c2e 7265 6c73 504b 0102 1400 1400 0000  l.relsPK........
+00001b90: 0800 0000 3f00 5bc9 828b 6707 0000 3438  ....?.[...g...48
+00001ba0: 0000 1800 0000 0000 0000 0000 0000 b681  ................
+00001bb0: b703 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00001bc0: 732f 7368 6565 7431 2e78 6d6c 504b 0102  s/sheet1.xmlPK..
+00001bd0: 1400 1400 0000 0800 0000 3f00 52cc e8ef  ..........?.R...
+00001be0: 4b01 0000 2702 0000 0f00 0000 0000 0000  K...'...........
+00001bf0: 0000 0000 b681 540b 0000 786c 2f77 6f72  ......T...xl/wor
+00001c00: 6b62 6f6f 6b2e 786d 6c50 4b01 0214 0014  kbook.xmlPK.....
+00001c10: 0000 0008 0000 003f 00aa f1c1 63bc 0200  .......?....c...
+00001c20: 0010 0e00 0014 0000 0000 0000 0000 0000  ................
+00001c30: 00b6 81cc 0c00 0078 6c2f 7368 6172 6564  .......xl/shared
+00001c40: 5374 7269 6e67 732e 786d 6c50 4b01 0214  Strings.xmlPK...
+00001c50: 0014 0000 0008 0000 003f 0071 1815 adfd  .........?.q....
+00001c60: 0100 003e 0500 000d 0000 0000 0000 0000  ...>............
+00001c70: 0000 00b6 81ba 0f00 0078 6c2f 7374 796c  .........xl/styl
+00001c80: 6573 2e78 6d6c 504b 0102 1400 1400 0000  es.xmlPK........
+00001c90: 0800 0000 3f00 e9a6 25b8 b205 0000 531b  ....?...%.....S.
+00001ca0: 0000 1300 0000 0000 0000 0000 0000 b681  ................
+00001cb0: e211 0000 786c 2f74 6865 6d65 2f74 6865  ....xl/theme/the
+00001cc0: 6d65 312e 786d 6c50 4b01 0214 0014 0000  me1.xmlPK.......
+00001cd0: 0008 0000 003f 0052 a5df e527 0100 0051  .....?.R...'...Q
+00001ce0: 0200 0011 0000 0000 0000 0000 0000 00b6  ................
+00001cf0: 81c5 1700 0064 6f63 5072 6f70 732f 636f  .....docProps/co
+00001d00: 7265 2e78 6d6c 504b 0102 1400 1400 0000  re.xmlPK........
+00001d10: 0800 0000 3f00 2738 8bc4 7b01 0000 1103  ....?.'8..{.....
+00001d20: 0000 1000 0000 0000 0000 0000 0000 b681  ................
+00001d30: 1b19 0000 646f 6350 726f 7073 2f61 7070  ....docProps/app
+00001d40: 2e78 6d6c 504b 0506 0000 0000 0a00 0a00  .xmlPK..........
+00001d50: 8002 0000 c41a 0000 0000                 ..........
```

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/formitems.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/formitems.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/gui_template.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/gui_template.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/tab_event_funcs.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/tab_event_funcs.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_event_funcs.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_event_funcs.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_event_updators.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_event_updators.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_frames.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_frames.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/forms/var_retractables.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/forms/var_retractables.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit/gui.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit/gui.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit_common/__init__.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit_common/__init__.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit_common/common.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit_common/common.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit_common/gpl.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit_common/gpl.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit_db/convertdict.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit_db/convertdict.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/nettoolkit_db/database.py` & `nettoolkit-1.6.2/nettoolkit/nettoolkit_db/database.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/juniper_oper.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/juniper_oper.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/md5_calculator.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/md5_calculator.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/forms/pw_enc_dec.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/forms/pw_enc_dec.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/hierarchy.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/hierarchy.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/hierarchy_rules.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/hierarchy_rules.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/jset.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/jset.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyJuniper/juniper.py` & `nettoolkit-1.6.2/nettoolkit/pyJuniper/juniper.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyNetCrypt/__init__.py` & `nettoolkit-1.6.2/nettoolkit/pyNetCrypt/__init__.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyNetCrypt/cpw_cracker.py` & `nettoolkit-1.6.2/nettoolkit/pyNetCrypt/cpw_cracker.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyNetCrypt/jpw_cracker.py` & `nettoolkit-1.6.2/nettoolkit/pyNetCrypt/jpw_cracker.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/__init__.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ------------------------------------------------------------------------------
 
 from .stencils import get_list_of_stencils
 from .database import DeviceData, CableMatrixData
 from .entities import ItemObjects, Connectors
 from .visio import VisioObject
 
-from .oper import DFGen
+from .oper import DFGen, CableMatrix
 from .devices import AdevDevices
 from .cablings import ADevCablings
 from .general import get_physical_if_up, get_physical_if_relevants
 from .general import get_patterns, update_pattern
 from .pyVig import pyVig
 # ------------------------------------------------------------------------------
```

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/cablings.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/cablings.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/database.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/database.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/devices.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/devices.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/entities.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/entities.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/forms/custom.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/forms/custom.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/forms/input_data.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/forms/input_data.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/general.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/general.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/maths.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/maths.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/oper.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/oper.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,18 @@
 
 	def custom_var_functions(self, **kwargs):
 		"""add/update custom `var` tab functions for object
 		"""		
 		for k, v in kwargs.items():
 			self.var_func_dict[k] = v
 
+	def __call__(self):
+		self.run()
 
-	def run(self, visio_gen=False):
+	def run(self):
 		"""iterate over all files for generating devices/cabling DataFrame details.
 		"""		
 		self.DCT = {}
 		for file in self.files:
 			DCT = DF_ConverT(file, self.default_stencil, self.line_pattern_style_separation_on, self.line_pattern_style_shift_no)
 			DCT.get_self_details(self.var_func_dict)
 			DCT.convert(self.func_dict)
@@ -322,14 +324,16 @@
 		"""cabling tab - add device model and serial numbers
 		"""		
 		self.cabling_merged_df['a_dev_model'] = self.cabling_merged_df.apply(lambda x: get_model_number(x, self.devices_merged_df, 'a_device'), axis=1)
 		self.cabling_merged_df['b_dev_model'] = self.cabling_merged_df.apply(lambda x: get_model_number(x, self.devices_merged_df, 'b_device'), axis=1)
 		self.cabling_merged_df['a_dev_serial'] = self.cabling_merged_df.apply(lambda x: get_serial_number(x, self.devices_merged_df, 'a_device'), axis=1)
 		self.cabling_merged_df['b_dev_serial'] = self.cabling_merged_df.apply(lambda x: get_serial_number(x, self.devices_merged_df, 'b_device'), axis=1)
 
+CableMatrix = DFGen
+
 # --------------------------------------------------------------------------------------------------
 
 def get_serial_number(df, devices_merged_df, device):
 	"""get serial number for match device
 
 	Args:
 		df (DataFrame): Cable Matrix DataFrame
```

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/pyVig.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/pyVig.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/static.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/static.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/stencils.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/stencils.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit/pyVig/visio.py` & `nettoolkit-1.6.2/nettoolkit/pyVig/visio.py`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/nettoolkit.egg-info/PKG-INFO` & `nettoolkit-1.6.2/nettoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettoolkit
-Version: 1.6.1
+Version: 1.6.2
 Summary: Tool Set for Networking Geeks
 Home-page: https://github.com/alias1978/nettoolkit
 Author: ALIASGAR - ALI
 Author-email: aholo2000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nettoolkit-1.6.1/nettoolkit.egg-info/SOURCES.txt` & `nettoolkit-1.6.2/nettoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nettoolkit-1.6.1/setup.py` & `nettoolkit-1.6.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nettoolkit",
-    version="1.6.1",
+    version="1.6.2",
     author="ALIASGAR - ALI",
     author_email="aholo2000@gmail.com",
     description="Tool Set for Networking Geeks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alias1978/nettoolkit",
     packages=setuptools.find_packages(),
```

