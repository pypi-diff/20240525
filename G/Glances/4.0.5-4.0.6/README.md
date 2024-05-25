# Comparing `tmp/glances-4.0.5.tar.gz` & `tmp/glances-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glances-4.0.5.tar", last modified: Sat May 18 09:31:20 2024, max compression
+gzip compressed data, was "glances-4.0.6.tar", last modified: Sat May 25 10:13:44 2024, max compression
```

## Comparing `glances-4.0.5.tar` & `glances-4.0.6.tar`

### file list

```diff
@@ -1,408 +1,408 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.349850 glances-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-18 09:31:15.000000 glances-4.0.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-18 09:31:15.000000 glances-4.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-18 09:31:15.000000 glances-4.0.5/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/Glances.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 09:31:20.000000 glances-4.0.5/Glances.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-18 09:31:15.000000 glances-4.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    73130 2024-05-18 09:31:15.000000 glances-4.0.5/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-05-18 09:31:20.349850 glances-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-05-18 09:31:15.000000 glances-4.0.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-18 09:31:15.000000 glances-4.0.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.289849 glances-4.0.5/conf/
--rw-r--r--   0 runner    (1001) docker     (127)    23757 2024-05-18 09:31:15.000000 glances-4.0.5/conf/glances.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.293849 glances-4.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-18 09:31:15.000000 glances-4.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-18 09:31:15.000000 glances-4.0.5/docs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.309849 glances-4.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Logo dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Text Logo dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/Glances Text Logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29273 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amp-dropbox.png
--rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amp-python-warning.png
--rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amp-python.png
--rw-r--r--   0 runner    (1001) docker     (127)    80498 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/amps.png
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/aws.png
--rw-r--r--   0 runner    (1001) docker     (127)    44160 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/browser.png
--rw-r--r--   0 runner    (1001) docker     (127)    21111 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/cloud.png
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/connected.png
--rw-r--r--   0 runner    (1001) docker     (127)    29245 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/connections.png
--rw-r--r--   0 runner    (1001) docker     (127)    34093 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/containers.png
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/cpu-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/cpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/disconnected.png
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/diskio.png
--rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/events.png
--rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/fs.png
--rw-r--r--   0 runner    (1001) docker     (127)    56273 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-architecture.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   123499 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)    92793 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-cgraph.svg
--rw-r--r--   0 runner    (1001) docker     (127)   114983 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-flame.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-influxdb.png
--rw-r--r--   0 runner    (1001) docker     (127)    33567 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-memory-profiling-with-history.png
--rw-r--r--   0 runner    (1001) docker     (127)    31797 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-memory-profiling-without-history.png
--rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-pyinstrument.html
--rw-r--r--   0 runner    (1001) docker     (127)   295283 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-responsive-webdesign.png
--rw-r--r--   0 runner    (1001) docker     (127)   435038 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/glances-summary.png
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/gpu.png
--rw-r--r--   0 runner    (1001) docker     (127)   141657 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/grafana.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/graph-load.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/hddtemp.png
--rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/header.png
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/ip.png
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/irq.png
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/load.png
--rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/loadpercent.png
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/mem-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/mem.png
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/monitored.png
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/network.png
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/per-cpu.png
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/pergpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/ports.png
--rw-r--r--   0 runner    (1001) docker     (127)    63154 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-extended.png
--rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)    53684 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-top.png
--rw-r--r--   0 runner    (1001) docker     (127)   227401 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)   151590 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/processlist.png
--rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/prometheus_exporter.png
--rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/prometheus_server.png
--rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/quicklook-percpu.png
--rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/quicklook.png
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/raid.png
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/reddit.png
--rw-r--r--   0 runner    (1001) docker     (127)  1089975 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screencast.gif
--rw-r--r--   0 runner    (1001) docker     (127)   265567 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot-web.png
--rw-r--r--   0 runner    (1001) docker     (127)    36097 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot-web2.png
--rw-r--r--   0 runner    (1001) docker     (127)  1098062 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot-wide.png
--rw-r--r--   0 runner    (1001) docker     (127)   508044 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/sensors.png
--rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/smart.png
--rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/sparkline.png
--rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/trend.png
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/twitter-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_static/wifi.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.309849 glances-4.0.5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-18 09:31:15.000000 glances-4.0.5/docs/_templates/links.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.313850 glances-4.0.5/docs/aoa/
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/actions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/amps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/cloud.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/connections.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/containers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/cpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/diskio.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/folders.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/fs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/gpu.rst
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/hddtemp.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/header.rst
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/irq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/load.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/memory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/network.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/ports.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/ps.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/quicklook.rst
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/raid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/smart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-18 09:31:15.000000 glances-4.0.5/docs/aoa/wifi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    53003 2024-05-18 09:31:15.000000 glances-4.0.5/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-05-18 09:31:15.000000 glances-4.0.5/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-18 09:31:15.000000 glances-4.0.5/docs/cmds.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-18 09:31:15.000000 glances-4.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-18 09:31:15.000000 glances-4.0.5/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.313850 glances-4.0.5/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 09:31:15.000000 glances-4.0.5/docs/dev/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   328258 2024-05-18 09:31:15.000000 glances-4.0.5/docs/dev/glances-cprofile.png
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-18 09:31:15.000000 glances-4.0.5/docs/docker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-18 09:31:15.000000 glances-4.0.5/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-18 09:31:15.000000 glances-4.0.5/docs/glances.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.317849 glances-4.0.5/docs/gw/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/cassandra.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/couchdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/csv.rst
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/elastic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/graph.rst
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/graphite.rst
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/influxdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/json.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/mongodb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/mqtt.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/opentsdb.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/rabbitmq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/restful.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/riemann.rst
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/statsd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-18 09:31:15.000000 glances-4.0.5/docs/gw/zeromq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-18 09:31:15.000000 glances-4.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-18 09:31:15.000000 glances-4.0.5/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-18 09:31:15.000000 glances-4.0.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.317849 glances-4.0.5/docs/man/
--rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-18 09:31:15.000000 glances-4.0.5/docs/man/glances.1
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-18 09:31:15.000000 glances-4.0.5/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-18 09:31:15.000000 glances-4.0.5/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 09:31:15.000000 glances-4.0.5/docs/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-18 09:31:15.000000 glances-4.0.5/glances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-18 09:31:15.000000 glances-4.0.5/glances/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-18 09:31:15.000000 glances-4.0.5/glances/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/amp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/default/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/nginx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/systemd/
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/systemd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/amps/systemv/
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps/systemv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-18 09:31:15.000000 glances-4.0.5/glances/amps_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-18 09:31:15.000000 glances-4.0.5/glances/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-18 09:31:15.000000 glances-4.0.5/glances/autodiscover.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-18 09:31:15.000000 glances-4.0.5/glances/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-18 09:31:15.000000 glances-4.0.5/glances/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-05-18 09:31:15.000000 glances-4.0.5/glances/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-18 09:31:15.000000 glances-4.0.5/glances/cpu_percent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-18 09:31:15.000000 glances-4.0.5/glances/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-18 09:31:15.000000 glances-4.0.5/glances/events_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/exports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.321850 glances-4.0.5/glances/exports/glances_cassandra/
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_cassandra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_couchdb/
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_couchdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_csv/
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_csv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_elasticsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_graphite/
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_graphite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_influxdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_influxdb2/
--rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_influxdb2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_json/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_mongodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_mqtt/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4955 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_mqtt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_opentsdb/
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_opentsdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_prometheus/
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_prometheus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_rabbitmq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_restful/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_restful/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_riemann/
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_riemann/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_statsd/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_statsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.325850 glances-4.0.5/glances/exports/glances_zeromq/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-18 09:31:15.000000 glances-4.0.5/glances/exports/glances_zeromq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-18 09:31:15.000000 glances-4.0.5/glances/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-18 09:31:15.000000 glances-4.0.5/glances/folder_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-18 09:31:15.000000 glances-4.0.5/glances/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-18 09:31:15.000000 glances-4.0.5/glances/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-18 09:31:15.000000 glances-4.0.5/glances/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-05-18 09:31:15.000000 glances-4.0.5/glances/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outdated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_bars.py
--rw-r--r--   0 runner    (1001) docker     (127)    48469 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_curses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_curses_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)    29542 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_restful_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_sparklines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_apidoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_stdout_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/glances_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/css/bootstrap.less
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/css/style.scss
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/css/variables.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/images/glances.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.329850 glances-4.0.5/glances/outputs/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/App.vue
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.333850 glances-4.0.5/glances/outputs/static/js/components/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/help.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-alert.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-amps.vue
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-cloud.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-connections.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-containers.vue
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-cpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-diskio.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-folders.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-fs.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-gpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-ip.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-irq.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-load.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-mem-more.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-mem.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-memswap.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-network.vue
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-now.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-percpu.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-ports.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-process.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-processcount.vue
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-processlist.vue
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-quicklook.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-raid.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-sensors.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-smart.vue
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-system.vue
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-uptime.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/components/plugin-wifi.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/filters.js
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/services.js
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/store.js
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/js/uiconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   452411 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/outputs/static/public/
--rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   448748 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/public/glances.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/outputs/static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-18 09:31:15.000000 glances-4.0.5/glances/outputs/static/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-18 09:31:15.000000 glances-4.0.5/glances/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-18 09:31:15.000000 glances-4.0.5/glances/password_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/__pycache__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/alert/
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/amps/
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/amps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/containers/
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/containers/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/engines/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/engines/podman.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/containers/stats_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/cpu/
--rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/cpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/diskio/
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/diskio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/folders/
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/folders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/fs/
--rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/fs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/gpu/
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/gpu/cards/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/cards/amd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/gpu/cards/nvidia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.337850 glances-4.0.5/glances/plugins/help/
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/help/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/irq/
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/irq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/load/
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/mem/
--rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/mem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/memswap/
--rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/memswap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/network/
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/now/
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/now/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/percpu/
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/percpu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46696 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/plugin/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/ports/
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/ports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/processcount/
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/processcount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/processlist/
--rw-r--r--   0 runner    (1001) docker     (127)    36550 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/processlist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/psutilversion/
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/psutilversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/quicklook/
--rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/quicklook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/raid/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/raid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/sensors/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/sensor/glances_batpercent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/sensors/sensor/glances_hddtemp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/smart/
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/smart/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/uptime/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/uptime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/version/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:31:20.341850 glances-4.0.5/glances/plugins/wifi/
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-18 09:31:15.000000 glances-4.0.5/glances/plugins/wifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-18 09:31:15.000000 glances-4.0.5/glances/ports_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    26258 2024-05-18 09:31:15.000000 glances-4.0.5/glances/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-18 09:31:15.000000 glances-4.0.5/glances/programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-18 09:31:15.000000 glances-4.0.5/glances/secure.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-18 09:31:15.000000 glances-4.0.5/glances/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-18 09:31:15.000000 glances-4.0.5/glances/snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-18 09:31:15.000000 glances-4.0.5/glances/standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-18 09:31:15.000000 glances-4.0.5/glances/static_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats_client_snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-18 09:31:15.000000 glances-4.0.5/glances/stats_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-18 09:31:15.000000 glances-4.0.5/glances/thresholds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-18 09:31:15.000000 glances-4.0.5/glances/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-18 09:31:15.000000 glances-4.0.5/glances/web_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-18 09:31:15.000000 glances-4.0.5/glances/webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-18 09:31:15.000000 glances-4.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 09:31:15.000000 glances-4.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:31:20.349850 glances-4.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4531 2024-05-18 09:31:15.000000 glances-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.538962 glances-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-25 10:13:40.000000 glances-4.0.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-25 10:13:40.000000 glances-4.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    42098 2024-05-25 10:13:40.000000 glances-4.0.6/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/Glances.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-05-25 10:13:44.000000 glances-4.0.6/Glances.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-25 10:13:44.000000 glances-4.0.6/Glances.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 10:13:44.000000 glances-4.0.6/Glances.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 10:13:44.000000 glances-4.0.6/Glances.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-25 10:13:44.000000 glances-4.0.6/Glances.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 10:13:44.000000 glances-4.0.6/Glances.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-25 10:13:40.000000 glances-4.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    73211 2024-05-25 10:13:40.000000 glances-4.0.6/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20468 2024-05-25 10:13:44.538962 glances-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16655 2024-05-25 10:13:40.000000 glances-4.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-25 10:13:40.000000 glances-4.0.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.474961 glances-4.0.6/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)    23757 2024-05-25 10:13:40.000000 glances-4.0.6/conf/glances.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.478961 glances-4.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-25 10:13:40.000000 glances-4.0.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-25 10:13:40.000000 glances-4.0.6/docs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.498962 glances-4.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/Glances Logo dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/Glances Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/Glances Text Logo dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/Glances Text Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29273 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/amp-dropbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9474 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/amp-python-warning.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/amp-python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    80498 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/amps.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/aws.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44160 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/browser.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21111 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/cloud.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/connected.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29245 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/connections.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34093 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/containers.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/cpu-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/cpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/disconnected.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/diskio.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13715 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/fs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56273 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-architecture.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   123499 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92793 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-cgraph.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   114983 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-flame.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-influxdb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33567 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-memory-profiling-with-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31797 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-memory-profiling-without-history.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-pyinstrument.html
+-rw-r--r--   0 runner    (1001) docker     (127)   295283 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-responsive-webdesign.png
+-rw-r--r--   0 runner    (1001) docker     (127)   435038 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/glances-summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/gpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)   141657 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/grafana.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/graph-load.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14415 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/hddtemp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19879 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/header.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/ip.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/irq.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/load.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/loadpercent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/mem-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/mem.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/monitored.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/network.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/per-cpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/pergpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/ports.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63154 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/processlist-extended.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160408 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/processlist-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53684 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/processlist-top.png
+-rw-r--r--   0 runner    (1001) docker     (127)   227401 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/processlist-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)   151590 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/processlist.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/prometheus_exporter.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91914 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/prometheus_server.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27582 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/quicklook-percpu.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17789 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/quicklook.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/raid.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1089975 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/screencast.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   265567 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/screenshot-web.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36097 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/screenshot-web2.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1098062 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/screenshot-wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)   508044 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/sensors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21500 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/smart.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/sparkline.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/trend.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/twitter-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_static/wifi.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.498962 glances-4.0.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-25 10:13:40.000000 glances-4.0.6/docs/_templates/links.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.502961 glances-4.0.6/docs/aoa/
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/amps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/cloud.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/connections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/cpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/diskio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/folders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/fs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/gpu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/hddtemp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/header.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/irq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/load.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/memory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/network.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/ports.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/ps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/quicklook.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/raid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/smart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-25 10:13:40.000000 glances-4.0.6/docs/aoa/wifi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    53040 2024-05-25 10:13:40.000000 glances-4.0.6/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)       28 2024-05-25 10:13:40.000000 glances-4.0.6/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     7977 2024-05-25 10:13:40.000000 glances-4.0.6/docs/cmds.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-25 10:13:40.000000 glances-4.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-25 10:13:40.000000 glances-4.0.6/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.502961 glances-4.0.6/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-25 10:13:40.000000 glances-4.0.6/docs/dev/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   328258 2024-05-25 10:13:40.000000 glances-4.0.6/docs/dev/glances-cprofile.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-25 10:13:40.000000 glances-4.0.6/docs/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-25 10:13:40.000000 glances-4.0.6/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-25 10:13:40.000000 glances-4.0.6/docs/glances.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.506961 glances-4.0.6/docs/gw/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/cassandra.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/couchdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/csv.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/elastic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/graph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/graphite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/influxdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/json.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/mongodb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/mqtt.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/opentsdb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/rabbitmq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/restful.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/riemann.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-25 10:13:40.000000 glances-4.0.6/docs/gw/zeromq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-25 10:13:40.000000 glances-4.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-25 10:13:40.000000 glances-4.0.6/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7251 2024-05-25 10:13:40.000000 glances-4.0.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.506961 glances-4.0.6/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (127)    19253 2024-05-25 10:13:40.000000 glances-4.0.6/docs/man/glances.1
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-25 10:13:40.000000 glances-4.0.6/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-25 10:13:40.000000 glances-4.0.6/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-25 10:13:40.000000 glances-4.0.6/docs/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.510961 glances-4.0.6/glances/
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-25 10:13:40.000000 glances-4.0.6/glances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-25 10:13:40.000000 glances-4.0.6/glances/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-25 10:13:40.000000 glances-4.0.6/glances/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.510961 glances-4.0.6/glances/amps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps/amp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.510961 glances-4.0.6/glances/amps/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.510961 glances-4.0.6/glances/amps/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps/nginx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.510961 glances-4.0.6/glances/amps/systemd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps/systemd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.510961 glances-4.0.6/glances/amps/systemv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps/systemv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-25 10:13:40.000000 glances-4.0.6/glances/amps_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-25 10:13:40.000000 glances-4.0.6/glances/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-05-25 10:13:40.000000 glances-4.0.6/glances/autodiscover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-25 10:13:40.000000 glances-4.0.6/glances/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-25 10:13:40.000000 glances-4.0.6/glances/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-05-25 10:13:40.000000 glances-4.0.6/glances/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-25 10:13:40.000000 glances-4.0.6/glances/cpu_percent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-25 10:13:40.000000 glances-4.0.6/glances/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-25 10:13:40.000000 glances-4.0.6/glances/events_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_cassandra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_cassandra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_couchdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_couchdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_csv/
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_csv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_elasticsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_graphite/
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_graphite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_influxdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_influxdb2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6482 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_influxdb2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_mongodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_mqtt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4955 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_mqtt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_opentsdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_opentsdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_prometheus/
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_prometheus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_rabbitmq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_restful/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_restful/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_riemann/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_riemann/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_statsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_statsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.514962 glances-4.0.6/glances/exports/glances_zeromq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-25 10:13:40.000000 glances-4.0.6/glances/exports/glances_zeromq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-25 10:13:40.000000 glances-4.0.6/glances/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-05-25 10:13:40.000000 glances-4.0.6/glances/folder_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-05-25 10:13:40.000000 glances-4.0.6/glances/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-25 10:13:40.000000 glances-4.0.6/glances/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-25 10:13:40.000000 glances-4.0.6/glances/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-05-25 10:13:40.000000 glances-4.0.6/glances/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outdated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.518962 glances-4.0.6/glances/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_bars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48469 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_curses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12555 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_curses_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29542 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_sparklines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_stdout_apidoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_stdout_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_stdout_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_stdout_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/glances_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.518962 glances-4.0.6/glances/outputs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.518962 glances-4.0.6/glances/outputs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/css/bootstrap.less
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/css/style.scss
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/css/variables.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.518962 glances-4.0.6/glances/outputs/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/images/glances.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.522961 glances-4.0.6/glances/outputs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    15387 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/App.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/outputs/static/js/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/help.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-alert.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-amps.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-cloud.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-connections.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-containers.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-cpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-diskio.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-folders.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-fs.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-gpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-ip.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-irq.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-load.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-mem-more.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-mem.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-memswap.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-network.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-now.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-percpu.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-ports.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-process.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-processcount.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-processlist.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-quicklook.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-raid.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-sensors.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-smart.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-system.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-uptime.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/components/plugin-wifi.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/filters.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/services.js
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/store.js
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/js/uiconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   452411 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/outputs/static/public/
+-rw-r--r--   0 runner    (1001) docker     (127)    50295 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   449982 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/public/glances.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/outputs/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-25 10:13:40.000000 glances-4.0.6/glances/outputs/static/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-25 10:13:40.000000 glances-4.0.6/glances/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-25 10:13:40.000000 glances-4.0.6/glances/password_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/plugins/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/__pycache__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/plugins/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/plugins/amps/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/amps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.526962 glances-4.0.6/glances/plugins/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/containers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/containers/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/containers/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/containers/engines/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13212 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/containers/engines/podman.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/containers/stats_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/cpu/
+-rw-r--r--   0 runner    (1001) docker     (127)    15498 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/cpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/diskio/
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/diskio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/folders/
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/folders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11663 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/fs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/gpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/gpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/gpu/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/gpu/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/gpu/cards/amd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/gpu/cards/nvidia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/help/
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/help/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/irq/
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/irq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/load/
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/mem/
+-rw-r--r--   0 runner    (1001) docker     (127)    10913 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/mem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/memswap/
+-rw-r--r--   0 runner    (1001) docker     (127)     7454 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/memswap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/now/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/now/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.530962 glances-4.0.6/glances/plugins/percpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/percpu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46696 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/plugin/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/ports/
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/ports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/processcount/
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/processcount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/processlist/
+-rw-r--r--   0 runner    (1001) docker     (127)    36550 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/processlist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/psutilversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/psutilversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/quicklook/
+-rw-r--r--   0 runner    (1001) docker     (127)    11764 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/quicklook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/raid/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/raid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/sensors/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/sensors/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/sensors/sensor/glances_batpercent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/sensors/sensor/glances_hddtemp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/smart/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/smart/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/uptime/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/uptime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 10:13:44.534962 glances-4.0.6/glances/plugins/wifi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-25 10:13:40.000000 glances-4.0.6/glances/plugins/wifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-25 10:13:40.000000 glances-4.0.6/glances/ports_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26258 2024-05-25 10:13:40.000000 glances-4.0.6/glances/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-25 10:13:40.000000 glances-4.0.6/glances/programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-25 10:13:40.000000 glances-4.0.6/glances/secure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-05-25 10:13:40.000000 glances-4.0.6/glances/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-25 10:13:40.000000 glances-4.0.6/glances/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-25 10:13:40.000000 glances-4.0.6/glances/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-25 10:13:40.000000 glances-4.0.6/glances/static_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14920 2024-05-25 10:13:40.000000 glances-4.0.6/glances/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-25 10:13:40.000000 glances-4.0.6/glances/stats_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-25 10:13:40.000000 glances-4.0.6/glances/stats_client_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-25 10:13:40.000000 glances-4.0.6/glances/stats_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-25 10:13:40.000000 glances-4.0.6/glances/thresholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-25 10:13:40.000000 glances-4.0.6/glances/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-25 10:13:40.000000 glances-4.0.6/glances/web_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-25 10:13:40.000000 glances-4.0.6/glances/webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-25 10:13:40.000000 glances-4.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 10:13:40.000000 glances-4.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 10:13:44.538962 glances-4.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4531 2024-05-25 10:13:40.000000 glances-4.0.6/setup.py
```

### Comparing `glances-4.0.5/AUTHORS` & `glances-4.0.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/CONTRIBUTING.md` & `glances-4.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/COPYING` & `glances-4.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/Glances.egg-info/PKG-INFO` & `glances-4.0.6/Glances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 4.0.5
+Version: 4.0.6
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `glances-4.0.5/Glances.egg-info/SOURCES.txt` & `glances-4.0.6/Glances.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/Glances.egg-info/requires.txt` & `glances-4.0.6/Glances.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/NEWS.rst` & `glances-4.0.6/NEWS.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 ==============================================================================
                                 Glances ChangeLog
 ==============================================================================
 
 ===============
+Version 4.0.6
+===============
+
+*  No GPU info on Web View #2796
+
+===============
 Version 4.0.5
 ===============
 
 * SensorType change in REST API breaks compatibility in 4.0.4 #2788
 * Please make pydantic optional dependency, not required one #2777
 * Update the Grafana dashboard #2780
 * 4.0.4 - On Glances startup "ERROR -- Can not init battery class #2776
```

