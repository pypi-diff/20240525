# Comparing `tmp/bioversions-0.5.98.tar.gz` & `tmp/bioversions-0.5.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioversions-0.5.98.tar", last modified: Fri Apr  7 00:46:36 2023, max compression
+gzip compressed data, was "bioversions-0.5.99.tar", last modified: Sun Apr  9 00:54:18 2023, max compression
```

## Comparing `bioversions-0.5.98.tar` & `bioversions-0.5.99.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.522766 bioversions-0.5.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-07 00:44:44.000000 bioversions-0.5.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-07 00:44:44.000000 bioversions-0.5.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-07 00:46:36.522766 bioversions-0.5.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-07 00:44:44.000000 bioversions-0.5.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.498766 bioversions-0.5.98/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.498766 bioversions-0.5.98/docs/_data/
--rw-r--r--   0 runner    (1001) docker     (123)   162967 2023-04-07 00:46:18.000000 bioversions-0.5.98/docs/_data/versions.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.498766 bioversions-0.5.98/docs/_includes/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/_includes/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/_includes/head.html
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/download.md
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-07 00:46:18.000000 bioversions-0.5.98/docs/failures.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.498766 bioversions-0.5.98/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-04-07 00:46:23.000000 bioversions-0.5.98/docs/img/has_release_url.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-07 00:46:23.000000 bioversions-0.5.98/docs/img/version_date_types.svg
--rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-07 00:46:23.000000 bioversions-0.5.98/docs/img/version_types.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.498766 bioversions-0.5.98/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    94099 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/source/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-07 00:44:44.000000 bioversions-0.5.98/docs/summary.md
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-07 00:44:44.000000 bioversions-0.5.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-07 00:46:36.526766 bioversions-0.5.98/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.494766 bioversions-0.5.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.502766 bioversions-0.5.98/src/bioversions/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.506766 bioversions-0.5.98/src/bioversions/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/resources/update.py
--rw-r--r--   0 runner    (1001) docker     (123)   265516 2023-04-07 00:46:18.000000 bioversions-0.5.98/src/bioversions/resources/versions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/slack_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.522766 bioversions-0.5.98/src/bioversions/sources/
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/antibodyregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/bigg.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/biofacquim.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/biogrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/chebi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/chembl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/chemidplus.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/complexportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/depmap.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/dgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/disgenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/drugbank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/drugcentral.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/ensembl.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/expasy.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/flybase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/guidetopharmacology.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/hgnc.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/homologene.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/intact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/interpro.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/itis.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/kegg.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/mirbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/moalmanac.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/msigdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/ncit.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/npass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/obo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/oncotree.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/pathbank.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/pathwaycommons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/pfam.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/pombase.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/pr.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/pubchem.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/reactome.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/rfam.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/rgd.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/rhea.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/rxnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/slm.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/stringdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/umls.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/unversioned.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/wikipathways.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/sources/zfin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.522766 bioversions-0.5.98/src/bioversions/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/twitter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-07 00:46:26.000000 bioversions-0.5.98/src/bioversions/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-07 00:44:44.000000 bioversions-0.5.98/src/bioversions/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.506766 bioversions-0.5.98/src/bioversions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-07 00:46:36.000000 bioversions-0.5.98/src/bioversions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-07 00:46:36.000000 bioversions-0.5.98/src/bioversions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:46:36.000000 bioversions-0.5.98/src/bioversions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-07 00:46:36.000000 bioversions-0.5.98/src/bioversions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:44:54.000000 bioversions-0.5.98/src/bioversions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-07 00:46:36.000000 bioversions-0.5.98/src/bioversions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 00:46:36.000000 bioversions-0.5.98/src/bioversions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:46:36.522766 bioversions-0.5.98/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-07 00:44:44.000000 bioversions-0.5.98/tests/test_bioversions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.204281 bioversions-0.5.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-09 00:52:08.000000 bioversions-0.5.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-09 00:52:08.000000 bioversions-0.5.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-09 00:54:18.204281 bioversions-0.5.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-09 00:52:08.000000 bioversions-0.5.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.180281 bioversions-0.5.99/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.180281 bioversions-0.5.99/docs/_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   163075 2023-04-09 00:53:56.000000 bioversions-0.5.99/docs/_data/versions.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.180281 bioversions-0.5.99/docs/_includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/_includes/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/_includes/head.html
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/download.md
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 00:53:56.000000 bioversions-0.5.99/docs/failures.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.184281 bioversions-0.5.99/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-04-09 00:54:02.000000 bioversions-0.5.99/docs/img/has_release_url.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-04-09 00:54:02.000000 bioversions-0.5.99/docs/img/version_date_types.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29489 2023-04-09 00:54:02.000000 bioversions-0.5.99/docs/img/version_types.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.184281 bioversions-0.5.99/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    94099 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/source/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-09 00:52:08.000000 bioversions-0.5.99/docs/summary.md
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-09 00:52:08.000000 bioversions-0.5.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-09 00:54:18.204281 bioversions-0.5.99/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.176281 bioversions-0.5.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.184281 bioversions-0.5.99/src/bioversions/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.188281 bioversions-0.5.99/src/bioversions/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/resources/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)   265700 2023-04-09 00:53:56.000000 bioversions-0.5.99/src/bioversions/resources/versions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/slack_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.200281 bioversions-0.5.99/src/bioversions/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/antibodyregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/bigg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/biofacquim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/biogrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/chebi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/chembl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/chemidplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/complexportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/depmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/dgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/disgenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/drugbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/drugcentral.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/ensembl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/flybase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/guidetopharmacology.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/hgnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/homologene.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/intact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/interpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/itis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/kegg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/moalmanac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/msigdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/ncit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/npass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/obo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/oncotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/pathbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/pathwaycommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/pfam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/pombase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/pr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/pubchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/reactome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/rfam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/rgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/rhea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/rxnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/slm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/stringdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/umls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/unversioned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/wikipathways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/sources/zfin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.204281 bioversions-0.5.99/src/bioversions/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/twitter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9712 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-09 00:54:07.000000 bioversions-0.5.99/src/bioversions/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-09 00:52:08.000000 bioversions-0.5.99/src/bioversions/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.188281 bioversions-0.5.99/src/bioversions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-09 00:54:18.000000 bioversions-0.5.99/src/bioversions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-09 00:54:18.000000 bioversions-0.5.99/src/bioversions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:54:18.000000 bioversions-0.5.99/src/bioversions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-09 00:54:18.000000 bioversions-0.5.99/src/bioversions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:52:22.000000 bioversions-0.5.99/src/bioversions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-09 00:54:18.000000 bioversions-0.5.99/src/bioversions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 00:54:18.000000 bioversions-0.5.99/src/bioversions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:54:18.204281 bioversions-0.5.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-09 00:52:08.000000 bioversions-0.5.99/tests/test_bioversions.py
```

### Comparing `bioversions-0.5.98/LICENSE` & `bioversions-0.5.99/LICENSE`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/PKG-INFO` & `bioversions-0.5.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioversions
-Version: 0.5.98
+Version: 0.5.99
 Summary: What's the current version for each biological database?
 Home-page: https://github.com/biopragmatics/bioversions
 Download-URL: https://github.com/biopragmatics/bioversions/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioversions Version: 0.5.98 Summary: What's the
+Metadata-Version: 2.1 Name: bioversions Version: 0.5.99 Summary: What's the
 current version for each biological database? Home-page: https://github.com/
 biopragmatics/bioversions Download-URL: https://github.com/biopragmatics/
 bioversions/releases Author: Charles Tapley Hoyt Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt Maintainer-email: cthoyt@gmail.com License: MIT
 Project-URL: Bug Tracker, https://github.com/biopragmatics/bioversions/issues
 Keywords: databases,biological databases Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: License :: OSI Approved ::
```

