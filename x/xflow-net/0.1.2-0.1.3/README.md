# Comparing `tmp/xflow-net-0.1.2.tar.gz` & `tmp/xflow-net-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.1.2.tar", last modified: Sat Jun 17 23:18:23 2023, max compression
+gzip compressed data, was "xflow-net-0.1.3.tar", last modified: Sat Jun 17 23:30:40 2023, max compression
```

## Comparing `xflow-net-0.1.2.tar` & `xflow-net-0.1.3.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.786841 xflow-net-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 23:18:10.000000 xflow-net-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-17 23:18:23.786841 xflow-net-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-17 23:18:10.000000 xflow-net-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.770841 xflow-net-0.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:18:10.000000 xflow-net-0.1.2/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-17 23:18:10.000000 xflow-net-0.1.2/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 23:18:10.000000 xflow-net-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-17 23:18:23.790841 xflow-net-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-17 23:18:10.000000 xflow-net-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.774841 xflow-net-0.1.2/xflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.774841 xflow-net-0.1.2/xflow/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/dataset/nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/dataset/pyg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.778841 xflow-net-0.1.2/xflow/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/diffusion/IC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/diffusion/LT.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/diffusion/SI.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/diffusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.778841 xflow-net-0.1.2/xflow/method/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.778841 xflow-net-0.1.2/xflow/method/cosasi/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.778841 xflow-net-0.1.2/xflow/method/cosasi/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/benchmark/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.778841 xflow-net-0.1.2/xflow/method/cosasi/contagion/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/contagion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/contagion/static_network_contagion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.782841 xflow-net-0.1.2/xflow/method/cosasi/source_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.782841 xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/jordan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/lisn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/netsleuth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.786841 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/earliest_infection_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/jordan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/lisn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/netsleuth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/rumor_centrality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/short_fat_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/source_inference/source_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.786841 xflow-net-0.1.2/xflow/method/cosasi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/utils/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/cosasi/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/im.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/method/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-17 23:18:10.000000 xflow-net-0.1.2/xflow/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:18:23.786841 xflow-net-0.1.2/xflow_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-17 23:18:23.000000 xflow-net-0.1.2/xflow_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-17 23:18:23.000000 xflow-net-0.1.2/xflow_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:18:23.000000 xflow-net-0.1.2/xflow_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 23:18:23.000000 xflow-net-0.1.2/xflow_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 23:18:23.000000 xflow-net-0.1.2/xflow_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.183646 xflow-net-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 23:30:27.000000 xflow-net-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-17 23:30:40.183646 xflow-net-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-17 23:30:27.000000 xflow-net-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.167645 xflow-net-0.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:30:27.000000 xflow-net-0.1.3/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-17 23:30:27.000000 xflow-net-0.1.3/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 23:30:28.000000 xflow-net-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-17 23:30:40.183646 xflow-net-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-17 23:30:28.000000 xflow-net-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.171645 xflow-net-0.1.3/xflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.171645 xflow-net-0.1.3/xflow/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/dataset/nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/dataset/pyg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.171645 xflow-net-0.1.3/xflow/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/diffusion/IC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/diffusion/LT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/diffusion/SI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/diffusion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.175645 xflow-net-0.1.3/xflow/method/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.175645 xflow-net-0.1.3/xflow/method/cosasi/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.175645 xflow-net-0.1.3/xflow/method/cosasi/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/benchmark/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.175645 xflow-net-0.1.3/xflow/method/cosasi/contagion/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/contagion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/contagion/static_network_contagion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.175645 xflow-net-0.1.3/xflow/method/cosasi/source_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/algorithm_details.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.179646 xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/jordan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/lisn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/netsleuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.179646 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/earliest_infection_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/jordan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/lisn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/netsleuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/rumor_centrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/short_fat_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/source_inference/source_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.183646 xflow-net-0.1.3/xflow/method/cosasi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15690 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/utils/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/cosasi/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14190 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/im.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/method/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-17 23:30:28.000000 xflow-net-0.1.3/xflow/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 23:30:40.183646 xflow-net-0.1.3/xflow_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-17 23:30:40.000000 xflow-net-0.1.3/xflow_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-17 23:30:40.000000 xflow-net-0.1.3/xflow_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 23:30:40.000000 xflow-net-0.1.3/xflow_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 23:30:40.000000 xflow-net-0.1.3/xflow_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 23:30:40.000000 xflow-net-0.1.3/xflow_net.egg-info/top_level.txt
```

### Comparing `xflow-net-0.1.2/LICENSE` & `xflow-net-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/PKG-INFO` & `xflow-net-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.1.2
+Version: 0.1.3
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xflow-net-0.1.2/README.md` & `xflow-net-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/examples/main.py` & `xflow-net-0.1.3/examples/main.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/setup.py` & `xflow-net-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'xflow-net'
 DESCRIPTION = 'a python library for graph flow'
 URL = 'https://xflow.network/'
 EMAIL = 'zchen@cse.msstate.edu'
 AUTHOR = 'XGraphing'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'networkx', 'ndlib', 'torch_geometric', 'cosasi'
 ]
 
 # What packages are optional?
