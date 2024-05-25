# Comparing `tmp/pyg_nightly-2.6.0.dev20240523.tar.gz` & `tmp/pyg_nightly-2.6.0.dev20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg_nightly-2.6.0.dev20240523.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyg_nightly-2.6.0.dev20240524.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyg_nightly-2.6.0.dev20240523.tar` & `pyg_nightly-2.6.0.dev20240524.tar`

### file list

```diff
@@ -1,612 +1,612 @@
--rw-r--r--   0        0        0    59797 2024-05-23 06:09:30.622542 pyg_nightly-2.6.0.dev20240523/README.md
--rw-r--r--   0        0        0     5269 2024-05-23 06:09:31.018552 pyg_nightly-2.6.0.dev20240523/pyproject.toml
--rw-r--r--   0        0        0     1247 2024-05-23 06:09:31.014552 pyg_nightly-2.6.0.dev20240523/torch_geometric/__init__.py
--rw-r--r--   0        0        0     1053 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/_compile.py
--rw-r--r--   0        0        0     1575 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/backend.py
--rw-r--r--   0        0        0    16842 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/config_store.py
--rw-r--r--   0        0        0      352 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/__init__.py
--rw-r--r--   0        0        0       23 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/datasets/__init__.py
--rw-r--r--   0        0        0      396 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/explain/__init__.py
--rw-r--r--   0        0        0    16972 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/explain/pgm_explainer.py
--rw-r--r--   0        0        0       72 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/nn/__init__.py
--rw-r--r--   0        0        0       23 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/nn/conv/__init__.py
--rw-r--r--   0        0        0      113 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/nn/models/__init__.py
--rw-r--r--   0        0        0    33280 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/nn/models/rbcd_attack.py
--rw-r--r--   0        0        0       23 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3882 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/__init__.py
--rw-r--r--   0        0        0     8767 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/batch.py
--rw-r--r--   0        0        0    12756 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/collate.py
--rw-r--r--   0        0        0    43512 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/data.py
--rw-r--r--   0        0        0    22734 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/database.py
--rw-r--r--   0        0        0     3083 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/datapipes.py
--rw-r--r--   0        0        0    16402 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/dataset.py
--rw-r--r--   0        0        0     1889 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/download.py
--rw-r--r--   0        0        0     2324 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/extract.py
--rw-r--r--   0        0        0    20205 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/feature_store.py
--rw-r--r--   0        0        0    13919 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/graph_store.py
--rw-r--r--   0        0        0    47993 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/hetero_data.py
--rw-r--r--   0        0        0     8294 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/hypergraph_data.py
--rw-r--r--   0        0        0    13513 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/in_memory_dataset.py
--rw-r--r--   0        0        0      178 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/lightning/__init__.py
--rw-r--r--   0        0        0    29265 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/lightning/datamodule.py
--rw-r--r--   0        0        0      463 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/makedirs.py
--rw-r--r--   0        0        0     6629 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/on_disk_dataset.py
--rw-r--r--   0        0        0     4503 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/remote_backend_utils.py
--rw-r--r--   0        0        0     5587 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/separate.py
--rw-r--r--   0        0        0    31622 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/storage.py
--rw-r--r--   0        0        0     5375 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/summary.py
--rw-r--r--   0        0        0    10055 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/temporal.py
--rw-r--r--   0        0        0     1089 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/data/view.py
--rw-r--r--   0        0        0     5770 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/__init__.py
--rw-r--r--   0        0        0     4471 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/actor.py
--rw-r--r--   0        0        0     5666 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/airfrans.py
--rw-r--r--   0        0        0     3913 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/airports.py
--rw-r--r--   0        0        0     3179 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/amazon.py
--rw-r--r--   0        0        0     3362 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/amazon_book.py
--rw-r--r--   0        0        0     3964 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/amazon_products.py
--rw-r--r--   0        0        0     5178 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/aminer.py
--rw-r--r--   0        0        0     5455 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/aqsol.py
--rw-r--r--   0        0        0     5975 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/attributed_graph_dataset.py
--rw-r--r--   0        0        0     4258 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ba2motif_dataset.py
--rw-r--r--   0        0        0     3700 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ba_multi_shapes.py
--rw-r--r--   0        0        0     3904 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ba_shapes.py
--rw-r--r--   0        0        0     4404 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/bitcoin_otc.py
--rw-r--r--   0        0        0     3959 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/brca_tgca.py
--rw-r--r--   0        0        0     4458 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/citation_full.py
--rw-r--r--   0        0        0     3138 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/coauthor.py
--rw-r--r--   0        0        0     4734 2024-05-23 06:09:30.674543 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/coma.py
--rw-r--r--   0        0        0     5311 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/cornell.py
--rw-r--r--   0        0        0     5416 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dblp.py
--rw-r--r--   0        0        0     5707 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dbp15k.py
--rw-r--r--   0        0        0     2511 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/deezer_europe.py
--rw-r--r--   0        0        0     4035 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dgraph.py
--rw-r--r--   0        0        0     6041 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dynamic_faust.py
--rw-r--r--   0        0        0     4605 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/elliptic.py
--rw-r--r--   0        0        0     3188 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/elliptic_temporal.py
--rw-r--r--   0        0        0     2834 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/email_eu_core.py
--rw-r--r--   0        0        0     7356 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/entities.py
--rw-r--r--   0        0        0     6103 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/explainer_dataset.py
--rw-r--r--   0        0        0     2431 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/facebook.py
--rw-r--r--   0        0        0    10554 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/fake.py
--rw-r--r--   0        0        0     4076 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/faust.py
--rw-r--r--   0        0        0     3964 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/flickr.py
--rw-r--r--   0        0        0     4080 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/freebase.py
--rw-r--r--   0        0        0     3598 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gdelt.py
--rw-r--r--   0        0        0     3189 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gdelt_lite.py
--rw-r--r--   0        0        0     9511 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ged_dataset.py
--rw-r--r--   0        0        0     2820 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gemsec.py
--rw-r--r--   0        0        0     4223 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/geometry.py
--rw-r--r--   0        0        0     2687 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/github.py
--rw-r--r--   0        0        0     6940 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gnn_benchmark_dataset.py
--rw-r--r--   0        0        0      272 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/__init__.py
--rw-r--r--   0        0        0      965 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-r--r--   0        0        0      939 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/base.py
--rw-r--r--   0        0        0      918 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/er_graph.py
--rw-r--r--   0        0        0     1159 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-r--r--   0        0        0     2599 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/tree_graph.py
--rw-r--r--   0        0        0     4224 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-r--r--   0        0        0     8846 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/hgb_dataset.py
--rw-r--r--   0        0        0     6763 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/hm.py
--rw-r--r--   0        0        0    11417 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/hydro_net.py
--rw-r--r--   0        0        0     4735 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/icews.py
--rw-r--r--   0        0        0     4611 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/igmc_dataset.py
--rw-r--r--   0        0        0     4223 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/imdb.py
--rw-r--r--   0        0        0     7293 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/infection_dataset.py
--rw-r--r--   0        0        0     3643 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/jodie.py
--rw-r--r--   0        0        0     3462 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/karate.py
--rw-r--r--   0        0        0     4572 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/last_fm.py
--rw-r--r--   0        0        0     2486 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/lastfm_asia.py
--rw-r--r--   0        0        0     6864 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/linkx_dataset.py
--rw-r--r--   0        0        0    11746 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/lrgb.py
--rw-r--r--   0        0        0     5244 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/malnet_tiny.py
--rw-r--r--   0        0        0    16734 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/md17.py
--rw-r--r--   0        0        0     3951 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-r--r--   0        0        0     3317 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/mnist_superpixels.py
--rw-r--r--   0        0        0     5347 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/modelnet.py
--rw-r--r--   0        0        0     7384 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/molecule_net.py
--rw-r--r--   0        0        0      272 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/__init__.py
--rw-r--r--   0        0        0      900 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/base.py
--rw-r--r--   0        0        0     1278 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/custom.py
--rw-r--r--   0        0        0      983 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/cycle.py
--rw-r--r--   0        0        0     1099 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/grid.py
--rw-r--r--   0        0        0      814 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/house.py
--rw-r--r--   0        0        0     4033 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/movie_lens.py
--rw-r--r--   0        0        0     6057 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/movie_lens_100k.py
--rw-r--r--   0        0        0     5396 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/movie_lens_1m.py
--rw-r--r--   0        0        0     3008 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/myket.py
--rw-r--r--   0        0        0     2863 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/nell.py
--rw-r--r--   0        0        0     5181 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/neurograph.py
--rw-r--r--   0        0        0     7481 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ogb_mag.py
--rw-r--r--   0        0        0     3585 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/omdb.py
--rw-r--r--   0        0        0     5161 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ose_gvcs.py
--rw-r--r--   0        0        0     4162 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/particle.py
--rw-r--r--   0        0        0    12041 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pascal.py
--rw-r--r--   0        0        0     4791 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pascal_pf.py
--rw-r--r--   0        0        0     5897 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pcpnet_dataset.py
--rw-r--r--   0        0        0     4207 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pcqm4m.py
--rw-r--r--   0        0        0     7201 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/planetoid.py
--rw-r--r--   0        0        0     3045 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/polblogs.py
--rw-r--r--   0        0        0     4999 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ppi.py
--rw-r--r--   0        0        0     3325 2024-05-23 06:09:30.678544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/qm7.py
--rw-r--r--   0        0        0    17186 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/qm9.py
--rw-r--r--   0        0        0     5317 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/rcdd.py
--rw-r--r--   0        0        0     3122 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/reddit.py
--rw-r--r--   0        0        0     4282 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/reddit2.py
--rw-r--r--   0        0        0     4535 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-r--r--   0        0        0     4553 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/s3dis.py
--rw-r--r--   0        0        0     8816 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/sbm_dataset.py
--rw-r--r--   0        0        0     8504 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/shapenet.py
--rw-r--r--   0        0        0     6316 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/shrec2016.py
--rw-r--r--   0        0        0     9433 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/snap_dataset.py
--rw-r--r--   0        0        0     3278 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/suite_sparse.py
--rw-r--r--   0        0        0     4170 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/taobao.py
--rw-r--r--   0        0        0     4632 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/tosca.py
--rw-r--r--   0        0        0     7847 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/tu_dataset.py
--rw-r--r--   0        0        0     3658 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/twitch.py
--rw-r--r--   0        0        0     7001 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/upfd.py
--rw-r--r--   0        0        0      182 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/utils/__init__.py
--rw-r--r--   0        0        0     1835 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/utils/cheatsheet.py
--rw-r--r--   0        0        0     4889 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/webkb.py
--rw-r--r--   0        0        0     3884 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/wikics.py
--rw-r--r--   0        0        0     4947 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/wikidata.py
--rw-r--r--   0        0        0     6640 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/wikipedia_network.py
--rw-r--r--   0        0        0     7028 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/willow_object_class.py
--rw-r--r--   0        0        0     8158 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/word_net.py
--rw-r--r--   0        0        0     3959 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/yelp.py
--rw-r--r--   0        0        0     6347 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/zinc.py
--rw-r--r--   0        0        0     1295 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/debug.py
--rw-r--r--   0        0        0      858 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/deprecation.py
--rw-r--r--   0        0        0      589 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/__init__.py
--rw-r--r--   0        0        0      418 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_context.py
--rw-r--r--   0        0        0     4933 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_link_neighbor_loader.py
--rw-r--r--   0        0        0     6492 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_loader.py
--rw-r--r--   0        0        0     4372 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_neighbor_loader.py
--rw-r--r--   0        0        0    42406 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_neighbor_sampler.py
--rw-r--r--   0        0        0     3309 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/event_loop.py
--rw-r--r--   0        0        0    19018 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/local_feature_store.py
--rw-r--r--   0        0        0     8408 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/local_graph_store.py
--rw-r--r--   0        0        0    14685 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/partition.py
--rw-r--r--   0        0        0     5753 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/rpc.py
--rw-r--r--   0        0        0     6567 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/utils.py
--rw-r--r--   0        0        0    69668 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/edge_index.py
--rw-r--r--   0        0        0     4756 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/experimental.py
--rw-r--r--   0        0        0      359 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/__init__.py
--rw-r--r--   0        0        0      496 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/__init__.py
--rw-r--r--   0        0        0     4545 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/attention_explainer.py
--rw-r--r--   0        0        0     6935 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/base.py
--rw-r--r--   0        0        0    12857 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/captum.py
--rw-r--r--   0        0        0     7346 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/captum_explainer.py
--rw-r--r--   0        0        0     2872 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-r--r--   0        0        0    12454 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-r--r--   0        0        0    21367 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/graphmask_explainer.py
--rw-r--r--   0        0        0    10371 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/pg_explainer.py
--rw-r--r--   0        0        0     2564 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/utils.py
--rw-r--r--   0        0        0     7834 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/config.py
--rw-r--r--   0        0        0    10667 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/explainer.py
--rw-r--r--   0        0        0    14934 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/explanation.py
--rw-r--r--   0        0        0      301 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/__init__.py
--rw-r--r--   0        0        0     1888 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/basic.py
--rw-r--r--   0        0        0     3063 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/faithfulness.py
--rw-r--r--   0        0        0     6157 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/fidelity.py
--rw-r--r--   0        0        0     1815 2024-05-23 06:09:30.682544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/__init__.py
--rw-r--r--   0        0        0      510 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/benchmark.py
--rw-r--r--   0        0        0     2371 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/checkpoint.py
--rw-r--r--   0        0        0      738 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/cmd_args.py
--rw-r--r--   0        0        0    17197 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/config.py
--rw-r--r--   0        0        0      389 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/act/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/config/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/encoder/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/head/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-r--r--   0        0        0     8435 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/layer/generalconv.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/loader/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/loss/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/network/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/pooling/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/stage/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/train/__init__.py
--rw-r--r--   0        0        0      221 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-r--r--   0        0        0      375 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/imports.py
--rw-r--r--   0        0        0      521 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/init.py
--rw-r--r--   0        0        0    11605 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/loader.py
--rw-r--r--   0        0        0    11314 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/logger.py
--rw-r--r--   0        0        0     1445 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/loss.py
--rw-r--r--   0        0        0     3110 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/model_builder.py
--rw-r--r--   0        0        0     1121 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/__init__.py
--rw-r--r--   0        0        0      855 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/act.py
--rw-r--r--   0        0        0     3034 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/encoder.py
--rw-r--r--   0        0        0     6373 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/gnn.py
--rw-r--r--   0        0        0     4603 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/head.py
--rw-r--r--   0        0        0    12500 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/layer.py
--rw-r--r--   0        0        0      288 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/pooling.py
--rw-r--r--   0        0        0     1383 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/transform.py
--rw-r--r--   0        0        0     2544 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/optim.py
--rw-r--r--   0        0        0     3954 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/register.py
--rw-r--r--   0        0        0     2653 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/train.py
--rw-r--r--   0        0        0        0 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/LICENSE
--rw-r--r--   0        0        0      641 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/__init__.py
--rw-r--r--   0        0        0     9349 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/agg_runs.py
--rw-r--r--   0        0        0     3045 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/comp_budget.py
--rw-r--r--   0        0        0     1342 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/device.py
--rw-r--r--   0        0        0      690 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/epoch.py
--rw-r--r--   0        0        0     2049 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/io.py
--rw-r--r--   0        0        0      624 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/plot.py
--rw-r--r--   0        0        0      199 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/tools.py
--rw-r--r--   0        0        0      790 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/home.py
--rw-r--r--   0        0        0    23512 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/index.py
--rw-r--r--   0        0        0    19267 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/inspector.py
--rw-r--r--   0        0        0      528 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/__init__.py
--rw-r--r--   0        0        0     6577 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/fs.py
--rw-r--r--   0        0        0     1177 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/npz.py
--rw-r--r--   0        0        0     1088 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/obj.py
--rw-r--r--   0        0        0     2762 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/off.py
--rw-r--r--   0        0        0     4667 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/planetoid.py
--rw-r--r--   0        0        0      489 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/ply.py
--rw-r--r--   0        0        0     1170 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/sdf.py
--rw-r--r--   0        0        0     4930 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/tu.py
--rw-r--r--   0        0        0      910 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/io/txt_array.py
--rw-r--r--   0        0        0      935 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/isinstance.py
--rw-r--r--   0        0        0      908 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/lazy_loader.py
--rw-r--r--   0        0        0     1835 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/__init__.py
--rw-r--r--   0        0        0     1615 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/base.py
--rw-r--r--   0        0        0     2106 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/cache.py
--rw-r--r--   0        0        0    13189 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/cluster.py
--rw-r--r--   0        0        0     1459 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/data_list_loader.py
--rw-r--r--   0        0        0     3527 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/dataloader.py
--rw-r--r--   0        0        0     1685 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/dense_data_loader.py
--rw-r--r--   0        0        0     4163 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/dynamic_batch_sampler.py
--rw-r--r--   0        0        0     8448 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/graph_saint.py
--rw-r--r--   0        0        0     6012 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/hgt_loader.py
--rw-r--r--   0        0        0    31462 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/ibmb_loader.py
--rw-r--r--   0        0        0     3754 2024-05-23 06:09:30.686544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/imbalanced_sampler.py
--rw-r--r--   0        0        0    16207 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/link_loader.py
--rw-r--r--   0        0        0    14383 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/link_neighbor_loader.py
--rw-r--r--   0        0        0    10931 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/mixin.py
--rw-r--r--   0        0        0    12452 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/neighbor_loader.py
--rw-r--r--   0        0        0     8513 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/neighbor_sampler.py
--rw-r--r--   0        0        0    11848 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/node_loader.py
--rw-r--r--   0        0        0     3236 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/prefetch.py
--rw-r--r--   0        0        0     2196 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/random_node_loader.py
--rw-r--r--   0        0        0     4173 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/shadow.py
--rw-r--r--   0        0        0     2248 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/temporal_dataloader.py
--rw-r--r--   0        0        0    14901 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/utils.py
--rw-r--r--   0        0        0     3518 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/zip_loader.py
--rw-r--r--   0        0        0      858 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/logging.py
--rw-r--r--   0        0        0      296 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/metrics/__init__.py
--rw-r--r--   0        0        0     7521 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/metrics/link_pred.py
--rw-r--r--   0        0        0      847 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/__init__.py
--rw-r--r--   0        0        0     1551 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/__init__.py
--rw-r--r--   0        0        0     3003 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/attention.py
--rw-r--r--   0        0        0     8244 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/base.py
--rw-r--r--   0        0        0    11011 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/basic.py
--rw-r--r--   0        0        0     2650 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/deep_sets.py
--rw-r--r--   0        0        0     6639 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/equilibrium.py
--rw-r--r--   0        0        0    12276 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/fused.py
--rw-r--r--   0        0        0     3801 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/gmt.py
--rw-r--r--   0        0        0     2193 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/gru.py
--rw-r--r--   0        0        0     4190 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/lcm.py
--rw-r--r--   0        0        0     2214 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/lstm.py
--rw-r--r--   0        0        0     2514 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/mlp.py
--rw-r--r--   0        0        0     8170 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/multi.py
--rw-r--r--   0        0        0     6189 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/quantile.py
--rw-r--r--   0        0        0     4638 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/scaler.py
--rw-r--r--   0        0        0     2446 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/set2set.py
--rw-r--r--   0        0        0     4207 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/set_transformer.py
--rw-r--r--   0        0        0     2507 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/sort.py
--rw-r--r--   0        0        0     8338 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/utils.py
--rw-r--r--   0        0        0     1126 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/variance_preserving.py
--rw-r--r--   0        0        0       76 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/attention/__init__.py
--rw-r--r--   0        0        0     7357 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/attention/performer.py
--rw-r--r--   0        0        0     3515 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/__init__.py
--rw-r--r--   0        0        0     3077 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/agnn_conv.py
--rw-r--r--   0        0        0     4387 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-r--r--   0        0        0     5983 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/appnp.py
--rw-r--r--   0        0        0     6585 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/arma_conv.py
--rw-r--r--   0        0        0     4014 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cg_conv.py
--rw-r--r--   0        0        0     6423 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cheb_conv.py
--rw-r--r--   0        0        0     5255 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cluster_gcn_conv.py
--rw-r--r--   0        0        0     5641 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/collect.jinja
--rw-r--r--   0        0        0      251 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/__init__.py
--rw-r--r--   0        0        0     6364 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/base.py
--rw-r--r--   0        0        0     2874 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-r--r--   0        0        0     4002 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-r--r--   0        0        0     2830 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-r--r--   0        0        0     2440 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/dir_gnn_conv.py
--rw-r--r--   0        0        0    12241 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/dna_conv.py
--rw-r--r--   0        0        0     5389 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/edge_conv.py
--rw-r--r--   0        0        0     2216 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/edge_updater.jinja
--rw-r--r--   0        0        0    10742 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/eg_conv.py
--rw-r--r--   0        0        0     9065 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/fa_conv.py
--rw-r--r--   0        0        0     4430 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/feast_conv.py
--rw-r--r--   0        0        0     6314 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/film_conv.py
--rw-r--r--   0        0        0     4495 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/fused_gat_conv.py
--rw-r--r--   0        0        0    16091 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gat_conv.py
--rw-r--r--   0        0        0     3518 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gated_graph_conv.py
--rw-r--r--   0        0        0    13639 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gatv2_conv.py
--rw-r--r--   0        0        0     7001 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gcn2_conv.py
--rw-r--r--   0        0        0    10415 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gcn_conv.py
--rw-r--r--   0        0        0     9722 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gen_conv.py
--rw-r--r--   0        0        0     7591 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/general_conv.py
--rw-r--r--   0        0        0     7411 2024-05-23 06:09:30.690544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gin_conv.py
--rw-r--r--   0        0        0     8315 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gmm_conv.py
--rw-r--r--   0        0        0     6672 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gps_conv.py
--rw-r--r--   0        0        0     3905 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/graph_conv.py
--rw-r--r--   0        0        0     4951 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gravnet_conv.py
--rw-r--r--   0        0        0     7198 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/han_conv.py
--rw-r--r--   0        0        0     6084 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/heat_conv.py
--rw-r--r--   0        0        0     6555 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/hetero_conv.py
--rw-r--r--   0        0        0     9043 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/hgt_conv.py
--rw-r--r--   0        0        0     8691 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/hypergraph_conv.py
--rw-r--r--   0        0        0     3494 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/le_conv.py
--rw-r--r--   0        0        0     2369 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/lg_conv.py
--rw-r--r--   0        0        0    43577 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/message_passing.py
--rw-r--r--   0        0        0     4340 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/mf_conv.py
--rw-r--r--   0        0        0     4554 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/mixhop_conv.py
--rw-r--r--   0        0        0     4759 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/nn_conv.py
--rw-r--r--   0        0        0     4908 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/pan_conv.py
--rw-r--r--   0        0        0     4892 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/pdn_conv.py
--rw-r--r--   0        0        0     8325 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/pna_conv.py
--rw-r--r--   0        0        0     4508 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/point_conv.py
--rw-r--r--   0        0        0     3278 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/point_gnn_conv.py
--rw-r--r--   0        0        0     5878 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/point_transformer_conv.py
--rw-r--r--   0        0        0     5363 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/ppf_conv.py
--rw-r--r--   0        0        0     7374 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/propagate.jinja
--rw-r--r--   0        0        0     5217 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-r--r--   0        0        0    22863 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/rgat_conv.py
--rw-r--r--   0        0        0    15666 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/rgcn_conv.py
--rw-r--r--   0        0        0     5812 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/sage_conv.py
--rw-r--r--   0        0        0     4543 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/sg_conv.py
--rw-r--r--   0        0        0     6190 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/signed_conv.py
--rw-r--r--   0        0        0     3888 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/simple_conv.py
--rw-r--r--   0        0        0     6314 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/spline_conv.py
--rw-r--r--   0        0        0     5131 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/ssg_conv.py
--rw-r--r--   0        0        0    12420 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/supergat_conv.py
--rw-r--r--   0        0        0     4164 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/tag_conv.py
--rw-r--r--   0        0        0    10407 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/transformer_conv.py
--rw-r--r--   0        0        0      852 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/utils/__init__.py
--rw-r--r--   0        0        0     2792 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-r--r--   0        0        0     3140 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/wl_conv.py
--rw-r--r--   0        0        0     2777 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-r--r--   0        0        0     5956 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/x_conv.py
--rw-r--r--   0        0        0     4764 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/data_parallel.py
--rw-r--r--   0        0        0      847 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/__init__.py
--rw-r--r--   0        0        0     4238 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_gat_conv.py
--rw-r--r--   0        0        0     3002 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-r--r--   0        0        0     2361 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_gin_conv.py
--rw-r--r--   0        0        0     2751 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_graph_conv.py
--rw-r--r--   0        0        0     2672 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_sage_conv.py
--rw-r--r--   0        0        0     3051 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/diff_pool.py
--rw-r--r--   0        0        0     6115 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dmon_pool.py
--rw-r--r--   0        0        0    17748 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/linear.py
--rw-r--r--   0        0        0     4111 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/mincut_pool.py
--rw-r--r--   0        0        0     3115 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/encoding.py
--rw-r--r--   0        0        0      129 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/functional/__init__.py
--rw-r--r--   0        0        0     1549 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/functional/bro.py
--rw-r--r--   0        0        0      863 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/functional/gini.py
--rw-r--r--   0        0        0    16055 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/fx.py
--rw-r--r--   0        0        0     1088 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/glob.py
--rw-r--r--   0        0        0     2457 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/inits.py
--rw-r--r--   0        0        0      290 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/__init__.py
--rw-r--r--   0        0        0     5902 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/base.py
--rw-r--r--   0        0        0     3234 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/complex.py
--rw-r--r--   0        0        0     2462 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/distmult.py
--rw-r--r--   0        0        0      771 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/loader.py
--rw-r--r--   0        0        0     3208 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/rotate.py
--rw-r--r--   0        0        0     3088 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/transe.py
--rw-r--r--   0        0        0     8937 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/lr_scheduler.py
--rw-r--r--   0        0        0     9512 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/model_hub.py
--rw-r--r--   0        0        0     1909 2024-05-23 06:09:30.694544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/__init__.py
--rw-r--r--   0        0        0     6634 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/attentive_fp.py
--rw-r--r--   0        0        0    10770 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/autoencoder.py
--rw-r--r--   0        0        0    31225 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/basic_gnn.py
--rw-r--r--   0        0        0     3971 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/captum.py
--rw-r--r--   0        0        0     6827 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/correct_and_smooth.py
--rw-r--r--   0        0        0     4197 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/deep_graph_infomax.py
--rw-r--r--   0        0        0     4339 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/deepgcn.py
--rw-r--r--   0        0        0    36186 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/dimenet.py
--rw-r--r--   0        0        0     5107 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/dimenet_utils.py
--rw-r--r--   0        0        0     7873 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/gnnff.py
--rw-r--r--   0        0        0     9246 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/graph_mixer.py
--rw-r--r--   0        0        0     5395 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/graph_unet.py
--rw-r--r--   0        0        0     3450 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/jumping_knowledge.py
--rw-r--r--   0        0        0     3908 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/label_prop.py
--rw-r--r--   0        0        0    12465 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/lightgcn.py
--rw-r--r--   0        0        0     5812 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/linkx.py
--rw-r--r--   0        0        0     2580 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/mask_label.py
--rw-r--r--   0        0        0     6540 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/meta.py
--rw-r--r--   0        0        0    10863 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/metapath2vec.py
--rw-r--r--   0        0        0    10315 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/mlp.py
--rw-r--r--   0        0        0     2378 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/neural_fingerprint.py
--rw-r--r--   0        0        0     7724 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/node2vec.py
--rw-r--r--   0        0        0     3538 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/pmlp.py
--rw-r--r--   0        0        0     8986 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/re_net.py
--rw-r--r--   0        0        0     2808 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/rect.py
--rw-r--r--   0        0        0    11796 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/rev_gnn.py
--rw-r--r--   0        0        0    16619 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/schnet.py
--rw-r--r--   0        0        0     9839 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/signed_gcn.py
--rw-r--r--   0        0        0    11878 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/tgn.py
--rw-r--r--   0        0        0    43192 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/visnet.py
--rw-r--r--   0        0        0     2373 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/module_dict.py
--rw-r--r--   0        0        0      106 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/nlp/__init__.py
--rw-r--r--   0        0        0     2070 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/nlp/sentence_transformer.py
--rw-r--r--   0        0        0      669 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/__init__.py
--rw-r--r--   0        0        0     8283 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/batch_norm.py
--rw-r--r--   0        0        0     4722 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/diff_group_norm.py
--rw-r--r--   0        0        0     2727 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/graph_norm.py
--rw-r--r--   0        0        0     1491 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/graph_size_norm.py
--rw-r--r--   0        0        0     4685 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/instance_norm.py
--rw-r--r--   0        0        0     7831 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/layer_norm.py
--rw-r--r--   0        0        0     1322 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-r--r--   0        0        0     1662 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/msg_norm.py
--rw-r--r--   0        0        0     2824 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/pair_norm.py
--rw-r--r--   0        0        0     2410 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/parameter_dict.py
--rw-r--r--   0        0        0    14129 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/__init__.py
--rw-r--r--   0        0        0     3967 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/approx_knn.py
--rw-r--r--   0        0        0     6683 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/asap.py
--rw-r--r--   0        0        0     3966 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/avg_pool.py
--rw-r--r--   0        0        0      287 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/connect/__init__.py
--rw-r--r--   0        0        0     4094 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/connect/base.py
--rw-r--r--   0        0        0     2190 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/connect/filter_edges.py
--rw-r--r--   0        0        0      273 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/consecutive.py
--rw-r--r--   0        0        0     1601 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/decimation.py
--rw-r--r--   0        0        0     8581 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/edge_pool.py
--rw-r--r--   0        0        0     3492 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/glob.py
--rw-r--r--   0        0        0     1291 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/graclus.py
--rw-r--r--   0        0        0    11343 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/knn.py
--rw-r--r--   0        0        0     4262 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/max_pool.py
--rw-r--r--   0        0        0     5377 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/mem_pool.py
--rw-r--r--   0        0        0     4366 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/pan_pool.py
--rw-r--r--   0        0        0      737 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/pool.py
--rw-r--r--   0        0        0     5838 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/sag_pool.py
--rw-r--r--   0        0        0      254 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/select/__init__.py
--rw-r--r--   0        0        0     3311 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/select/base.py
--rw-r--r--   0        0        0     5305 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/select/topk.py
--rw-r--r--   0        0        0     5159 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/topk_pool.py
--rw-r--r--   0        0        0     2736 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/voxel_grid.py
--rw-r--r--   0        0        0      426 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/reshape.py
--rw-r--r--   0        0        0     6155 2024-05-23 06:09:30.698544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/resolver.py
--rw-r--r--   0        0        0     1054 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/sequential.jinja
--rw-r--r--   0        0        0     5534 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/sequential.py
--rw-r--r--   0        0        0     5821 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/summary.py
--rw-r--r--   0        0        0     1282 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_fixed_size_transformer.py
--rw-r--r--   0        0        0     6519 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_hetero_module.py
--rw-r--r--   0        0        0    18407 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_hetero_transformer.py
--rw-r--r--   0        0        0    23121 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_hetero_with_bases_transformer.py
--rw-r--r--   0        0        0      129 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/unpool/__init__.py
--rw-r--r--   0        0        0     2586 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/unpool/knn_interpolate.py
--rw-r--r--   0        0        0      863 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/__init__.py
--rw-r--r--   0        0        0     5256 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/benchmark.py
--rw-r--r--   0        0        0    11793 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/profile.py
--rw-r--r--   0        0        0    16706 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/profiler.py
--rw-r--r--   0        0        0     5497 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/utils.py
--rw-r--r--   0        0        0     1273 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/resolver.py
--rw-r--r--   0        0        0      512 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/__init__.py
--rw-r--r--   0        0        0    26515 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/base.py
--rw-r--r--   0        0        0     2721 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/hgt_sampler.py
--rw-r--r--   0        0        0    33974 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/neighbor_sampler.py
--rw-r--r--   0        0        0     5485 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/utils.py
--rw-r--r--   0        0        0      372 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/seed.py
--rw-r--r--   0        0        0     1060 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/template.py
--rw-r--r--   0        0        0     1249 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/__init__.py
--rw-r--r--   0        0        0     4606 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/asserts.py
--rw-r--r--   0        0        0     2604 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/data.py
--rw-r--r--   0        0        0     8583 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/decorators.py
--rw-r--r--   0        0        0     2227 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/distributed.py
--rw-r--r--   0        0        0     2158 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/feature_store.py
--rw-r--r--   0        0        0     1044 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/graph_store.py
--rw-r--r--   0        0        0     4181 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/__init__.py
--rw-r--r--   0        0        0    14235 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_metapaths.py
--rw-r--r--   0        0        0     6065 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_positional_encoding.py
--rw-r--r--   0        0        0     2085 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_remaining_self_loops.py
--rw-r--r--   0        0        0     2024 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_self_loops.py
--rw-r--r--   0        0        0     1298 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/base_transform.py
--rw-r--r--   0        0        0     2464 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/cartesian.py
--rw-r--r--   0        0        0      645 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/center.py
--rw-r--r--   0        0        0     1658 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/compose.py
--rw-r--r--   0        0        0     2005 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/constant.py
--rw-r--r--   0        0        0     1264 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/delaunay.py
--rw-r--r--   0        0        0     2360 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/distance.py
--rw-r--r--   0        0        0     1083 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/face_to_edge.py
--rw-r--r--   0        0        0     3056 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/feature_propagation.py
--rw-r--r--   0        0        0     2426 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/fixed_points.py
--rw-r--r--   0        0        0     1397 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/gcn_norm.py
--rw-r--r--   0        0        0    20201 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/gdc.py
--rw-r--r--   0        0        0     1028 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/generate_mesh_normals.py
--rw-r--r--   0        0        0     2564 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/grid_sampling.py
--rw-r--r--   0        0        0     4102 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/half_hop.py
--rw-r--r--   0        0        0     2536 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/knn_graph.py
--rw-r--r--   0        0        0     2497 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/laplacian_lambda_max.py
--rw-r--r--   0        0        0     2161 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/largest_connected_components.py
--rw-r--r--   0        0        0     3730 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/line_graph.py
--rw-r--r--   0        0        0     1997 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/linear_transformation.py
--rw-r--r--   0        0        0     2144 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/local_cartesian.py
--rw-r--r--   0        0        0     1480 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/local_degree_profile.py
--rw-r--r--   0        0        0     4813 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/mask.py
--rw-r--r--   0        0        0     6075 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/node_property_split.py
--rw-r--r--   0        0        0     1028 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/normalize_features.py
--rw-r--r--   0        0        0     1782 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/normalize_rotation.py
--rw-r--r--   0        0        0      666 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/normalize_scale.py
--rw-r--r--   0        0        0     1584 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/one_hot_degree.py
--rw-r--r--   0        0        0    21041 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/pad.py
--rw-r--r--   0        0        0     1794 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/point_pair_features.py
--rw-r--r--   0        0        0     2213 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/polar.py
--rw-r--r--   0        0        0     2043 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/radius_graph.py
--rw-r--r--   0        0        0     1033 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_flip.py
--rw-r--r--   0        0        0     1721 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_jitter.py
--rw-r--r--   0        0        0    15181 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_link_split.py
--rw-r--r--   0        0        0     5853 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_node_split.py
--rw-r--r--   0        0        0     1946 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_rotate.py
--rw-r--r--   0        0        0     1261 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_scale.py
--rw-r--r--   0        0        0     1365 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_shear.py
--rw-r--r--   0        0        0     1929 2024-05-23 06:09:30.702544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/remove_duplicated_edges.py
--rw-r--r--   0        0        0     2449 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/remove_isolated_nodes.py
--rw-r--r--   0        0        0      932 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/remove_training_classes.py
--rw-r--r--   0        0        0     6509 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/rooted_subgraph.py
--rw-r--r--   0        0        0     2280 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/sample_points.py
--rw-r--r--   0        0        0     2329 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/sign.py
--rw-r--r--   0        0        0     2320 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/spherical.py
--rw-r--r--   0        0        0     1009 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/svd_feature_reduction.py
--rw-r--r--   0        0        0     1659 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/target_indegree.py
--rw-r--r--   0        0        0     2456 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_dense.py
--rw-r--r--   0        0        0     1470 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_device.py
--rw-r--r--   0        0        0     5580 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_sparse_tensor.py
--rw-r--r--   0        0        0     2697 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_superpixels.py
--rw-r--r--   0        0        0     2972 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_undirected.py
--rw-r--r--   0        0        0     1313 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/two_hop.py
--rw-r--r--   0        0        0     2860 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/virtual_node.py
--rw-r--r--   0        0        0    13536 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/typing.py
--rw-r--r--   0        0        0     4790 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2347 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_assortativity.py
--rw-r--r--   0        0        0     6769 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_coalesce.py
--rw-r--r--   0        0        0     1017 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_degree.py
--rw-r--r--   0        0        0     2562 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_grid.py
--rw-r--r--   0        0        0     5090 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_homophily.py
--rw-r--r--   0        0        0     1283 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_index_sort.py
--rw-r--r--   0        0        0     1403 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_lexsort.py
--rw-r--r--   0        0        0    14672 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_negative_sampling.py
--rw-r--r--   0        0        0     1167 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_normalized_cut.py
--rw-r--r--   0        0        0     1404 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_one_hot.py
--rw-r--r--   0        0        0    13389 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_scatter.py
--rw-r--r--   0        0        0     1976 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_segment.py
--rw-r--r--   0        0        0     2439 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_select.py
--rw-r--r--   0        0        0     3242 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_softmax.py
--rw-r--r--   0        0        0     4500 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_sort_edge_index.py
--rw-r--r--   0        0        0     5794 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_spmm.py
--rw-r--r--   0        0        0    18311 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_subgraph.py
--rw-r--r--   0        0        0     3606 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_to_dense_adj.py
--rw-r--r--   0        0        0     4582 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_to_dense_batch.py
--rw-r--r--   0        0        0     3569 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_train_test_split_edges.py
--rw-r--r--   0        0        0     5300 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_tree_decomposition.py
--rw-r--r--   0        0        0     8307 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_trim_to_layer.py
--rw-r--r--   0        0        0     2378 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_unbatch.py
--rw-r--r--   0        0        0     8601 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/augmentation.py
--rw-r--r--   0        0        0    21740 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/convert.py
--rw-r--r--   0        0        0     3047 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/cross_entropy.py
--rw-r--r--   0        0        0    11416 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/dropout.py
--rw-r--r--   0        0        0     1675 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/embedding.py
--rw-r--r--   0        0        0      703 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/functions.py
--rw-r--r--   0        0        0     4668 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/geodesic.py
--rw-r--r--   0        0        0     5542 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/hetero.py
--rw-r--r--   0        0        0     3588 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/isolated.py
--rw-r--r--   0        0        0     3695 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/laplacian.py
--rw-r--r--   0        0        0    23051 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/loop.py
--rw-r--r--   0        0        0     5918 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/map.py
--rw-r--r--   0        0        0     2340 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/mask.py
--rw-r--r--   0        0        0     4387 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/mesh_laplacian.py
--rw-r--r--   0        0        0      699 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/mixin.py
--rw-r--r--   0        0        0     3310 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/nested.py
--rw-r--r--   0        0        0     3750 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/noise_scheduler.py
--rw-r--r--   0        0        0     2176 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/num_nodes.py
--rw-r--r--   0        0        0     4055 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/ppr.py
--rw-r--r--   0        0        0     5148 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/random.py
--rw-r--r--   0        0        0      815 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/repeat.py
--rw-r--r--   0        0        0     6291 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/smiles.py
--rw-r--r--   0        0        0    24894 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/sparse.py
--rw-r--r--   0        0        0     6222 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/undirected.py
--rw-r--r--   0        0        0      154 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/visualization/__init__.py
--rw-r--r--   0        0        0     4813 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/visualization/graph.py
--rw-r--r--   0        0        0      477 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/visualization/influence.py
--rw-r--r--   0        0        0      413 2024-05-23 06:09:30.706544 pyg_nightly-2.6.0.dev20240523/torch_geometric/warnings.py
--rw-r--r--   0        0        0    62945 1970-01-01 00:00:00.000000 pyg_nightly-2.6.0.dev20240523/PKG-INFO
+-rw-r--r--   0        0        0    59797 2024-05-24 06:15:48.208160 pyg_nightly-2.6.0.dev20240524/README.md
+-rw-r--r--   0        0        0     5269 2024-05-24 06:15:48.628158 pyg_nightly-2.6.0.dev20240524/pyproject.toml
+-rw-r--r--   0        0        0     1247 2024-05-24 06:15:48.624158 pyg_nightly-2.6.0.dev20240524/torch_geometric/__init__.py
+-rw-r--r--   0        0        0     1053 2024-05-24 06:15:48.256160 pyg_nightly-2.6.0.dev20240524/torch_geometric/_compile.py
+-rw-r--r--   0        0        0     1575 2024-05-24 06:15:48.256160 pyg_nightly-2.6.0.dev20240524/torch_geometric/backend.py
+-rw-r--r--   0        0        0    16842 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/config_store.py
+-rw-r--r--   0        0        0      352 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/datasets/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/explain/__init__.py
+-rw-r--r--   0        0        0    16972 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/explain/pgm_explainer.py
+-rw-r--r--   0        0        0       72 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/nn/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/nn/conv/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/nn/models/__init__.py
+-rw-r--r--   0        0        0    33280 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/nn/models/rbcd_attack.py
+-rw-r--r--   0        0        0       23 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/transforms/__init__.py
+-rw-r--r--   0        0        0     3882 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/__init__.py
+-rw-r--r--   0        0        0     8767 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/batch.py
+-rw-r--r--   0        0        0    12756 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/collate.py
+-rw-r--r--   0        0        0    43512 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/data.py
+-rw-r--r--   0        0        0    22734 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/database.py
+-rw-r--r--   0        0        0     3083 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/datapipes.py
+-rw-r--r--   0        0        0    16402 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/dataset.py
+-rw-r--r--   0        0        0     1889 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/download.py
+-rw-r--r--   0        0        0     2324 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/extract.py
+-rw-r--r--   0        0        0    20205 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/feature_store.py
+-rw-r--r--   0        0        0    13919 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/graph_store.py
+-rw-r--r--   0        0        0    47993 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/hetero_data.py
+-rw-r--r--   0        0        0     8294 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/hypergraph_data.py
+-rw-r--r--   0        0        0    13513 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/in_memory_dataset.py
+-rw-r--r--   0        0        0      178 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/lightning/__init__.py
+-rw-r--r--   0        0        0    29265 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/lightning/datamodule.py
+-rw-r--r--   0        0        0      463 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/makedirs.py
+-rw-r--r--   0        0        0     6629 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/on_disk_dataset.py
+-rw-r--r--   0        0        0     4503 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/remote_backend_utils.py
+-rw-r--r--   0        0        0     5587 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/separate.py
+-rw-r--r--   0        0        0    31622 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/storage.py
+-rw-r--r--   0        0        0     5375 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/summary.py
+-rw-r--r--   0        0        0    10055 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/temporal.py
+-rw-r--r--   0        0        0     1089 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/data/view.py
+-rw-r--r--   0        0        0     5770 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4471 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/actor.py
+-rw-r--r--   0        0        0     5666 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/airfrans.py
+-rw-r--r--   0        0        0     3913 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/airports.py
+-rw-r--r--   0        0        0     3179 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/amazon.py
+-rw-r--r--   0        0        0     3362 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/amazon_book.py
+-rw-r--r--   0        0        0     3964 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/amazon_products.py
+-rw-r--r--   0        0        0     5178 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/aminer.py
+-rw-r--r--   0        0        0     5455 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/aqsol.py
+-rw-r--r--   0        0        0     5975 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-r--r--   0        0        0     4258 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ba2motif_dataset.py
+-rw-r--r--   0        0        0     3700 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ba_multi_shapes.py
+-rw-r--r--   0        0        0     3904 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ba_shapes.py
+-rw-r--r--   0        0        0     4404 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/bitcoin_otc.py
+-rw-r--r--   0        0        0     3959 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/brca_tgca.py
+-rw-r--r--   0        0        0     4458 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/citation_full.py
+-rw-r--r--   0        0        0     3138 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/coauthor.py
+-rw-r--r--   0        0        0     4734 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/coma.py
+-rw-r--r--   0        0        0     5311 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/cornell.py
+-rw-r--r--   0        0        0     5416 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dblp.py
+-rw-r--r--   0        0        0     5707 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dbp15k.py
+-rw-r--r--   0        0        0     2511 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/deezer_europe.py
+-rw-r--r--   0        0        0     4035 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dgraph.py
+-rw-r--r--   0        0        0     6041 2024-05-24 06:15:48.260160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dynamic_faust.py
+-rw-r--r--   0        0        0     4605 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/elliptic.py
+-rw-r--r--   0        0        0     3188 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/elliptic_temporal.py
+-rw-r--r--   0        0        0     2834 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/email_eu_core.py
+-rw-r--r--   0        0        0     7356 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/entities.py
+-rw-r--r--   0        0        0     6103 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/explainer_dataset.py
+-rw-r--r--   0        0        0     2431 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/facebook.py
+-rw-r--r--   0        0        0    10554 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/fake.py
+-rw-r--r--   0        0        0     4076 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/faust.py
+-rw-r--r--   0        0        0     3964 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/flickr.py
+-rw-r--r--   0        0        0     4080 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/freebase.py
+-rw-r--r--   0        0        0     3598 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gdelt.py
+-rw-r--r--   0        0        0     3189 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gdelt_lite.py
+-rw-r--r--   0        0        0     9511 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ged_dataset.py
+-rw-r--r--   0        0        0     2820 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gemsec.py
+-rw-r--r--   0        0        0     4223 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/geometry.py
+-rw-r--r--   0        0        0     2687 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/github.py
+-rw-r--r--   0        0        0     6940 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gnn_benchmark_dataset.py
+-rw-r--r--   0        0        0      272 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/__init__.py
+-rw-r--r--   0        0        0      965 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-r--r--   0        0        0      939 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/base.py
+-rw-r--r--   0        0        0      918 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-r--r--   0        0        0     1159 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-r--r--   0        0        0     2599 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/tree_graph.py
+-rw-r--r--   0        0        0     4224 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-r--r--   0        0        0     8846 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/hgb_dataset.py
+-rw-r--r--   0        0        0     6763 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/hm.py
+-rw-r--r--   0        0        0    11417 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/hydro_net.py
+-rw-r--r--   0        0        0     4735 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/icews.py
+-rw-r--r--   0        0        0     4611 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/igmc_dataset.py
+-rw-r--r--   0        0        0     4223 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/imdb.py
+-rw-r--r--   0        0        0     7293 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/infection_dataset.py
+-rw-r--r--   0        0        0     3643 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/jodie.py
+-rw-r--r--   0        0        0     3462 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/karate.py
+-rw-r--r--   0        0        0     4572 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/last_fm.py
+-rw-r--r--   0        0        0     2486 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/lastfm_asia.py
+-rw-r--r--   0        0        0     6864 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/linkx_dataset.py
+-rw-r--r--   0        0        0    11746 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/lrgb.py
+-rw-r--r--   0        0        0     5244 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/malnet_tiny.py
+-rw-r--r--   0        0        0    16734 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/md17.py
+-rw-r--r--   0        0        0     3951 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-r--r--   0        0        0     3317 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/mnist_superpixels.py
+-rw-r--r--   0        0        0     5347 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/modelnet.py
+-rw-r--r--   0        0        0     7384 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/molecule_net.py
+-rw-r--r--   0        0        0      272 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/base.py
+-rw-r--r--   0        0        0     1278 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/custom.py
+-rw-r--r--   0        0        0      983 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/cycle.py
+-rw-r--r--   0        0        0     1099 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/grid.py
+-rw-r--r--   0        0        0      814 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/house.py
+-rw-r--r--   0        0        0     4033 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/movie_lens.py
+-rw-r--r--   0        0        0     6057 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/movie_lens_100k.py
+-rw-r--r--   0        0        0     5396 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/movie_lens_1m.py
+-rw-r--r--   0        0        0     3008 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/myket.py
+-rw-r--r--   0        0        0     2863 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/nell.py
+-rw-r--r--   0        0        0     5181 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/neurograph.py
+-rw-r--r--   0        0        0     7481 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ogb_mag.py
+-rw-r--r--   0        0        0     3585 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/omdb.py
+-rw-r--r--   0        0        0     5161 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ose_gvcs.py
+-rw-r--r--   0        0        0     4162 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/particle.py
+-rw-r--r--   0        0        0    12041 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pascal.py
+-rw-r--r--   0        0        0     4791 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pascal_pf.py
+-rw-r--r--   0        0        0     5897 2024-05-24 06:15:48.264160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pcpnet_dataset.py
+-rw-r--r--   0        0        0     4207 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pcqm4m.py
+-rw-r--r--   0        0        0     7201 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/planetoid.py
+-rw-r--r--   0        0        0     3045 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/polblogs.py
+-rw-r--r--   0        0        0     4999 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ppi.py
+-rw-r--r--   0        0        0     3325 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/qm7.py
+-rw-r--r--   0        0        0    17186 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/qm9.py
+-rw-r--r--   0        0        0     5317 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/rcdd.py
+-rw-r--r--   0        0        0     3122 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/reddit.py
+-rw-r--r--   0        0        0     4282 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/reddit2.py
+-rw-r--r--   0        0        0     4535 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-r--r--   0        0        0     4553 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/s3dis.py
+-rw-r--r--   0        0        0     8816 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/sbm_dataset.py
+-rw-r--r--   0        0        0     8504 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/shapenet.py
+-rw-r--r--   0        0        0     6316 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/shrec2016.py
+-rw-r--r--   0        0        0     9433 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/snap_dataset.py
+-rw-r--r--   0        0        0     3278 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/suite_sparse.py
+-rw-r--r--   0        0        0     4170 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/taobao.py
+-rw-r--r--   0        0        0     4632 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/tosca.py
+-rw-r--r--   0        0        0     7847 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/tu_dataset.py
+-rw-r--r--   0        0        0     3658 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/twitch.py
+-rw-r--r--   0        0        0     7001 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/upfd.py
+-rw-r--r--   0        0        0      182 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1835 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/utils/cheatsheet.py
+-rw-r--r--   0        0        0     4889 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/webkb.py
+-rw-r--r--   0        0        0     3884 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/wikics.py
+-rw-r--r--   0        0        0     4947 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/wikidata.py
+-rw-r--r--   0        0        0     6640 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/wikipedia_network.py
+-rw-r--r--   0        0        0     7028 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/willow_object_class.py
+-rw-r--r--   0        0        0     8158 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/word_net.py
+-rw-r--r--   0        0        0     3959 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/yelp.py
+-rw-r--r--   0        0        0     6347 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/zinc.py
+-rw-r--r--   0        0        0     1295 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/debug.py
+-rw-r--r--   0        0        0      858 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/deprecation.py
+-rw-r--r--   0        0        0      589 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_context.py
+-rw-r--r--   0        0        0     4933 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_link_neighbor_loader.py
+-rw-r--r--   0        0        0     6492 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_loader.py
+-rw-r--r--   0        0        0     4372 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_neighbor_loader.py
+-rw-r--r--   0        0        0    42406 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_neighbor_sampler.py
+-rw-r--r--   0        0        0     3309 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/event_loop.py
+-rw-r--r--   0        0        0    19018 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/local_feature_store.py
+-rw-r--r--   0        0        0     8408 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/local_graph_store.py
+-rw-r--r--   0        0        0    14685 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/partition.py
+-rw-r--r--   0        0        0     5753 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/rpc.py
+-rw-r--r--   0        0        0     6567 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/utils.py
+-rw-r--r--   0        0        0    69668 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/edge_index.py
+-rw-r--r--   0        0        0     4756 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/experimental.py
+-rw-r--r--   0        0        0      359 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/__init__.py
+-rw-r--r--   0        0        0      496 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/__init__.py
+-rw-r--r--   0        0        0     4545 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-r--r--   0        0        0     6935 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/base.py
+-rw-r--r--   0        0        0    12857 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/captum.py
+-rw-r--r--   0        0        0     7346 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-r--r--   0        0        0     2872 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-r--r--   0        0        0    12454 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-r--r--   0        0        0    21367 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/graphmask_explainer.py
+-rw-r--r--   0        0        0    10371 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-r--r--   0        0        0     2564 2024-05-24 06:15:48.268160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/utils.py
+-rw-r--r--   0        0        0     7834 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/config.py
+-rw-r--r--   0        0        0    10667 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/explainer.py
+-rw-r--r--   0        0        0    14934 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/explanation.py
+-rw-r--r--   0        0        0      301 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/__init__.py
+-rw-r--r--   0        0        0     1888 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/basic.py
+-rw-r--r--   0        0        0     3063 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/faithfulness.py
+-rw-r--r--   0        0        0     6157 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/fidelity.py
+-rw-r--r--   0        0        0     1815 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/__init__.py
+-rw-r--r--   0        0        0      510 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/benchmark.py
+-rw-r--r--   0        0        0     2371 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/checkpoint.py
+-rw-r--r--   0        0        0      738 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/cmd_args.py
+-rw-r--r--   0        0        0    17197 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/config.py
+-rw-r--r--   0        0        0      389 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/act/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/config/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/encoder/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/head/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-r--r--   0        0        0     8435 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/layer/generalconv.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/loader/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/loss/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/network/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/optimizer/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/pooling/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/stage/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/train/__init__.py
+-rw-r--r--   0        0        0      221 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/imports.py
+-rw-r--r--   0        0        0      521 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/init.py
+-rw-r--r--   0        0        0    11605 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/loader.py
+-rw-r--r--   0        0        0    11314 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/logger.py
+-rw-r--r--   0        0        0     1445 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/loss.py
+-rw-r--r--   0        0        0     3110 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/model_builder.py
+-rw-r--r--   0        0        0     1121 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/__init__.py
+-rw-r--r--   0        0        0      855 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/act.py
+-rw-r--r--   0        0        0     3034 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/encoder.py
+-rw-r--r--   0        0        0     6373 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/gnn.py
+-rw-r--r--   0        0        0     4603 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/head.py
+-rw-r--r--   0        0        0    12500 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/layer.py
+-rw-r--r--   0        0        0      288 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/pooling.py
+-rw-r--r--   0        0        0     1383 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/transform.py
+-rw-r--r--   0        0        0     2544 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/optim.py
+-rw-r--r--   0        0        0     3954 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/register.py
+-rw-r--r--   0        0        0     2653 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/train.py
+-rw-r--r--   0        0        0        0 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/LICENSE
+-rw-r--r--   0        0        0      641 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/__init__.py
+-rw-r--r--   0        0        0     9349 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/agg_runs.py
+-rw-r--r--   0        0        0     3045 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/comp_budget.py
+-rw-r--r--   0        0        0     1342 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/device.py
+-rw-r--r--   0        0        0      690 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/epoch.py
+-rw-r--r--   0        0        0     2049 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/io.py
+-rw-r--r--   0        0        0      624 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/plot.py
+-rw-r--r--   0        0        0      199 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/tools.py
+-rw-r--r--   0        0        0      790 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/home.py
+-rw-r--r--   0        0        0    23512 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/index.py
+-rw-r--r--   0        0        0    19267 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/inspector.py
+-rw-r--r--   0        0        0      528 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/__init__.py
+-rw-r--r--   0        0        0     6577 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/fs.py
+-rw-r--r--   0        0        0     1177 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/npz.py
+-rw-r--r--   0        0        0     1088 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/obj.py
+-rw-r--r--   0        0        0     2762 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/off.py
+-rw-r--r--   0        0        0     4667 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/planetoid.py
+-rw-r--r--   0        0        0      489 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/ply.py
+-rw-r--r--   0        0        0     1170 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/sdf.py
+-rw-r--r--   0        0        0     4930 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/tu.py
+-rw-r--r--   0        0        0      910 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/io/txt_array.py
+-rw-r--r--   0        0        0      935 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/isinstance.py
+-rw-r--r--   0        0        0      908 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/lazy_loader.py
+-rw-r--r--   0        0        0     1835 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/__init__.py
+-rw-r--r--   0        0        0     1615 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/base.py
+-rw-r--r--   0        0        0     2106 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/cache.py
+-rw-r--r--   0        0        0    13189 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/cluster.py
+-rw-r--r--   0        0        0     1459 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/data_list_loader.py
+-rw-r--r--   0        0        0     3527 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/dataloader.py
+-rw-r--r--   0        0        0     1685 2024-05-24 06:15:48.272160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/dense_data_loader.py
+-rw-r--r--   0        0        0     4163 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-r--r--   0        0        0     8448 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/graph_saint.py
+-rw-r--r--   0        0        0     6012 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/hgt_loader.py
+-rw-r--r--   0        0        0    31462 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/ibmb_loader.py
+-rw-r--r--   0        0        0     3754 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/imbalanced_sampler.py
+-rw-r--r--   0        0        0    16207 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/link_loader.py
+-rw-r--r--   0        0        0    14383 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/link_neighbor_loader.py
+-rw-r--r--   0        0        0    10931 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/mixin.py
+-rw-r--r--   0        0        0    12452 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/neighbor_loader.py
+-rw-r--r--   0        0        0     8513 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/neighbor_sampler.py
+-rw-r--r--   0        0        0    11848 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/node_loader.py
+-rw-r--r--   0        0        0     3236 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/prefetch.py
+-rw-r--r--   0        0        0     2196 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/random_node_loader.py
+-rw-r--r--   0        0        0     4173 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/shadow.py
+-rw-r--r--   0        0        0     2248 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/temporal_dataloader.py
+-rw-r--r--   0        0        0    14901 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/utils.py
+-rw-r--r--   0        0        0     3518 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/zip_loader.py
+-rw-r--r--   0        0        0      858 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/logging.py
+-rw-r--r--   0        0        0      296 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/metrics/__init__.py
+-rw-r--r--   0        0        0     7521 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/metrics/link_pred.py
+-rw-r--r--   0        0        0      847 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/__init__.py
+-rw-r--r--   0        0        0     1551 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/__init__.py
+-rw-r--r--   0        0        0     3003 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/attention.py
+-rw-r--r--   0        0        0     8244 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/base.py
+-rw-r--r--   0        0        0    11011 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/basic.py
+-rw-r--r--   0        0        0     2650 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/deep_sets.py
+-rw-r--r--   0        0        0     6639 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/equilibrium.py
+-rw-r--r--   0        0        0    12276 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/fused.py
+-rw-r--r--   0        0        0     3801 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/gmt.py
+-rw-r--r--   0        0        0     2193 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/gru.py
+-rw-r--r--   0        0        0     4190 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/lcm.py
+-rw-r--r--   0        0        0     2214 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/lstm.py
+-rw-r--r--   0        0        0     2514 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/mlp.py
+-rw-r--r--   0        0        0     8170 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/multi.py
+-rw-r--r--   0        0        0     6189 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/quantile.py
+-rw-r--r--   0        0        0     4638 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/scaler.py
+-rw-r--r--   0        0        0     2446 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/set2set.py
+-rw-r--r--   0        0        0     4207 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/set_transformer.py
+-rw-r--r--   0        0        0     2507 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/sort.py
+-rw-r--r--   0        0        0     8338 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/utils.py
+-rw-r--r--   0        0        0     1126 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/variance_preserving.py
+-rw-r--r--   0        0        0       76 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/attention/__init__.py
+-rw-r--r--   0        0        0     7357 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/attention/performer.py
+-rw-r--r--   0        0        0     3515 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/__init__.py
+-rw-r--r--   0        0        0     3077 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/agnn_conv.py
+-rw-r--r--   0        0        0     4387 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-r--r--   0        0        0     5983 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/appnp.py
+-rw-r--r--   0        0        0     6585 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/arma_conv.py
+-rw-r--r--   0        0        0     4014 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cg_conv.py
+-rw-r--r--   0        0        0     6423 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cheb_conv.py
+-rw-r--r--   0        0        0     5255 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cluster_gcn_conv.py
+-rw-r--r--   0        0        0     5641 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/collect.jinja
+-rw-r--r--   0        0        0      251 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-r--r--   0        0        0     6364 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/base.py
+-rw-r--r--   0        0        0     2874 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-r--r--   0        0        0     4002 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-r--r--   0        0        0     2830 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-r--r--   0        0        0     2440 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/dir_gnn_conv.py
+-rw-r--r--   0        0        0    12241 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/dna_conv.py
+-rw-r--r--   0        0        0     5389 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/edge_conv.py
+-rw-r--r--   0        0        0     2216 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/edge_updater.jinja
+-rw-r--r--   0        0        0    10742 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/eg_conv.py
+-rw-r--r--   0        0        0     9065 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/fa_conv.py
+-rw-r--r--   0        0        0     4430 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/feast_conv.py
+-rw-r--r--   0        0        0     6314 2024-05-24 06:15:48.276160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/film_conv.py
+-rw-r--r--   0        0        0     4495 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-r--r--   0        0        0    16091 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gat_conv.py
+-rw-r--r--   0        0        0     3518 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-r--r--   0        0        0    13639 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gatv2_conv.py
+-rw-r--r--   0        0        0     7001 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gcn2_conv.py
+-rw-r--r--   0        0        0    10415 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gcn_conv.py
+-rw-r--r--   0        0        0     9722 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gen_conv.py
+-rw-r--r--   0        0        0     7591 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/general_conv.py
+-rw-r--r--   0        0        0     7411 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gin_conv.py
+-rw-r--r--   0        0        0     8315 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gmm_conv.py
+-rw-r--r--   0        0        0     6672 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gps_conv.py
+-rw-r--r--   0        0        0     3905 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/graph_conv.py
+-rw-r--r--   0        0        0     4951 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gravnet_conv.py
+-rw-r--r--   0        0        0     7198 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/han_conv.py
+-rw-r--r--   0        0        0     6084 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/heat_conv.py
+-rw-r--r--   0        0        0     6555 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/hetero_conv.py
+-rw-r--r--   0        0        0     9043 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/hgt_conv.py
+-rw-r--r--   0        0        0     8691 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-r--r--   0        0        0     3494 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/le_conv.py
+-rw-r--r--   0        0        0     2369 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/lg_conv.py
+-rw-r--r--   0        0        0    43577 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/message_passing.py
+-rw-r--r--   0        0        0     4340 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/mf_conv.py
+-rw-r--r--   0        0        0     4554 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/mixhop_conv.py
+-rw-r--r--   0        0        0     4759 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/nn_conv.py
+-rw-r--r--   0        0        0     4908 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/pan_conv.py
+-rw-r--r--   0        0        0     4892 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/pdn_conv.py
+-rw-r--r--   0        0        0     8325 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/pna_conv.py
+-rw-r--r--   0        0        0     4508 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/point_conv.py
+-rw-r--r--   0        0        0     3278 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-r--r--   0        0        0     5878 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-r--r--   0        0        0     5363 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/ppf_conv.py
+-rw-r--r--   0        0        0     7374 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/propagate.jinja
+-rw-r--r--   0        0        0     5217 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-r--r--   0        0        0    22863 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/rgat_conv.py
+-rw-r--r--   0        0        0    15666 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/rgcn_conv.py
+-rw-r--r--   0        0        0     5812 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/sage_conv.py
+-rw-r--r--   0        0        0     4543 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/sg_conv.py
+-rw-r--r--   0        0        0     6190 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/signed_conv.py
+-rw-r--r--   0        0        0     3888 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/simple_conv.py
+-rw-r--r--   0        0        0     6314 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/spline_conv.py
+-rw-r--r--   0        0        0     5131 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/ssg_conv.py
+-rw-r--r--   0        0        0    12420 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/supergat_conv.py
+-rw-r--r--   0        0        0     4164 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/tag_conv.py
+-rw-r--r--   0        0        0    10407 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/transformer_conv.py
+-rw-r--r--   0        0        0      852 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/utils/__init__.py
+-rw-r--r--   0        0        0     2792 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-r--r--   0        0        0     3140 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/wl_conv.py
+-rw-r--r--   0        0        0     2777 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-r--r--   0        0        0     5956 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/x_conv.py
+-rw-r--r--   0        0        0     4764 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/data_parallel.py
+-rw-r--r--   0        0        0      847 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/__init__.py
+-rw-r--r--   0        0        0     4238 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-r--r--   0        0        0     3002 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-r--r--   0        0        0     2361 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-r--r--   0        0        0     2751 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-r--r--   0        0        0     2672 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-r--r--   0        0        0     3051 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/diff_pool.py
+-rw-r--r--   0        0        0     6115 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dmon_pool.py
+-rw-r--r--   0        0        0    17748 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/linear.py
+-rw-r--r--   0        0        0     4111 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/mincut_pool.py
+-rw-r--r--   0        0        0     3115 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/encoding.py
+-rw-r--r--   0        0        0      129 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/functional/__init__.py
+-rw-r--r--   0        0        0     1549 2024-05-24 06:15:48.280160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/functional/bro.py
+-rw-r--r--   0        0        0      863 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/functional/gini.py
+-rw-r--r--   0        0        0    16055 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/fx.py
+-rw-r--r--   0        0        0     1088 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/glob.py
+-rw-r--r--   0        0        0     2457 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/inits.py
+-rw-r--r--   0        0        0      290 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/__init__.py
+-rw-r--r--   0        0        0     5902 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/base.py
+-rw-r--r--   0        0        0     3234 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/complex.py
+-rw-r--r--   0        0        0     2462 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/distmult.py
+-rw-r--r--   0        0        0      771 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/loader.py
+-rw-r--r--   0        0        0     3208 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/rotate.py
+-rw-r--r--   0        0        0     3088 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/transe.py
+-rw-r--r--   0        0        0     8937 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/lr_scheduler.py
+-rw-r--r--   0        0        0     9512 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/model_hub.py
+-rw-r--r--   0        0        0     1909 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/__init__.py
+-rw-r--r--   0        0        0     6634 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/attentive_fp.py
+-rw-r--r--   0        0        0    10770 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/autoencoder.py
+-rw-r--r--   0        0        0    31225 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/basic_gnn.py
+-rw-r--r--   0        0        0     3971 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/captum.py
+-rw-r--r--   0        0        0     6827 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/correct_and_smooth.py
+-rw-r--r--   0        0        0     4197 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-r--r--   0        0        0     4339 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/deepgcn.py
+-rw-r--r--   0        0        0    36186 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/dimenet.py
+-rw-r--r--   0        0        0     5107 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/dimenet_utils.py
+-rw-r--r--   0        0        0     7873 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/gnnff.py
+-rw-r--r--   0        0        0     9246 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/graph_mixer.py
+-rw-r--r--   0        0        0     5395 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/graph_unet.py
+-rw-r--r--   0        0        0     3450 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/jumping_knowledge.py
+-rw-r--r--   0        0        0     3908 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/label_prop.py
+-rw-r--r--   0        0        0    12465 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/lightgcn.py
+-rw-r--r--   0        0        0     5812 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/linkx.py
+-rw-r--r--   0        0        0     2580 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/mask_label.py
+-rw-r--r--   0        0        0     6540 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/meta.py
+-rw-r--r--   0        0        0    10863 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/metapath2vec.py
+-rw-r--r--   0        0        0    10315 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/mlp.py
+-rw-r--r--   0        0        0     2378 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/neural_fingerprint.py
+-rw-r--r--   0        0        0     7724 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/node2vec.py
+-rw-r--r--   0        0        0     3538 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/pmlp.py
+-rw-r--r--   0        0        0     8986 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/re_net.py
+-rw-r--r--   0        0        0     2808 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/rect.py
+-rw-r--r--   0        0        0    11796 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/rev_gnn.py
+-rw-r--r--   0        0        0    16619 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/schnet.py
+-rw-r--r--   0        0        0     9839 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/signed_gcn.py
+-rw-r--r--   0        0        0    11878 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/tgn.py
+-rw-r--r--   0        0        0    43192 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/visnet.py
+-rw-r--r--   0        0        0     2373 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/module_dict.py
+-rw-r--r--   0        0        0      106 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/nlp/__init__.py
+-rw-r--r--   0        0        0     2070 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/nlp/sentence_transformer.py
+-rw-r--r--   0        0        0      669 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/__init__.py
+-rw-r--r--   0        0        0     8283 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/batch_norm.py
+-rw-r--r--   0        0        0     4722 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/diff_group_norm.py
+-rw-r--r--   0        0        0     2727 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/graph_norm.py
+-rw-r--r--   0        0        0     1491 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/graph_size_norm.py
+-rw-r--r--   0        0        0     4685 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/instance_norm.py
+-rw-r--r--   0        0        0     7831 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/layer_norm.py
+-rw-r--r--   0        0        0     1322 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-r--r--   0        0        0     1662 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/msg_norm.py
+-rw-r--r--   0        0        0     2824 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/pair_norm.py
+-rw-r--r--   0        0        0     2410 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/parameter_dict.py
+-rw-r--r--   0        0        0    14129 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/approx_knn.py
+-rw-r--r--   0        0        0     6683 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/asap.py
+-rw-r--r--   0        0        0     3966 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/avg_pool.py
+-rw-r--r--   0        0        0      287 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/connect/__init__.py
+-rw-r--r--   0        0        0     4094 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/connect/base.py
+-rw-r--r--   0        0        0     2190 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/connect/filter_edges.py
+-rw-r--r--   0        0        0      273 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/consecutive.py
+-rw-r--r--   0        0        0     1601 2024-05-24 06:15:48.284160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/decimation.py
+-rw-r--r--   0        0        0     8581 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/edge_pool.py
+-rw-r--r--   0        0        0     3492 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/glob.py
+-rw-r--r--   0        0        0     1291 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/graclus.py
+-rw-r--r--   0        0        0    11343 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/knn.py
+-rw-r--r--   0        0        0     4262 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/max_pool.py
+-rw-r--r--   0        0        0     5377 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/mem_pool.py
+-rw-r--r--   0        0        0     4366 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/pan_pool.py
+-rw-r--r--   0        0        0      737 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/pool.py
+-rw-r--r--   0        0        0     5838 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/sag_pool.py
+-rw-r--r--   0        0        0      254 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/select/__init__.py
+-rw-r--r--   0        0        0     3311 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/select/base.py
+-rw-r--r--   0        0        0     5305 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/select/topk.py
+-rw-r--r--   0        0        0     5159 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/topk_pool.py
+-rw-r--r--   0        0        0     2736 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/voxel_grid.py
+-rw-r--r--   0        0        0      426 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/reshape.py
+-rw-r--r--   0        0        0     6155 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/resolver.py
+-rw-r--r--   0        0        0     1054 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/sequential.jinja
+-rw-r--r--   0        0        0     5534 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/sequential.py
+-rw-r--r--   0        0        0     5821 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/summary.py
+-rw-r--r--   0        0        0     1282 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-r--r--   0        0        0     6519 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_hetero_module.py
+-rw-r--r--   0        0        0    18407 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_hetero_transformer.py
+-rw-r--r--   0        0        0    23121 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_hetero_with_bases_transformer.py
+-rw-r--r--   0        0        0      129 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/unpool/__init__.py
+-rw-r--r--   0        0        0     2586 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/unpool/knn_interpolate.py
+-rw-r--r--   0        0        0      863 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/__init__.py
+-rw-r--r--   0        0        0     5256 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/benchmark.py
+-rw-r--r--   0        0        0    11793 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/profile.py
+-rw-r--r--   0        0        0    16706 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/profiler.py
+-rw-r--r--   0        0        0     5497 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/utils.py
+-rw-r--r--   0        0        0     1273 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/resolver.py
+-rw-r--r--   0        0        0      512 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/__init__.py
+-rw-r--r--   0        0        0    26515 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/base.py
+-rw-r--r--   0        0        0     2721 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/hgt_sampler.py
+-rw-r--r--   0        0        0    33974 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/neighbor_sampler.py
+-rw-r--r--   0        0        0     5485 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/utils.py
+-rw-r--r--   0        0        0      372 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/seed.py
+-rw-r--r--   0        0        0     1060 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/template.py
+-rw-r--r--   0        0        0     1249 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/__init__.py
+-rw-r--r--   0        0        0     4606 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/asserts.py
+-rw-r--r--   0        0        0     2604 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/data.py
+-rw-r--r--   0        0        0     8583 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/decorators.py
+-rw-r--r--   0        0        0     2227 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/distributed.py
+-rw-r--r--   0        0        0     2158 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/feature_store.py
+-rw-r--r--   0        0        0     1044 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/graph_store.py
+-rw-r--r--   0        0        0     4181 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0    14235 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_metapaths.py
+-rw-r--r--   0        0        0     6065 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_positional_encoding.py
+-rw-r--r--   0        0        0     2085 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_remaining_self_loops.py
+-rw-r--r--   0        0        0     2024 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_self_loops.py
+-rw-r--r--   0        0        0     1298 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/base_transform.py
+-rw-r--r--   0        0        0     2464 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/cartesian.py
+-rw-r--r--   0        0        0      645 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/center.py
+-rw-r--r--   0        0        0     1658 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/compose.py
+-rw-r--r--   0        0        0     2005 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/constant.py
+-rw-r--r--   0        0        0     1264 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/delaunay.py
+-rw-r--r--   0        0        0     2360 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/distance.py
+-rw-r--r--   0        0        0     1083 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/face_to_edge.py
+-rw-r--r--   0        0        0     3056 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/feature_propagation.py
+-rw-r--r--   0        0        0     2426 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/fixed_points.py
+-rw-r--r--   0        0        0     1397 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/gcn_norm.py
+-rw-r--r--   0        0        0    20201 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/gdc.py
+-rw-r--r--   0        0        0     1028 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/generate_mesh_normals.py
+-rw-r--r--   0        0        0     2564 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/grid_sampling.py
+-rw-r--r--   0        0        0     4102 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/half_hop.py
+-rw-r--r--   0        0        0     2536 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/knn_graph.py
+-rw-r--r--   0        0        0     2497 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-r--r--   0        0        0     2161 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/largest_connected_components.py
+-rw-r--r--   0        0        0     3730 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/line_graph.py
+-rw-r--r--   0        0        0     1997 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/linear_transformation.py
+-rw-r--r--   0        0        0     2144 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/local_cartesian.py
+-rw-r--r--   0        0        0     1480 2024-05-24 06:15:48.288160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/local_degree_profile.py
+-rw-r--r--   0        0        0     4813 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/mask.py
+-rw-r--r--   0        0        0     6075 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/node_property_split.py
+-rw-r--r--   0        0        0     1028 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/normalize_features.py
+-rw-r--r--   0        0        0     1782 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/normalize_rotation.py
+-rw-r--r--   0        0        0      666 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/normalize_scale.py
+-rw-r--r--   0        0        0     1584 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/one_hot_degree.py
+-rw-r--r--   0        0        0    21041 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/pad.py
+-rw-r--r--   0        0        0     1794 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/point_pair_features.py
+-rw-r--r--   0        0        0     2213 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/polar.py
+-rw-r--r--   0        0        0     2043 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/radius_graph.py
+-rw-r--r--   0        0        0     1033 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_flip.py
+-rw-r--r--   0        0        0     1721 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_jitter.py
+-rw-r--r--   0        0        0    15181 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_link_split.py
+-rw-r--r--   0        0        0     5853 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_node_split.py
+-rw-r--r--   0        0        0     1946 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_rotate.py
+-rw-r--r--   0        0        0     1261 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_scale.py
+-rw-r--r--   0        0        0     1365 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_shear.py
+-rw-r--r--   0        0        0     1929 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-r--r--   0        0        0     2449 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-r--r--   0        0        0      932 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/remove_training_classes.py
+-rw-r--r--   0        0        0     6509 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/rooted_subgraph.py
+-rw-r--r--   0        0        0     2280 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/sample_points.py
+-rw-r--r--   0        0        0     2329 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/sign.py
+-rw-r--r--   0        0        0     2320 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/spherical.py
+-rw-r--r--   0        0        0     1009 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/svd_feature_reduction.py
+-rw-r--r--   0        0        0     1659 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/target_indegree.py
+-rw-r--r--   0        0        0     2456 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_dense.py
+-rw-r--r--   0        0        0     1470 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_device.py
+-rw-r--r--   0        0        0     5580 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_sparse_tensor.py
+-rw-r--r--   0        0        0     2697 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_superpixels.py
+-rw-r--r--   0        0        0     2972 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_undirected.py
+-rw-r--r--   0        0        0     1313 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/two_hop.py
+-rw-r--r--   0        0        0     2860 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/virtual_node.py
+-rw-r--r--   0        0        0    13536 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/typing.py
+-rw-r--r--   0        0        0     4790 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_assortativity.py
+-rw-r--r--   0        0        0     6769 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_coalesce.py
+-rw-r--r--   0        0        0     1017 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_degree.py
+-rw-r--r--   0        0        0     2562 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_grid.py
+-rw-r--r--   0        0        0     5090 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_homophily.py
+-rw-r--r--   0        0        0     1283 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_index_sort.py
+-rw-r--r--   0        0        0     1403 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_lexsort.py
+-rw-r--r--   0        0        0    14672 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_negative_sampling.py
+-rw-r--r--   0        0        0     1167 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_normalized_cut.py
+-rw-r--r--   0        0        0     1404 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_one_hot.py
+-rw-r--r--   0        0        0    13389 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_scatter.py
+-rw-r--r--   0        0        0     1976 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_segment.py
+-rw-r--r--   0        0        0     2439 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_select.py
+-rw-r--r--   0        0        0     3242 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_softmax.py
+-rw-r--r--   0        0        0     4500 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_sort_edge_index.py
+-rw-r--r--   0        0        0     5794 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_spmm.py
+-rw-r--r--   0        0        0    18311 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_subgraph.py
+-rw-r--r--   0        0        0     3606 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_to_dense_adj.py
+-rw-r--r--   0        0        0     4582 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_to_dense_batch.py
+-rw-r--r--   0        0        0     3569 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_train_test_split_edges.py
+-rw-r--r--   0        0        0     5300 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_tree_decomposition.py
+-rw-r--r--   0        0        0     8307 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_trim_to_layer.py
+-rw-r--r--   0        0        0     2378 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_unbatch.py
+-rw-r--r--   0        0        0     8601 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/augmentation.py
+-rw-r--r--   0        0        0    21740 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/convert.py
+-rw-r--r--   0        0        0     3047 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/cross_entropy.py
+-rw-r--r--   0        0        0    11416 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/dropout.py
+-rw-r--r--   0        0        0     1675 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/embedding.py
+-rw-r--r--   0        0        0      703 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/functions.py
+-rw-r--r--   0        0        0     4668 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/geodesic.py
+-rw-r--r--   0        0        0     5542 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/hetero.py
+-rw-r--r--   0        0        0     3588 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/isolated.py
+-rw-r--r--   0        0        0     3695 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/laplacian.py
+-rw-r--r--   0        0        0    23051 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/loop.py
+-rw-r--r--   0        0        0     5918 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/map.py
+-rw-r--r--   0        0        0     2340 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/mask.py
+-rw-r--r--   0        0        0     4387 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/mesh_laplacian.py
+-rw-r--r--   0        0        0      699 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/mixin.py
+-rw-r--r--   0        0        0     3310 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/nested.py
+-rw-r--r--   0        0        0     3750 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/noise_scheduler.py
+-rw-r--r--   0        0        0     2176 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/num_nodes.py
+-rw-r--r--   0        0        0     4055 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/ppr.py
+-rw-r--r--   0        0        0     5148 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/random.py
+-rw-r--r--   0        0        0      815 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/repeat.py
+-rw-r--r--   0        0        0     6291 2024-05-24 06:15:48.292160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/smiles.py
+-rw-r--r--   0        0        0    24894 2024-05-24 06:15:48.296160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/sparse.py
+-rw-r--r--   0        0        0     6222 2024-05-24 06:15:48.296160 pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/undirected.py
+-rw-r--r--   0        0        0      154 2024-05-24 06:15:48.296160 pyg_nightly-2.6.0.dev20240524/torch_geometric/visualization/__init__.py
+-rw-r--r--   0        0        0     4813 2024-05-24 06:15:48.296160 pyg_nightly-2.6.0.dev20240524/torch_geometric/visualization/graph.py
+-rw-r--r--   0        0        0      477 2024-05-24 06:15:48.296160 pyg_nightly-2.6.0.dev20240524/torch_geometric/visualization/influence.py
+-rw-r--r--   0        0        0      413 2024-05-24 06:15:48.296160 pyg_nightly-2.6.0.dev20240524/torch_geometric/warnings.py
+-rw-r--r--   0        0        0    62945 1970-01-01 00:00:00.000000 pyg_nightly-2.6.0.dev20240524/PKG-INFO
```

