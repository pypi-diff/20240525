# Comparing `tmp/pygda-0.0.1.tar.gz` & `tmp/pygda-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygda-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pygda-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pygda-0.0.1.tar` & `pygda-0.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5186 2024-05-11 02:39:24.799728 pygda-0.0.1/README.md
--rw-r--r--   0        0        0      172 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/__init__.py
--rw-r--r--   0        0        0      576 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/__init__.py
--rw-r--r--   0        0        0     2856 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/airport.py
--rw-r--r--   0        0        0     2393 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/arxiv.py
--rw-r--r--   0        0        0     2748 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/blog.py
--rw-r--r--   0        0        0     3237 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/citation.py
--rw-r--r--   0        0        0     2800 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/elliptic.py
--rw-r--r--   0        0        0     4523 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/facebook.py
--rw-r--r--   0        0        0     2416 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/mag.py
--rw-r--r--   0        0        0     2779 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/squirrel.py
--rw-r--r--   0        0        0     4370 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/twitch.py
--rw-r--r--   0        0        0     2421 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/datasets/twitter.py
--rw-r--r--   0        0        0      383 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/metrics/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-14 08:33:04.399695 pygda-0.0.1/pygda/metrics/metrics.py
--rw-r--r--   0        0        0      697 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/models/__init__.py
--rw-r--r--   0        0        0     7414 2024-05-15 07:31:38.239685 pygda-0.0.1/pygda/models/a2gnn.py
--rw-r--r--   0        0        0    11327 2024-05-15 07:35:06.295685 pygda-0.0.1/pygda/models/acdne.py
--rw-r--r--   0        0        0     9514 2024-05-16 05:22:19.555676 pygda-0.0.1/pygda/models/adagcn.py
--rw-r--r--   0        0        0    13352 2024-05-15 07:38:50.419685 pygda-0.0.1/pygda/models/asn.py
--rw-r--r--   0        0        0     4383 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/models/base.py
--rw-r--r--   0        0        0     8615 2024-05-16 08:21:19.395674 pygda-0.0.1/pygda/models/cwgcn.py
--rw-r--r--   0        0        0    11770 2024-05-15 07:39:20.411685 pygda-0.0.1/pygda/models/dane.py
--rw-r--r--   0        0        0    11852 2024-05-16 09:00:46.931674 pygda-0.0.1/pygda/models/dgda.py
--rw-r--r--   0        0        0    12125 2024-05-16 08:16:30.755674 pygda-0.0.1/pygda/models/dmgnn.py
--rw-r--r--   0        0        0     5895 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/models/gnn.py
--rw-r--r--   0        0        0     7557 2024-05-16 05:30:12.747676 pygda-0.0.1/pygda/models/grade.py
--rw-r--r--   0        0        0     8903 2024-05-16 07:50:03.843675 pygda-0.0.1/pygda/models/jhgda.py
--rw-r--r--   0        0        0     5961 2024-05-16 08:09:23.503674 pygda-0.0.1/pygda/models/kbl.py
--rw-r--r--   0        0        0    23357 2024-05-16 09:21:23.087674 pygda-0.0.1/pygda/models/pa.py
--rw-r--r--   0        0        0     7477 2024-05-16 08:38:02.947674 pygda-0.0.1/pygda/models/sagda.py
--rw-r--r--   0        0        0    10339 2024-05-16 06:00:37.739675 pygda-0.0.1/pygda/models/specreg.py
--rw-r--r--   0        0        0    18281 2024-05-16 06:10:08.483675 pygda-0.0.1/pygda/models/strurw.py
--rw-r--r--   0        0        0     7827 2024-05-15 07:36:43.751685 pygda-0.0.1/pygda/models/udagcn.py
--rw-r--r--   0        0        0     1180 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/a2gnn_base.py
--rw-r--r--   0        0        0     4612 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/acdne_base.py
--rw-r--r--   0        0        0     2770 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/adagcn_base.py
--rw-r--r--   0        0        0     6921 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/asn_base.py
--rw-r--r--   0        0        0      469 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/attention.py
--rw-r--r--   0        0        0     4766 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/cached_gcn_conv.py
--rw-r--r--   0        0        0     4107 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/cwgcn_base.py
--rw-r--r--   0        0        0     1926 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/deepwalk_pretrain.py
--rw-r--r--   0        0        0    11050 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/dgda_base.py
--rw-r--r--   0        0        0     9982 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/gmm_clustering.py
--rw-r--r--   0        0        0     3573 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/gnn_base.py
--rw-r--r--   0        0        0     2833 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/grade_base.py
--rw-r--r--   0        0        0    12117 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/jhgda_base.py
--rw-r--r--   0        0        0    39000 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/kbl_base.py
--rw-r--r--   0        0        0     4045 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/mixup_base.py
--rw-r--r--   0        0        0     7526 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/mixup_gcnconv.py
--rw-r--r--   0        0        0     3671 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/ppmi_conv.py
--rw-r--r--   0        0        0     6842 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/prop_gcn_conv.py
--rw-r--r--   0        0        0      303 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/reverse_layer.py
--rw-r--r--   0        0        0    11146 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/reweight_gnn.py
--rw-r--r--   0        0        0     7161 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/sagda_base.py
--rw-r--r--   0        0        0     4303 2024-05-10 10:40:36.119735 pygda-0.0.1/pygda/nn/udagcn_base.py
--rw-r--r--   0        0        0       71 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/utils/__init__.py
--rw-r--r--   0        0        0     2061 2024-05-11 07:12:00.991726 pygda-0.0.1/pygda/utils/mmd.py
--rw-r--r--   0        0        0      917 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/utils/svd_transform.py
--rw-r--r--   0        0        0     1912 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/utils/utility.py
--rw-r--r--   0        0        0       21 2024-05-10 10:40:36.115735 pygda-0.0.1/pygda/version.py
--rw-r--r--   0        0        0      467 2024-05-24 07:49:35.871592 pygda-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5586 1970-01-01 00:00:00.000000 pygda-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5322 2024-05-24 09:10:45.063592 pygda-0.0.2/README.md
+-rw-r--r--   0        0        0      172 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/__init__.py
+-rw-r--r--   0        0        0      576 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/__init__.py
+-rw-r--r--   0        0        0     2856 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/airport.py
+-rw-r--r--   0        0        0     2393 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/arxiv.py
+-rw-r--r--   0        0        0     2748 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/blog.py
+-rw-r--r--   0        0        0     3237 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/citation.py
+-rw-r--r--   0        0        0     2800 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/elliptic.py
+-rw-r--r--   0        0        0     4523 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/facebook.py
+-rw-r--r--   0        0        0     2416 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/mag.py
+-rw-r--r--   0        0        0     2779 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/squirrel.py
+-rw-r--r--   0        0        0     4370 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/twitch.py
+-rw-r--r--   0        0        0     2421 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/datasets/twitter.py
+-rw-r--r--   0        0        0      383 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/metrics/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-14 08:33:04.399695 pygda-0.0.2/pygda/metrics/metrics.py
+-rw-r--r--   0        0        0      697 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/models/__init__.py
+-rw-r--r--   0        0        0     7414 2024-05-15 07:31:38.239685 pygda-0.0.2/pygda/models/a2gnn.py
+-rw-r--r--   0        0        0    11327 2024-05-15 07:35:06.295685 pygda-0.0.2/pygda/models/acdne.py
+-rw-r--r--   0        0        0     9514 2024-05-16 05:22:19.555676 pygda-0.0.2/pygda/models/adagcn.py
+-rw-r--r--   0        0        0    13352 2024-05-15 07:38:50.419685 pygda-0.0.2/pygda/models/asn.py
+-rw-r--r--   0        0        0     4383 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/models/base.py
+-rw-r--r--   0        0        0     8615 2024-05-16 08:21:19.395674 pygda-0.0.2/pygda/models/cwgcn.py
+-rw-r--r--   0        0        0    11770 2024-05-15 07:39:20.411685 pygda-0.0.2/pygda/models/dane.py
+-rw-r--r--   0        0        0    11852 2024-05-16 09:00:46.931674 pygda-0.0.2/pygda/models/dgda.py
+-rw-r--r--   0        0        0    12125 2024-05-16 08:16:30.755674 pygda-0.0.2/pygda/models/dmgnn.py
+-rw-r--r--   0        0        0     5895 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/models/gnn.py
+-rw-r--r--   0        0        0     7557 2024-05-16 05:30:12.747676 pygda-0.0.2/pygda/models/grade.py
+-rw-r--r--   0        0        0     8903 2024-05-16 07:50:03.843675 pygda-0.0.2/pygda/models/jhgda.py
+-rw-r--r--   0        0        0     5961 2024-05-16 08:09:23.503674 pygda-0.0.2/pygda/models/kbl.py
+-rw-r--r--   0        0        0    23357 2024-05-16 09:21:23.087674 pygda-0.0.2/pygda/models/pa.py
+-rw-r--r--   0        0        0     7477 2024-05-16 08:38:02.947674 pygda-0.0.2/pygda/models/sagda.py
+-rw-r--r--   0        0        0    10339 2024-05-16 06:00:37.739675 pygda-0.0.2/pygda/models/specreg.py
+-rw-r--r--   0        0        0    18281 2024-05-16 06:10:08.483675 pygda-0.0.2/pygda/models/strurw.py
+-rw-r--r--   0        0        0     7827 2024-05-24 11:54:32.367591 pygda-0.0.2/pygda/models/udagcn.py
+-rw-r--r--   0        0        0     1180 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/a2gnn_base.py
+-rw-r--r--   0        0        0     4612 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/acdne_base.py
+-rw-r--r--   0        0        0     2770 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/adagcn_base.py
+-rw-r--r--   0        0        0     6921 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/asn_base.py
+-rw-r--r--   0        0        0      469 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/attention.py
+-rw-r--r--   0        0        0     4136 2024-05-24 11:54:11.819590 pygda-0.0.2/pygda/nn/cached_gcn_conv.py
+-rw-r--r--   0        0        0     4107 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/cwgcn_base.py
+-rw-r--r--   0        0        0     1926 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/deepwalk_pretrain.py
+-rw-r--r--   0        0        0    11050 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/dgda_base.py
+-rw-r--r--   0        0        0     9982 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/gmm_clustering.py
+-rw-r--r--   0        0        0     3573 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/gnn_base.py
+-rw-r--r--   0        0        0     2833 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/grade_base.py
+-rw-r--r--   0        0        0    12117 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/jhgda_base.py
+-rw-r--r--   0        0        0    39000 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/kbl_base.py
+-rw-r--r--   0        0        0     4045 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/mixup_base.py
+-rw-r--r--   0        0        0     7526 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/mixup_gcnconv.py
+-rw-r--r--   0        0        0     3696 2024-05-24 11:53:55.491591 pygda-0.0.2/pygda/nn/ppmi_conv.py
+-rw-r--r--   0        0        0     6842 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/prop_gcn_conv.py
+-rw-r--r--   0        0        0      303 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/reverse_layer.py
+-rw-r--r--   0        0        0    11146 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/reweight_gnn.py
+-rw-r--r--   0        0        0     7161 2024-05-10 10:40:36.119735 pygda-0.0.2/pygda/nn/sagda_base.py
+-rw-r--r--   0        0        0     4303 2024-05-24 11:54:21.971591 pygda-0.0.2/pygda/nn/udagcn_base.py
+-rw-r--r--   0        0        0       71 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/utils/__init__.py
+-rw-r--r--   0        0        0     2061 2024-05-11 07:12:00.991726 pygda-0.0.2/pygda/utils/mmd.py
+-rw-r--r--   0        0        0     1028 2024-05-24 11:01:48.275591 pygda-0.0.2/pygda/utils/svd_transform.py
+-rw-r--r--   0        0        0     1912 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/utils/utility.py
+-rw-r--r--   0        0        0       21 2024-05-10 10:40:36.115735 pygda-0.0.2/pygda/version.py
+-rw-r--r--   0        0        0      467 2024-05-24 14:09:47.955590 pygda-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 pygda-0.0.2/PKG-INFO
```

### Comparing `pygda-0.0.1/README.md` & `pygda-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,32 +19,43 @@
 **PyGDA is featured for:**
 * **Consistent APIs and comprehensive documentation.**
 * **Cover 15+ graph domain adaptation models.**
 * **Scalable architecture that efficiently handles large graph datasets through mini-batching and sampling techniques.**
 * **Seamlessly integrated data processing with PyG, ensuring full compatibility with PyG data structures.**
 
 ## Installation