### Comparing `bioversions-0.5.98/README.md` & `bioversions-0.5.99/README.md`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/docs/_data/versions.yml` & `bioversions-0.5.99/docs/_data/versions.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 annotations:
   author: runner
-  date: '2023-04-07'
-  revision: 400
+  date: '2023-04-09'
+  revision: 401
 database:
 - name: A nomenclatural ontology for biological names
   prefix: nomen
   releases:
   - retrieved: '2022-01-11'
     version: '2019-04-17'
   vtype: date
@@ -4667,14 +4667,16 @@
     version: '2023-04-04'
   - retrieved: '2023-04-05'
     version: '2023-04-05'
   - retrieved: '2023-04-06'
     version: '2023-04-06'
   - retrieved: '2023-04-07'
     version: '2023-04-07'
+  - retrieved: '2023-04-09'
+    version: '2023-04-09'
   vtype: date
 - name: SWO (The Software Ontology)
   prefix: swo
   releases:
   - retrieved: '2021-02-02'
     version: '1.7'
   vtype: semver
@@ -6144,14 +6146,16 @@
     version: '2023-04-02'
   - retrieved: '2023-04-05'
     version: '2023-04-03'
   - retrieved: '2023-04-06'
     version: '2023-04-04'
   - retrieved: '2023-04-07'
     version: '2023-04-05'