### Comparing `glances-4.0.5/PKG-INFO` & `glances-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glances
-Version: 4.0.5
+Version: 4.0.6
 Summary: A cross-platform curses-based monitoring tool
 Home-page: https://github.com/nicolargo/glances
 Author: Nicolas Hennion
 Author-email: nicolas@nicolargo.com
 License: LGPLv3
 Keywords: cli curses monitoring system
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `glances-4.0.5/README.rst` & `glances-4.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/SECURITY.md` & `glances-4.0.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/conf/glances.conf` & `glances-4.0.6/conf/glances.conf`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/Makefile` & `glances-4.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/Glances Logo dark.svg` & `glances-4.0.6/docs/_static/Glances Logo dark.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/Glances Logo.svg` & `glances-4.0.6/docs/_static/Glances Logo.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/Glances Text Logo dark.svg` & `glances-4.0.6/docs/_static/Glances Text Logo dark.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/Glances Text Logo.svg` & `glances-4.0.6/docs/_static/Glances Text Logo.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/amp-dropbox.png` & `glances-4.0.6/docs/_static/amp-dropbox.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/amp-python-warning.png` & `glances-4.0.6/docs/_static/amp-python-warning.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/amp-python.png` & `glances-4.0.6/docs/_static/amp-python.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/amps.png` & `glances-4.0.6/docs/_static/amps.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/aws.png` & `glances-4.0.6/docs/_static/aws.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/browser.png` & `glances-4.0.6/docs/_static/browser.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/cloud.png` & `glances-4.0.6/docs/_static/cloud.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/connected.png` & `glances-4.0.6/docs/_static/connected.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/connections.png` & `glances-4.0.6/docs/_static/connections.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/containers.png` & `glances-4.0.6/docs/_static/containers.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/cpu-wide.png` & `glances-4.0.6/docs/_static/cpu-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/cpu.png` & `glances-4.0.6/docs/_static/cpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/disconnected.png` & `glances-4.0.6/docs/_static/disconnected.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/diskio.png` & `glances-4.0.6/docs/_static/diskio.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/events.png` & `glances-4.0.6/docs/_static/events.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/folders.png` & `glances-4.0.6/docs/_static/folders.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/fs.png` & `glances-4.0.6/docs/_static/fs.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-architecture.excalidraw` & `glances-4.0.6/docs/_static/glances-architecture.excalidraw`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-architecture.png` & `glances-4.0.6/docs/_static/glances-architecture.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-cgraph.svg` & `glances-4.0.6/docs/_static/glances-cgraph.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-flame.svg` & `glances-4.0.6/docs/_static/glances-flame.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-influxdb.png` & `glances-4.0.6/docs/_static/glances-influxdb.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-memory-profiling-with-history.png` & `glances-4.0.6/docs/_static/glances-memory-profiling-with-history.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-memory-profiling-without-history.png` & `glances-4.0.6/docs/_static/glances-memory-profiling-without-history.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-pyinstrument.html` & `glances-4.0.6/docs/_static/glances-pyinstrument.html`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-responsive-webdesign.png` & `glances-4.0.6/docs/_static/glances-responsive-webdesign.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/glances-summary.png` & `glances-4.0.6/docs/_static/glances-summary.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/gpu.png` & `glances-4.0.6/docs/_static/gpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/grafana.png` & `glances-4.0.6/docs/_static/grafana.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/graph-load.svg` & `glances-4.0.6/docs/_static/graph-load.svg`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/hddtemp.png` & `glances-4.0.6/docs/_static/hddtemp.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/header.png` & `glances-4.0.6/docs/_static/header.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/ip.png` & `glances-4.0.6/docs/_static/ip.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/irq.png` & `glances-4.0.6/docs/_static/irq.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/load.png` & `glances-4.0.6/docs/_static/load.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/loadpercent.png` & `glances-4.0.6/docs/_static/loadpercent.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/mem-wide.png` & `glances-4.0.6/docs/_static/mem-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/mem.png` & `glances-4.0.6/docs/_static/mem.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/monitored.png` & `glances-4.0.6/docs/_static/monitored.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/network.png` & `glances-4.0.6/docs/_static/network.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/per-cpu.png` & `glances-4.0.6/docs/_static/per-cpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/pergpu.png` & `glances-4.0.6/docs/_static/pergpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/ports.png` & `glances-4.0.6/docs/_static/ports.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/processlist-extended.png` & `glances-4.0.6/docs/_static/processlist-extended.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/processlist-filter.png` & `glances-4.0.6/docs/_static/processlist-filter.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/processlist-top.png` & `glances-4.0.6/docs/_static/processlist-top.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/processlist-wide.png` & `glances-4.0.6/docs/_static/processlist-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/processlist.png` & `glances-4.0.6/docs/_static/processlist.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/prometheus_exporter.png` & `glances-4.0.6/docs/_static/prometheus_exporter.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/prometheus_server.png` & `glances-4.0.6/docs/_static/prometheus_server.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/quicklook-percpu.png` & `glances-4.0.6/docs/_static/quicklook-percpu.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/quicklook.png` & `glances-4.0.6/docs/_static/quicklook.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/raid.png` & `glances-4.0.6/docs/_static/raid.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/reddit.png` & `glances-4.0.6/docs/_static/reddit.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/screencast.gif` & `glances-4.0.6/docs/_static/screencast.gif`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/screenshot-web.png` & `glances-4.0.6/docs/_static/screenshot-web.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/screenshot-web2.png` & `glances-4.0.6/docs/_static/screenshot-web2.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/screenshot-wide.png` & `glances-4.0.6/docs/_static/screenshot-wide.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/screenshot.png` & `glances-4.0.6/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/sensors.png` & `glances-4.0.6/docs/_static/sensors.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/smart.png` & `glances-4.0.6/docs/_static/smart.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/sparkline.png` & `glances-4.0.6/docs/_static/sparkline.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/trend.png` & `glances-4.0.6/docs/_static/trend.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/twitter-icon.png` & `glances-4.0.6/docs/_static/twitter-icon.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/_static/wifi.png` & `glances-4.0.6/docs/_static/wifi.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/actions.rst` & `glances-4.0.6/docs/aoa/actions.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/amps.rst` & `glances-4.0.6/docs/aoa/amps.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/connections.rst` & `glances-4.0.6/docs/aoa/connections.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/containers.rst` & `glances-4.0.6/docs/aoa/containers.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/cpu.rst` & `glances-4.0.6/docs/aoa/cpu.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/diskio.rst` & `glances-4.0.6/docs/aoa/diskio.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/events.rst` & `glances-4.0.6/docs/aoa/events.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/folders.rst` & `glances-4.0.6/docs/aoa/folders.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/fs.rst` & `glances-4.0.6/docs/aoa/fs.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/gpu.rst` & `glances-4.0.6/docs/aoa/gpu.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/hddtemp.rst` & `glances-4.0.6/docs/aoa/hddtemp.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/header.rst` & `glances-4.0.6/docs/aoa/header.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/index.rst` & `glances-4.0.6/docs/aoa/index.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/irq.rst` & `glances-4.0.6/docs/aoa/irq.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/load.rst` & `glances-4.0.6/docs/aoa/load.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/memory.rst` & `glances-4.0.6/docs/aoa/memory.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/network.rst` & `glances-4.0.6/docs/aoa/network.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/ports.rst` & `glances-4.0.6/docs/aoa/ports.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/ps.rst` & `glances-4.0.6/docs/aoa/ps.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/quicklook.rst` & `glances-4.0.6/docs/aoa/quicklook.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/raid.rst` & `glances-4.0.6/docs/aoa/raid.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/sensors.rst` & `glances-4.0.6/docs/aoa/sensors.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/smart.rst` & `glances-4.0.6/docs/aoa/smart.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/aoa/wifi.rst` & `glances-4.0.6/docs/aoa/wifi.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/api.rst` & `glances-4.0.6/docs/api.rst`

 * *Files 2% similar despite different names*

```diff
@@ -137,24 +137,24 @@
       "countmax": None,
       "countmin": 1.0,
       "key": "name",
       "name": "Dropbox",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 0.1488208770751953},
+      "timer": 0.3419933319091797},
      {"count": 0,
       "countmax": 20.0,
       "countmin": None,
       "key": "name",
       "name": "Python",
       "refresh": 3.0,
       "regex": True,
       "result": None,
-      "timer": 0.14876770973205566}]
+      "timer": 0.34189915657043457}]
 
 Fields descriptions:
 
 * **name**: AMP name (unit is *None*)
 * **result**: AMP result (a string) (unit is *None*)
 * **refresh**: AMP refresh interval (unit is *second*)
 * **timer**: Time until next refresh (unit is *second*)
@@ -174,15 +174,15 @@
                   "countmax": None,
                   "countmin": 1.0,
                   "key": "name",
                   "name": "Dropbox",
                   "refresh": 3.0,
                   "regex": True,
                   "result": None,
-                  "timer": 0.1488208770751953}]}
+                  "timer": 0.3419933319091797}]}
 
 GET cloud
 ---------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/cloud
@@ -261,22 +261,22 @@
 GET cpu
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/cpu
     {"cpucore": 16,
-     "ctx_switches": 26785017,
+     "ctx_switches": 226080767,
      "guest": 0.0,
-     "idle": 1.0,
-     "interrupts": 31606155,
+     "idle": 0.0,
+     "interrupts": 212524511,
      "iowait": 0.0,
      "irq": 0.0,
      "nice": 0.0,
-     "soft_interrupts": 7987786,
+     "soft_interrupts": 73033693,
      "steal": 0.0,
      "syscalls": 0,
      "system": 0.0,
      "total": 0.0,
      "user": 0.0}
 
 Fields descriptions:
@@ -316,22 +316,22 @@
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/diskio
     [{"disk_name": "nvme0n1",
       "key": "disk_name",
-      "read_bytes": 3989510656,
-      "read_count": 136457,
-      "write_bytes": 4117681152,
-      "write_count": 166108},
+      "read_bytes": 4815501824,
+      "read_count": 206134,
+      "write_bytes": 13422109696,
+      "write_count": 782837},
      {"disk_name": "nvme0n1p1",
       "key": "disk_name",
-      "read_bytes": 7476224,
-      "read_count": 576,
+      "read_bytes": 7484416,
+      "read_count": 592,
       "write_bytes": 1024,
       "write_count": 2}]
 
 Fields descriptions:
 
 * **disk_name**: Disk name (unit is *None*)
 * **read_count**: Number of reads (unit is *number*)