-Note: PyGDA depends on [PyTorch](https://pytorch.org/), [PyG](https://pytorch-geometric.readthedocs.io/en/latest/), and [PyTorch Sparse](https://github.com/rusty1s/pytorch_sparse). PyGDA does not automatically install these libraries for you. Please use the provided links above to install them separately in order to run PyGDA successfully.
+Note: PyGDA depends on [PyTorch](https://pytorch.org/), [PyG](https://pytorch-geometric.readthedocs.io/en/latest/), [PyTorch Sparse](https://github.com/rusty1s/pytorch_sparse) and [Pytorch Scatter](https://github.com/rusty1s/pytorch_scatter). PyGDA does not automatically install these libraries for you. Please install them separately in order to run PyGDA successfully.
+
+**Required Dependencies:**
+
 * torch>=1.13.1
 * torch_geometric>=2.4.0
 * torch_sparse>=0.6.15
+* torch_scatter>=2.1.0
+* python3
+* scipy
+* sklearn
+* numpy
+* cvxpy
+* tqdm
+
+**Installing with pip:**
+```
+pip install pygda
+```
+
+or 
 
 **Installation for local development:**
 ```
 git clone https://github.com/pygda-team/pygda
 cd pygda
+pip install -e .
 ```
 
-**Required Dependencies:**
-* python
-* scipy
-* sklearn
-* numpy
-* cvxpy
-
 ## Quick Start
 
 ### Step 1: Load Data
 ```
 from pygda.datasets import CitationDataset
 
 source_dataset = CitationDataset(path, args.source)
```

### Comparing `pygda-0.0.1/pygda/datasets/__init__.py` & `pygda-0.0.2/pygda/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/airport.py` & `pygda-0.0.2/pygda/datasets/airport.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/arxiv.py` & `pygda-0.0.2/pygda/datasets/arxiv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/blog.py` & `pygda-0.0.2/pygda/datasets/blog.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/citation.py` & `pygda-0.0.2/pygda/datasets/citation.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/elliptic.py` & `pygda-0.0.2/pygda/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/facebook.py` & `pygda-0.0.2/pygda/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/mag.py` & `pygda-0.0.2/pygda/datasets/mag.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/squirrel.py` & `pygda-0.0.2/pygda/datasets/squirrel.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/twitch.py` & `pygda-0.0.2/pygda/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/datasets/twitter.py` & `pygda-0.0.2/pygda/datasets/twitter.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/metrics/metrics.py` & `pygda-0.0.2/pygda/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/__init__.py` & `pygda-0.0.2/pygda/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/a2gnn.py` & `pygda-0.0.2/pygda/models/a2gnn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/acdne.py` & `pygda-0.0.2/pygda/models/acdne.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/adagcn.py` & `pygda-0.0.2/pygda/models/adagcn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/asn.py` & `pygda-0.0.2/pygda/models/asn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/base.py` & `pygda-0.0.2/pygda/models/base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/cwgcn.py` & `pygda-0.0.2/pygda/models/cwgcn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/dane.py` & `pygda-0.0.2/pygda/models/dane.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/dgda.py` & `pygda-0.0.2/pygda/models/dgda.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/dmgnn.py` & `pygda-0.0.2/pygda/models/dmgnn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/gnn.py` & `pygda-0.0.2/pygda/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/grade.py` & `pygda-0.0.2/pygda/models/grade.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/jhgda.py` & `pygda-0.0.2/pygda/models/jhgda.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/kbl.py` & `pygda-0.0.2/pygda/models/kbl.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/pa.py` & `pygda-0.0.2/pygda/models/pa.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/sagda.py` & `pygda-0.0.2/pygda/models/sagda.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/specreg.py` & `pygda-0.0.2/pygda/models/specreg.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/strurw.py` & `pygda-0.0.2/pygda/models/strurw.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/models/udagcn.py` & `pygda-0.0.2/pygda/models/udagcn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/__init__.py` & `pygda-0.0.2/pygda/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/a2gnn_base.py` & `pygda-0.0.2/pygda/nn/a2gnn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/acdne_base.py` & `pygda-0.0.2/pygda/nn/acdne_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/adagcn_base.py` & `pygda-0.0.2/pygda/nn/adagcn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/asn_base.py` & `pygda-0.0.2/pygda/nn/asn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/cached_gcn_conv.py` & `pygda-0.0.2/pygda/nn/cached_gcn_conv.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,92 +38,69 @@
             :class:`torch_geometric.nn.conv.MessagePassing`.
     """
 
     def __init__(self, in_channels, out_channels,
                  weight=None,
                  bias=None,
                  improved=False,
-                 use_bias=True, **kwargs):
+                 use_bias=True,
+                 **kwargs):
         super().__init__(aggr='add', **kwargs)
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.improved = improved
         self.cache_dict = {}
 
-        # self.weight = Parameter(torch.Tensor(in_channels, out_channels))
-        #
-        # if bias:
-        #     self.bias = Parameter(torch.Tensor(out_channels))
-        # else:
-        #     self.register_parameter('bias', None)
-
-
         if weight is None:
             self.weight = Parameter(torch.Tensor(in_channels, out_channels).to(torch.float32))
             glorot(self.weight)
         else:
             self.weight = weight
-            # print("use shared weight")
 
         if bias is None:
             if use_bias:
                 self.bias = Parameter(torch.Tensor(out_channels).to(torch.float32))
             else:
                 self.register_parameter('bias', None)
             zeros(self.bias)
         else:
             self.bias = bias
-            # print("use shared bias")
-
-        # self.reset_parameters()
-
-    # def reset_parameters(self):
-    #     glorot(self.weight)
-    #     zeros(self.bias)
-        # self.cached_result = None
-        # self.cached_num_edges = None
 
     @staticmethod
-    def norm(edge_index, num_nodes, edge_weight=None, improved=False,
-             dtype=None):
+    def norm(edge_index, num_nodes, edge_weight=None, improved=False, dtype=None):
         if edge_weight is None:
-            edge_weight = torch.ones((edge_index.size(1), ), dtype=dtype,
-                                     device=edge_index.device)
+            edge_weight = torch.ones((edge_index.size(1), ), dtype=dtype, device=edge_index.device)
 
         fill_value = 1 if not improved else 2
         edge_index, edge_weight = add_remaining_self_loops(
             edge_index, edge_weight, fill_value, num_nodes)
 
         row, col = edge_index
         deg = scatter_add(edge_weight, row, dim=0, dim_size=num_nodes)
         deg_inv_sqrt = deg.pow(-0.5)
         deg_inv_sqrt[deg_inv_sqrt == float('inf')] = 0
 
         return edge_index, deg_inv_sqrt[row] * edge_weight * deg_inv_sqrt[col]
 
     def forward(self, x, edge_index, cache_name="default_cache", edge_weight=None):
         """"""
-
         x = torch.matmul(x, self.weight)
 
         if not cache_name in self.cache_dict:
-            edge_index, norm = self.norm(edge_index, x.size(0), edge_weight,
-                                         self.improved, x.dtype)
+            edge_index, norm = self.norm(edge_index, x.size(0), edge_weight, self.improved, x.dtype)
             self.cache_dict[cache_name] = edge_index, norm
         else:
             edge_index, norm = self.cache_dict[cache_name]
 
-
         return self.propagate(edge_index, x=x, norm=norm)
 
     def message(self, x_j, norm):
         return norm.view(-1, 1) * x_j
 
     def update(self, aggr_out):
         if self.bias is not None:
             aggr_out = aggr_out + self.bias
         return aggr_out
 
     def __repr__(self):
-        return '{}({}, {})'.format(self.__class__.__name__, self.in_channels,
-                                   self.out_channels)
+        return '{}({}, {})'.format(self.__class__.__name__, self.in_channels, self.out_channels)
```

### Comparing `pygda-0.0.1/pygda/nn/cwgcn_base.py` & `pygda-0.0.2/pygda/nn/cwgcn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/deepwalk_pretrain.py` & `pygda-0.0.2/pygda/nn/deepwalk_pretrain.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/dgda_base.py` & `pygda-0.0.2/pygda/nn/dgda_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/gmm_clustering.py` & `pygda-0.0.2/pygda/nn/gmm_clustering.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/gnn_base.py` & `pygda-0.0.2/pygda/nn/gnn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/grade_base.py` & `pygda-0.0.2/pygda/nn/grade_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/jhgda_base.py` & `pygda-0.0.2/pygda/nn/jhgda_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/kbl_base.py` & `pygda-0.0.2/pygda/nn/kbl_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/mixup_base.py` & `pygda-0.0.2/pygda/nn/mixup_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/mixup_gcnconv.py` & `pygda-0.0.2/pygda/nn/mixup_gcnconv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/ppmi_conv.py` & `pygda-0.0.2/pygda/nn/ppmi_conv.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 from torch_geometric.utils import add_remaining_self_loops
 import numpy as np
 from tqdm import tqdm
 from .cached_gcn_conv import CachedGCNConv
 
 
 class PPMIConv(CachedGCNConv):
-
-    def __init__(self, in_channels, out_channels,
-                 weight=None, bias=None, improved=False, use_bias=True,
-                 path_len=5,
-                 **kwargs):
+    def __init__(
+        self,
+        in_channels,
+        out_channels,
+        weight=None,
+        bias=None,
+        improved=False,
+        use_bias=True,
+        path_len=5,
+        **kwargs
+        ):
         super().__init__(in_channels, out_channels, weight, bias, improved, use_bias, **kwargs)
         self.path_len = path_len
 
-    def norm(self, edge_index, num_nodes, edge_weight=None, improved=False,
-             dtype=None):
+    def norm(self, edge_index, num_nodes, edge_weight=None, improved=False, dtype=None):
 
         adj_dict = {}
 
         def add_edge(a, b):
             if a in adj_dict:
                 neighbors = adj_dict[a]
             else:
@@ -79,30 +84,30 @@
             for b, prob in normed_walk_counter.items():
                 prob_sums[b] += prob
 
         ppmis = {}
 
         for a, normed_walk_counter in normed_walk_counters.items():
             for b, prob in normed_walk_counter.items():
-                ppmi = np.log(prob / prob_sums[b] * len(prob_sums) / self.path_len)
+                ppmi = max(np.log(prob / prob_sums[b] * len(prob_sums) / self.path_len), 0)
                 ppmis[(a, b)] = ppmi
 
         new_edge_index = []
         edge_weight = []
         for (a, b), ppmi in ppmis.items():
             new_edge_index.append([a, b])
             edge_weight.append(ppmi)
 
         edge_index = torch.tensor(new_edge_index).t().to(gpu_device)
         edge_weight = torch.tensor(edge_weight).to(gpu_device)
 
-
         fill_value = 1 if not improved else 2
         edge_index, edge_weight = add_remaining_self_loops(
             edge_index, edge_weight, fill_value, num_nodes)
 
         row, col = edge_index
         deg = scatter_add(edge_weight, row, dim=0, dim_size=num_nodes)
+
         deg_inv_sqrt = deg.pow(-0.5)
         deg_inv_sqrt[deg_inv_sqrt == float('inf')] = 0
 
         return edge_index, (deg_inv_sqrt[row] * edge_weight * deg_inv_sqrt[col]).type(torch.float32)
```

### Comparing `pygda-0.0.1/pygda/nn/prop_gcn_conv.py` & `pygda-0.0.2/pygda/nn/prop_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/reweight_gnn.py` & `pygda-0.0.2/pygda/nn/reweight_gnn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/sagda_base.py` & `pygda-0.0.2/pygda/nn/sagda_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/nn/udagcn_base.py` & `pygda-0.0.2/pygda/nn/udagcn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/utils/mmd.py` & `pygda-0.0.2/pygda/utils/mmd.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/pygda/utils/svd_transform.py` & `pygda-0.0.2/pygda/utils/svd_transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 import torch
 import numpy as np
 from torch_geometric.utils import get_laplacian
 from sklearn.decomposition import TruncatedSVD
 
 
 def svd_transform(data, processed_paths):
-    num_node = data.x.shape[0]
+    num_node = data.y.shape[0]
     edge_index, edge_weight = get_laplacian(data.edge_index, num_nodes=num_node)
     edge_index = edge_index.numpy()
     edge_weight = edge_weight.numpy()
     adj = np.zeros((num_node, num_node), dtype=np.float32)
     adj[edge_index[0,:], edge_index[1,:]] = edge_weight
 
-    pca = TruncatedSVD(n_components=1000, n_iter=20, random_state=42)
+    if num_node < 1000:
+        pca = TruncatedSVD(n_components=100, n_iter=20, random_state=42)
+    else:
+        pca = TruncatedSVD(n_components=1000, n_iter=20, random_state=42)
     pca.fit(adj)
 
     torch.save(torch.tensor(pca.explained_variance_ ** 0.5, dtype=torch.float32 ), processed_paths + 'eival.pt')
     torch.save(torch.tensor(pca.components_, dtype=torch.float32 ), processed_paths + 'eivec.pt')
 
     data.eival = torch.load(processed_paths + 'eival.pt')
     data.eivec = torch.load(processed_paths + 'eivec.pt')
```

### Comparing `pygda-0.0.1/pygda/utils/utility.py` & `pygda-0.0.2/pygda/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.1/PKG-INFO` & `pygda-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygda
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python library for Graph Domain Adaptation
 Author: pygda-team
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy
@@ -33,32 +33,43 @@
 **PyGDA is featured for:**
 * **Consistent APIs and comprehensive documentation.**
 * **Cover 15+ graph domain adaptation models.**
 * **Scalable architecture that efficiently handles large graph datasets through mini-batching and sampling techniques.**
 * **Seamlessly integrated data processing with PyG, ensuring full compatibility with PyG data structures.**
 
 ## Installation
-Note: PyGDA depends on [PyTorch](https://pytorch.org/), [PyG](https://pytorch-geometric.readthedocs.io/en/latest/), and [PyTorch Sparse](https://github.com/rusty1s/pytorch_sparse). PyGDA does not automatically install these libraries for you. Please use the provided links above to install them separately in order to run PyGDA successfully.
+Note: PyGDA depends on [PyTorch](https://pytorch.org/), [PyG](https://pytorch-geometric.readthedocs.io/en/latest/), [PyTorch Sparse](https://github.com/rusty1s/pytorch_sparse) and [Pytorch Scatter](https://github.com/rusty1s/pytorch_scatter). PyGDA does not automatically install these libraries for you. Please install them separately in order to run PyGDA successfully.
+
+**Required Dependencies:**
+
 * torch>=1.13.1
 * torch_geometric>=2.4.0
 * torch_sparse>=0.6.15
+* torch_scatter>=2.1.0
+* python3
+* scipy
+* sklearn
+* numpy
+* cvxpy
+* tqdm
+
+**Installing with pip:**
+```
+pip install pygda
+```
+
+or 
 
 **Installation for local development:**
 ```
 git clone https://github.com/pygda-team/pygda
 cd pygda
+pip install -e .
 ```
 
-**Required Dependencies:**
-* python
-* scipy
-* sklearn
-* numpy
-* cvxpy
-
 ## Quick Start
 
 ### Step 1: Load Data
 ```
 from pygda.datasets import CitationDataset
 
 source_dataset = CitationDataset(path, args.source)
```

