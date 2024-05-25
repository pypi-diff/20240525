# Comparing `tmp/qulab-2.0.2.tar.gz` & `tmp/qulab-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.0.2.tar", last modified: Fri May 24 02:30:50 2024, max compression
+gzip compressed data, was "qulab-2.0.3.tar", last modified: Sat May 25 06:48:37 2024, max compression
```

## Comparing `qulab-2.0.2.tar` & `qulab-2.0.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.797087 qulab-2.0.2/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-24 02:30:21.000000 qulab-2.0.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-24 02:30:21.000000 qulab-2.0.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3464 2024-05-24 02:30:50.796704 qulab-2.0.2/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.796382 qulab-2.0.2/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3464 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2256 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      188 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-24 02:30:50.000000 qulab-2.0.2/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-24 02:30:21.000000 qulab-2.0.2/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1772 2024-05-24 02:30:21.000000 qulab-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.784091 qulab-2.0.2/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      430 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.785620 qulab-2.0.2/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.787476 qulab-2.0.2/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11521 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    15402 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    23030 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     1024 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.788409 qulab-2.0.2/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.788628 qulab-2.0.2/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.789978 qulab-2.0.2/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.790658 qulab-2.0.2/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.791253 qulab-2.0.2/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.791573 qulab-2.0.2/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.792922 qulab-2.0.2/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.794783 qulab-2.0.2/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.795771 qulab-2.0.2/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-24 02:30:21.000000 qulab-2.0.2/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-24 02:30:50.797126 qulab-2.0.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-24 02:30:21.000000 qulab-2.0.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.796000 qulab-2.0.2/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-24 02:30:21.000000 qulab-2.0.2/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-24 02:30:50.796189 qulab-2.0.2/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-24 02:30:21.000000 qulab-2.0.2/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.385120 qulab-2.0.3/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-25 06:48:04.000000 qulab-2.0.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-25 06:48:04.000000 qulab-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-25 06:48:37.384899 qulab-2.0.3/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384608 qulab-2.0.3/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2256 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-25 06:48:37.000000 qulab-2.0.3/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-25 06:48:04.000000 qulab-2.0.3/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-25 06:48:04.000000 qulab-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.372473 qulab-2.0.3/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      430 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.375289 qulab-2.0.3/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.376668 qulab-2.0.3/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11521 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    15402 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    22494 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.377480 qulab-2.0.3/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.377762 qulab-2.0.3/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.378958 qulab-2.0.3/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.379432 qulab-2.0.3/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.379956 qulab-2.0.3/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.380203 qulab-2.0.3/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.381358 qulab-2.0.3/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.383003 qulab-2.0.3/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384104 qulab-2.0.3/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-25 06:48:04.000000 qulab-2.0.3/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-25 06:48:37.385154 qulab-2.0.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-25 06:48:04.000000 qulab-2.0.3/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384234 qulab-2.0.3/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-25 06:48:04.000000 qulab-2.0.3/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-25 06:48:37.384354 qulab-2.0.3/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-25 06:48:04.000000 qulab-2.0.3/tests/test_scan.py
```

### Comparing `qulab-2.0.2/LICENSE` & `qulab-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/PKG-INFO` & `qulab-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.2
+Version: 2.0.3
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
@@ -28,14 +28,15 @@
 Requires-Dist: click>=7.1.2
 Requires-Dist: dill>=0.3.6
 Requires-Dist: GitPython>=3.1.14
 Requires-Dist: ipython>=7.4.0
 Requires-Dist: ipywidgets>=7.4.2
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: matplotlib>=3.7.2
+Requires-Dist: nevergrad>=1.0.2
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: ply>=3.11
 Requires-Dist: pyzmq>=25.1.0
 Requires-Dist: scipy>=1.0.0
 Requires-Dist: watchdog>=4.0.0
 
 # QuLab