### Comparing `pyg_nightly-2.6.0.dev20240523/README.md` & `pyg_nightly-2.6.0.dev20240524/README.md`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/pyproject.toml` & `pyg_nightly-2.6.0.dev20240524/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="pyg-nightly"
-version="2.6.0.dev20240523"
+version="2.6.0.dev20240524"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.8"
 keywords=[
```

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.6.0.dev20240523'
+__version__ = '2.6.0.dev20240524'
 
 __all__ = [
     'Index',
     'EdgeIndex',
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
```

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/_compile.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/_compile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/backend.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/backend.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/config_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/config_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/explain/pgm_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/contrib/nn/models/rbcd_attack.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/batch.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/collate.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/collate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/data.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/database.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/database.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/datapipes.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/download.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/extract.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/feature_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/graph_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/hetero_data.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/hetero_data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/hypergraph_data.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/hypergraph_data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/in_memory_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/lightning/datamodule.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/on_disk_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/on_disk_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/remote_backend_utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/separate.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/storage.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/storage.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/summary.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/temporal.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/data/view.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/actor.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/airfrans.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/airports.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/amazon.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/amazon_book.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/amazon_book.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/amazon_products.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/aminer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/aqsol.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/attributed_graph_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ba2motif_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ba_multi_shapes.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ba_shapes.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/bitcoin_otc.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/brca_tgca.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/brca_tgca.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/citation_full.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/coauthor.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/coma.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/cornell.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/cornell.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dblp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dbp15k.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/deezer_europe.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dgraph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/dynamic_faust.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/elliptic.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/elliptic_temporal.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/elliptic_temporal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/email_eu_core.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/entities.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/explainer_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/facebook.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/fake.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/faust.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/flickr.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/freebase.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gdelt.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gdelt_lite.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gdelt_lite.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ged_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gemsec.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/geometry.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/github.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/gnn_benchmark_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/ba_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/er_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/grid_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/graph_generator/tree_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/graph_generator/tree_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/heterophilous_graph_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/hgb_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/hm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/hm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/hydro_net.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/icews.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/igmc_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/igmc_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/imdb.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/infection_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/jodie.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/karate.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/last_fm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/lastfm_asia.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/linkx_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/lrgb.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/malnet_tiny.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/md17.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/mnist_superpixels.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/modelnet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/molecule_net.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/custom.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/cycle.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/grid.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/motif_generator/house.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/movie_lens.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/movie_lens_100k.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/movie_lens_100k.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/movie_lens_1m.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/movie_lens_1m.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/myket.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/myket.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/nell.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/neurograph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/neurograph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ogb_mag.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/omdb.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ose_gvcs.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ose_gvcs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/particle.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pascal.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pascal_pf.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pcpnet_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/pcqm4m.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/pcqm4m.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/planetoid.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/polblogs.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/ppi.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/qm7.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/qm9.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/rcdd.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/rcdd.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/reddit.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/reddit2.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/rel_link_pred_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/s3dis.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/sbm_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/shapenet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/shrec2016.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/snap_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/suite_sparse.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/taobao.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/tosca.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/tu_dataset.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/twitch.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/upfd.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/utils/cheatsheet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/webkb.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/wikics.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/wikidata.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/wikidata.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/wikipedia_network.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/willow_object_class.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/word_net.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/yelp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/datasets/zinc.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/debug.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/deprecation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_link_neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/dist_neighbor_sampler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/dist_neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/event_loop.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/event_loop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/local_feature_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/local_feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/local_graph_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/local_graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/partition.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/partition.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/rpc.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/rpc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/distributed/utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/edge_index.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/edge_index.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/experimental.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/attention_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/captum.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/captum_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/dummy_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/gnn_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/graphmask_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/pg_explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/algorithm/utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/config.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/explainer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/explanation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/basic.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/faithfulness.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/explain/metric/fidelity.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/checkpoint.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/cmd_args.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/config.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/contrib/layer/generalconv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/init.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/init.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/logger.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/loss.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/model_builder.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/act.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/encoder.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/gnn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/head.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/layer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/models/transform.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/optim.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/register.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/train.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/agg_runs.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/comp_budget.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/device.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/epoch.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/io.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/graphgym/utils/plot.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/home.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/index.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/index.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/inspector.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/inspector.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/fs.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/fs.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/npz.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/obj.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/off.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/planetoid.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/sdf.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/tu.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/tu.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/io/txt_array.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/isinstance.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/isinstance.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/lazy_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/cache.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/cache.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/cluster.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/cluster.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/data_list_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/dataloader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/dense_data_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/dynamic_batch_sampler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/graph_saint.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/hgt_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/ibmb_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/ibmb_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/imbalanced_sampler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/link_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/link_neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/link_neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/mixin.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/neighbor_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/neighbor_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/neighbor_sampler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/node_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/prefetch.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/prefetch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/random_node_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/shadow.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/temporal_dataloader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/loader/zip_loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/logging.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/metrics/link_pred.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/metrics/link_pred.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/attention.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/basic.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/deep_sets.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/equilibrium.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/equilibrium.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/fused.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/gmt.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/gru.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/lcm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/lcm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/lstm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/mlp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/multi.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/quantile.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/quantile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/scaler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/set2set.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/set_transformer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/sort.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/aggr/variance_preserving.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/aggr/variance_preserving.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/attention/performer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/attention/performer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/agnn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/antisymmetric_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/appnp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/arma_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cg_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cheb_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cluster_gcn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/collect.jinja` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/collect.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/gat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/cugraph/sage_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/dir_gnn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/dir_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/dna_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/edge_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/edge_updater.jinja` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/edge_updater.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/eg_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/fa_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/feast_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/film_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/fused_gat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gated_graph_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gatv2_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gcn2_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gcn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gen_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/general_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gin_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gmm_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gps_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/graph_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/gravnet_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/han_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/heat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/hetero_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/hgt_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/hypergraph_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/le_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/lg_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/message_passing.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/message_passing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/mf_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/mixhop_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/mixhop_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/nn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/pan_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/pdn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/pna_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/point_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/point_gnn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/point_transformer_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/ppf_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/propagate.jinja` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/propagate.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/res_gated_graph_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/rgat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/rgcn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/sage_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/sg_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/signed_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/simple_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/spline_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/ssg_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/supergat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/tag_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/transformer_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/utils/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/utils/cheatsheet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/wl_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/wl_conv_continuous.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/conv/x_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/data_parallel.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_gat_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_gcn_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_gin_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_graph_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dense_sage_conv.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/diff_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/dmon_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/linear.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/dense/mincut_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/encoding.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/functional/bro.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/functional/gini.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/fx.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/glob.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/inits.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/complex.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/distmult.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/loader.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/rotate.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/kge/transe.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/lr_scheduler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/model_hub.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/attentive_fp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/autoencoder.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/basic_gnn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/basic_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/captum.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/correct_and_smooth.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/deep_graph_infomax.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/deepgcn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/dimenet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/dimenet_utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/gnnff.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/graph_mixer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/graph_mixer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/graph_unet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/jumping_knowledge.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/label_prop.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/lightgcn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/linkx.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/mask_label.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/meta.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/metapath2vec.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/mlp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/neural_fingerprint.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/neural_fingerprint.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/node2vec.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/pmlp.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/pmlp.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/re_net.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/rect.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/rev_gnn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/schnet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/signed_gcn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/tgn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/models/visnet.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/models/visnet.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/module_dict.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/nlp/sentence_transformer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/nlp/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/batch_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/diff_group_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/graph_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/graph_size_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/instance_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/layer_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/mean_subtraction_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/msg_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/norm/pair_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/parameter_dict.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/approx_knn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/approx_knn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/asap.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/avg_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/connect/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/connect/filter_edges.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/connect/filter_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/decimation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/edge_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/glob.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/graclus.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/knn.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/knn.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/max_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/mem_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/pan_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/sag_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/select/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/select/topk.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/select/topk.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/topk_pool.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/pool/voxel_grid.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/resolver.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/sequential.jinja` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/sequential.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/summary.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_fixed_size_transformer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_hetero_module.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_hetero_transformer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/nn/unpool/knn_interpolate.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/benchmark.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/profile.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/profiler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/profile/utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/resolver.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/base.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/base.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/hgt_sampler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/neighbor_sampler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/sampler/utils.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/sampler/utils.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/template.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/template.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/asserts.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/data.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/data.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/decorators.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/distributed.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/distributed.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/feature_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/testing/graph_store.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_metapaths.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_metapaths.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_positional_encoding.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_remaining_self_loops.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_remaining_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/add_self_loops.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/base_transform.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/cartesian.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/center.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/center.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/compose.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/constant.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/constant.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/delaunay.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/distance.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/distance.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/face_to_edge.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/face_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/feature_propagation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/feature_propagation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/fixed_points.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/fixed_points.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/gcn_norm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/gcn_norm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/gdc.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/gdc.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/generate_mesh_normals.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/grid_sampling.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/half_hop.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/half_hop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/knn_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/knn_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/laplacian_lambda_max.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/largest_connected_components.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/largest_connected_components.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/line_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/line_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/linear_transformation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/linear_transformation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/local_cartesian.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/local_cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/local_degree_profile.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/local_degree_profile.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/mask.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/node_property_split.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/node_property_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/normalize_features.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/normalize_features.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/normalize_rotation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/normalize_rotation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/normalize_scale.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/one_hot_degree.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/one_hot_degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/pad.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/point_pair_features.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/point_pair_features.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/polar.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/polar.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/radius_graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/radius_graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_flip.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_flip.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_jitter.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_jitter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_link_split.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_link_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_node_split.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_node_split.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_rotate.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_rotate.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_scale.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_scale.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/random_shear.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/random_shear.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/remove_duplicated_edges.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/remove_isolated_nodes.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/remove_training_classes.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/remove_training_classes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/rooted_subgraph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/rooted_subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/sample_points.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/sample_points.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/sign.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/sign.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/spherical.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/svd_feature_reduction.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/target_indegree.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/target_indegree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_dense.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_dense.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_device.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_device.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_sparse_tensor.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_superpixels.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/to_undirected.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/to_undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/two_hop.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/two_hop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/transforms/virtual_node.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/transforms/virtual_node.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/typing.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/typing.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/__init__.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_assortativity.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_assortativity.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_coalesce.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_coalesce.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_degree.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_degree.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_grid.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_grid.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_homophily.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_homophily.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_index_sort.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_index_sort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_lexsort.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_lexsort.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_negative_sampling.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_negative_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_normalized_cut.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_normalized_cut.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_one_hot.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_one_hot.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_scatter.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_scatter.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_segment.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_segment.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_select.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_select.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_softmax.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_softmax.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_sort_edge_index.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_spmm.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_spmm.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_subgraph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_to_dense_adj.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_to_dense_batch.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_train_test_split_edges.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_tree_decomposition.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_trim_to_layer.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/_unbatch.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/_unbatch.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/augmentation.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/convert.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/cross_entropy.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/dropout.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/embedding.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/functions.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/functions.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/geodesic.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/hetero.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/isolated.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/laplacian.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/loop.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/map.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/map.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/mask.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/mesh_laplacian.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/mixin.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/nested.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/noise_scheduler.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/noise_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/num_nodes.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/ppr.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/ppr.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/random.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/repeat.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/repeat.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/smiles.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/sparse.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/utils/undirected.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/torch_geometric/visualization/graph.py` & `pyg_nightly-2.6.0.dev20240524/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `pyg_nightly-2.6.0.dev20240523/PKG-INFO` & `pyg_nightly-2.6.0.dev20240524/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-nightly
-Version: 2.6.0.dev20240523
+Version: 2.6.0.dev20240524
 Summary: Graph Neural Network Library for PyTorch
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
 Author-email: Matthias Fey <matthias@pyg.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

