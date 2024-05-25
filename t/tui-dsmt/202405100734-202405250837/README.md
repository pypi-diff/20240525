# Comparing `tmp/tui_dsmt-202405100734.tar.gz` & `tmp/tui_dsmt-202405250837.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202405100734.tar", last modified: Fri May 10 07:34:48 2024, max compression
+gzip compressed data, was "tui_dsmt-202405250837.tar", last modified: Sat May 25 08:37:12 2024, max compression
```

## Comparing `tui_dsmt-202405100734.tar` & `tui_dsmt-202405250837.tar`

### file list

```diff
@@ -1,69 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.455278 tui_dsmt-202405100734/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-10 07:34:48.455278 tui_dsmt-202405100734/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 07:34:48.455278 tui_dsmt-202405100734/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1324 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.415277 tui_dsmt-202405100734/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.419277 tui_dsmt-202405100734/src/tui_dsmt/
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.423277 tui_dsmt-202405100734/src/tui_dsmt/clustering/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/PAM.py
--rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2691 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/animation.py
--rw-rw-rw-   0 root         (0) root         (0)    19467 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/draw.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4488 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/hierarchical.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/clustering/interactive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.427277 tui_dsmt-202405100734/src/tui_dsmt/fpm/
--rw-rw-rw-   0 root         (0) root         (0)    14098 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/BruteForceFI.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalFPTree.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalPatternBase.py
--rw-rw-rw-   0 root         (0) root         (0)    11867 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/FPTree.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/HashTree.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/Itemset.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGrid.py
--rw-rw-rw-   0 root         (0) root         (0)     5942 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridApriori.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridECLAT.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialItemset.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/TransactionDatabase.py
--rw-rw-rw-   0 root         (0) root         (0)   112752 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/fpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.435277 tui_dsmt-202405100734/src/tui_dsmt/graph/
--rw-rw-rw-   0 root         (0) root         (0)     3894 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/BFS.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/BipartiteFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/DFS.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/Dijkstra.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/EdmondsKarp.py
--rw-rw-rw-   0 root         (0) root         (0)     4747 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/FordFulkerson.py
--rw-rw-rw-   0 root         (0) root         (0)     4860 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/FruchtermanReingold.py
--rw-rw-rw-   0 root         (0) root         (0)     4461 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/Hall.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/InteractiveGraph.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/Kruskal.py
--rw-rw-rw-   0 root         (0) root         (0)     4877 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/LabelPropagation.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/MaximumFlow.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/RandomWalk.py
--rw-rw-rw-   0 root         (0) root         (0)   420281 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     5267 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/game.py
--rw-rw-rw-   0 root         (0) root         (0)     6426 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/html.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/representation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.435277 tui_dsmt-202405100734/src/tui_dsmt/graph/resources/
--rw-rw-rw-   0 root         (0) root         (0)  8978701 2024-05-08 12:12:17.000000 tui_dsmt-202405100734/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt/jpanim/
--rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/JupyterAnimation.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls-ff.html
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls.html
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/script.js
--rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/style.css
--rw-rw-rw-   0 root         (0) root         (0)   147897 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt/util/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-08 06:56:21.000000 tui_dsmt-202405100734/src/tui_dsmt/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 07:34:48.451278 tui_dsmt-202405100734/src/tui_dsmt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-10 07:34:48.000000 tui_dsmt-202405100734/src/tui_dsmt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.505414 tui_dsmt-202405250837/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-25 08:37:12.505414 tui_dsmt-202405250837/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 08:37:12.505414 tui_dsmt-202405250837/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1355 2024-05-25 08:24:02.000000 tui_dsmt-202405250837/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.481414 tui_dsmt-202405250837/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.485414 tui_dsmt-202405250837/src/tui_dsmt/
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.485414 tui_dsmt-202405250837/src/tui_dsmt/clustering/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/PAM.py
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/animation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19467 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/hierarchical.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/clustering/interactive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.489414 tui_dsmt-202405250837/src/tui_dsmt/fpm/
+-rw-rw-rw-   0 root         (0) root         (0)    14098 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/BruteForceFI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/ConditionalFPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/ConditionalPatternBase.py
+-rw-rw-rw-   0 root         (0) root         (0)    11873 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/FPTree.py
+-rw-rw-rw-   0 root         (0) root         (0)    19208 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/HashTree.py
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/Itemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/ItemsetGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5942 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/ItemsetGridApriori.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/ItemsetGridECLAT.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/SequentialDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-05-25 08:24:02.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/SequentialItemset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/TransactionDatabase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2024-05-25 08:24:02.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-25 08:24:02.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.489414 tui_dsmt-202405250837/src/tui_dsmt/fpm/resources/
+-rw-rw-rw-   0 root         (0) root         (0)    52516 2024-05-25 08:24:02.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/resources/website_tracking.csv
+-rw-rw-rw-   0 root         (0) root         (0)   125202 2024-05-25 08:24:02.000000 tui_dsmt-202405250837/src/tui_dsmt/fpm/resources/website_tracking2.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.493414 tui_dsmt-202405250837/src/tui_dsmt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/BFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/BipartiteFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/BronKerbosch.py
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/DFS.py
+-rw-rw-rw-   0 root         (0) root         (0)     5843 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/Dijkstra.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/EdmondsKarp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4747 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/FordFulkerson.py
+-rw-rw-rw-   0 root         (0) root         (0)     4860 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/FruchtermanReingold.py
+-rw-rw-rw-   0 root         (0) root         (0)     4461 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/Hall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/InteractiveGraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/Kruskal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/LabelPropagation.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/MarkovClusterAlgorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/MaximumFlow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/RandomWalk.py
+-rw-rw-rw-   0 root         (0) root         (0)   420395 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2024-05-23 09:06:34.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     5267 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/game.py
+-rw-rw-rw-   0 root         (0) root         (0)     6426 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/html.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/representation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.493414 tui_dsmt-202405250837/src/tui_dsmt/graph/resources/
+-rw-rw-rw-   0 root         (0) root         (0)  8978701 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.501414 tui_dsmt-202405250837/src/tui_dsmt/jpanim/
+-rw-rw-rw-   0 root         (0) root         (0)     2935 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/JupyterAnimation.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.501414 tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/controls-ff.html
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/controls.html
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/script.js
+-rw-rw-rw-   0 root         (0) root         (0)      193 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/style.css
+-rw-rw-rw-   0 root         (0) root         (0)   147897 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/vue-3.4.24.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.505414 tui_dsmt-202405250837/src/tui_dsmt/util/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-18 09:15:33.000000 tui_dsmt-202405250837/src/tui_dsmt/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 08:37:12.505414 tui_dsmt-202405250837/src/tui_dsmt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-25 08:37:12.000000 tui_dsmt-202405250837/src/tui_dsmt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2117 2024-05-25 08:37:12.000000 tui_dsmt-202405250837/src/tui_dsmt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 08:37:12.000000 tui_dsmt-202405250837/src/tui_dsmt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-25 08:37:12.000000 tui_dsmt-202405250837/src/tui_dsmt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-25 08:37:12.000000 tui_dsmt-202405250837/src/tui_dsmt.egg-info/top_level.txt
```

### Comparing `tui_dsmt-202405100734/PKG-INFO` & `tui_dsmt-202405250837/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202405100734
+Version: 202405250837
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202405100734/setup.py` & `tui_dsmt-202405250837/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,13 +34,14 @@
         'pyarrow~=15.0.2',
         'pyfpgrowth~=1.0',
         'scikit-learn~=1.4.2',
         'scikit-learn-extra~=0.3.0'
     ],
     package_data={
         'tui_dsmt': [
+            'fpm/resources/*',
             'graph/resources/*',
             'jpanim/resources/*'
         ]
     },
     include_package_data=True
 )
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/__init__.py` & `tui_dsmt-202405250837/src/tui_dsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/clustering/PAM.py` & `tui_dsmt-202405250837/src/tui_dsmt/clustering/PAM.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/clustering/animation.py` & `tui_dsmt-202405250837/src/tui_dsmt/clustering/animation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/clustering/datasets.py` & `tui_dsmt-202405250837/src/tui_dsmt/clustering/datasets.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/clustering/evaluation.py` & `tui_dsmt-202405250837/src/tui_dsmt/clustering/evaluation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/clustering/hierarchical.py` & `tui_dsmt-202405250837/src/tui_dsmt/clustering/hierarchical.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/clustering/interactive.py` & `tui_dsmt-202405250837/src/tui_dsmt/clustering/interactive.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/BruteForceFI.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/BruteForceFI.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalFPTree.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/ConditionalFPTree.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/ConditionalPatternBase.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/ConditionalPatternBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,17 @@
                 return 'rgba(99, 110, 250, 0.5)'
             else:
                 return 'transparent'
 
         frames = {
             'Ende der Transaktionen': {
                 **{
-                    f'name_{node}': f'{node[-1]} ({names[node]})' if len(node) > 0 else fp_tree.head_name[::-1]
+                    f'name_{node}': f'{node[-1]} ({names[node]})' if len(node) > 0 else (
+                        fp_tree.head_name[::-1] if fp_tree.head_name not in ('{}', '}{') else '{}'
+                    )
                     for node in fp_tree.graph.nodes
                 },
                 **{
                     f'node_{node}': {
                         'backgroundColor': '#636EFA',
                         'color': 'whitesmoke'
                     }
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/FPTree.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/FPTree.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..jpanim import JupyterAnimation
 from .. import color_secondary
 
 TRANSACTION_LIST = List[Tuple[int, Union[Itemset, Tuple]]]
 
 
 # Das rumgepatche am Namen mit [::-1] fällt mir noch auf die Füße...
+# z.B. #74
 class FPTree(JupyterAnimation):
     def __init__(self, transactions: TRANSACTION_LIST, min_supp: int, head_name: str = '{}', sort: bool = True,
                  custom_item_order: Iterator = None):
         self.transactions: TRANSACTION_LIST = transactions
         self.min_supp: int = min_supp
         self.head_name: str = head_name
 
@@ -54,15 +55,15 @@
 
         # frame generation
         frames = {
             'Initialisierung': {
                 'current_transaction': '',
                 'cleaned_transaction': '',
                 **{
-                    f'name_{node}': node[-1] if len(node) > 0 else (head_name if head_name == '{}' else head_name[::-1])
+                    f'name_{node}': node[-1] if len(node) > 0 else (head_name[::-1] if head_name != '{}' else '{}')
                     for node in self.graph.nodes
                 },
                 **{
                     f'node_{node}': {
                         'backgroundColor': '#636EFA',
                         'color': 'whitesmoke',
                         'display': 'none' if node != '' else 'flex'
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/HashTree.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/HashTree.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     def insert(self, values: Tuple, d: int = 0, retry: bool = False) -> Iterator:
         hashed = self.hash_function(values[d])
 
         if not retry:
             yield f'Hash {d + 1}: {values[d]} -> {hashed} (Itemset: {values})', {
                 **{
                     f'{self.name}_{i}_bg': f'rgb({color_primary})' if i == hashed else 'white'
-                    for i in range(len(values))
+                    for i in range(self.hash_outputs)
                 },
                 **{
                     f'item_{i}_bg': f'rgb({color_primary})' if i == d else 'transparent'
-                    for i in range(len(values))
+                    for i in range(self.hash_outputs)
                 }
             }
 
         # Try to insert the itemset.
         try:
             yield from self.children[hashed].insert(values, d + 1)
 
@@ -90,15 +90,15 @@
                     pass
 
             yield f'Aufteilen des Blattes (Itemset: {values})', {
                 f'{old_leaf.name}_leaf': False,
                 f'{new_inner.name}_inner': True,
                 **{
                     f'{new_inner.name}_{i}_bg': f'rgb({color_secondary})'
-                    for i in range(len(values))
+                    for i in range(self.hash_outputs)
                 },
                 **{
                     f'{c.name}_leaf': True
                     for c in new_inner.children.values()
                 },
                 **{
                     f'{c.name}_text': '<br>'.join(f'({", ".join(map(str, t))})' for t in c.table)
@@ -144,21 +144,29 @@
 
     def __str__(self, d: int = 0) -> str:
         return str(self.table)
 
 
 class HashTree(JupyterAnimation):
     def __init__(self, candidates: List, hash_function: Callable, hash_outputs: int, table_size: int = 3):
-        base_width = 1.5
-
         self.candidates: List = candidates
         self.hash_function: Callable = hash_function
         self.hash_outputs: int = hash_outputs
         self.table_size: int = table_size
 
+        # Calculate some basic measurements to scale boxes
+        # and calculate positions.
+        for c in candidates:
+            base_width = len(c) * 0.5
+            break
+        else:
+            raise AssertionError('Kandidatenmenge ist leer')
+
+        base_height = table_size * 1.4
+
         # Create a hashtree to calculate node positions. Store
         # the actions happened during the creating as frames.
         self.root = HashInner(hash_function, hash_outputs, table_size)
 
         self._frames = {
             'Initialisierung der Wurzel': {
                 f'{self.root.name}_inner': True,
@@ -277,15 +285,15 @@
         # Therefore, they share the same positions and we only
         # hide or display whatever we need in the current frame.
         leaves = []
 
         for el, *_ in self.root.traverse():
             style = {
                 'width': f'{3 * base_width}rem',
-                'height': '5rem',
+                'height': f'{base_height}rem',
                 'padding': '0.2rem 0.4rem',
                 'font-size': '90%',
                 'position': 'absolute',
                 'left': f'calc({x_pos[el.name]} * 100% - {1.5 * base_width}rem)',
                 'top': f'calc({y_pos[el.name]} * 100%)',
                 'box-sizing': 'border-box',
                 'border': '1px solid black',
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/Itemset.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/Itemset.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGrid.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/ItemsetGrid.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridApriori.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/ItemsetGridApriori.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/ItemsetGridECLAT.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/ItemsetGridECLAT.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialDatabase.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/SequentialItemset.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/SequentialItemset.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,8 +34,8 @@
             if e == prefix[i]:
                 i += 1
 
             if i == len(prefix):
                 return SequentialItemset(*self[k:])
 
     def __str__(self):
-        return f'<{", ".join(self)}>'
+        return f'<{", ".join(map(str, self))}>'
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/fpm/TransactionDatabase.py` & `tui_dsmt-202405250837/src/tui_dsmt/fpm/TransactionDatabase.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/BFS.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/BFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/BipartiteFlow.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/BipartiteFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/DFS.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/DFS.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/Dijkstra.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/Dijkstra.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/FordFulkerson.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/FordFulkerson.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/FruchtermanReingold.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/FruchtermanReingold.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/Hall.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/Hall.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/InteractiveGraph.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/InteractiveGraph.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/Kruskal.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/Kruskal.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/LabelPropagation.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/LabelPropagation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/MaximumFlow.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/MaximumFlow.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/RandomWalk.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/RandomWalk.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/__init__.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import re
 
 import matplotlib.pyplot as plt
 import networkx as nx
 
 from .BFS import BFS
 from .BipartiteFlow import BipartiteFlow
+from .BronKerbosch import BronKerbosch
 from .DFS import DFS
 from .Dijkstra import Dijkstra
 from .EdmondsKarp import EdmondsKarp
 from .FordFulkerson import FordFulkerson
 from .FruchtermanReingold import FruchtermanReingold
 from .Hall import Hall
 from .InteractiveGraph import InteractiveGraph
 from .Kruskal import Kruskal
 from .LabelPropagation import LabelPropagation
 from .MaximumFlow import MaximumFlow
 from .game import guess_adj_list, guess_adj_matrix
 from .RandomWalk import RandomWalk
 from .representation import draw_adj_list, draw_adj_matrix
 
+
+def set_label(c):
+    s = ','.join(map(str, c))
+    return f'{{{s}}}'
+
+
 # Städte im deutschen Sprachhrraum
 dach_cities = nx.Graph()
 dach_cities.add_edge('Hannover', 'Frankfurt', d=350)
 dach_cities.add_edge('Hannover', 'Hamburg', d=150)
 dach_cities.add_edge('Hannover', 'Berlin', d=290)
 dach_cities.add_edge('Frankfurt', 'Zürich', d=400)
 dach_cities.add_edge('Berlin', 'Wien', d=680)
@@ -7354,22 +7361,22 @@
 
 small_communities = nx.Graph()
 small_communities.add_edge(1, 2)
 small_communities.add_edge(1, 3)
 small_communities.add_edge(1, 4)
 small_communities.add_edge(2, 3)
 small_communities.add_edge(2, 4)
-#small_communities.add_edge(2, 5)
+# small_communities.add_edge(2, 5)
 small_communities.add_edge(3, 4)
 small_communities.add_edge(3, 15)
 small_communities.add_edge(4, 7)
 small_communities.add_edge(5, 6)
 small_communities.add_edge(5, 7)
 small_communities.add_edge(6, 7)
-#small_communities.add_edge(7, 8)
+# small_communities.add_edge(7, 8)
 small_communities.add_edge(8, 9)
 small_communities.add_edge(8, 11)
 small_communities.add_edge(8, 13)
 small_communities.add_edge(8, 15)
 small_communities.add_edge(9, 10)
 small_communities.add_edge(10, 11)
 small_communities.add_edge(11, 12)
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/game.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/game.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/html.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/html.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/representation.py` & `tui_dsmt-202405250837/src/tui_dsmt/graph/representation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2` & `tui_dsmt-202405250837/src/tui_dsmt/graph/resources/dewiki_sample.pickle.bz2`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/jpanim/JupyterAnimation.py` & `tui_dsmt-202405250837/src/tui_dsmt/jpanim/JupyterAnimation.py`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls-ff.html` & `tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/controls-ff.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/controls.html` & `tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/controls.html`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/script.js` & `tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/script.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt/jpanim/resources/vue-3.4.24.js` & `tui_dsmt-202405250837/src/tui_dsmt/jpanim/resources/vue-3.4.24.js`

 * *Files identical despite different names*

### Comparing `tui_dsmt-202405100734/src/tui_dsmt.egg-info/PKG-INFO` & `tui_dsmt-202405250837/src/tui_dsmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tui_dsmt
-Version: 202405100734
+Version: 202405250837
 Summary: everything you need for our jupyter notebooks
 Home-page: https://dbgit.prakinf.tu-ilmenau.de/lectures/data-science-methoden-und-techniken
 Author: Eric Tröbs
 Author-email: eric.troebs@tu-ilmenau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tui_dsmt-202405100734/src/tui_dsmt.egg-info/SOURCES.txt` & `tui_dsmt-202405250837/src/tui_dsmt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,20 @@
 src/tui_dsmt/fpm/ItemsetGrid.py
 src/tui_dsmt/fpm/ItemsetGridApriori.py
 src/tui_dsmt/fpm/ItemsetGridECLAT.py
 src/tui_dsmt/fpm/SequentialDatabase.py
 src/tui_dsmt/fpm/SequentialItemset.py
 src/tui_dsmt/fpm/TransactionDatabase.py
 src/tui_dsmt/fpm/__init__.py
+src/tui_dsmt/fpm/datasets.py
+src/tui_dsmt/fpm/resources/website_tracking.csv
+src/tui_dsmt/fpm/resources/website_tracking2.json
 src/tui_dsmt/graph/BFS.py
 src/tui_dsmt/graph/BipartiteFlow.py
+src/tui_dsmt/graph/BronKerbosch.py
 src/tui_dsmt/graph/DFS.py
 src/tui_dsmt/graph/Dijkstra.py
 src/tui_dsmt/graph/EdmondsKarp.py
 src/tui_dsmt/graph/FordFulkerson.py
 src/tui_dsmt/graph/FruchtermanReingold.py
 src/tui_dsmt/graph/Hall.py
 src/tui_dsmt/graph/InteractiveGraph.py
```