```

### Comparing `qulab-2.0.2/QuLab.egg-info/PKG-INFO` & `qulab-2.0.3/QuLab.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.2
+Version: 2.0.3
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
@@ -28,14 +28,15 @@
 Requires-Dist: click>=7.1.2
 Requires-Dist: dill>=0.3.6
 Requires-Dist: GitPython>=3.1.14
 Requires-Dist: ipython>=7.4.0
 Requires-Dist: ipywidgets>=7.4.2
 Requires-Dist: loguru>=0.7.2
 Requires-Dist: matplotlib>=3.7.2
+Requires-Dist: nevergrad>=1.0.2
 Requires-Dist: numpy>=1.13.3
 Requires-Dist: ply>=3.11
 Requires-Dist: pyzmq>=25.1.0
 Requires-Dist: scipy>=1.0.0
 Requires-Dist: watchdog>=4.0.0
 
 # QuLab
```

### Comparing `qulab-2.0.2/QuLab.egg-info/SOURCES.txt` & `qulab-2.0.3/QuLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/README.md` & `qulab-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/pyproject.toml` & `qulab-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "click>=7.1.2",
     "dill>=0.3.6",
     "GitPython>=3.1.14",
     "ipython>=7.4.0",
     "ipywidgets>=7.4.2",
     "loguru>=0.7.2",
     "matplotlib>=3.7.2",
+    "nevergrad>=1.0.2",
     "numpy>=1.13.3",
     "ply>=3.11",
     "pyzmq>=25.1.0",
     "scipy>=1.0.0",
     "watchdog>=4.0.0"
 ]
 dynamic = ["version"]
```

### Comparing `qulab-2.0.2/qulab/monitor/config.py` & `qulab-2.0.3/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/dataset.py` & `qulab-2.0.3/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/event_queue.py` & `qulab-2.0.3/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/mainwindow.py` & `qulab-2.0.3/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/monitor.py` & `qulab-2.0.3/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/ploter.py` & `qulab-2.0.3/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/qt_compat.py` & `qulab-2.0.3/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/monitor/toolbar.py` & `qulab-2.0.3/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/curd.py` & `qulab-2.0.3/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/expression.py` & `qulab-2.0.3/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/models.py` & `qulab-2.0.3/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/optimize.py` & `qulab-2.0.3/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/query_record.py` & `qulab-2.0.3/qulab/scan/query_record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/recorder.py` & `qulab-2.0.3/qulab/scan/recorder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/scan/scan.py` & `qulab-2.0.3/qulab/scan/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,95 +1,39 @@
-import ast
 import asyncio
+import datetime
 import inspect
 import itertools
+import os
+import re
 import sys
 import uuid
 from graphlib import TopologicalSorter
 from pathlib import Path
 from types import MethodType
-from typing import Any, Callable, Type
+from typing import Any, Awaitable, Callable, Iterable, Type
 
 import dill
 import numpy as np
 import skopt
 import zmq
 from skopt.space import Categorical, Integer, Real
 from tqdm.notebook import tqdm
 
 from ..sys.rpc.zmq_socket import ZMQContextManager
 from .expression import Env, Expression, Symbol
 from .optimize import NgOptimizer
 from .recorder import Record
+from .utils import async_zip, call_function
 
+__process_uuid = uuid.uuid1()
+__task_counter = itertools.count()
 