@@ -359,18 +359,18 @@
                    "dm-1"]}
 
 Get a specific item when field matches the given value::
 
     # curl http://localhost:61208/api/4/diskio/disk_name/nvme0n1
     {"nvme0n1": [{"disk_name": "nvme0n1",
                   "key": "disk_name",
-                  "read_bytes": 3989510656,
-                  "read_count": 136457,
-                  "write_bytes": 4117681152,
-                  "write_count": 166108}]}
+                  "read_bytes": 4815501824,
+                  "read_count": 206134,
+                  "write_bytes": 13422109696,
+                  "write_count": 782837}]}
 
 GET folders
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/folders
@@ -389,21 +389,21 @@
 GET fs
 ------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/fs
     [{"device_name": "/dev/mapper/ubuntu--vg-ubuntu--lv",
-      "free": 905288650752,
+      "free": 904885006336,
       "fs_type": "ext4",
       "key": "mnt_point",
       "mnt_point": "/",
       "percent": 5.0,
       "size": 1003736440832,
-      "used": 47385284608}]
+      "used": 47788929024}]
 
 Fields descriptions:
 
 * **device_name**: Device name (unit is *None*)
 * **fs_type**: File system type (unit is *None*)
 * **mnt_point**: Mount point (unit is *None*)
 * **size**: Total size (unit is *byte*)
@@ -416,21 +416,21 @@
     # curl http://localhost:61208/api/4/fs/mnt_point
     {"mnt_point": ["/"]}
 
 Get a specific item when field matches the given value::
 
     # curl http://localhost:61208/api/4/fs/mnt_point//
     {"/": [{"device_name": "/dev/mapper/ubuntu--vg-ubuntu--lv",
-            "free": 905288650752,
+            "free": 904885006336,
             "fs_type": "ext4",
             "key": "mnt_point",
             "mnt_point": "/",
             "percent": 5.0,
             "size": 1003736440832,
-            "used": 47385284608}]}
+            "used": 47788929024}]}
 
 GET gpu
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/gpu
@@ -495,44 +495,47 @@
 
 GET load
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/load
-    {"cpucore": 16, "min1": 0.748046875, "min15": 0.57373046875, "min5": 0.7265625}
+    {"cpucore": 16,
+     "min1": 0.521484375,
+     "min15": 1.1435546875,
+     "min5": 0.9404296875}
 
 Fields descriptions:
 
 * **min1**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 1 minute (unit is *float*)
 * **min5**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 5 minutes (unit is *float*)
 * **min15**: Average sum of the number of processes waiting in the run-queue plus the number currently executing over 15 minutes (unit is *float*)
 * **cpucore**: Total number of CPU core (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/load/min1
-    {"min1": 0.748046875}
+    {"min1": 0.521484375}
 
 GET mem
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/mem
-    {"active": 5833261056,
-     "available": 10653102080,
-     "buffers": 250515456,
-     "cached": 5880537088,
-     "free": 10653102080,
-     "inactive": 3567583232,
-     "percent": 35.1,
-     "shared": 705511424,
+    {"active": 8715345920,
+     "available": 7980945408,
+     "buffers": 456585216,
+     "cached": 7151083520,
+     "free": 7980945408,
+     "inactive": 4241293312,
+     "percent": 51.4,
+     "shared": 793468928,
      "total": 16422486016,
-     "used": 5769383936}
+     "used": 8441540608}
 
 Fields descriptions:
 
 * **total**: Total physical memory available (unit is *bytes*)
 * **available**: The actual amount of available memory that can be given instantly to processes that request more memory in bytes; this is calculated by summing different memory values depending on the platform (e.g. free + buffers + cached on Linux) and it is supposed to be used to monitor actual memory usage in a cross platform fashion (unit is *bytes*)
 * **percent**: The percentage usage calculated as (total - available) / total * 100 (unit is *percent*)
 * **used**: Memory used, calculated differently depending on the platform and designed for informational purposes only (unit is *bytes*)
@@ -551,21 +554,21 @@
 
 GET memswap
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/memswap
-    {"free": 4294963200,
+    {"free": 4294176768,
      "percent": 0.0,
      "sin": 0,
-     "sout": 0,
+     "sout": 110592,
      "time_since_update": 1,
      "total": 4294963200,
-     "used": 0}
+     "used": 786432}
 
 Fields descriptions:
 
 * **total**: Total swap memory (unit is *bytes*)
 * **used**: Used swap memory (unit is *bytes*)
 * **free**: Free swap memory (unit is *bytes*)
 * **percent**: Used swap memory in percentage (unit is *percent*)
@@ -582,23 +585,23 @@
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/network
     [{"alias": None,
       "bytes_all": 0,
-      "bytes_all_gauge": 451852439,
+      "bytes_all_gauge": 1278105663,
       "bytes_recv": 0,
-      "bytes_recv_gauge": 428042038,
+      "bytes_recv_gauge": 979859126,
       "bytes_sent": 0,
-      "bytes_sent_gauge": 23810401,
+      "bytes_sent_gauge": 298246537,
       "interface_name": "wlp0s20f3",
       "key": "interface_name",
       "speed": 0,
-      "time_since_update": 0.15277767181396484}]
+      "time_since_update": 0.34995555877685547}]
 
 Fields descriptions:
 
 * **interface_name**: Interface name (unit is *None*)
 * **alias**: Interface alias name (optional) (unit is *None*)
 * **bytes_recv**: Number of bytes received (unit is *byte*)
 * **bytes_recv_rate_per_sec**: Number of bytes received per second (unit is *byte* per second)
@@ -619,60 +622,60 @@
     {"interface_name": ["wlp0s20f3"]}
 
 Get a specific item when field matches the given value::
 
     # curl http://localhost:61208/api/4/network/interface_name/wlp0s20f3
     {"wlp0s20f3": [{"alias": None,
                     "bytes_all": 0,
-                    "bytes_all_gauge": 451852439,
+                    "bytes_all_gauge": 1278105663,
                     "bytes_recv": 0,
-                    "bytes_recv_gauge": 428042038,
+                    "bytes_recv_gauge": 979859126,
                     "bytes_sent": 0,
-                    "bytes_sent_gauge": 23810401,
+                    "bytes_sent_gauge": 298246537,
                     "interface_name": "wlp0s20f3",
                     "key": "interface_name",
                     "speed": 0,
-                    "time_since_update": 0.15277767181396484}]}
+                    "time_since_update": 0.34995555877685547}]}
 
 GET now
 -------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/now