+  - retrieved: '2023-04-09'
+    version: '2023-04-07'
   vtype: date
 - name: Zebrafish Phenotype Ontology
   prefix: zp
   releases:
   - retrieved: '2021-02-02'
     version: '2020-08-02'
   - retrieved: '2021-12-14'
```

### Comparing `bioversions-0.5.98/docs/_includes/footer.html` & `bioversions-0.5.99/docs/_includes/footer.html`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/docs/_includes/head.html` & `bioversions-0.5.99/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/docs/download.md` & `bioversions-0.5.99/docs/download.md`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/docs/img/has_release_url.svg` & `bioversions-0.5.99/docs/img/has_release_url.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 662d 7379 6e74 6178 2d6e 7323 223e 0a20  f-syntax-ns#">. 
 000001e0: 2020 3c63 633a 576f 726b 3e0a 2020 2020    <cc:Work>.    
 000001f0: 3c64 633a 7479 7065 2072 6466 3a72 6573  <dc:type rdf:res
 00000200: 6f75 7263 653d 2268 7474 703a 2f2f 7075  ource="http://pu
 00000210: 726c 2e6f 7267 2f64 632f 6463 6d69 7479  rl.org/dc/dcmity
 00000220: 7065 2f53 7469 6c6c 496d 6167 6522 2f3e  pe/StillImage"/>
 00000230: 0a20 2020 203c 6463 3a64 6174 653e 3230  .    <dc:date>20
-00000240: 3233 2d30 342d 3037 5430 303a 3436 3a32  23-04-07T00:46:2
-00000250: 332e 3433 3237 3230 3c2f 6463 3a64 6174  3.432720</dc:dat
+00000240: 3233 2d30 342d 3039 5430 303a 3534 3a30  23-04-09T00:54:0
+00000250: 322e 3731 3236 3339 3c2f 6463 3a64 6174  2.712639</dc:dat
 00000260: 653e 0a20 2020 203c 6463 3a66 6f72 6d61  e>.    <dc:forma
 00000270: 743e 696d 6167 652f 7376 672b 786d 6c3c  t>image/svg+xml<
 00000280: 2f64 633a 666f 726d 6174 3e0a 2020 2020  /dc:format>.    
 00000290: 3c64 633a 6372 6561 746f 723e 0a20 2020  <dc:creator>.   
 000002a0: 2020 3c63 633a 4167 656e 743e 0a20 2020    <cc:Agent>.   
 000002b0: 2020 203c 6463 3a74 6974 6c65 3e4d 6174     <dc:title>Mat
 000002c0: 706c 6f74 6c69 6220 7633 2e37 2e31 2c20  plotlib v3.7.1,