-async def call_function(func: Callable | Expression, variables: dict[str,
-                                                                     Any]):
-    if isinstance(func, Expression):
-        env = Env()
-        for name in func.symbols():
-            if name in variables:
-                if inspect.isawaitable(variables[name]):
-                    variables[name] = await variables[name]
-                env.variables[name] = variables[name]
-            else:
-                raise ValueError(f'{name} is not provided.')
-        return func.eval(env)
-
-    try:
-        sig = inspect.signature(func)
-    except:
-        return func()
-    args = []
-    for name, param in sig.parameters.items():
-        if param.kind == param.POSITIONAL_OR_KEYWORD:
-            if name in variables:
-                if inspect.isawaitable(variables[name]):
-                    variables[name] = await variables[name]
-                args.append(variables[name])
-            elif param.default is not param.empty:
-                args.append(param.default)
-            else:
-                raise ValueError(f'parameter {name} is not provided.')
-        elif param.kind == param.VAR_POSITIONAL:
-            raise ValueError('not support VAR_POSITIONAL')
-        elif param.kind == param.VAR_KEYWORD:
-            ret = func(**variables)
-            if inspect.isawaitable(ret):
-                ret = await ret
-            return ret
-    ret = func(*args)
-    if inspect.isawaitable(ret):
-        ret = await ret
-    return ret
-
-
-async def async_next(aiter):
-    try:
-        if hasattr(aiter, '__anext__'):
-            return await aiter.__anext__()
-        else:
-            return next(aiter)
-    except StopIteration:
-        raise StopAsyncIteration from None
 
-
-async def async_zip(*aiters):
-    aiters = [
-        ait.__aiter__() if hasattr(ait, '__aiter__') else iter(ait)
-        for ait in aiters
-    ]
-    try:
-        while True:
-            # 使用 asyncio.gather 等待所有异步生成器返回下一个元素
-            result = await asyncio.gather(*(async_next(ait) for ait in aiters))
-            yield tuple(result)
-    except StopAsyncIteration:
-        # 当任一异步生成器耗尽时停止迭代
-        return
+def task_uuid():
+    return uuid.uuid3(__process_uuid, str(next(__task_counter)))
 
 
 def _get_depends(func: Callable):
     try:
         sig = inspect.signature(func)
     except:
         return []
@@ -104,25 +48,14 @@
         elif param.kind == param.VAR_KEYWORD:
             pass
         elif param.kind == param.VAR_POSITIONAL:
             raise ValueError('not support VAR_POSITIONAL')
     return args
 
 
-def is_valid_identifier(s: str) -> bool:
-    """
-    Check if a string is a valid identifier.
-    """
-    try:
-        ast.parse(f"f({s}=0)")
-        return True
-    except SyntaxError:
-        return False
-
-
 class OptimizeSpace():
 
     def __init__(self, optimizer: 'Optimizer', space):
         self.optimizer = optimizer
         self.space = space
         self.name = None
 
@@ -220,43 +153,56 @@
 
     def __getattr__(self, attr):
         return Promise(self.task, None, attr)
 
 
 class Scan():
 
+    def __new__(cls, *args, mixin=None, **kwds):
+        if mixin is None:
+            return super().__new__(cls)
+        for k in dir(mixin):
+            if not hasattr(cls, k):
+                try:
+                    setattr(cls, k, getattr(mixin, k))
+                except:
+                    pass
+        return super().__new__(cls)
+
     def __init__(self,
                  app: str = 'task',
                  tags: tuple[str] = (),
-                 database: str | Path | None = 'tcp://127.0.0.1:6789'):
-        self.id = f"{app}({str(uuid.uuid1())})"
+                 database: str | Path | None = 'tcp://127.0.0.1:6789',
+                 mixin=None):
+        self.id = task_uuid()
         self.record = None
         self.namespace = {}
         self.description = {
             'app': app,
             'tags': tags,
             'loops': {},
             'consts': {},
             'functions': {},
             'optimizers': {},
             'actions': {},
             'dependents': {},
             'order': {},
             'filters': {},
-            'total': {},
-            'compiled': False,
+            'total': {}
         }
         self._current_level = 0
         self.variables = {}
         self._task = None
         self.sock = None
         self.database = database
-        self._variables = {}
         self._sem = asyncio.Semaphore(100)
-        self._bar = {}
+        self._bar: dict[int, tqdm] = {}
+        self._hide_patterns = [r'^__.*', r'.*__$']
+        self._hide_pattern_re = re.compile('|'.join(self._hide_patterns))
+        self._task_queue = asyncio.Queue()
 
     def __getstate__(self) -> dict:
         state = self.__dict__.copy()
         del state['record']
         del state['sock']
         del state['_task']
         del state['_sem']