-    {"custom": "2024-05-18 11:03:48 CEST", "iso": "2024-05-18T11:03:48+02:00"}
+    {"custom": "2024-05-25 12:07:37 CEST", "iso": "2024-05-25T12:07:37+02:00"}
 
 Fields descriptions:
 
 * **custom**: Current date in custom format (unit is *None*)
 * **iso**: Current date in ISO 8601 format (unit is *None*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/now/iso
-    {"iso": "2024-05-18T11:03:48+02:00"}
+    {"iso": "2024-05-25T12:07:37+02:00"}
 
 GET percpu
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/percpu
     [{"cpu_number": 0,
       "guest": 0.0,
       "guest_nice": 0.0,
-      "idle": 1.0,
+      "idle": 0.0,
       "iowait": 0.0,
       "irq": 0.0,
       "key": "cpu_number",
       "nice": 0.0,
       "softirq": 0.0,
       "steal": 0.0,
       "system": 0.0,
-      "total": 99.0,
+      "total": 100.0,
       "user": 0.0},
      {"cpu_number": 1,
       "guest": 0.0,
       "guest_nice": 0.0,
       "idle": 0.0,
       "iowait": 0.0,
       "irq": 0.0,
@@ -712,15 +715,15 @@
     # curl http://localhost:61208/api/4/ports
     [{"description": "DefaultGateway",
       "host": "192.168.1.1",
       "indice": "port_0",
       "port": 0,
       "refresh": 30,
       "rtt_warning": None,
-      "status": 0.004889,
+      "status": 0.007397,
       "timeout": 3}]
 
 Fields descriptions:
 
 * **host**: Measurement is be done on this host (or IP address) (unit is *None*)
 * **port**: Measurement is be done on this port (0 for ICMP) (unit is *None*)
 * **description**: Human readable description for the host/port (unit is *None*)
@@ -740,37 +743,37 @@
     # curl http://localhost:61208/api/4/ports/host/192.168.1.1
     {"192.168.1.1": [{"description": "DefaultGateway",
                       "host": "192.168.1.1",
                       "indice": "port_0",
                       "port": 0,
                       "refresh": 30,
                       "rtt_warning": None,
-                      "status": 0.004889,
+                      "status": 0.007397,
                       "timeout": 3}]}
 
 GET processcount
 ----------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/processcount
-    {"pid_max": 0, "running": 0, "sleeping": 276, "thread": 1568, "total": 407}
+    {"pid_max": 0, "running": 1, "sleeping": 292, "thread": 1764, "total": 431}
 
 Fields descriptions:
 
 * **total**: Total number of processes (unit is *number*)
 * **running**: Total number of running processes (unit is *number*)
 * **sleeping**: Total number of sleeping processes (unit is *number*)
 * **thread**: Total number of threads (unit is *number*)
 * **pid_max**: Maximum number of processes (unit is *number*)
 
 Get a specific field::
 
     # curl http://localhost:61208/api/4/processcount/total
-    {"total": 407}
+    {"total": 431}
 
 GET processlist
 ---------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/processlist
@@ -804,32 +807,32 @@
 -------------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/quicklook
     {"cpu": 0.0,
      "cpu_hz": 4475000000.0,
-     "cpu_hz_current": 1871619687.4999998,
+     "cpu_hz_current": 1245390687.5,
      "cpu_log_core": 16,
      "cpu_name": "13th Gen Intel(R) Core(TM) i7-13620H",
      "cpu_phys_core": 10,
-     "load": 3.6,
-     "mem": 35.1,
+     "load": 7.1,
+     "mem": 51.4,
      "percpu": [{"cpu_number": 0,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 1,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
@@ -878,75 +881,75 @@
                  "steal": 0.0,
                  "system": 0.0,
                  "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 5,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 6,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
-                 "system": 1.0,
+                 "system": 0.0,
                  "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 7,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 8,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 9,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 10,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
@@ -956,23 +959,23 @@
                  "steal": 0.0,
                  "system": 0.0,
                  "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 11,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 12,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
@@ -995,23 +998,23 @@
                  "steal": 0.0,
                  "system": 0.0,
                  "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 14,
                  "guest": 0.0,
                  "guest_nice": 0.0,
-                 "idle": 1.0,
+                 "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
                  "key": "cpu_number",
                  "nice": 0.0,
                  "softirq": 0.0,
                  "steal": 0.0,
                  "system": 0.0,
-                 "total": 99.0,
+                 "total": 100.0,
                  "user": 0.0},
                 {"cpu_number": 15,
                  "guest": 0.0,
                  "guest_nice": 0.0,
                  "idle": 0.0,
                  "iowait": 0.0,
                  "irq": 0.0,
@@ -1056,22 +1059,22 @@
 
     # curl http://localhost:61208/api/4/sensors
     [{"critical": None,
       "key": "label",
       "label": "Ambient",
       "type": "SensorType.CPU_TEMP",
       "unit": "C",
-      "value": 38,
+      "value": 35,
       "warning": 0},
      {"critical": None,
       "key": "label",
       "label": "Ambient 3",
       "type": "SensorType.CPU_TEMP",
       "unit": "C",
-      "value": 33,
+      "value": 30,
       "warning": 0}]
 
 Fields descriptions:
 
 * **label**: Sensor label (unit is *None*)
 * **unit**: Sensor unit (unit is *None*)
 * **value**: Sensor value (unit is *number*)
@@ -1124,15 +1127,15 @@
 
     # curl http://localhost:61208/api/4/sensors/label/Ambient
     {"Ambient": [{"critical": None,
                   "key": "label",
                   "label": "Ambient",
                   "type": "SensorType.CPU_TEMP",
                   "unit": "C",
-                  "value": 38,
+                  "value": 35,
                   "warning": 0}]}
 
 GET smart
 ---------
 
 Get plugin stats::
 
@@ -1168,23 +1171,23 @@
 
 GET uptime
 ----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/uptime
-    "4 days, 11:56:37"
+    "11 days, 13:00:18"
 
 GET version
 -----------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/version
-    "4.0.5"
+    "4.0.6"
 
 GET wifi
 --------
 
 Get plugin stats::
 
     # curl http://localhost:61208/api/4/wifi
@@ -1244,42 +1247,42 @@
 
 GET stats history
 -----------------
 
 History of a plugin::
 
     # curl http://localhost:61208/api/4/cpu/history
-    {"system": [["2024-05-18T11:03:49.609837", 0.0],
-                ["2024-05-18T11:03:50.653488", 1.0],
-                ["2024-05-18T11:03:51.701403", 1.0]],
-     "user": [["2024-05-18T11:03:49.609825", 0.0],
-              ["2024-05-18T11:03:50.653484", 0.0],
-              ["2024-05-18T11:03:51.701393", 0.0]]}
+    {"system": [["2024-05-25T12:07:39.021345", 0.0],
+                ["2024-05-25T12:07:40.053748", 0.0],
+                ["2024-05-25T12:07:41.134700", 0.0]],
+     "user": [["2024-05-25T12:07:39.021338", 0.0],
+              ["2024-05-25T12:07:40.053742", 1.0],
+              ["2024-05-25T12:07:41.134683", 1.0]]}
 
 Limit history to last 2 values::
 
     # curl http://localhost:61208/api/4/cpu/history/2
-    {"system": [["2024-05-18T11:03:50.653488", 1.0],
-                ["2024-05-18T11:03:51.701403", 1.0]],
-     "user": [["2024-05-18T11:03:50.653484", 0.0],
-              ["2024-05-18T11:03:51.701393", 0.0]]}
+    {"system": [["2024-05-25T12:07:40.053748", 0.0],
+                ["2024-05-25T12:07:41.134700", 0.0]],
+     "user": [["2024-05-25T12:07:40.053742", 1.0],
+              ["2024-05-25T12:07:41.134683", 1.0]]}
 
 History for a specific field::
 
     # curl http://localhost:61208/api/4/cpu/system/history
-    {"system": [["2024-05-18T11:03:48.519990", 0.0],
-                ["2024-05-18T11:03:49.609837", 0.0],
-                ["2024-05-18T11:03:50.653488", 1.0],
-                ["2024-05-18T11:03:51.701403", 1.0]]}
+    {"system": [["2024-05-25T12:07:37.851785", 0.0],
+                ["2024-05-25T12:07:39.021345", 0.0],
+                ["2024-05-25T12:07:40.053748", 0.0],
+                ["2024-05-25T12:07:41.134700", 0.0]]}
 
 Limit history for a specific field to last 2 values::
 
     # curl http://localhost:61208/api/4/cpu/system/history
-    {"system": [["2024-05-18T11:03:50.653488", 1.0],
-                ["2024-05-18T11:03:51.701403", 1.0]]}
+    {"system": [["2024-05-25T12:07:40.053748", 0.0],
+                ["2024-05-25T12:07:41.134700", 0.0]]}
 
 GET limits (used for thresholds)
 --------------------------------
 
 All limits/thresholds::
 
     # curl http://localhost:61208/api/4/all/limits
```

### Comparing `glances-4.0.5/docs/cmds.rst` & `glances-4.0.6/docs/cmds.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/conf.py` & `glances-4.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/config.rst` & `glances-4.0.6/docs/config.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/dev/glances-cprofile.png` & `glances-4.0.6/docs/dev/glances-cprofile.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/docker.rst` & `glances-4.0.6/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/glances.rst` & `glances-4.0.6/docs/glances.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/cassandra.rst` & `glances-4.0.6/docs/gw/cassandra.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/couchdb.rst` & `glances-4.0.6/docs/gw/couchdb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/csv.rst` & `glances-4.0.6/docs/gw/csv.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/graph.rst` & `glances-4.0.6/docs/gw/graph.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/graphite.rst` & `glances-4.0.6/docs/gw/graphite.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/influxdb.rst` & `glances-4.0.6/docs/gw/influxdb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/kafka.rst` & `glances-4.0.6/docs/gw/kafka.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/mongodb.rst` & `glances-4.0.6/docs/gw/mongodb.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/mqtt.rst` & `glances-4.0.6/docs/gw/mqtt.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/prometheus.rst` & `glances-4.0.6/docs/gw/prometheus.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/restful.rst` & `glances-4.0.6/docs/gw/restful.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/statsd.rst` & `glances-4.0.6/docs/gw/statsd.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/gw/zeromq.rst` & `glances-4.0.6/docs/gw/zeromq.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/index.rst` & `glances-4.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/install.rst` & `glances-4.0.6/docs/install.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/make.bat` & `glances-4.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/man/glances.1` & `glances-4.0.6/docs/man/glances.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "GLANCES" "1" "May 18, 2024" "4.0.5" "Glances"
+.TH "GLANCES" "1" "May 25, 2024" "4.0.6" "Glances"
 .SH NAME
 glances \- An eye on your system
 .SH SYNOPSIS
 .sp
 \fBglances\fP [OPTIONS]
 .SH DESCRIPTION
 .sp
```

### Comparing `glances-4.0.5/docs/objects.inv` & `glances-4.0.6/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/docs/quickstart.rst` & `glances-4.0.6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/__init__.py` & `glances-4.0.6/glances/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import signal
 import sys
 import tracemalloc
 
 # Global name
 # Version should start and end with a numerical char
 # See https://packaging.python.org/specifications/core-metadata/#version
-__version__ = '4.0.5'
+__version__ = '4.0.6'
 __apiversion__ = '4'
 __author__ = 'Nicolas Hennion <nicolas@nicolargo.com>'
 __license__ = 'LGPLv3'
 
 # Import psutil
 try:
     from psutil import __version__ as psutil_version
```

### Comparing `glances-4.0.5/glances/actions.py` & `glances-4.0.6/glances/actions.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/amps/amp.py` & `glances-4.0.6/glances/amps/amp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/amps/default/__init__.py` & `glances-4.0.6/glances/amps/default/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/amps/nginx/__init__.py` & `glances-4.0.6/glances/amps/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/amps/systemd/__init__.py` & `glances-4.0.6/glances/amps/systemd/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/amps/systemv/__init__.py` & `glances-4.0.6/glances/amps/systemv/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/amps_list.py` & `glances-4.0.6/glances/amps_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/attribute.py` & `glances-4.0.6/glances/attribute.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/autodiscover.py` & `glances-4.0.6/glances/autodiscover.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/client.py` & `glances-4.0.6/glances/client.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/client_browser.py` & `glances-4.0.6/glances/client_browser.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/config.py` & `glances-4.0.6/glances/config.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/cpu_percent.py` & `glances-4.0.6/glances/cpu_percent.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/event.py` & `glances-4.0.6/glances/event.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/events_list.py` & `glances-4.0.6/glances/events_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/export.py` & `glances-4.0.6/glances/exports/export.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_cassandra/__init__.py` & `glances-4.0.6/glances/exports/glances_cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_couchdb/__init__.py` & `glances-4.0.6/glances/exports/glances_couchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_csv/__init__.py` & `glances-4.0.6/glances/exports/glances_csv/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_elasticsearch/__init__.py` & `glances-4.0.6/glances/exports/glances_elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_graph/__init__.py` & `glances-4.0.6/glances/exports/glances_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_graphite/__init__.py` & `glances-4.0.6/glances/exports/glances_graphite/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_influxdb/__init__.py` & `glances-4.0.6/glances/exports/glances_influxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_influxdb2/__init__.py` & `glances-4.0.6/glances/exports/glances_influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_json/__init__.py` & `glances-4.0.6/glances/exports/glances_json/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_kafka/__init__.py` & `glances-4.0.6/glances/exports/glances_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_mongodb/__init__.py` & `glances-4.0.6/glances/exports/glances_mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_mqtt/__init__.py` & `glances-4.0.6/glances/exports/glances_mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_opentsdb/__init__.py` & `glances-4.0.6/glances/exports/glances_opentsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_prometheus/__init__.py` & `glances-4.0.6/glances/exports/glances_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_rabbitmq/__init__.py` & `glances-4.0.6/glances/exports/glances_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_restful/__init__.py` & `glances-4.0.6/glances/exports/glances_restful/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_riemann/__init__.py` & `glances-4.0.6/glances/exports/glances_riemann/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_statsd/__init__.py` & `glances-4.0.6/glances/exports/glances_statsd/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/exports/glances_zeromq/__init__.py` & `glances-4.0.6/glances/exports/glances_zeromq/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/filter.py` & `glances-4.0.6/glances/filter.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/folder_list.py` & `glances-4.0.6/glances/folder_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/globals.py` & `glances-4.0.6/glances/globals.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/history.py` & `glances-4.0.6/glances/history.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/logger.py` & `glances-4.0.6/glances/logger.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/main.py` & `glances-4.0.6/glances/main.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outdated.py` & `glances-4.0.6/glances/outdated.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_bars.py` & `glances-4.0.6/glances/outputs/glances_bars.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_curses.py` & `glances-4.0.6/glances/outputs/glances_curses.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_curses_browser.py` & `glances-4.0.6/glances/outputs/glances_curses_browser.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_restful_api.py` & `glances-4.0.6/glances/outputs/glances_restful_api.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_sparklines.py` & `glances-4.0.6/glances/outputs/glances_sparklines.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_stdout.py` & `glances-4.0.6/glances/outputs/glances_stdout.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_stdout_apidoc.py` & `glances-4.0.6/glances/outputs/glances_stdout_apidoc.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_stdout_csv.py` & `glances-4.0.6/glances/outputs/glances_stdout_csv.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_stdout_issue.py` & `glances-4.0.6/glances/outputs/glances_stdout_issue.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_stdout_json.py` & `glances-4.0.6/glances/outputs/glances_stdout_json.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/glances_unicode.py` & `glances-4.0.6/glances/outputs/glances_unicode.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/README.md` & `glances-4.0.6/glances/outputs/static/README.md`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/css/bootstrap.less` & `glances-4.0.6/glances/outputs/static/css/bootstrap.less`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/css/style.scss` & `glances-4.0.6/glances/outputs/static/css/style.scss`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/images/favicon.ico` & `glances-4.0.6/glances/outputs/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/images/glances.png` & `glances-4.0.6/glances/outputs/static/images/glances.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/App.vue` & `glances-4.0.6/glances/outputs/static/js/App.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/help.vue` & `glances-4.0.6/glances/outputs/static/js/components/help.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-alert.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-alert.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-amps.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-amps.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-cloud.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-cloud.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-connections.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-connections.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-containers.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-containers.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-cpu.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-cpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-diskio.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-diskio.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-folders.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-folders.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-fs.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-fs.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-gpu.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-gpu.vue`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,79 @@
 <template>
-    <section id="gpu" class="plugin">
-        <div class="gpu-name title">
-            {{ name }}
-        </div>
-        <div class="table">
-            <div class="table-row" v-if="args.meangpu || gpus.length === 1">
-                <div class="table-cell text-left">proc:</div>
-                <div class="table-cell" :class="getMeanDecoration('proc')" v-if="mean.proc != null">
-                    {{ $filters.number(mean.proc, 0) }}%
-                </div>
-                <div class="table-cell" v-if="mean.proc == null">N/A</div>
+    <section class="plugin" id="gpu" v-if="gpus != undefined">
+        <!-- single gpu -->
+        <template v-if="gpus.length === 1">
+            <div class="title gpu-name">{{ name }}</div>
+            <div class="table">
+                <template v-for="(gpu, gpuId) in gpus" :key="gpuId">
+                    <div class="table-row">
+                        <div class="table-cell text-left">proc:</div>
+                        <div class="table-cell" :class="getDecoration(gpu.gpu_id, 'proc')" v-if="gpu.proc != null">{{ $filters.number(gpu.proc, 0) }}%</div>
+                        <div class="table-cell" v-if="gpu.proc == null">N/A</div>
+                    </div>
+                    <div class="table-row">
+                        <div class="table-cell text-left">mem:</div>
+                        <div class="table-cell" :class="getDecoration(gpu.gpu_id, 'mem')" v-if="gpu.mem != null">{{ $filters.number(gpu.mem, 0) }}%</div>
+                        <div class="table-cell" v-if="gpu.mem == null">N/A</div>
+                    </div>
+                    <div class="table-row">
+                        <div class="table-cell text-left">temp:</div>
+                        <div class="table-cell" :class="getDecoration(gpu.gpu_id, 'temperature')" v-if="gpu.temperature != null">{{ $filters.number(gpu.temperature, 0) }}°C</div>
+                        <div class="table-cell" v-if="gpu.temperature == null">N/A</div>
+                    </div>
+                </template>
             </div>
-            <div class="table-row" v-if="args.meangpu || gpus.length === 1">
-                <div class="table-cell text-left">mem:</div>
-                <div class="table-cell" :class="getMeanDecoration('mem')" v-if="mean.mem != null">
-                    {{ $filters.number(mean.mem, 0) }}%
+        </template>
+
+        <!-- multiple gpus - one line per gpu (no mean) -->
+        <template v-if="!args.meangpu && gpus.length > 1">
+            <div class="title gpu-name">{{ name }}</div>
+            <div class="table">
+                <div class="table-row" v-for="(gpu, gpuId) in gpus" :key="gpuId">
+                    <div class="table-cell text-left">{{ gpu.gpu_id }}:</div>
+                    <div class="table-cell" :class="getDecoration(gpu.gpu_id, 'proc')" v-if="gpu.proc != null">{{ $filters.number(gpu.proc, 0) }}%</div>
+                    <div class="table-cell" v-if="gpu.proc == null">N/A</div>
+                    <div class="table-cell text-left" style="padding-left: 10px">mem:</div>
+                    <div class="table-cell" :class="getDecoration(gpu.gpu_id, 'mem')" v-if="gpu.mem != null">{{ $filters.number(gpu.mem, 0) }}%</div>
+                    <div class="table-cell" v-if="gpu.mem == null">N/A</div>
                 </div>
-                <div class="table-cell" v-if="mean.mem == null">N/A</div>
             </div>
-            <div class="table-row" v-if="args.meangpu || gpus.length === 1">
-                <div class="table-cell text-left">temperature:</div>
-                <div
-                    class="table-cell"
-                    :class="getMeanDecoration('temperature')"
-                    v-if="mean.temperature != null"
-                >
-                    {{ $filters.number(mean.temperature, 0) }}°
+        </template>
+
+        <!-- multiple gpus - mean -->
+        <template v-if="args.meangpu && gpus.length > 1">
+            <div class="title gpu-name">{{ name }}</div>
+            <div class="table">
+                <div class="table-row">
+                    <div class="table-cell text-left">proc mean:</div>
+                    <div class="table-cell" :class="getMeanDecoration('proc')" v-if="mean.proc != null">
+                        {{ $filters.number(mean.proc, 0) }}%
+                    </div>
+                    <div class="table-cell" v-if="mean.proc == null">N/A</div>
                 </div>
-                <div class="table-cell" v-if="mean.temperature == null">N/A</div>
-            </div>
-            <template v-if="!args.meangpu && gpus.length > 1">
-                <div class="table-row" v-for="(gpu, gpuId) in gpus" :key="gpuId">
-                    <div class="table-cell text-left">
-                        {{ gpu.gpu_id }}:
-                        <span :class="getDecoration(gpu.gpu_id, 'proc')" v-if="gpu.proc != null">
-                            {{ $filters.number(gpu.proc, 0) }}%
-                        </span>
-                        <span v-if="gpu.proc == null">N/A</span>
-                        mem:
-                        <span :class="getDecoration(gpu.gpu_id, 'mem')" v-if="gpu.mem != null">
-                            {{ $filters.number(gpu.mem, 0) }}%
-                        </span>
-                        <span v-if="gpu.mem == null">N/A</span>
-                        temp:
-                        <span
-                            :class="getDecoration(gpu.gpu_id, 'temperature')"
-                            v-if="gpu.temperature != null"
-                        >
-                            {{ $filters.number(gpu.temperature, 0) }}C
-                        </span>
-                        <span v-if="gpu.temperature == null">N/A</span>
+                <div class="table-row">
+                    <div class="table-cell text-left">mem mean:</div>
+                    <div class="table-cell" :class="getMeanDecoration('mem')" v-if="mean.mem != null">
+                        {{ $filters.number(mean.mem, 0) }}%
                     </div>
+                    <div class="table-cell" v-if="mean.mem == null">N/A</div>
                 </div>
-            </template>
-        </div>
+                <div class="table-row">
+                    <div class="table-cell text-left">temp mean:</div>
+                    <div
+                        class="table-cell"
+                        :class="getMeanDecoration('temperature')"
+                        v-if="mean.temperature != null"
+                    >
+                        {{ $filters.number(mean.temperature, 0) }}°
+                    </div>
+                    <div class="table-cell" v-if="mean.temperature == null">N/A</div>
+                </div>
+            </div>
+        </template>
     </section>
 </template>
 
 <script>
 import { store } from '../store.js';
 
 export default {
@@ -120,12 +136,12 @@
         getDecoration(gpuId, value) {
             if (this.view[gpuId][value] === undefined) {
                 return;
             }
             return this.view[gpuId][value].decoration.toLowerCase();
         },
         getMeanDecoration(value) {
-            return this.getDecoration(0, value);
+            return 'DEFAULT';
         }
     }
 };
 </script>
```

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-ip.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-ip.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-irq.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-irq.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-load.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-load.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-mem-more.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-mem-more.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-mem.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-mem.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-memswap.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-memswap.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-network.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-network.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-now.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-now.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-percpu.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-percpu.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-ports.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-ports.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-process.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-process.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-processcount.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-processcount.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-processlist.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-processlist.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-quicklook.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-quicklook.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-raid.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-raid.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-sensors.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-sensors.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-smart.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-smart.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-system.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-system.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/components/plugin-wifi.vue` & `glances-4.0.6/glances/outputs/static/js/components/plugin-wifi.vue`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/filters.js` & `glances-4.0.6/glances/outputs/static/js/filters.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/js/services.js` & `glances-4.0.6/glances/outputs/static/js/services.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/package-lock.json` & `glances-4.0.6/glances/outputs/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/package.json` & `glances-4.0.6/glances/outputs/static/package.json`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png` & `glances-4.0.6/glances/outputs/static/public/1272f6e9e8f9d6bfd6de.png`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/public/favicon.ico` & `glances-4.0.6/glances/outputs/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/outputs/static/public/glances.js` & `glances-4.0.6/glances/outputs/static/public/glances.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -15907,69 +15907,114 @@
                         [Ds, !s.args.fs_free_space]
                     ]), On(wi("span", null, pe(e.$filters.bytes(t.free)), 513), [
                         [Ds, s.args.fs_free_space]
                     ])], 2), wi("div", Fd, pe(e.$filters.bytes(t.size)), 1)])))), 128))])
                 }]
             ]),
             Hd = {
-                id: "gpu",
-                class: "plugin"
+                key: 0,
+                class: "plugin",
+                id: "gpu"
             },
             Vd = {
-                class: "gpu-name title"
+                class: "title gpu-name"
             },
             Gd = {
                 class: "table"
             },
             Wd = {
-                key: 0,
                 class: "table-row"
             },
             Zd = wi("div", {
                 class: "table-cell text-left"
             }, "proc:", -1),
             Kd = {
                 key: 1,
                 class: "table-cell"
             },
             Qd = {
-                key: 1,
                 class: "table-row"
             },
             Xd = wi("div", {
                 class: "table-cell text-left"
             }, "mem:", -1),
             Jd = {
                 key: 1,
                 class: "table-cell"
             },
             Yd = {
-                key: 2,
                 class: "table-row"
             },
             ef = wi("div", {
                 class: "table-cell text-left"
-            }, "temperature:", -1),
+            }, "temp:", -1),
             tf = {
                 key: 1,
                 class: "table-cell"
             },
             nf = {
-                class: "table-cell text-left"
+                class: "title gpu-name"
             },
             rf = {
-                key: 1
+                class: "table"
             },
             sf = {
-                key: 3
+                class: "table-cell text-left"
             },
             of = {
-                key: 5
+                key: 1,
+                class: "table-cell"
+            },
+            af = wi("div", {
+                class: "table-cell text-left",
+                style: {
+                    "padding-left": "10px"
+                }
+            }, "mem:", -1),
+            lf = {
+                key: 3,
+                class: "table-cell"
+            },
+            cf = {
+                class: "title gpu-name"
+            },
+            uf = {
+                class: "table"
+            },
+            df = {
+                class: "table-row"
+            },
+            ff = wi("div", {
+                class: "table-cell text-left"
+            }, "proc mean:", -1),
+            pf = {
+                key: 1,
+                class: "table-cell"
+            },
+            hf = {
+                class: "table-row"
+            },
+            gf = wi("div", {
+                class: "table-cell text-left"
+            }, "mem mean:", -1),
+            mf = {
+                key: 1,
+                class: "table-cell"
+            },
+            bf = {
+                class: "table-row"
+            },
+            vf = wi("div", {
+                class: "table-cell text-left"
+            }, "temp mean:", -1),
+            yf = {
+                key: 1,
+                class: "table-cell"
             };
-        const af = {
+        const wf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: Uo
@@ -16008,70 +16053,80 @@
                         return e.proc = e.proc / t.length, e.mem = e.mem / t.length, e.temperature = e.temperature / t.length, e
                     }
                 },
                 methods: {
                     getDecoration(e, t) {
                         if (void 0 !== this.view[e][t]) return this.view[e][t].decoration.toLowerCase()
                     },
-                    getMeanDecoration(e) {
-                        return this.getDecoration(0, e)
-                    }
+                    getMeanDecoration: e => "DEFAULT"
                 }
             },