```

### Comparing `bioversions-0.5.98/docs/img/version_date_types.svg` & `bioversions-0.5.99/docs/img/version_date_types.svg`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 662d 7379 6e74 6178 2d6e 7323 223e 0a20  f-syntax-ns#">. 
 000001e0: 2020 3c63 633a 576f 726b 3e0a 2020 2020    <cc:Work>.    
 000001f0: 3c64 633a 7479 7065 2072 6466 3a72 6573  <dc:type rdf:res
 00000200: 6f75 7263 653d 2268 7474 703a 2f2f 7075  ource="http://pu
 00000210: 726c 2e6f 7267 2f64 632f 6463 6d69 7479  rl.org/dc/dcmity
 00000220: 7065 2f53 7469 6c6c 496d 6167 6522 2f3e  pe/StillImage"/>
 00000230: 0a20 2020 203c 6463 3a64 6174 653e 3230  .    <dc:date>20
-00000240: 3233 2d30 342d 3037 5430 303a 3436 3a32  23-04-07T00:46:2
-00000250: 332e 3336 3430 3631 3c2f 6463 3a64 6174  3.364061</dc:dat
+00000240: 3233 2d30 342d 3039 5430 303a 3534 3a30  23-04-09T00:54:0
+00000250: 322e 3631 3135 3531 3c2f 6463 3a64 6174  2.611551</dc:dat
 00000260: 653e 0a20 2020 203c 6463 3a66 6f72 6d61  e>.    <dc:forma
 00000270: 743e 696d 6167 652f 7376 672b 786d 6c3c  t>image/svg+xml<
 00000280: 2f64 633a 666f 726d 6174 3e0a 2020 2020  /dc:format>.    
 00000290: 3c64 633a 6372 6561 746f 723e 0a20 2020  <dc:creator>.   
 000002a0: 2020 3c63 633a 4167 656e 743e 0a20 2020    <cc:Agent>.   
 000002b0: 2020 203c 6463 3a74 6974 6c65 3e4d 6174     <dc:title>Mat
 000002c0: 706c 6f74 6c69 6220 7633 2e37 2e31 2c20  plotlib v3.7.1,
```

### Comparing `bioversions-0.5.98/docs/img/version_types.svg` & `bioversions-0.5.99/docs/img/version_types.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 662d 7379 6e74 6178 2d6e 7323 223e 0a20  f-syntax-ns#">. 
 000001e0: 2020 3c63 633a 576f 726b 3e0a 2020 2020    <cc:Work>.    
 000001f0: 3c64 633a 7479 7065 2072 6466 3a72 6573  <dc:type rdf:res
 00000200: 6f75 7263 653d 2268 7474 703a 2f2f 7075  ource="http://pu
 00000210: 726c 2e6f 7267 2f64 632f 6463 6d69 7479  rl.org/dc/dcmity
 00000220: 7065 2f53 7469 6c6c 496d 6167 6522 2f3e  pe/StillImage"/>
 00000230: 0a20 2020 203c 6463 3a64 6174 653e 3230  .    <dc:date>20
-00000240: 3233 2d30 342d 3037 5430 303a 3436 3a32  23-04-07T00:46:2
-00000250: 332e 3236 3439 3437 3c2f 6463 3a64 6174  3.264947</dc:dat
+00000240: 3233 2d30 342d 3039 5430 303a 3534 3a30  23-04-09T00:54:0
+00000250: 322e 3437 3232 3533 3c2f 6463 3a64 6174  2.472253</dc:dat
 00000260: 653e 0a20 2020 203c 6463 3a66 6f72 6d61  e>.    <dc:forma
 00000270: 743e 696d 6167 652f 7376 672b 786d 6c3c  t>image/svg+xml<
 00000280: 2f64 633a 666f 726d 6174 3e0a 2020 2020  /dc:format>.    
 00000290: 3c64 633a 6372 6561 746f 723e 0a20 2020  <dc:creator>.   
 000002a0: 2020 3c63 633a 4167 656e 743e 0a20 2020    <cc:Agent>.   
 000002b0: 2020 203c 6463 3a74 6974 6c65 3e4d 6174     <dc:title>Mat
 000002c0: 706c 6f74 6c69 6220 7633 2e37 2e31 2c20  plotlib v3.7.1,
```

### Comparing `bioversions-0.5.98/docs/index.md` & `bioversions-0.5.99/docs/index.md`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/docs/source/logo.png` & `bioversions-0.5.99/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/docs/summary.md` & `bioversions-0.5.99/docs/summary.md`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/setup.cfg` & `bioversions-0.5.99/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bioversions
-version = 0.5.98
+version = 0.5.99
 description = What's the current version for each biological database?
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/bioversions
 download_url = https://github.com/biopragmatics/bioversions/releases
 project_urls = 
 	Bug Tracker = https://github.com/biopragmatics/bioversions/issues