@@ -274,29 +220,39 @@
     @property
     def current_level(self):
         return self._current_level
 
     async def emit(self, current_level, step, position, variables: dict[str,
                                                                         Any]):
         for key, value in list(variables.items()):
-            if inspect.isawaitable(value):
+            if inspect.isawaitable(value) and not self.hiden(key):
                 variables[key] = await value
         if self.sock is not None:
             await self.sock.send_pyobj({
                 'task': self.id,
                 'method': 'record_append',
                 'record_id': self.record.id,
                 'level': current_level,
                 'step': step,
                 'position': position,
-                'variables': variables
+                'variables': {
+                    k: v
+                    for k, v in variables.items() if not self.hiden(k)
+                }
             })
         else:
             self.record.append(current_level, step, position, variables)
 
+    def hide(self, name: str):
+        self._hide_patterns.append(re.compile(name))
+        self._hide_pattern_re = re.compile('|'.join(self._hide_patterns))
+
+    def hiden(self, name: str) -> bool:
+        return bool(self._hide_pattern_re.match(name))
+
     async def _filter(self, variables: dict[str, Any], level: int = 0):
         try:
             return all([
                 await call_function(fun, variables) for fun in itertools.chain(
                     self.description['filters'].get(level, []),
                     self.description['filters'].get(-1, []))
             ])
@@ -313,27 +269,25 @@
         else:
             try:
                 scripts = ('shell',
                            [sys.executable, __main__.__file__, *sys.argv[1:]])
             except:
                 scripts = ('', [])
 
+        self.description['ctime'] = datetime.datetime.now()
+        self.description['scripts'] = scripts
+        self.description['env'] = {k: v for k, v in os.environ.items()}
         if self.sock is not None:
             await self.sock.send_pyobj({
                 'task':
                 self.id,
                 'method':
                 'record_create',
                 'description':
-                dill.dumps(self.description),
-                # 'env':
-                # dill.dumps(__main__.__dict__),
-                'scripts':
-                scripts,
-                'tags': []
+                dill.dumps(self.description)
             })
 
             record_id = await self.sock.recv_pyobj()
             return Record(record_id, self.database, self.description)
         return Record(None, self.database, self.description)
 
     def get(self, name: str):
@@ -352,15 +306,15 @@
     def add_depends(self, name: str, depends: list[str]):
         if isinstance(depends, str):
             depends = [depends]
         if name not in self.description['dependents']:
             self.description['dependents'][name] = set()
         self.description['dependents'][name].update(depends)
 
-    def add_filter(self, func, level):
+    def add_filter(self, func: Callable, level: int):
         """
         Add a filter function to the scan.
 
         Args:
             func: A callable object or an instance of Expression.
             level: The level of the scan to add the filter. -1 means any level.
         """
@@ -423,16 +377,25 @@
                         method,
                         maxiter,
                         minimize=False,
                         **kwds)
         self.description['optimizers'][name] = opt
         return opt
 
+    async def _update_progress(self):
+        while True:
+            task = await self._task_queue.get()
+            if isinstance(task, asyncio.Event):
+                task.set()
+            elif inspect.isawaitable(task):
+                await task
+
     async def _run(self):
-        self.assymbly()
+        assymbly(self.description)
+        task = asyncio.create_task(self._update_progress())
         self.variables = self.description['consts'].copy()
         for level, total in self.description['total'].items():
             if total == np.inf:
                 total = None
             self._bar[level] = tqdm(total=total)
         for group in self.description['order'].get(-1, []):
             for name in group:
@@ -447,14 +410,15 @@
                 self.record = await self.create_record()
                 await self.work()
         else:
             self.record = await self.create_record()
             await self.work()
         for level, bar in self._bar.items():
             bar.close()
+        task.cancel()
         return self.variables
 
     async def done(self):
         if self._task is not None:
             try:
                 await self._task
             except asyncio.CancelledError:
@@ -464,205 +428,57 @@
         import asyncio
         self._task = asyncio.create_task(self._run())
 
     def cancel(self):
         if self._task is not None:
             self._task.cancel()
 
-    def assymbly(self):
-        if self.description['compiled']:
-            return
-
-        mapping = {
-            label: level
-            for level, label in enumerate(
-                sorted(
-                    set(self.description['loops'].keys())
-                    | set(self.description['actions'].keys()) - {-1}))
-        }
-
-        if -1 in self.description['actions']:
-            mapping[-1] = max(mapping.values()) + 1
-
-        self.description['loops'] = dict(
-            sorted([(mapping[k], v)
-                    for k, v in self.description['loops'].items()]))
-        self.description['actions'] = {
-            mapping[k]: v
-            for k, v in self.description['actions'].items()
-        }
-
-        for level, loops in self.description['loops'].items():
-            self.description['total'][level] = np.inf
-            for name, space in loops:
-                try:
-                    self.description['total'][level] = min(
-                        self.description['total'][level], len(space))
-                except:
-                    pass
-
-        dependents = self.description['dependents'].copy()
-
-        for level in range(len(mapping)):
-            range_list = self.description['loops'].get(level, [])
-            if level > 0:
-                if f'#__loop_{level}' not in self.description['dependents']:
-                    dependents[f'#__loop_{level}'] = []
-                dependents[f'#__loop_{level}'].append(f'#__loop_{level-1}')
-            for name, _ in range_list:
-                if name not in self.description['dependents']:
-                    dependents[name] = []
-                dependents[name].append(f'#__loop_{level}')
-
-        def _get_all_depends(key, graph):
-            ret = set()
-            if key not in graph:
-                return ret
-
-            for e in graph[key]:
-                ret.update(_get_all_depends(e, graph))
-            ret.update(graph[key])
-            return ret
-
-        full_depends = {}
-        for key in dependents:
-            full_depends[key] = _get_all_depends(key, dependents)
-
-        levels = {}
-        passed = set()
-        all_keys = set()
-        for level in reversed(self.description['loops'].keys()):
-            tag = f'#__loop_{level}'
-            for key, deps in full_depends.items():
-                all_keys.update(deps)
-                all_keys.add(key)
-                if key.startswith('#__loop_'):
-                    continue
-                if tag in deps:
-                    if level not in levels:
-                        levels[level] = set()
-                    if key not in passed:
-                        passed.add(key)
-                        levels[level].add(key)
-        levels[-1] = {
-            key
-            for key in all_keys - passed if not key.startswith('#__loop_')
-        }
-
-        order = []
-        ts = TopologicalSorter(dependents)
-        ts.prepare()
-        while ts.is_active():
-            ready = ts.get_ready()
-            order.append(ready)
-            for k in ready:
-                ts.done(k)
-
-        self.description['order'] = {}
-
-        for level in sorted(levels):
-            keys = set(levels[level])
-            self.description['order'][level] = []
-            for ready in order:
-                ready = list(keys & set(ready))
-                if ready:
-                    self.description['order'][level].append(ready)
-                    keys -= set(ready)
-
-        self.description['compiled'] = True
-
-    async def _iter_level(self, level, variables):
-        iters = {}
-        env = Env()
-        env.variables = variables
-        opts = {}
-
-        for name, iter in self.description['loops'][level]:
-            if isinstance(iter, OptimizeSpace):
-                if iter.optimizer.name not in opts:
-                    opts[iter.optimizer.name] = iter.optimizer.create()
-            elif isinstance(iter, Expression):
-                iters[name] = iter.eval(env)
-            elif callable(iter):
-                iters[name] = await call_function(iter, variables)
-            else:
-                iters[name] = iter
-
-        maxiter = 0xffffffff
-        for name, opt in opts.items():
-            opt_cfg = self.description['optimizers'][name]
-            maxiter = min(maxiter, opt_cfg.maxiter)
-
-        async for args in async_zip(*iters.values(), range(maxiter)):
-            variables.update(dict(zip(iters.keys(), args[:-1])))
-            for name, opt in opts.items():
-                args = opt.ask()
-                opt_cfg = self.description['optimizers'][name]
-                variables.update({
-                    n: v
-                    for n, v in zip(opt_cfg.dimensions.keys(), args)
-                })
-
-            for group in self.description['order'].get(level, []):
-                for name in group:
-                    if name in self.description['functions']:
-                        variables[name] = await call_function(
-                            self.description['functions'][name], variables)
-
-            yield variables
-
-            for name, opt in opts.items():
-                opt_cfg = self.description['optimizers'][name]
-                args = [variables[n] for n in opt_cfg.dimensions.keys()]
-                if name not in variables:
-                    raise ValueError(f'{name} not in variables.')
-                fun = variables[name]
-                if inspect.isawaitable(fun):
-                    fun = await fun
-                if opt_cfg.minimize:
-                    opt.tell(args, fun)
-                else:
-                    opt.tell(args, -fun)
-
-        for name, opt in opts.items():
-            opt_cfg = self.description['optimizers'][name]
-            result = opt.get_result()
-            variables.update({
-                n: v
-                for n, v in zip(opt_cfg.dimensions.keys(), result.x)
-            })
-            variables[name] = result.fun
-        if opts:
-            yield variables
+    async def _reset_progress_bar(self, level):
+        if level in self._bar:
+            self._bar[level].reset()
+
+    async def _update_progress_bar(self, level, n: int):
+        if level in self._bar:
+            self._bar[level].update(n)
 
     async def iter(self, **kwds):
         if self.current_level >= len(self.description['loops']):
             return
         step = 0
         position = 0
         task = None
