# Comparing `tmp/TaGra-0.1.7.tar.gz` & `tmp/TaGra-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TaGra-0.1.7.tar", last modified: Sun May 19 13:52:03 2024, max compression
+gzip compressed data, was "TaGra-0.1.8.tar", last modified: Sat May 25 10:07:01 2024, max compression
```

## Comparing `TaGra-0.1.7.tar` & `TaGra-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:52:03.966589 TaGra-0.1.7/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.7/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 13:52:03.962589 TaGra-0.1.7/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)     3116 2024-05-19 00:21:18.000000 TaGra-0.1.7/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:52:03.962589 TaGra-0.1.7/TaGra.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 13:52:03.000000 TaGra-0.1.7/TaGra.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-19 13:52:03.000000 TaGra-0.1.7/TaGra.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-19 13:52:03.000000 TaGra-0.1.7/TaGra.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-19 13:52:03.000000 TaGra-0.1.7/TaGra.egg-info/entry_points.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-19 13:52:03.000000 TaGra-0.1.7/TaGra.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-19 13:52:03.000000 TaGra-0.1.7/TaGra.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-19 13:52:03.966589 TaGra-0.1.7/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-19 13:51:59.000000 TaGra-0.1.7/setup.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:52:03.962589 TaGra-0.1.7/tagra/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.7/tagra/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.7/tagra/analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.7/tagra/config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.7/tagra/graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.7/tagra/preprocessing.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7300 2024-05-19 13:51:10.000000 TaGra-0.1.7/tagra/utils.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:52:03.962589 TaGra-0.1.7/tests/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.7/tests/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.7/tests/test_analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.7/tests/test_config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.7/tests/test_graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.7/tests/test_preprocessing.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-25 10:07:01.173871 TaGra-0.1.8/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.8/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-25 10:07:01.173871 TaGra-0.1.8/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3116 2024-05-19 00:21:18.000000 TaGra-0.1.8/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-25 10:07:01.173871 TaGra-0.1.8/TaGra.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-25 10:07:01.000000 TaGra-0.1.8/TaGra.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-25 10:07:01.000000 TaGra-0.1.8/TaGra.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-25 10:07:01.000000 TaGra-0.1.8/TaGra.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-25 10:07:01.000000 TaGra-0.1.8/TaGra.egg-info/entry_points.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-25 10:07:01.000000 TaGra-0.1.8/TaGra.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-25 10:07:01.000000 TaGra-0.1.8/TaGra.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-25 10:07:01.173871 TaGra-0.1.8/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-25 10:06:54.000000 TaGra-0.1.8/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-25 10:07:01.173871 TaGra-0.1.8/tagra/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.8/tagra/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.8/tagra/analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.8/tagra/config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.8/tagra/graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.8/tagra/preprocessing.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     8768 2024-05-25 10:06:21.000000 TaGra-0.1.8/tagra/utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-25 10:07:01.173871 TaGra-0.1.8/tests/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.8/tests/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.8/tests/test_analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.8/tests/test_config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.8/tests/test_graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.8/tests/test_preprocessing.py
```

### Comparing `TaGra-0.1.7/LICENSE` & `TaGra-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/PKG-INFO` & `TaGra-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.7
+Version: 0.1.8
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TaGra-0.1.7/README.md` & `TaGra-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/TaGra.egg-info/PKG-INFO` & `TaGra-0.1.8/TaGra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.7
+Version: 0.1.8
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TaGra-0.1.7/setup.py` & `TaGra-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TaGra',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'scikit-learn',
         'matplotlib',
         'networkx',
```

### Comparing `TaGra-0.1.7/tagra/analysis.py` & `TaGra-0.1.8/tagra/analysis.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tagra/config.py` & `TaGra-0.1.8/tagra/config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tagra/graph.py` & `TaGra-0.1.8/tagra/graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tagra/preprocessing.py` & `TaGra-0.1.8/tagra/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tagra/utils.py` & `TaGra-0.1.8/tagra/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -168,7 +168,42 @@
         color_array = cmap(colors)
         node_color = [color_array[unique_dict[key]] for key in y]
     nx.draw(G, pos, with_labels=True, node_size=50, font_size=8, node_color = node_color)
     plt.title("Graph of Relations Based on Manifold Learning Transformed Data")
     if outpath:
         plt.savefig(outpath)
         print(f'{datetime.datetime.now()}: Graph saved in {outpath}')
+
+def measure_mixing_matrix(G, communities):
+    N_communities = len(communities.keys())
+    community_edge_count = np.zeros((N_communities, N_communities))
+
+    # Create a mapping from node to its community
+    node_to_community = {}
+    for community, nodes in communities.items():
+        for node in nodes:
+            node_to_community[node] = community
+
+    # Check if all nodes in the graph are covered by the communities
+    graph_nodes = set(G.nodes())
+    community_nodes = set(node_to_community.keys())
+    if graph_nodes != community_nodes:
+        missing_in_communities = graph_nodes - community_nodes
+        missing_in_graph = community_nodes - graph_nodes
+        raise ValueError(
+            f"The nodes in the communities do not match the nodes in the graph.\n"
+            f"Nodes in the graph not in communities: {missing_in_communities}\n"
+            f"Nodes in communities not in the graph: {missing_in_graph}"
+        )
+
+    # Iterate over all edges in the graph
+    for source, target in G.edges():
+        if source in node_to_community and target in node_to_community:
+            c_source = node_to_community[source]
+            c_target = node_to_community[target]
+            if not G.is_directed():
+                community_edge_count[c_source, c_target] += 1
+                community_edge_count[c_target, c_source] += 1
+            else:
+                community_edge_count[c_source, c_target] += 1
+
+    return community_edge_count
```

### Comparing `TaGra-0.1.7/tests/test_analysis.py` & `TaGra-0.1.8/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tests/test_config.py` & `TaGra-0.1.8/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tests/test_graph.py` & `TaGra-0.1.8/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.7/tests/test_preprocessing.py` & `TaGra-0.1.8/tests/test_preprocessing.py`

 * *Files identical despite different names*