-            lf = (0, nc.Z)(af, [
+            xf = (0, nc.Z)(wf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Hd, [wi("div", Vd, pe(s.name), 1), wi("div", Gd, [s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Wd, [Zd, null != s.mean.proc ? (li(), pi("div", {
+                    return null != s.gpus ? (li(), pi("section", Hd, [Ti(" single gpu "), 1 === s.gpus.length ? (li(), pi(ni, {
+                        key: 0
+                    }, [wi("div", Vd, pe(s.name), 1), wi("div", Gd, [(li(!0), pi(ni, null, pr(s.gpus, ((t, n) => (li(), pi(ni, {
+                        key: n
+                    }, [wi("div", Wd, [Zd, null != t.proc ? (li(), pi("div", {
                         key: 0,
-                        class: ce(["table-cell", s.getMeanDecoration("proc")])
-                    }, pe(e.$filters.number(s.mean.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.proc ? (li(), pi("div", Kd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Qd, [Xd, null != s.mean.mem ? (li(), pi("div", {
+                        class: ce(["table-cell", s.getDecoration(t.gpu_id, "proc")])
+                    }, pe(e.$filters.number(t.proc, 0)) + "%", 3)) : Ti("v-if", !0), null == t.proc ? (li(), pi("div", Kd, "N/A")) : Ti("v-if", !0)]), wi("div", Qd, [Xd, null != t.mem ? (li(), pi("div", {
                         key: 0,
-                        class: ce(["table-cell", s.getMeanDecoration("mem")])
-                    }, pe(e.$filters.number(s.mean.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.mem ? (li(), pi("div", Jd, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), s.args.meangpu || 1 === s.gpus.length ? (li(), pi("div", Yd, [ef, null != s.mean.temperature ? (li(), pi("div", {
+                        class: ce(["table-cell", s.getDecoration(t.gpu_id, "mem")])
+                    }, pe(e.$filters.number(t.mem, 0)) + "%", 3)) : Ti("v-if", !0), null == t.mem ? (li(), pi("div", Jd, "N/A")) : Ti("v-if", !0)]), wi("div", Yd, [ef, null != t.temperature ? (li(), pi("div", {
                         key: 0,
-                        class: ce(["table-cell", s.getMeanDecoration("temperature")])
-                    }, pe(e.$filters.number(s.mean.temperature, 0)) + "° ", 3)) : Ti("v-if", !0), null == s.mean.temperature ? (li(), pi("div", tf, "N/A")) : Ti("v-if", !0)])) : Ti("v-if", !0), !s.args.meangpu && s.gpus.length > 1 ? (li(!0), pi(ni, {
-                        key: 3
-                    }, pr(s.gpus, ((t, n) => (li(), pi("div", {
+                        class: ce(["table-cell", s.getDecoration(t.gpu_id, "temperature")])
+                    }, pe(e.$filters.number(t.temperature, 0)) + "°C", 3)) : Ti("v-if", !0), null == t.temperature ? (li(), pi("div", tf, "N/A")) : Ti("v-if", !0)])], 64)))), 128))])], 64)) : Ti("v-if", !0), Ti(" multiple gpus - one line per gpu (no mean) "), !s.args.meangpu && s.gpus.length > 1 ? (li(), pi(ni, {
+                        key: 1
+                    }, [wi("div", nf, pe(s.name), 1), wi("div", rf, [(li(!0), pi(ni, null, pr(s.gpus, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", nf, [Si(pe(t.gpu_id) + ": ", 1), null != t.proc ? (li(), pi("span", {
+                    }, [wi("div", sf, pe(t.gpu_id) + ":", 1), null != t.proc ? (li(), pi("div", {
                         key: 0,
-                        class: ce(s.getDecoration(t.gpu_id, "proc"))
-                    }, pe(e.$filters.number(t.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == t.proc ? (li(), pi("span", rf, "N/A")) : Ti("v-if", !0), Si(" mem: "), null != t.mem ? (li(), pi("span", {
+                        class: ce(["table-cell", s.getDecoration(t.gpu_id, "proc")])
+                    }, pe(e.$filters.number(t.proc, 0)) + "%", 3)) : Ti("v-if", !0), null == t.proc ? (li(), pi("div", of, "N/A")) : Ti("v-if", !0), af, null != t.mem ? (li(), pi("div", {
                         key: 2,
-                        class: ce(s.getDecoration(t.gpu_id, "mem"))
-                    }, pe(e.$filters.number(t.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == t.mem ? (li(), pi("span", sf, "N/A")) : Ti("v-if", !0), Si(" temp: "), null != t.temperature ? (li(), pi("span", {
-                        key: 4,
-                        class: ce(s.getDecoration(t.gpu_id, "temperature"))
-                    }, pe(e.$filters.number(t.temperature, 0)) + "C ", 3)) : Ti("v-if", !0), null == t.temperature ? (li(), pi("span", of, "N/A")) : Ti("v-if", !0)])])))), 128)) : Ti("v-if", !0)])])
+                        class: ce(["table-cell", s.getDecoration(t.gpu_id, "mem")])
+                    }, pe(e.$filters.number(t.mem, 0)) + "%", 3)) : Ti("v-if", !0), null == t.mem ? (li(), pi("div", lf, "N/A")) : Ti("v-if", !0)])))), 128))])], 64)) : Ti("v-if", !0), Ti(" multiple gpus - mean "), s.args.meangpu && s.gpus.length > 1 ? (li(), pi(ni, {
+                        key: 2
+                    }, [wi("div", cf, pe(s.name), 1), wi("div", uf, [wi("div", df, [ff, null != s.mean.proc ? (li(), pi("div", {
+                        key: 0,
+                        class: ce(["table-cell", s.getMeanDecoration("proc")])
+                    }, pe(e.$filters.number(s.mean.proc, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.proc ? (li(), pi("div", pf, "N/A")) : Ti("v-if", !0)]), wi("div", hf, [gf, null != s.mean.mem ? (li(), pi("div", {
+                        key: 0,
+                        class: ce(["table-cell", s.getMeanDecoration("mem")])
+                    }, pe(e.$filters.number(s.mean.mem, 0)) + "% ", 3)) : Ti("v-if", !0), null == s.mean.mem ? (li(), pi("div", mf, "N/A")) : Ti("v-if", !0)]), wi("div", bf, [vf, null != s.mean.temperature ? (li(), pi("div", {
+                        key: 0,
+                        class: ce(["table-cell", s.getMeanDecoration("temperature")])
+                    }, pe(e.$filters.number(s.mean.temperature, 0)) + "° ", 3)) : Ti("v-if", !0), null == s.mean.temperature ? (li(), pi("div", yf, "N/A")) : Ti("v-if", !0)])])], 64)) : Ti("v-if", !0)])) : Ti("v-if", !0)
                 }]
             ]),
-            cf = {
+            _f = {
                 key: 0,
                 class: "plugin",
                 id: "ip"
             },
-            uf = {
+            kf = {
                 key: 0,
                 class: "title"
             },
-            df = {
+            Sf = {
                 key: 1
             },
-            ff = {
+            Cf = {
                 key: 2,
                 class: "title"
             },
-            pf = {
+            Tf = {
                 key: 3
             },
-            hf = {
+            Af = {
                 key: 4
             };
-        const gf = {
+        const Ef = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     ipStats() {
@@ -16090,44 +16145,44 @@
                         return this.ipStats.public_address
                     },
                     publicInfo() {
                         return this.ipStats.public_info_human
                     }
                 }
             },
-            mf = (0, nc.Z)(gf, [
+            Of = (0, nc.Z)(Ef, [
                 ["render", function(e, t, n, r, i, s) {
-                    return s.address ? (li(), pi("section", cf, [s.address ? (li(), pi("span", uf, "IP")) : Ti("v-if", !0), s.address ? (li(), pi("span", df, pe(s.address) + "/" + pe(s.maskCdir), 1)) : Ti("v-if", !0), s.publicAddress ? (li(), pi("span", ff, "Pub")) : Ti("v-if", !0), s.publicAddress ? (li(), pi("span", pf, pe(s.publicAddress), 1)) : Ti("v-if", !0), s.publicInfo ? (li(), pi("span", hf, pe(s.publicInfo), 1)) : Ti("v-if", !0)])) : Ti("v-if", !0)
+                    return s.address ? (li(), pi("section", _f, [s.address ? (li(), pi("span", kf, "IP")) : Ti("v-if", !0), s.address ? (li(), pi("span", Sf, pe(s.address) + "/" + pe(s.maskCdir), 1)) : Ti("v-if", !0), s.publicAddress ? (li(), pi("span", Cf, "Pub")) : Ti("v-if", !0), s.publicAddress ? (li(), pi("span", Tf, pe(s.publicAddress), 1)) : Ti("v-if", !0), s.publicInfo ? (li(), pi("span", Af, pe(s.publicInfo), 1)) : Ti("v-if", !0)])) : Ti("v-if", !0)
                 }]
             ]),
-            bf = {
+            If = {
                 class: "plugin",
                 id: "irq"
             },
-            vf = {
+            Pf = {
                 key: 0,
                 class: "table-row"
             },
-            yf = [wi("div", {
+            Nf = [wi("div", {
                 class: "table-cell text-left title"
             }, "IRQ", -1), wi("div", {
                 class: "table-cell"
             }, null, -1), wi("div", {
                 class: "table-cell"
             }, "Rate/s", -1)],
-            wf = {
+            Lf = {
                 class: "table-cell text-left"
             },
-            xf = wi("div", {
+            Df = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            _f = {
+            Mf = {
                 class: "table-cell"
             };
-        const kf = {
+        const jf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16137,61 +16192,61 @@
                         return this.stats.map((e => ({
                             irq_line: e.irq_line,
                             irq_rate: e.irq_rate
                         })))
                     }
                 }
             },
-            Sf = (0, nc.Z)(kf, [
+            Rf = (0, nc.Z)(jf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", bf, [s.irqs.length > 0 ? (li(), pi("div", vf, yf)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.irqs, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", If, [s.irqs.length > 0 ? (li(), pi("div", Pf, Nf)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.irqs, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", wf, pe(e.irq_line), 1), xf, wi("div", _f, [wi("span", null, pe(e.irq_rate), 1)])])))), 128))])
+                    }, [wi("div", Lf, pe(e.irq_line), 1), Df, wi("div", Mf, [wi("span", null, pe(e.irq_rate), 1)])])))), 128))])
                 }]
             ]),
-            Cf = {
+            qf = {
                 key: 0,
                 id: "load",
                 class: "plugin"
             },
-            Tf = {
+            Bf = {
                 class: "table"
             },
-            Af = {
+            Uf = {
                 class: "table-row"
             },
-            Ef = wi("div", {
+            Ff = wi("div", {
                 class: "table-cell text-left title"
             }, "LOAD", -1),
-            Of = {
+            zf = {
                 class: "table-cell"
             },
-            If = {
+            $f = {
                 class: "table-row"
             },
-            Pf = wi("div", {
+            Hf = wi("div", {
                 class: "table-cell text-left"
             }, "1 min:", -1),
-            Nf = {
+            Vf = {
                 class: "table-cell"
             },
-            Lf = {
+            Gf = {
                 class: "table-row"
             },
-            Df = wi("div", {
+            Wf = wi("div", {
                 class: "table-cell text-left"
             }, "5 min:", -1),
-            Mf = {
+            Zf = {
                 class: "table-row"
             },
-            jf = wi("div", {
+            Kf = wi("div", {
                 class: "table-cell text-left"
             }, "15 min:", -1);
-        const Rf = {
+        const Qf = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16215,61 +16270,61 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            qf = (0, nc.Z)(Rf, [
+            Xf = (0, nc.Z)(Qf, [
                 ["render", function(e, t, n, r, i, s) {
-                    return null != s.cpucore ? (li(), pi("section", Cf, [wi("div", Tf, [wi("div", Af, [Ef, wi("div", Of, pe(s.cpucore) + "-core", 1)]), wi("div", If, [Pf, wi("div", Nf, pe(e.$filters.number(s.min1, 2)), 1)]), wi("div", Lf, [Df, wi("div", {
+                    return null != s.cpucore ? (li(), pi("section", qf, [wi("div", Bf, [wi("div", Uf, [Ff, wi("div", zf, pe(s.cpucore) + "-core", 1)]), wi("div", $f, [Hf, wi("div", Vf, pe(e.$filters.number(s.min1, 2)), 1)]), wi("div", Gf, [Wf, wi("div", {
                         class: ce(["table-cell", s.getDecoration("min5")])
-                    }, pe(e.$filters.number(s.min5, 2)), 3)]), wi("div", Mf, [jf, wi("div", {
+                    }, pe(e.$filters.number(s.min5, 2)), 3)]), wi("div", Zf, [Kf, wi("div", {
                         class: ce(["table-cell", s.getDecoration("min15")])
                     }, pe(e.$filters.number(s.min15, 2)), 3)])])])) : Ti("v-if", !0)
                 }]
             ]),
-            Bf = {
+            Jf = {
                 id: "mem",
                 class: "plugin"
             },
-            Uf = {
+            Yf = {
                 class: "table"
             },
-            Ff = {
+            ep = {
                 class: "table-row"
             },
-            zf = wi("div", {
+            tp = wi("div", {
                 class: "table-cell text-left title"
             }, "MEM", -1),
-            $f = {
+            np = {
                 class: "table-row"
             },
-            Hf = wi("div", {
+            rp = wi("div", {
                 class: "table-cell text-left"
             }, "total:", -1),
-            Vf = {
+            ip = {
                 class: "table-cell"
             },
-            Gf = {
+            sp = {
                 class: "table-row"
             },
-            Wf = wi("div", {
+            op = wi("div", {
                 class: "table-cell text-left"
             }, "used:", -1),
-            Zf = {
+            ap = {
                 class: "table-row"
             },
-            Kf = wi("div", {
+            lp = wi("div", {
                 class: "table-cell text-left"
             }, "free:", -1),
-            Qf = {
+            cp = {
                 class: "table-cell"
             };
-        const Xf = {
+        const up = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16293,67 +16348,67 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Jf = (0, nc.Z)(Xf, [
+            dp = (0, nc.Z)(up, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Bf, [wi("div", Uf, [wi("div", Ff, [zf, wi("div", {
+                    return li(), pi("section", Jf, [wi("div", Yf, [wi("div", ep, [tp, wi("div", {
                         class: ce(["table-cell", s.getDecoration("percent")])
-                    }, pe(s.percent) + "%", 3)]), wi("div", $f, [Hf, wi("div", Vf, pe(e.$filters.bytes(s.total)), 1)]), wi("div", Gf, [Wf, wi("div", {
+                    }, pe(s.percent) + "%", 3)]), wi("div", np, [rp, wi("div", ip, pe(e.$filters.bytes(s.total)), 1)]), wi("div", sp, [op, wi("div", {
                         class: ce(["table-cell", s.getDecoration("used")])
-                    }, pe(e.$filters.bytes(s.used, 2)), 3)]), wi("div", Zf, [Kf, wi("div", Qf, pe(e.$filters.bytes(s.free)), 1)])])])
+                    }, pe(e.$filters.bytes(s.used, 2)), 3)]), wi("div", ap, [lp, wi("div", cp, pe(e.$filters.bytes(s.free)), 1)])])])
                 }]
             ]),
-            Yf = {
+            fp = {
                 id: "mem-more",
                 class: "plugin"
             },
-            ep = {
+            pp = {
                 class: "table"
             },
-            tp = {
+            hp = {
                 class: "table-row"
             },
-            np = wi("div", {
+            gp = wi("div", {
                 class: "table-cell text-left"
             }, "active:", -1),
-            rp = {
+            mp = {
                 class: "table-cell"
             },
-            ip = {
+            bp = {
                 class: "table-row"
             },
-            sp = wi("div", {
+            vp = wi("div", {
                 class: "table-cell text-left"
             }, "inactive:", -1),
-            op = {
+            yp = {
                 class: "table-cell"
             },
-            ap = {
+            wp = {
                 class: "table-row"
             },
-            lp = wi("div", {
+            xp = wi("div", {
                 class: "table-cell text-left"
             }, "buffers:", -1),
-            cp = {
+            _p = {
                 class: "table-cell"
             },
-            up = {
+            kp = {
                 class: "table-row"
             },
-            dp = wi("div", {
+            Sp = wi("div", {
                 class: "table-cell text-left"
             }, "cached:", -1),
-            fp = {
+            Cp = {
                 class: "table-cell"
             };
-        const pp = {
+        const Tp = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16369,65 +16424,65 @@
                         return this.stats.buffers
                     },
                     cached() {
                         return this.stats.cached
                     }
                 }
             },
-            hp = (0, nc.Z)(pp, [
+            Ap = (0, nc.Z)(Tp, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Yf, [wi("div", ep, [On(wi("div", tp, [np, wi("div", rp, pe(e.$filters.bytes(s.active)), 1)], 512), [
+                    return li(), pi("section", fp, [wi("div", pp, [On(wi("div", hp, [gp, wi("div", mp, pe(e.$filters.bytes(s.active)), 1)], 512), [
                         [Ds, null != s.active]
-                    ]), On(wi("div", ip, [sp, wi("div", op, pe(e.$filters.bytes(s.inactive)), 1)], 512), [
+                    ]), On(wi("div", bp, [vp, wi("div", yp, pe(e.$filters.bytes(s.inactive)), 1)], 512), [
                         [Ds, null != s.inactive]
-                    ]), On(wi("div", ap, [lp, wi("div", cp, pe(e.$filters.bytes(s.buffers)), 1)], 512), [
+                    ]), On(wi("div", wp, [xp, wi("div", _p, pe(e.$filters.bytes(s.buffers)), 1)], 512), [
                         [Ds, null != s.buffers]
-                    ]), On(wi("div", up, [dp, wi("div", fp, pe(e.$filters.bytes(s.cached)), 1)], 512), [
+                    ]), On(wi("div", kp, [Sp, wi("div", Cp, pe(e.$filters.bytes(s.cached)), 1)], 512), [
                         [Ds, null != s.cached]
                     ])])])
                 }]
             ]),
-            gp = {
+            Ep = {
                 id: "memswap",
                 class: "plugin"
             },
-            mp = {
+            Op = {
                 class: "table"
             },
-            bp = {
+            Ip = {
                 class: "table-row"
             },
-            vp = wi("div", {
+            Pp = wi("div", {
                 class: "table-cell text-left title"
             }, "SWAP", -1),
-            yp = {
+            Np = {
                 class: "table-row"
             },
-            wp = wi("div", {
+            Lp = wi("div", {
                 class: "table-cell text-left"
             }, "total:", -1),
-            xp = {
+            Dp = {
                 class: "table-cell"
             },
-            _p = {
+            Mp = {
                 class: "table-row"
             },
-            kp = wi("div", {
+            jp = wi("div", {
                 class: "table-cell text-left"
             }, "used:", -1),
-            Sp = {
+            Rp = {
                 class: "table-row"
             },
-            Cp = wi("div", {
+            qp = wi("div", {
                 class: "table-cell text-left"
             }, "free:", -1),
-            Tp = {
+            Bp = {
                 class: "table-cell"
             };
-        const Ap = {
+        const Up = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16451,73 +16506,73 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            Ep = (0, nc.Z)(Ap, [
+            Fp = (0, nc.Z)(Up, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", gp, [wi("div", mp, [wi("div", bp, [vp, wi("div", {
+                    return li(), pi("section", Ep, [wi("div", Op, [wi("div", Ip, [Pp, wi("div", {
                         class: ce(["table-cell", s.getDecoration("percent")])
-                    }, pe(s.percent) + "%", 3)]), wi("div", yp, [wp, wi("div", xp, pe(e.$filters.bytes(s.total)), 1)]), wi("div", _p, [kp, wi("div", {
+                    }, pe(s.percent) + "%", 3)]), wi("div", Np, [Lp, wi("div", Dp, pe(e.$filters.bytes(s.total)), 1)]), wi("div", Mp, [jp, wi("div", {
                         class: ce(["table-cell", s.getDecoration("used")])
-                    }, pe(e.$filters.bytes(s.used)), 3)]), wi("div", Sp, [Cp, wi("div", Tp, pe(e.$filters.bytes(s.free)), 1)])])])
+                    }, pe(e.$filters.bytes(s.used)), 3)]), wi("div", Rp, [qp, wi("div", Bp, pe(e.$filters.bytes(s.free)), 1)])])])
                 }]
             ]),
-            Op = {
+            zp = {
                 class: "plugin",
                 id: "network"
             },
-            Ip = {
+            $p = {
                 class: "table-row"
             },
-            Pp = wi("div", {
+            Hp = wi("div", {
                 class: "table-cell text-left title"
             }, "NETWORK", -1),
-            Np = {
+            Vp = {
                 class: "table-cell"
             },
-            Lp = {
+            Gp = {
                 class: "table-cell"
             },
-            Dp = {
+            Wp = {
                 class: "table-cell"
             },
-            Mp = {
+            Zp = {
                 class: "table-cell"
             },
-            jp = {
+            Kp = {
                 class: "table-cell"
             },
-            Rp = {
+            Qp = {
                 class: "table-cell"
             },
-            qp = {
+            Xp = {
                 class: "table-cell"
             },
-            Bp = {
+            Jp = {
                 class: "table-cell"
             },
-            Up = {
+            Yp = {
                 class: "table-cell text-left"
             },
-            Fp = {
+            eh = {
                 class: "visible-lg-inline"
             },
-            zp = {
+            th = {
                 class: "hidden-lg"
             },
-            $p = {
+            nh = {
                 class: "table-cell"
             },
-            Hp = {
+            rh = {
                 class: "table-cell"
             };
-        const Vp = {
+        const ih = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: Uo
@@ -16543,124 +16598,124 @@
                                 bytes_all: e.bytes_all
                             }
                         }));
                         return (0, dc.orderBy)(e, ["interfaceName"])
                     }
                 }
             },
-            Gp = (0, nc.Z)(Vp, [
+            sh = (0, nc.Z)(ih, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Op, [wi("div", Ip, [Pp, On(wi("div", Np, "Rx/s", 512), [
+                    return li(), pi("section", zp, [wi("div", $p, [Hp, On(wi("div", Vp, "Rx/s", 512), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Lp, "Tx/s", 512), [
+                    ]), On(wi("div", Gp, "Tx/s", 512), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Dp, null, 512), [
+                    ]), On(wi("div", Wp, null, 512), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
-                    ]), On(wi("div", Mp, "Rx+Tx/s", 512), [
+                    ]), On(wi("div", Zp, "Rx+Tx/s", 512), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
-                    ]), On(wi("div", jp, "Rx", 512), [
+                    ]), On(wi("div", Kp, "Rx", 512), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Rp, "Tx", 512), [
+                    ]), On(wi("div", Qp, "Tx", 512), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", qp, null, 512), [
+                    ]), On(wi("div", Xp, null, 512), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
-                    ]), On(wi("div", Bp, "Rx+Tx", 512), [
+                    ]), On(wi("div", Jp, "Rx+Tx", 512), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
                     ])]), (li(!0), pi(ni, null, pr(s.networks, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", Up, [wi("span", Fp, pe(t.ifname), 1), wi("span", zp, pe(e.$filters.minSize(t.ifname)), 1)]), On(wi("div", {
+                    }, [wi("div", Yp, [wi("span", eh, pe(t.ifname), 1), wi("span", th, pe(e.$filters.minSize(t.ifname)), 1)]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.bytes_recv_rate_per_sec) : e.$filters.bits(t.bytes_recv_rate_per_sec)), 513), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.bytes_sent_rate_per_sec) : e.$filters.bits(t.bytes_sent_rate_per_sec)), 513), [
                         [Ds, !s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", $p, null, 512), [
+                    ]), On(wi("div", nh, null, 512), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.bytes_all_rate_per_sec) : e.$filters.bits(t.bytes_all_rate_per_sec)), 513), [
                         [Ds, !s.args.network_cumul && s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.bytes_recv) : e.$filters.bits(t.bytes_recv)), 513), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.bytes_sent) : e.$filters.bits(t.bytes_sent)), 513), [
                         [Ds, s.args.network_cumul && !s.args.network_sum]
-                    ]), On(wi("div", Hp, null, 512), [
+                    ]), On(wi("div", rh, null, 512), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(s.args.byte ? e.$filters.bytes(t.bytes_all) : e.$filters.bits(t.bytes_all)), 513), [
                         [Ds, s.args.network_cumul && s.args.network_sum]
                     ])])))), 128))])
                 }]
             ]),
-            Wp = {
+            oh = {
                 id: "now",
                 class: "plugin"
             },
-            Zp = {
+            ah = {
                 class: "table-row"
             },
-            Kp = {
+            lh = {
                 class: "table-cell text-left"
             };
-        const Qp = {
+        const ch = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     date_iso() {
                         return this.data.stats.now.iso
                     }
                 },
                 methods: {
                     localDate: e => new Date(e).toLocaleString()
                 }
             },
-            Xp = (0, nc.Z)(Qp, [
+            uh = (0, nc.Z)(ch, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Wp, [wi("div", Zp, [wi("div", Kp, pe(s.localDate(s.date_iso)), 1)])])
+                    return li(), pi("section", oh, [wi("div", ah, [wi("div", lh, pe(s.localDate(s.date_iso)), 1)])])
                 }]
             ]),
-            Jp = {
+            dh = {
                 id: "percpu",
                 class: "plugin"
             },
-            Yp = {
+            fh = {
                 class: "table"
             },
-            eh = {
+            ph = {
                 class: "table-row"
             },
-            th = {
+            hh = {
                 key: 0,
                 class: "table-cell text-left title"
             },
-            nh = {
+            gh = {
                 key: 1,
                 class: "table-cell"
             },
-            rh = Ci('<div class="table-cell">user</div><div class="table-cell">system</div><div class="table-cell">idle</div><div class="table-cell">iowait</div><div class="table-cell">steal</div>', 5),
-            ih = {
+            mh = Ci('<div class="table-cell">user</div><div class="table-cell">system</div><div class="table-cell">idle</div><div class="table-cell">iowait</div><div class="table-cell">steal</div>', 5),
+            bh = {
                 key: 0,
                 class: "table-cell text-left"
             },
-            sh = {
+            vh = {
                 key: 1,
                 class: "table-cell"
             };
-        const oh = {
+        const yh = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: Uo
@@ -16678,20 +16733,20 @@
                 },
                 methods: {
                     getUserAlert: e => $o.getAlert("percpu", "percpu_user_", e.user),
                     getSystemAlert: e => $o.getAlert("percpu", "percpu_system_", e.system),
                     getIOWaitAlert: e => $o.getAlert("percpu", "percpu_iowait_", e.system)
                 }
             },
-            ah = (0, nc.Z)(oh, [
+            wh = (0, nc.Z)(yh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Jp, [wi("div", Yp, [wi("div", eh, [s.args.disable_quicklook ? (li(), pi("div", th, "CPU")) : Ti("v-if", !0), s.args.disable_quicklook ? (li(), pi("div", nh, "total")) : Ti("v-if", !0), rh]), (li(!0), pi(ni, null, pr(s.percpuStats, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", dh, [wi("div", fh, [wi("div", ph, [s.args.disable_quicklook ? (li(), pi("div", hh, "CPU")) : Ti("v-if", !0), s.args.disable_quicklook ? (li(), pi("div", gh, "total")) : Ti("v-if", !0), mh]), (li(!0), pi(ni, null, pr(s.percpuStats, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [s.args.disable_quicklook ? (li(), pi("div", ih, " CPU" + pe(e.cpu_number), 1)) : Ti("v-if", !0), s.args.disable_quicklook ? (li(), pi("div", sh, pe(e.total) + "% ", 1)) : Ti("v-if", !0), wi("div", {
+                    }, [s.args.disable_quicklook ? (li(), pi("div", bh, " CPU" + pe(e.cpu_number), 1)) : Ti("v-if", !0), s.args.disable_quicklook ? (li(), pi("div", vh, pe(e.total) + "% ", 1)) : Ti("v-if", !0), wi("div", {
                         class: ce(["table-cell", s.getUserAlert(e)])
                     }, pe(e.user) + "% ", 3), wi("div", {
                         class: ce(["table-cell", s.getSystemAlert(e)])
                     }, pe(e.system) + "% ", 3), On(wi("div", {
                         class: "table-cell"
                     }, pe(e.idle) + "% ", 513), [
                         [Ds, null != e.idle]
@@ -16702,46 +16757,46 @@
                     ]), On(wi("div", {
                         class: "table-cell"
                     }, pe(e.steal) + "% ", 513), [
                         [Ds, null != e.steal]
                     ])])))), 128))])])
                 }]
             ]),
-            lh = {
+            xh = {
                 class: "plugin",
                 id: "ports"
             },
-            ch = {
+            _h = {
                 class: "table-cell text-left"
             },
-            uh = wi("div", {
+            kh = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            dh = {
+            Sh = {
                 key: 0
             },
-            fh = {
+            Ch = {
                 key: 1
             },
-            ph = {
+            Th = {
                 key: 2
             },
-            hh = {
+            Ah = {
                 key: 3
             },
-            gh = {
+            Eh = {
                 key: 0
             },
-            mh = {
+            Oh = {
                 key: 1
             },
-            bh = {
+            Ih = {
                 key: 2
             };
-        const vh = {
+        const Ph = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16752,54 +16807,54 @@
                     }
                 },
                 methods: {
                     getPortDecoration: e => null === e.status ? "careful" : !1 === e.status ? "critical" : null !== e.rtt_warning && e.status > e.rtt_warning ? "warning" : "ok",
                     getWebDecoration: e => null === e.status ? "careful" : -1 === [200, 301, 302].indexOf(e.status) ? "critical" : null !== e.rtt_warning && e.elapsed > e.rtt_warning ? "warning" : "ok"
                 }
             },
-            yh = (0, nc.Z)(vh, [
+            Nh = (0, nc.Z)(Ph, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", lh, [(li(!0), pi(ni, null, pr(s.ports, ((t, n) => (li(), pi("div", {
+                    return li(), pi("section", xh, [(li(!0), pi(ni, null, pr(s.ports, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", ch, [Ti(" prettier-ignore "), Si(" " + pe(e.$filters.minSize(t.description ? t.description : t.host + " " + t.port, 20)), 1)]), uh, t.host ? (li(), pi("div", {
+                    }, [wi("div", _h, [Ti(" prettier-ignore "), Si(" " + pe(e.$filters.minSize(t.description ? t.description : t.host + " " + t.port, 20)), 1)]), kh, t.host ? (li(), pi("div", {
                         key: 0,
                         class: ce([s.getPortDecoration(t), "table-cell"])
-                    }, ["null" == t.status ? (li(), pi("span", dh, "Scanning")) : "false" == t.status ? (li(), pi("span", fh, "Timeout")) : "true" == t.status ? (li(), pi("span", ph, "Open")) : (li(), pi("span", hh, pe(e.$filters.number(1e3 * t.status, 0)) + "ms", 1))], 2)) : Ti("v-if", !0), t.url ? (li(), pi("div", {
+                    }, ["null" == t.status ? (li(), pi("span", Sh, "Scanning")) : "false" == t.status ? (li(), pi("span", Ch, "Timeout")) : "true" == t.status ? (li(), pi("span", Th, "Open")) : (li(), pi("span", Ah, pe(e.$filters.number(1e3 * t.status, 0)) + "ms", 1))], 2)) : Ti("v-if", !0), t.url ? (li(), pi("div", {
                         key: 1,
                         class: ce([s.getWebDecoration(t), "table-cell"])
-                    }, ["null" == t.status ? (li(), pi("span", gh, "Scanning")) : "Error" == t.status ? (li(), pi("span", mh, "Error")) : (li(), pi("span", bh, "Code " + pe(t.status), 1))], 2)) : Ti("v-if", !0)])))), 128))])
+                    }, ["null" == t.status ? (li(), pi("span", Eh, "Scanning")) : "Error" == t.status ? (li(), pi("span", Oh, "Error")) : (li(), pi("span", Ih, "Code " + pe(t.status), 1))], 2)) : Ti("v-if", !0)])))), 128))])
                 }]
             ]),
-            wh = {
+            Lh = {
                 key: 0
             },
-            xh = {
+            Dh = {
                 key: 1
             },
-            _h = {
+            Mh = {
                 key: 0,
                 class: "row"
             },
-            kh = {
+            jh = {
                 class: "col-lg-18"
             };
-        const Sh = {
+        const Rh = {
                 id: "amps",
                 class: "plugin"
             },
-            Ch = {
+            qh = {
                 class: "table"
             },
-            Th = {
+            Bh = {
                 key: 0,
                 class: "table-cell text-left"
             },
-            Ah = ["innerHTML"];
-        const Eh = {
+            Uh = ["innerHTML"];
+        const Fh = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -16815,38 +16870,38 @@
                             n = e.countmin,
                             r = e.countmax;
                         let i = "ok";
                         return i = t > 0 ? (null === n || t >= n) && (null === r || t <= r) ? "ok" : "careful" : null === n ? "ok" : "critical", i
                     }
                 }
             },
-            Oh = (0, nc.Z)(Eh, [
+            zh = (0, nc.Z)(Fh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Sh, [wi("div", Ch, [(li(!0), pi(ni, null, pr(s.processes, ((t, n) => (li(), pi("div", {
+                    return li(), pi("section", Rh, [wi("div", qh, [(li(!0), pi(ni, null, pr(s.processes, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
                     }, [wi("div", {
                         class: ce(["table-cell text-left", s.getNameDecoration(t)])
-                    }, pe(t.name), 3), t.regex ? (li(), pi("div", Th, pe(t.count), 1)) : Ti("v-if", !0), wi("div", {
+                    }, pe(t.name), 3), t.regex ? (li(), pi("div", Bh, pe(t.count), 1)) : Ti("v-if", !0), wi("div", {
                         class: "table-cell text-left process-result",
                         innerHTML: e.$filters.nl2br(t.result)
-                    }, null, 8, Ah)])))), 128))])])
+                    }, null, 8, Uh)])))), 128))])])
                 }]
             ]),
-            Ih = {
+            $h = {
                 id: "processcount",
                 class: "plugin"
             },
-            Ph = wi("span", {
+            Hh = wi("span", {
                 class: "title"
             }, "TASKS", -1),
-            Nh = {
+            Vh = {
                 class: "title"
             };
-        const Lh = {
+        const Gh = {
                 props: {
                     data: {
                         type: Object
                     },
                     sorter: {
                         type: Object
                     }
@@ -16874,68 +16929,68 @@
                         return this.stats.stopped || 0
                     },
                     thread() {
                         return this.stats.thread || 0
                     }
                 }
             },
-            Dh = (0, nc.Z)(Lh, [
+            Wh = (0, nc.Z)(Gh, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Ih, [Ph, wi("span", null, pe(s.total) + " (" + pe(s.thread) + " thr),", 1), wi("span", null, pe(s.running) + " run,", 1), wi("span", null, pe(s.sleeping) + " slp,", 1), wi("span", null, pe(s.stopped) + " oth", 1), wi("span", null, pe(s.args.programs ? "Programs" : "Threads"), 1), wi("span", Nh, pe(n.sorter.auto ? "sorted automatically" : "sorted"), 1), wi("span", null, "by " + pe(n.sorter.getColumnLabel(n.sorter.column)), 1)])
+                    return li(), pi("section", $h, [Hh, wi("span", null, pe(s.total) + " (" + pe(s.thread) + " thr),", 1), wi("span", null, pe(s.running) + " run,", 1), wi("span", null, pe(s.sleeping) + " slp,", 1), wi("span", null, pe(s.stopped) + " oth", 1), wi("span", null, pe(s.args.programs ? "Programs" : "Threads"), 1), wi("span", Vh, pe(n.sorter.auto ? "sorted automatically" : "sorted"), 1), wi("span", null, "by " + pe(n.sorter.getColumnLabel(n.sorter.column)), 1)])
                 }]
             ]),
-            Mh = {
+            Zh = {
                 id: "processlist-plugin",
                 class: "plugin"
             },
-            jh = {
+            Kh = {
                 class: "table"
             },
-            Rh = {
+            Qh = {
                 class: "table-row"
             },
-            qh = wi("div", {
+            Xh = wi("div", {
                 class: "table-cell width-80 hidden-xs hidden-sm"
             }, "VIRT", -1),
-            Bh = wi("div", {
+            Jh = wi("div", {
                 class: "table-cell width-80 hidden-xs hidden-sm"
             }, "RES", -1),
-            Uh = wi("div", {
+            Yh = wi("div", {
                 class: "table-cell width-80"
             }, "PID", -1),
-            Fh = wi("div", {
+            eg = wi("div", {
                 class: "table-cell width-60"
             }, "NI", -1),
-            zh = wi("div", {
+            tg = wi("div", {
                 class: "table-cell width-60"
             }, "S", -1),
-            $h = {
+            ng = {
                 class: "table-cell width-80"
             },
-            Hh = {
+            rg = {
                 class: "table-cell width-80"
             },
-            Vh = {
+            ig = {
                 class: "table-cell width-80"
             },
-            Gh = {
+            sg = {
                 class: "table-cell width-100 text-left"
             },
-            Wh = {
+            og = {
                 key: 0,
                 class: "table-cell width-100 hidden-xs hidden-sm"
             },
-            Zh = {
+            ag = {
                 key: 1,
                 class: "table-cell width-80 hidden-xs hidden-sm"
             },
-            Kh = {
+            lg = {
                 class: "table-cell width-80 text-left hidden-xs hidden-sm"
             };
-        const Qh = {
+        const cg = {
                 props: {
                     data: {
                         type: Object
                     },
                     sorter: {
                         type: Object
                     }
@@ -16969,36 +17024,36 @@
                     }
                 },
                 methods: {
                     getCpuPercentAlert: e => $o.getAlert("processlist", "processlist_cpu_", e.cpu_percent),
                     getMemoryPercentAlert: e => $o.getAlert("processlist", "processlist_mem_", e.cpu_percent)
                 }
             },
-            Xh = {
+            ug = {
                 components: {
-                    GlancesPluginAmps: Oh,
-                    GlancesPluginProcesscount: Dh,
-                    GlancesPluginProcesslist: (0, nc.Z)(Qh, [
+                    GlancesPluginAmps: zh,
+                    GlancesPluginProcesscount: Wh,
+                    GlancesPluginProcesslist: (0, nc.Z)(cg, [
                         ["render", function(e, t, n, r, i, s) {
-                            return li(), pi(ni, null, [Ti(" prettier-ignore "), wi("section", Mh, [wi("div", jh, [wi("div", Rh, [wi("div", {
+                            return li(), pi(ni, null, [Ti(" prettier-ignore "), wi("section", Zh, [wi("div", Kh, [wi("div", Qh, [wi("div", {
                                 class: ce(["table-cell width-60", ["sortable", "cpu_percent" === n.sorter.column && "sort"]]),
                                 onClick: t[0] || (t[0] = t => e.$emit("update:sorter", "cpu_percent"))
                             }, " CPU% ", 2), wi("div", {
                                 class: ce(["table-cell width-60", ["sortable", "memory_percent" === n.sorter.column && "sort"]]),
                                 onClick: t[1] || (t[1] = t => e.$emit("update:sorter", "memory_percent"))
-                            }, " MEM% ", 2), qh, Bh, Uh, wi("div", {
+                            }, " MEM% ", 2), Xh, Jh, Yh, wi("div", {
                                 class: ce(["table-cell width-100 text-left", ["sortable", "username" === n.sorter.column && "sort"]]),
                                 onClick: t[2] || (t[2] = t => e.$emit("update:sorter", "username"))
                             }, " USER ", 2), wi("div", {
                                 class: ce(["table-cell width-100 hidden-xs hidden-sm", ["sortable", "timemillis" === n.sorter.column && "sort"]]),
                                 onClick: t[3] || (t[3] = t => e.$emit("update:sorter", "timemillis"))
                             }, " TIME+ ", 2), wi("div", {
                                 class: ce(["table-cell width-80 text-left hidden-xs hidden-sm", ["sortable", "num_threads" === n.sorter.column && "sort"]]),
                                 onClick: t[4] || (t[4] = t => e.$emit("update:sorter", "num_threads"))
-                            }, " THR ", 2), Fh, zh, On(wi("div", {
+                            }, " THR ", 2), eg, tg, On(wi("div", {
                                 class: ce(["table-cell width-80 hidden-xs hidden-sm", ["sortable", "io_counters" === n.sorter.column && "sort"]]),
                                 onClick: t[5] || (t[5] = t => e.$emit("update:sorter", "io_counters"))
                             }, " IOR/s ", 2), [
                                 [Ds, s.ioReadWritePresent]
                             ]), On(wi("div", {
                                 class: ce(["table-cell width-80 text-left hidden-xs hidden-sm", ["sortable", "io_counters" === n.sorter.column && "sort"]]),
                                 onClick: t[6] || (t[6] = t => e.$emit("update:sorter", "io_counters"))
@@ -17010,21 +17065,21 @@
                             }, " Command ", 2)]), (li(!0), pi(ni, null, pr(s.processes, ((t, n) => (li(), pi("div", {
                                 class: "table-row",
                                 key: n
                             }, [wi("div", {
                                 class: ce(["table-cell width-60", s.getCpuPercentAlert(t)])
                             }, pe(-1 == t.cpu_percent ? "?" : e.$filters.number(t.cpu_percent, 1)), 3), wi("div", {
                                 class: ce(["table-cell width-60", s.getMemoryPercentAlert(t)])
-                            }, pe(-1 == t.memory_percent ? "?" : e.$filters.number(t.memory_percent, 1)), 3), wi("div", $h, pe(e.$filters.bytes(t.memvirt)), 1), wi("div", Hh, pe(e.$filters.bytes(t.memres)), 1), wi("div", Vh, pe(t.pid), 1), wi("div", Gh, pe(t.username), 1), "?" != t.timeplus ? (li(), pi("div", Wh, [On(wi("span", {
+                            }, pe(-1 == t.memory_percent ? "?" : e.$filters.number(t.memory_percent, 1)), 3), wi("div", ng, pe(e.$filters.bytes(t.memvirt)), 1), wi("div", rg, pe(e.$filters.bytes(t.memres)), 1), wi("div", ig, pe(t.pid), 1), wi("div", sg, pe(t.username), 1), "?" != t.timeplus ? (li(), pi("div", og, [On(wi("span", {
                                 class: "highlight"
                             }, pe(t.timeplus.hours) + "h", 513), [
                                 [Ds, t.timeplus.hours > 0]
                             ]), Si(" " + pe(e.$filters.leftPad(t.timeplus.minutes, 2, "0")) + ":" + pe(e.$filters.leftPad(t.timeplus.seconds, 2, "0")) + " ", 1), On(wi("span", null, "." + pe(e.$filters.leftPad(t.timeplus.milliseconds, 2, "0")), 513), [
                                 [Ds, t.timeplus.hours <= 0]
-                            ])])) : Ti("v-if", !0), "?" == t.timeplus ? (li(), pi("div", Zh, "?")) : Ti("v-if", !0), wi("div", Kh, pe(-1 == t.num_threads ? "?" : t.num_threads), 1), wi("div", {
+                            ])])) : Ti("v-if", !0), "?" == t.timeplus ? (li(), pi("div", ag, "?")) : Ti("v-if", !0), wi("div", lg, pe(-1 == t.num_threads ? "?" : t.num_threads), 1), wi("div", {
                                 class: ce(["table-cell width-60", {
                                     nice: t.isNice
                                 }])
                             }, pe(e.$filters.exclamation(t.nice)), 3), wi("div", {
                                 class: ce(["table-cell width-60", {
                                     status: "R" == t.status
                                 }])
@@ -17088,88 +17143,88 @@
                                     } [e] || e
                                 }
                             })
                         }
                     }
                 }
             },
-            Jh = (0, nc.Z)(Xh, [
+            dg = (0, nc.Z)(ug, [
                 ["render", function(e, t, n, r, i, s) {
                     const o = cr("glances-plugin-processcount"),
                         a = cr("glances-plugin-amps"),
                         l = cr("glances-plugin-processlist");
-                    return s.args.disable_process ? (li(), pi("div", wh, "PROCESSES DISABLED (press 'z' to display)")) : (li(), pi("div", xh, [xi(o, {
+                    return s.args.disable_process ? (li(), pi("div", Lh, "PROCESSES DISABLED (press 'z' to display)")) : (li(), pi("div", Dh, [xi(o, {
                         sorter: i.sorter,
                         data: n.data
-                    }, null, 8, ["sorter", "data"]), s.args.disable_amps ? Ti("v-if", !0) : (li(), pi("div", _h, [wi("div", kh, [xi(a, {
+                    }, null, 8, ["sorter", "data"]), s.args.disable_amps ? Ti("v-if", !0) : (li(), pi("div", Mh, [wi("div", jh, [xi(a, {
                         data: n.data
                     }, null, 8, ["data"])])])), xi(l, {
                         sorter: i.sorter,
                         data: n.data,
                         "onUpdate:sorter": t[0] || (t[0] = e => s.args.sort_processes_key = e)
                     }, null, 8, ["sorter", "data"])]))
                 }]
             ]),
-            Yh = {
+            fg = {
                 id: "quicklook",
                 class: "plugin"
             },
-            eg = {
+            pg = {
                 class: "cpu-name text-left"
             },
-            tg = {
+            hg = {
                 class: "table"
             },
-            ng = {
+            gg = {
                 key: 0,
                 class: "table-row"
             },
-            rg = wi("div", {
+            mg = wi("div", {
                 class: "table-cell text-left"
             }, "CPU", -1),
-            ig = {
+            bg = {
                 class: "table-cell"
             },
-            sg = {
+            vg = {
                 class: "progress"
             },
-            og = ["aria-valuenow"],
-            ag = {
+            yg = ["aria-valuenow"],
+            wg = {
                 class: "table-cell"
             },
-            lg = {
+            xg = {
                 class: "table-cell text-left"
             },
-            cg = {
+            _g = {
                 class: "table-cell"
             },
-            ug = {
+            kg = {
                 class: "progress"
             },
-            dg = ["aria-valuenow"],
-            fg = {
+            Sg = ["aria-valuenow"],
+            Cg = {
                 class: "table-cell"
             },
-            pg = {
+            Tg = {
                 class: "table-row"
             },
-            hg = {
+            Ag = {
                 class: "table-cell text-left"
             },
-            gg = {
+            Eg = {
                 class: "table-cell"
             },
-            mg = {
+            Og = {
                 class: "progress"
             },
-            bg = ["aria-valuenow"],
-            vg = {
+            Ig = ["aria-valuenow"],
+            Pg = {
                 class: "table-cell"
             };
-        const yg = {
+        const Ng = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: Uo
@@ -17228,67 +17283,67 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e]) return this.view[e].decoration.toLowerCase()
                     }
                 }
             },
-            wg = (0, nc.Z)(yg, [
+            Lg = (0, nc.Z)(Ng, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Yh, [wi("div", eg, pe(s.cpu_name), 1), Ti(' <div class="cpu-freq text-right" v-if="cpu_hz_current">\n            {{ cpu_hz_current }}/{{ cpu_hz }}Ghz\n        </div> '), wi("div", tg, [s.args.percpu ? Ti("v-if", !0) : (li(), pi("div", ng, [rg, wi("div", ig, [wi("div", sg, [wi("div", {
+                    return li(), pi("section", fg, [wi("div", pg, pe(s.cpu_name), 1), Ti(' <div class="cpu-freq text-right" v-if="cpu_hz_current">\n            {{ cpu_hz_current }}/{{ cpu_hz }}Ghz\n        </div> '), wi("div", hg, [s.args.percpu ? Ti("v-if", !0) : (li(), pi("div", gg, [mg, wi("div", bg, [wi("div", vg, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration("cpu")}`),
                         role: "progressbar",
                         "aria-valuenow": s.cpu,
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${s.cpu}%;`)
-                    }, "   ", 14, og)])]), wi("div", ag, pe(s.cpu) + "%", 1)])), s.args.percpu ? (li(!0), pi(ni, {
+                    }, "   ", 14, yg)])]), wi("div", wg, pe(s.cpu) + "%", 1)])), s.args.percpu ? (li(!0), pi(ni, {
                         key: 1
                     }, pr(s.percpus, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", lg, "CPU" + pe(e.number), 1), wi("div", cg, [wi("div", ug, [wi("div", {
+                    }, [wi("div", xg, "CPU" + pe(e.number), 1), wi("div", _g, [wi("div", kg, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration("cpu")}`),
                         role: "progressbar",
                         "aria-valuenow": e.total,
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${e.total}%;`)
-                    }, "   ", 14, dg)])]), wi("div", fg, pe(e.total) + "%", 1)])))), 128)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.stats_list_after_cpu, (e => (li(), pi("div", pg, [wi("div", hg, pe(e.toUpperCase()), 1), wi("div", gg, [wi("div", mg, [wi("div", {
+                    }, "   ", 14, Sg)])]), wi("div", Cg, pe(e.total) + "%", 1)])))), 128)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.stats_list_after_cpu, (e => (li(), pi("div", Tg, [wi("div", Ag, pe(e.toUpperCase()), 1), wi("div", Eg, [wi("div", Og, [wi("div", {
                         class: ce(`progress-bar progress-bar-${s.getDecoration(e)}`),
                         role: "progressbar",
                         "aria-valuenow": s.stats[e],
                         "aria-valuemin": "0",
                         "aria-valuemax": "100",
                         style: ie(`width: ${s.stats[e]}%;`)
-                    }, "   ", 14, bg)])]), wi("div", vg, pe(s.stats[e]) + "%", 1)])))), 256))])])
+                    }, "   ", 14, Ig)])]), wi("div", Pg, pe(s.stats[e]) + "%", 1)])))), 256))])])
                 }]
             ]),
-            xg = {
+            Dg = {
                 class: "plugin",
                 id: "raid"
             },
-            _g = {
+            Mg = {
                 key: 0,
                 class: "table-row"
             },
-            kg = [wi("div", {
+            jg = [wi("div", {
                 class: "table-cell text-left title"
             }, "RAID disks", -1), wi("div", {
                 class: "table-cell"
             }, "Used", -1), wi("div", {
                 class: "table-cell"
             }, "Total", -1)],
-            Sg = {
+            Rg = {
                 class: "table-cell text-left"
             },
-            Cg = {
+            qg = {
                 class: "warning"
             };
-        const Tg = {
+        const Bg = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -17318,20 +17373,20 @@
                         return this.disks.length > 0
                     }
                 },
                 methods: {
                     getAlert: e => e.inactive ? "critical" : e.degraded ? "warning" : "ok"
                 }
             },
-            Ag = (0, nc.Z)(Tg, [
+            Ug = (0, nc.Z)(Bg, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", xg, [s.hasDisks ? (li(), pi("div", _g, kg)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.disks, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", Dg, [s.hasDisks ? (li(), pi("div", Mg, jg)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.disks, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", Sg, [Si(pe(e.type.toUpperCase()) + " " + pe(e.name) + " ", 1), On(wi("div", Cg, "└─ Degraded mode", 512), [
+                    }, [wi("div", Rg, [Si(pe(e.type.toUpperCase()) + " " + pe(e.name) + " ", 1), On(wi("div", qg, "└─ Degraded mode", 512), [
                         [Ds, e.degraded]
                     ]), On(wi("div", null, "   └─ " + pe(e.config), 513), [
                         [Ds, e.degraded]
                     ]), On(wi("div", {
                         class: "critical"
                     }, "└─ Status " + pe(e.status), 513), [
                         [Ds, e.inactive]
@@ -17346,49 +17401,49 @@
                     ]), On(wi("div", {
                         class: ce(["table-cell", s.getAlert(e)])
                     }, pe(e.available), 3), [
                         [Ds, "active" == e.status]
                     ])])))), 128))])
                 }]
             ]),
-            Eg = {
+            Fg = {
                 id: "smart",
                 class: "plugin"
             },
-            Og = wi("div", {
+            zg = wi("div", {
                 class: "table-row"
             }, [wi("div", {
                 class: "table-cell text-left title"
             }, "SMART disks"), wi("div", {
                 class: "table-cell"
             }), wi("div", {
                 class: "table-cell"
             })], -1),
-            Ig = {
+            $g = {
                 class: "table-row"
             },
-            Pg = {
+            Hg = {
                 class: "table-cell text-left text-truncate"
             },
-            Ng = wi("div", {
+            Vg = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            Lg = wi("div", {
+            Gg = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            Dg = {
+            Wg = {
                 class: "table-cell text-left"
             },
-            Mg = wi("div", {
+            Zg = wi("div", {
                 class: "table-cell"
             }, null, -1),
-            jg = {
+            Kg = {
                 class: "table-cell text-truncate"
             };
-        const Rg = {
+        const Qg = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -17402,42 +17457,42 @@
                                 name: t,
                                 details: n
                             }
                         }))
                     }
                 }
             },
-            qg = (0, nc.Z)(Rg, [
+            Xg = (0, nc.Z)(Qg, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Eg, [Og, (li(!0), pi(ni, null, pr(s.drives, ((e, t) => (li(), pi(ni, {
+                    return li(), pi("section", Fg, [zg, (li(!0), pi(ni, null, pr(s.drives, ((e, t) => (li(), pi(ni, {
                         key: t
-                    }, [wi("div", Ig, [wi("div", Pg, pe(e.name), 1), Ng, Lg]), (li(!0), pi(ni, null, pr(e.details, ((e, t) => (li(), pi("div", {
+                    }, [wi("div", $g, [wi("div", Hg, pe(e.name), 1), Vg, Gg]), (li(!0), pi(ni, null, pr(e.details, ((e, t) => (li(), pi("div", {
                         key: t,
                         class: "table-row"
-                    }, [wi("div", Dg, "  " + pe(e.name), 1), Mg, wi("div", jg, [wi("span", null, pe(e.raw), 1)])])))), 128))], 64)))), 128))])
+                    }, [wi("div", Wg, "  " + pe(e.name), 1), Zg, wi("div", Kg, [wi("span", null, pe(e.raw), 1)])])))), 128))], 64)))), 128))])
                 }]
             ]),
-            Bg = {
+            Jg = {
                 class: "plugin",
                 id: "sensors"
             },
-            Ug = {
+            Yg = {
                 key: 0,
                 class: "table-row"
             },
-            Fg = [wi("div", {
+            em = [wi("div", {
                 class: "table-cell text-left title"
             }, "SENSORS", -1)],
-            zg = {
+            tm = {
                 class: "table-cell text-left"
             },
-            $g = wi("div", {
+            nm = wi("div", {
                 class: "table-cell"
             }, null, -1);
-        const Hg = {
+        const rm = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: Uo
@@ -17458,36 +17513,36 @@
                 },
                 methods: {
                     getDecoration(e) {
                         if (void 0 !== this.view[e].value.decoration) return this.view[e].value.decoration.toLowerCase()
                     }
                 }
             },
-            Vg = (0, nc.Z)(Hg, [
+            im = (0, nc.Z)(rm, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Bg, [s.sensors.length > 0 ? (li(), pi("div", Ug, Fg)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.sensors, ((e, t) => (li(), pi("div", {
+                    return li(), pi("section", Jg, [s.sensors.length > 0 ? (li(), pi("div", Yg, em)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.sensors, ((e, t) => (li(), pi("div", {
                         class: "table-row",
                         key: t
-                    }, [wi("div", zg, pe(e.label), 1), $g, wi("div", {
+                    }, [wi("div", tm, pe(e.label), 1), nm, wi("div", {
                         class: ce(["table-cell", s.getDecoration(e.label)])
                     }, pe(e.value) + pe(e.unit), 3)])))), 128))])
                 }]
             ]),
-            Gg = {
+            sm = {
                 class: "plugin",
                 id: "system"
             },
-            Wg = {
+            om = {
                 key: 0,
                 class: "critical"
             },
-            Zg = {
+            am = {
                 class: "title"
             };
-        const Kg = {
+        const lm = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 data: () => ({
                     store: Uo
@@ -17503,62 +17558,62 @@
                         return this.stats.hr_name
                     },
                     isDisconnected() {
                         return "FAILURE" === this.store.status
                     }
                 }
             },
-            Qg = (0, nc.Z)(Kg, [
+            cm = (0, nc.Z)(lm, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Gg, [s.isDisconnected ? (li(), pi("span", Wg, "Disconnected from")) : Ti("v-if", !0), wi("span", Zg, pe(s.hostname), 1), wi("span", null, pe(s.humanReadableName), 1)])
+                    return li(), pi("section", sm, [s.isDisconnected ? (li(), pi("span", om, "Disconnected from")) : Ti("v-if", !0), wi("span", am, pe(s.hostname), 1), wi("span", null, pe(s.humanReadableName), 1)])
                 }]
             ]),
-            Xg = {
+            um = {
                 class: "plugin",
                 id: "uptime"
             };
-        const Jg = {
+        const dm = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     value() {
                         return this.data.stats.uptime
                     }
                 }
             },
-            Yg = (0, nc.Z)(Jg, [
+            fm = (0, nc.Z)(dm, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", Xg, [wi("span", null, "Uptime: " + pe(s.value), 1)])
+                    return li(), pi("section", um, [wi("span", null, "Uptime: " + pe(s.value), 1)])
                 }]
             ]),
-            em = {
+            pm = {
                 class: "plugin",
                 id: "wifi"
             },
-            tm = {
+            hm = {
                 key: 0,
                 class: "table-row"
             },
-            nm = [wi("div", {
+            gm = [wi("div", {
                 class: "table-cell text-left title"
             }, "WIFI", -1), wi("div", {
                 class: "table-cell"
             }, null, -1), wi("div", {
                 class: "table-cell"
             }, "dBm", -1)],
-            rm = {
+            mm = {
                 class: "table-cell text-left"
             },
-            im = wi("div", {
+            bm = wi("div", {
                 class: "table-cell"
             }, null, -1);
-        const sm = {
+        const vm = {
                 props: {
                     data: {
                         type: Object
                     }
                 },
                 computed: {
                     stats() {
@@ -17579,55 +17634,55 @@
                 },
                 methods: {
                     getDecoration(e, t) {
                         if (void 0 !== this.view[e.ssid][t]) return this.view[e.ssid][t].decoration.toLowerCase()
                     }
                 }
             },
-            om = (0, nc.Z)(sm, [
+            ym = (0, nc.Z)(vm, [
                 ["render", function(e, t, n, r, i, s) {
-                    return li(), pi("section", em, [s.hotspots.length > 0 ? (li(), pi("div", tm, nm)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.hotspots, ((t, n) => (li(), pi("div", {
+                    return li(), pi("section", pm, [s.hotspots.length > 0 ? (li(), pi("div", hm, gm)) : Ti("v-if", !0), (li(!0), pi(ni, null, pr(s.hotspots, ((t, n) => (li(), pi("div", {
                         class: "table-row",
                         key: n
-                    }, [wi("div", rm, pe(e.$filters.limitTo(t.ssid, 20)), 1), im, wi("div", {
+                    }, [wi("div", mm, pe(e.$filters.limitTo(t.ssid, 20)), 1), bm, wi("div", {
                         class: ce(["table-cell", s.getDecoration(t, "quality_level")])
                     }, pe(t.quality_level), 3)])))), 128))])
                 }]
             ]),
-            am = JSON.parse('{"t":["network","ports","wifi","connections","diskio","fs","irq","folders","raid","smart","sensors","now"]}'),
-            lm = {
+            wm = JSON.parse('{"t":["network","ports","wifi","connections","diskio","fs","irq","folders","raid","smart","sensors","now"]}'),
+            xm = {
                 components: {
                     GlancesHelp: rc,
                     GlancesPluginAlert: pc,
                     GlancesPluginCloud: bc,
                     GlancesPluginConnections: Uc,
                     GlancesPluginCpu: ju,
                     GlancesPluginDiskio: id,
                     GlancesPluginContainers: Cd,
                     GlancesPluginFolders: Ld,
                     GlancesPluginFs: $d,
-                    GlancesPluginGpu: lf,
-                    GlancesPluginIp: mf,
-                    GlancesPluginIrq: Sf,
-                    GlancesPluginLoad: qf,
-                    GlancesPluginMem: Jf,
-                    GlancesPluginMemMore: hp,
-                    GlancesPluginMemswap: Ep,
-                    GlancesPluginNetwork: Gp,
-                    GlancesPluginNow: Xp,
-                    GlancesPluginPercpu: ah,
-                    GlancesPluginPorts: yh,
-                    GlancesPluginProcess: Jh,
-                    GlancesPluginQuicklook: wg,
-                    GlancesPluginRaid: Ag,
-                    GlancesPluginSensors: Vg,
-                    GlancesPluginSmart: qg,
-                    GlancesPluginSystem: Qg,
-                    GlancesPluginUptime: Yg,
-                    GlancesPluginWifi: om
+                    GlancesPluginGpu: xf,
+                    GlancesPluginIp: Of,
+                    GlancesPluginIrq: Rf,
+                    GlancesPluginLoad: Xf,
+                    GlancesPluginMem: dp,
+                    GlancesPluginMemMore: Ap,
+                    GlancesPluginMemswap: Fp,
+                    GlancesPluginNetwork: sh,
+                    GlancesPluginNow: uh,
+                    GlancesPluginPercpu: wh,
+                    GlancesPluginPorts: Nh,
+                    GlancesPluginProcess: dg,
+                    GlancesPluginQuicklook: Lg,
+                    GlancesPluginRaid: Ug,
+                    GlancesPluginSensors: im,
+                    GlancesPluginSmart: Xg,
+                    GlancesPluginSystem: cm,
+                    GlancesPluginUptime: fm,
+                    GlancesPluginWifi: ym
                 },
                 data: () => ({
                     store: Uo
                 }),
                 computed: {
                     args() {
                         return this.store.args || {}
@@ -17650,15 +17705,15 @@
                     title() {
                         const {
                             data: e
                         } = this, t = e.stats && e.stats.system && e.stats.system.hostname || "";
                         return t ? `${t} - Glances` : "Glances"
                     },
                     leftMenu() {
-                        return void 0 !== this.config.outputs && void 0 !== this.config.outputs.left_menu ? this.config.outputs.left_menu.split(",") : am.t
+                        return void 0 !== this.config.outputs && void 0 !== this.config.outputs.left_menu ? this.config.outputs.left_menu.split(",") : wm.t
                     }
                 },
                 watch: {
                     title() {
                         document && (document.title = this.title)
                     }
                 },
@@ -17740,28 +17795,28 @@
                         t = isFinite(e["refresh-time"]) ? parseInt(e["refresh-time"], 10) : void 0;
                     Ho.init(t), this.setupHotKeys()
                 },
                 beforeUnmount() {
                     jo.unbind()
                 }
             };
-        const cm = ((...e) => {
+        const _m = ((...e) => {
             const t = qs().createApp(...e);
             const {
                 mount: n
             } = t;
             return t.mount = e => {
                 const r = Bs(e);
                 if (!r) return;
                 const i = t._component;
                 L(i) || i.render || i.template || (i.template = r.innerHTML), r.innerHTML = "";
                 const s = n(r, !1, r instanceof SVGElement);
                 return r instanceof Element && (r.removeAttribute("v-cloak"), r.setAttribute("data-v-app", "")), s
             }, t
-        })((0, nc.Z)(lm, [
+        })((0, nc.Z)(xm, [
             ["render", function(e, t, n, r, i, s) {
                 const o = cr("glances-help"),
                     a = cr("glances-plugin-system"),
                     l = cr("glances-plugin-ip"),
                     c = cr("glances-plugin-uptime"),
                     u = cr("glances-plugin-cloud"),
                     d = cr("glances-plugin-quicklook"),
@@ -17816,10 +17871,10 @@
                     data: s.data
                 }, null, 8, ["data"]), s.args.disable_alert ? Ti("v-if", !0) : (li(), hi(x, {
                     key: 1,
                     data: s.data
                 }, null, 8, ["data"]))])])])])) : (li(), pi("div", Us, Fs))
             }]
         ]));
-        cm.config.globalProperties.$filters = e, cm.mount("#app")
+        _m.config.globalProperties.$filters = e, _m.mount("#app")
     })()
 })();
```

### Comparing `glances-4.0.5/glances/outputs/static/webpack.config.js` & `glances-4.0.6/glances/outputs/static/webpack.config.js`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/password.py` & `glances-4.0.6/glances/password.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/password_list.py` & `glances-4.0.6/glances/password_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/alert/__init__.py` & `glances-4.0.6/glances/plugins/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/amps/__init__.py` & `glances-4.0.6/glances/plugins/amps/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/cloud/__init__.py` & `glances-4.0.6/glances/plugins/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/connections/__init__.py` & `glances-4.0.6/glances/plugins/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/containers/__init__.py` & `glances-4.0.6/glances/plugins/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/containers/engines/docker.py` & `glances-4.0.6/glances/plugins/containers/engines/docker.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/containers/engines/podman.py` & `glances-4.0.6/glances/plugins/containers/engines/podman.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/containers/stats_streamer.py` & `glances-4.0.6/glances/plugins/containers/stats_streamer.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/core/__init__.py` & `glances-4.0.6/glances/plugins/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/cpu/__init__.py` & `glances-4.0.6/glances/plugins/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/diskio/__init__.py` & `glances-4.0.6/glances/plugins/diskio/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/folders/__init__.py` & `glances-4.0.6/glances/plugins/folders/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/fs/__init__.py` & `glances-4.0.6/glances/plugins/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/gpu/__init__.py` & `glances-4.0.6/glances/plugins/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/gpu/cards/amd.py` & `glances-4.0.6/glances/plugins/gpu/cards/amd.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/gpu/cards/nvidia.py` & `glances-4.0.6/glances/plugins/gpu/cards/nvidia.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/help/__init__.py` & `glances-4.0.6/glances/plugins/help/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/ip/__init__.py` & `glances-4.0.6/glances/plugins/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/irq/__init__.py` & `glances-4.0.6/glances/plugins/irq/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/load/__init__.py` & `glances-4.0.6/glances/plugins/load/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/mem/__init__.py` & `glances-4.0.6/glances/plugins/mem/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/memswap/__init__.py` & `glances-4.0.6/glances/plugins/memswap/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/network/__init__.py` & `glances-4.0.6/glances/plugins/network/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/now/__init__.py` & `glances-4.0.6/glances/plugins/now/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/percpu/__init__.py` & `glances-4.0.6/glances/plugins/percpu/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/plugin/model.py` & `glances-4.0.6/glances/plugins/plugin/model.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/ports/__init__.py` & `glances-4.0.6/glances/plugins/ports/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/processcount/__init__.py` & `glances-4.0.6/glances/plugins/processcount/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/processlist/__init__.py` & `glances-4.0.6/glances/plugins/processlist/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/psutilversion/__init__.py` & `glances-4.0.6/glances/plugins/psutilversion/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/quicklook/__init__.py` & `glances-4.0.6/glances/plugins/quicklook/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/raid/__init__.py` & `glances-4.0.6/glances/plugins/raid/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/sensors/__init__.py` & `glances-4.0.6/glances/plugins/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/sensors/sensor/glances_batpercent.py` & `glances-4.0.6/glances/plugins/sensors/sensor/glances_batpercent.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/sensors/sensor/glances_hddtemp.py` & `glances-4.0.6/glances/plugins/sensors/sensor/glances_hddtemp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/smart/__init__.py` & `glances-4.0.6/glances/plugins/smart/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/system/__init__.py` & `glances-4.0.6/glances/plugins/system/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/uptime/__init__.py` & `glances-4.0.6/glances/plugins/uptime/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/version/__init__.py` & `glances-4.0.6/glances/plugins/version/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/plugins/wifi/__init__.py` & `glances-4.0.6/glances/plugins/wifi/__init__.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/ports_list.py` & `glances-4.0.6/glances/ports_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/processes.py` & `glances-4.0.6/glances/processes.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/programs.py` & `glances-4.0.6/glances/programs.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/secure.py` & `glances-4.0.6/glances/secure.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/server.py` & `glances-4.0.6/glances/server.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/snmp.py` & `glances-4.0.6/glances/snmp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/standalone.py` & `glances-4.0.6/glances/standalone.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/static_list.py` & `glances-4.0.6/glances/static_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/stats.py` & `glances-4.0.6/glances/stats.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/stats_client.py` & `glances-4.0.6/glances/stats_client.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/stats_client_snmp.py` & `glances-4.0.6/glances/stats_client_snmp.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/stats_server.py` & `glances-4.0.6/glances/stats_server.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/thresholds.py` & `glances-4.0.6/glances/thresholds.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/timer.py` & `glances-4.0.6/glances/timer.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/web_list.py` & `glances-4.0.6/glances/web_list.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/glances/webserver.py` & `glances-4.0.6/glances/webserver.py`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/pyproject.toml` & `glances-4.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glances-4.0.5/setup.py` & `glances-4.0.6/setup.py`

 * *Files identical despite different names*