-        if self.current_level in self._bar:
-            self._bar[self.current_level].reset()
-        async for variables in self._iter_level(self.current_level,
-                                                self.variables):
+        self._task_queue.put_nowait(
+            self._reset_progress_bar(self.current_level))
+        async for variables in _iter_level(
+                self.variables,
+                self.description['loops'].get(self.current_level, []),
+                self.description['order'].get(self.current_level, []),
+                self.description['functions'], self.description['optimizers']):
             self._current_level += 1
             if await self._filter(variables, self.current_level - 1):
                 yield variables
                 task = asyncio.create_task(
                     self.emit(self.current_level - 1, step, position,
                               variables.copy()))
                 step += 1
             position += 1
             self._current_level -= 1
-            if self.current_level in self._bar:
-                self._bar[self.current_level].update(1)
+            self._task_queue.put_nowait(
+                self._update_progress_bar(self.current_level, 1))
         if task is not None:
             await task
         if self.current_level == 0:
             await self.emit(self.current_level - 1, 0, 0, {})
+            for name, value in self.variables.items():
+                if inspect.isawaitable(value):
+                    self.variables[name] = await value
+            while not self._task_queue.empty():
+                task = self._task_queue.get_nowait()
+                if inspect.isawaitable(task):
+                    await task
 
     async def work(self, **kwds):
         if self.current_level in self.description['actions']:
             action = self.description['actions'][self.current_level]
             coro = action(self, **kwds)
             if inspect.isawaitable(coro):
                 await coro