```

### Comparing `bioversions-0.5.98/src/bioversions/charts.py` & `bioversions-0.5.99/src/bioversions/charts.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/cli.py` & `bioversions-0.5.99/src/bioversions/cli.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/resources/__init__.py` & `bioversions-0.5.99/src/bioversions/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/resources/update.py` & `bioversions-0.5.99/src/bioversions/resources/update.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/resources/versions.json` & `bioversions-0.5.99/src/bioversions/resources/versions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166660739165136%*

 * *Differences: {"'annotations'": "{'revision': 401, 'date': '2023-04-09'}",*

 * * "'database'": "{339: {'releases': {insert: [(243, OrderedDict([('retrieved', '2023-04-09'), "*

 * *               "('version', '2023-04-09')]))]}}, 394: {'releases': {insert: [(292, "*

 * *               "OrderedDict([('retrieved', '2023-04-09'), ('version', '2023-04-07')]))]}}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "annotations": {
         "author": "runner",
-        "date": "2023-04-07",
-        "revision": 400
+        "date": "2023-04-09",
+        "revision": 401
     },
     "database": [
         {
             "name": "A nomenclatural ontology for biological names",
             "prefix": "nomen",
             "releases": [
                 {
@@ -8567,14 +8567,18 @@
                 {
                     "retrieved": "2023-04-06",
                     "version": "2023-04-06"
                 },
                 {
                     "retrieved": "2023-04-07",
                     "version": "2023-04-07"
+                },
+                {
+                    "retrieved": "2023-04-09",
+                    "version": "2023-04-09"
                 }
             ],
             "vtype": "date"
         },
         {
             "name": "SWO (The Software Ontology)",
             "prefix": "swo",
@@ -11128,14 +11132,18 @@
                 {
                     "retrieved": "2023-04-06",
                     "version": "2023-04-04"
                 },
                 {
                     "retrieved": "2023-04-07",
                     "version": "2023-04-05"
+                },
+                {
+                    "retrieved": "2023-04-09",
+                    "version": "2023-04-07"
                 }
             ],
             "vtype": "date"
         },
         {
             "name": "Zebrafish Phenotype Ontology",
             "prefix": "zp",
```

### Comparing `bioversions-0.5.98/src/bioversions/slack_client.py` & `bioversions-0.5.99/src/bioversions/slack_client.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/__init__.py` & `bioversions-0.5.99/src/bioversions/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/antibodyregistry.py` & `bioversions-0.5.99/src/bioversions/sources/antibodyregistry.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/bigg.py` & `bioversions-0.5.99/src/bioversions/sources/bigg.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/biofacquim.py` & `bioversions-0.5.99/src/bioversions/sources/biofacquim.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/biogrid.py` & `bioversions-0.5.99/src/bioversions/sources/biogrid.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/cellosaurus.py` & `bioversions-0.5.99/src/bioversions/sources/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/chebi.py` & `bioversions-0.5.99/src/bioversions/sources/chebi.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/chembl.py` & `bioversions-0.5.99/src/bioversions/sources/chembl.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/chemidplus.py` & `bioversions-0.5.99/src/bioversions/sources/chemidplus.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/complexportal.py` & `bioversions-0.5.99/src/bioversions/sources/complexportal.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/depmap.py` & `bioversions-0.5.99/src/bioversions/sources/depmap.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/dgi.py` & `bioversions-0.5.99/src/bioversions/sources/dgi.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/disgenet.py` & `bioversions-0.5.99/src/bioversions/sources/disgenet.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/drugbank.py` & `bioversions-0.5.99/src/bioversions/sources/drugbank.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/drugcentral.py` & `bioversions-0.5.99/src/bioversions/sources/drugcentral.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/ensembl.py` & `bioversions-0.5.99/src/bioversions/sources/ensembl.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/expasy.py` & `bioversions-0.5.99/src/bioversions/sources/expasy.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/flybase.py` & `bioversions-0.5.99/src/bioversions/sources/flybase.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/guidetopharmacology.py` & `bioversions-0.5.99/src/bioversions/sources/guidetopharmacology.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/hgnc.py` & `bioversions-0.5.99/src/bioversions/sources/hgnc.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/homologene.py` & `bioversions-0.5.99/src/bioversions/sources/homologene.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/intact.py` & `bioversions-0.5.99/src/bioversions/sources/intact.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/interpro.py` & `bioversions-0.5.99/src/bioversions/sources/interpro.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/itis.py` & `bioversions-0.5.99/src/bioversions/sources/itis.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/kegg.py` & `bioversions-0.5.99/src/bioversions/sources/kegg.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/mesh.py` & `bioversions-0.5.99/src/bioversions/sources/mesh.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/mirbase.py` & `bioversions-0.5.99/src/bioversions/sources/mirbase.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/moalmanac.py` & `bioversions-0.5.99/src/bioversions/sources/moalmanac.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/msigdb.py` & `bioversions-0.5.99/src/bioversions/sources/msigdb.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/ncit.py` & `bioversions-0.5.99/src/bioversions/sources/ncit.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/npass.py` & `bioversions-0.5.99/src/bioversions/sources/npass.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/obo.py` & `bioversions-0.5.99/src/bioversions/sources/obo.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/ols.py` & `bioversions-0.5.99/src/bioversions/sources/ols.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/oncotree.py` & `bioversions-0.5.99/src/bioversions/sources/oncotree.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/pathbank.py` & `bioversions-0.5.99/src/bioversions/sources/pathbank.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/pathwaycommons.py` & `bioversions-0.5.99/src/bioversions/sources/pathwaycommons.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/pfam.py` & `bioversions-0.5.99/src/bioversions/sources/pfam.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/pombase.py` & `bioversions-0.5.99/src/bioversions/sources/pombase.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/pr.py` & `bioversions-0.5.99/src/bioversions/sources/pr.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/pubchem.py` & `bioversions-0.5.99/src/bioversions/sources/pubchem.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/reactome.py` & `bioversions-0.5.99/src/bioversions/sources/reactome.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/rfam.py` & `bioversions-0.5.99/src/bioversions/sources/rfam.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/rgd.py` & `bioversions-0.5.99/src/bioversions/sources/rgd.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/rhea.py` & `bioversions-0.5.99/src/bioversions/sources/rhea.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/rxnorm.py` & `bioversions-0.5.99/src/bioversions/sources/rxnorm.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/sgd.py` & `bioversions-0.5.99/src/bioversions/sources/sgd.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/slm.py` & `bioversions-0.5.99/src/bioversions/sources/slm.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/stringdb.py` & `bioversions-0.5.99/src/bioversions/sources/stringdb.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/umls.py` & `bioversions-0.5.99/src/bioversions/sources/umls.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/uniprot.py` & `bioversions-0.5.99/src/bioversions/sources/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/wikipathways.py` & `bioversions-0.5.99/src/bioversions/sources/wikipathways.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/sources/zfin.py` & `bioversions-0.5.99/src/bioversions/sources/zfin.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/templates/base.html` & `bioversions-0.5.99/src/bioversions/templates/base.html`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/templates/home.html` & `bioversions-0.5.99/src/bioversions/templates/home.html`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/twitter_client.py` & `bioversions-0.5.99/src/bioversions/twitter_client.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/utils.py` & `bioversions-0.5.99/src/bioversions/utils.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions/version.py` & `bioversions-0.5.99/src/bioversions/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from subprocess import CalledProcessError, check_output  # noqa: S404
 
 __all__ = [
     "VERSION",
 ]
 
-VERSION = "0.5.98"
+VERSION = "0.5.99"
 
 
 def get_git_hash() -> str:
     """Get the bioversions git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `bioversions-0.5.98/src/bioversions/wsgi.py` & `bioversions-0.5.99/src/bioversions/wsgi.py`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/src/bioversions.egg-info/PKG-INFO` & `bioversions-0.5.99/src/bioversions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioversions
-Version: 0.5.98
+Version: 0.5.99
 Summary: What's the current version for each biological database?
 Home-page: https://github.com/biopragmatics/bioversions
 Download-URL: https://github.com/biopragmatics/bioversions/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioversions Version: 0.5.98 Summary: What's the
+Metadata-Version: 2.1 Name: bioversions Version: 0.5.99 Summary: What's the
 current version for each biological database? Home-page: https://github.com/
 biopragmatics/bioversions Download-URL: https://github.com/biopragmatics/
 bioversions/releases Author: Charles Tapley Hoyt Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt Maintainer-email: cthoyt@gmail.com License: MIT
 Project-URL: Bug Tracker, https://github.com/biopragmatics/bioversions/issues
 Keywords: databases,biological databases Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: License :: OSI Approved ::
```

### Comparing `bioversions-0.5.98/src/bioversions.egg-info/SOURCES.txt` & `bioversions-0.5.99/src/bioversions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioversions-0.5.98/tests/test_bioversions.py` & `bioversions-0.5.99/tests/test_bioversions.py`

 * *Files identical despite different names*