@@ -98,15 +98,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={NAME: ["source_inference/algorithm_details.json"]},
+    package_data={'xflow': ["method/cosasi/source_inference/algorithm_details.json"]},
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
```

### Comparing `xflow-net-0.1.2/xflow/dataset/nx.py` & `xflow-net-0.1.3/xflow/dataset/nx.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/dataset/pyg.py` & `xflow-net-0.1.3/xflow/dataset/pyg.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/diffusion/IC.py` & `xflow-net-0.1.3/xflow/diffusion/IC.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/diffusion/LT.py` & `xflow-net-0.1.3/xflow/diffusion/LT.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/diffusion/SI.py` & `xflow-net-0.1.3/xflow/diffusion/SI.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/benchmark/benchmark.py` & `xflow-net-0.1.3/xflow/method/cosasi/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/contagion/static_network_contagion.py` & `xflow-net-0.1.3/xflow/method/cosasi/contagion/static_network_contagion.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/jordan.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/jordan.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/lisn.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/lisn.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/multiple_source/netsleuth.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/multiple_source/netsleuth.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/earliest_infection_first.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/earliest_infection_first.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/jordan.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/jordan.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/lisn.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/lisn.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/netsleuth.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/netsleuth.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/rumor_centrality.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/rumor_centrality.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/single_source/short_fat_tree.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/single_source/short_fat_tree.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/source_inference/source_results.py` & `xflow-net-0.1.3/xflow/method/cosasi/source_inference/source_results.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/utils/estimators.py` & `xflow-net-0.1.3/xflow/method/cosasi/utils/estimators.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/cosasi/utils/helpers.py` & `xflow-net-0.1.3/xflow/method/cosasi/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/ibm.py` & `xflow-net-0.1.3/xflow/method/ibm.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/method/im.py` & `xflow-net-0.1.3/xflow/method/im.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/util.py` & `xflow-net-0.1.3/xflow/util.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow/visualization.py` & `xflow-net-0.1.3/xflow/visualization.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.1.2/xflow_net.egg-info/PKG-INFO` & `xflow-net-0.1.3/xflow_net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.1.2
+Version: 0.1.3
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xflow-net-0.1.2/xflow_net.egg-info/SOURCES.txt` & `xflow-net-0.1.3/xflow_net.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 xflow/method/sl.py
 xflow/method/cosasi/__init__.py
 xflow/method/cosasi/benchmark/__init__.py
 xflow/method/cosasi/benchmark/benchmark.py
 xflow/method/cosasi/contagion/__init__.py
 xflow/method/cosasi/contagion/static_network_contagion.py
 xflow/method/cosasi/source_inference/__init__.py
+xflow/method/cosasi/source_inference/algorithm_details.json
 xflow/method/cosasi/source_inference/source_results.py
 xflow/method/cosasi/source_inference/multiple_source/__init__.py
 xflow/method/cosasi/source_inference/multiple_source/jordan.py
 xflow/method/cosasi/source_inference/multiple_source/lisn.py
 xflow/method/cosasi/source_inference/multiple_source/netsleuth.py
 xflow/method/cosasi/source_inference/single_source/__init__.py
 xflow/method/cosasi/source_inference/single_source/earliest_infection_first.py
```