@@ -679,23 +495,199 @@
 
         Args:
             action: A callable object.
             level: The level of the scan to mount the action.
         """
         self.description['actions'][level] = action
 
-    async def promise(self, awaitable):
+    async def promise(self, awaitable: Awaitable) -> Promise:
         """
         Promise to calculate asynchronous function and return the result in future.
 
         Args:
             awaitable: An awaitable object.
 
         Returns:
             Promise: A promise object.
         """
         async with self._sem:
-            return Promise(asyncio.create_task(self._await(awaitable)))
+            task = asyncio.create_task(self._await(awaitable))
+            self._task_queue.put_nowait(task)
+            return Promise(task)
 
-    async def _await(self, awaitable):
+    async def _await(self, awaitable: Awaitable):
         async with self._sem:
             return await awaitable
+
+
+def assymbly(description):
+    mapping = {
+        label: level
+        for level, label in enumerate(
+            sorted(
+                set(description['loops'].keys())
+                | {k
+                   for k in description['actions'].keys() if k >= 0}))
+    }
+
+    if -1 in description['actions']:
+        mapping[-1] = max(mapping.values()) + 1
+
+    levels = sorted(mapping.values())
+    for k in description['actions'].keys():
+        if k < -1:
+            mapping[k] = levels[k]
+
+    description['loops'] = dict(
+        sorted([(mapping[k], v) for k, v in description['loops'].items()]))
+    description['actions'] = {
+        mapping[k]: v
+        for k, v in description['actions'].items()
+    }
+
+    for level, loops in description['loops'].items():
+        description['total'][level] = np.inf
+        for name, space in loops:
+            try:
+                description['total'][level] = min(description['total'][level],
+                                                  len(space))
+            except:
+                pass
+
+    dependents = description['dependents'].copy()
+
+    for level in levels:
+        range_list = description['loops'].get(level, [])
+        if level > 0:
+            if f'#__loop_{level}' not in description['dependents']:
+                dependents[f'#__loop_{level}'] = []
+            dependents[f'#__loop_{level}'].append(f'#__loop_{level-1}')
+        for name, _ in range_list:
+            if name not in description['dependents']:
+                dependents[name] = []
+            dependents[name].append(f'#__loop_{level}')
+
+    def _get_all_depends(key, graph):
+        ret = set()
+        if key not in graph:
+            return ret
+
+        for e in graph[key]:
+            ret.update(_get_all_depends(e, graph))
+        ret.update(graph[key])
+        return ret
+
+    full_depends = {}
+    for key in dependents:
+        full_depends[key] = _get_all_depends(key, dependents)
+
+    levels = {}
+    passed = set()
+    all_keys = set()
+    for level in reversed(description['loops'].keys()):
+        tag = f'#__loop_{level}'
+        for key, deps in full_depends.items():
+            all_keys.update(deps)
+            all_keys.add(key)
+            if key.startswith('#__loop_'):
+                continue
+            if tag in deps:
+                if level not in levels:
+                    levels[level] = set()
+                if key not in passed:
+                    passed.add(key)
+                    levels[level].add(key)
+    levels[-1] = {
+        key
+        for key in all_keys - passed if not key.startswith('#__loop_')
+    }
+
+    order = []
+    ts = TopologicalSorter(dependents)
+    ts.prepare()
+    while ts.is_active():
+        ready = ts.get_ready()
+        order.append(ready)
+        for k in ready:
+            ts.done(k)
+
+    description['order'] = {}
+
+    for level in sorted(levels):
+        keys = set(levels[level])
+        description['order'][level] = []
+        for ready in order:
+            ready = list(keys & set(ready))
+            if ready:
+                description['order'][level].append(ready)
+                keys -= set(ready)
+    return description
+
+
+async def _iter_level(variables,
+                      iters: list[tuple[str, Iterable | Expression | Callable
+                                        | OptimizeSpace]],
+                      order: list[list[str]],
+                      functions: dict[str, Callable | Expression],
+                      optimizers: dict[str, Optimizer]):
+    iters_d = {}
+    env = Env()
+    env.variables = variables
+    opts = {}
+
+    for name, iter in iters:
+        if isinstance(iter, OptimizeSpace):
+            if iter.optimizer.name not in opts:
+                opts[iter.optimizer.name] = iter.optimizer.create()
+        elif isinstance(iter, Expression):
+            iters_d[name] = iter.eval(env)
+        elif callable(iter):
+            iters_d[name] = await call_function(iter, variables)
+        else:
+            iters_d[name] = iter
+
+    maxiter = 0xffffffff
+    for name, opt in opts.items():
+        opt_cfg = optimizers[name]
+        maxiter = min(maxiter, opt_cfg.maxiter)
+
+    async for args in async_zip(*iters_d.values(), range(maxiter)):
+        variables.update(dict(zip(iters_d.keys(), args[:-1])))
+        for name, opt in opts.items():
+            args = opt.ask()
+            opt_cfg = optimizers[name]
+            variables.update({
+                n: v
+                for n, v in zip(opt_cfg.dimensions.keys(), args)
+            })
+
+        for group in order:
+            for name in group:
+                if name in functions:
+                    variables[name] = await call_function(
+                        functions[name], variables)
+
+        yield variables
+
+        for name, opt in opts.items():
+            opt_cfg = optimizers[name]
+            args = [variables[n] for n in opt_cfg.dimensions.keys()]
+            if name not in variables:
+                raise ValueError(f'{name} not in variables.')
+            fun = variables[name]
+            if inspect.isawaitable(fun):
+                fun = await fun
+            if opt_cfg.minimize:
+                opt.tell(args, fun)
+            else:
+                opt.tell(args, -fun)
+
+    for name, opt in opts.items():
+        opt_cfg = optimizers[name]
+        result = opt.get_result()
+        variables.update({
+            n: v
+            for n, v in zip(opt_cfg.dimensions.keys(), result.x)
+        })
+        variables[name] = result.fun
+    if opts:
+        yield variables
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qulab-2.0.2/qulab/storage/__main__.py` & `qulab-2.0.3/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/backend/redis.py` & `qulab-2.0.3/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/base_dataset.py` & `qulab-2.0.3/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/chunk.py` & `qulab-2.0.3/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/dataset.py` & `qulab-2.0.3/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/file.py` & `qulab-2.0.3/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/__init__.py` & `qulab-2.0.3/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/config.py` & `qulab-2.0.3/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/file.py` & `qulab-2.0.3/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/ipy.py` & `qulab-2.0.3/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/models.py` & `qulab-2.0.3/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/record.py` & `qulab-2.0.3/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/report.py` & `qulab-2.0.3/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/models/tag.py` & `qulab-2.0.3/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/storage/storage.py` & `qulab-2.0.3/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/chat.py` & `qulab-2.0.3/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/device/basedevice.py` & `qulab-2.0.3/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/device/loader.py` & `qulab-2.0.3/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/device/utils.py` & `qulab-2.0.3/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.0.3/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/ipy_events.py` & `qulab-2.0.3/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/bencoder.py` & `qulab-2.0.3/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/cli.py` & `qulab-2.0.3/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/dhcp.py` & `qulab-2.0.3/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/dhcpd.py` & `qulab-2.0.3/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/kad.py` & `qulab-2.0.3/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/kcp.py` & `qulab-2.0.3/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/net/nginx.py` & `qulab-2.0.3/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/progress.py` & `qulab-2.0.3/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/exceptions.py` & `qulab-2.0.3/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/msgpack.py` & `qulab-2.0.3/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/msgpack.pyi` & `qulab-2.0.3/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/rpc.py` & `qulab-2.0.3/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/serialize.py` & `qulab-2.0.3/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/server.py` & `qulab-2.0.3/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/socket.py` & `qulab-2.0.3/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/utils.py` & `qulab-2.0.3/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/sys/rpc/zmq_socket.py` & `qulab-2.0.3/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/__init__.py` & `qulab-2.0.3/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/__main__.py` & `qulab-2.0.3/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/_autoplot.py` & `qulab-2.0.3/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/plot_layout.py` & `qulab-2.0.3/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/plot_seq.py` & `qulab-2.0.3/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/qdat.py` & `qulab-2.0.3/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/qulab/visualization/widgets.py` & `qulab-2.0.3/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.2/setup.py` & `qulab-2.0.3/setup.py`

 * *Files identical despite different names*

