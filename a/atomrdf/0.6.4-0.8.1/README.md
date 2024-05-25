# Comparing `tmp/atomrdf-0.6.4.tar.gz` & `tmp/atomrdf-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomrdf-0.6.4.tar", last modified: Mon Apr 29 20:45:59 2024, max compression
+gzip compressed data, was "atomrdf-0.8.1.tar", last modified: Sat May 25 20:57:35 2024, max compression
```

## Comparing `atomrdf-0.6.4.tar` & `atomrdf-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.375579 atomrdf-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 20:45:56.000000 atomrdf-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 20:45:56.000000 atomrdf-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 20:45:59.375579 atomrdf-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-29 20:45:56.000000 atomrdf-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.367579 atomrdf-0.6.4/atomrdf/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.371579 atomrdf-0.6.4/atomrdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52930 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/dft_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/md_template.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/data/podo.owl
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    38763 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/json_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.371579 atomrdf-0.6.4/atomrdf/network/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/network/term.py
--rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    59158 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.371579 atomrdf-0.6.4/atomrdf/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/workflow/pyiron.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-04-29 20:45:56.000000 atomrdf-0.6.4/atomrdf/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.375579 atomrdf-0.6.4/atomrdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 20:45:59.000000 atomrdf-0.6.4/atomrdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:45:59.375579 atomrdf-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-29 20:45:59.000000 atomrdf-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:45:59.375579 atomrdf-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_structuregraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_term.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_visualise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-29 20:45:56.000000 atomrdf-0.6.4/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.349317 atomrdf-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-25 20:57:32.000000 atomrdf-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-25 20:57:32.000000 atomrdf-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-25 20:57:35.349317 atomrdf-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-25 20:57:32.000000 atomrdf-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.341317 atomrdf-0.8.1/atomrdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.345317 atomrdf-0.8.1/atomrdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    72592 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    74534 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/dft_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/md_template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    35493 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52331 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/json_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.345317 atomrdf-0.8.1/atomrdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73462 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.345317 atomrdf-0.8.1/atomrdf/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.345317 atomrdf-0.8.1/atomrdf/workflow/pyiron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/pyiron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/pyiron/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/pyiron/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/pyiron/pyiron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/pyiron/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-05-25 20:57:32.000000 atomrdf-0.8.1/atomrdf/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.349317 atomrdf-0.8.1/atomrdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-25 20:57:35.000000 atomrdf-0.8.1/atomrdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-25 20:57:35.000000 atomrdf-0.8.1/atomrdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:57:35.000000 atomrdf-0.8.1/atomrdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:57:35.000000 atomrdf-0.8.1/atomrdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-25 20:57:35.000000 atomrdf-0.8.1/atomrdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 20:57:35.000000 atomrdf-0.8.1/atomrdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:57:35.349317 atomrdf-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-25 20:57:35.000000 atomrdf-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:57:35.349317 atomrdf-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_structuregraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-25 20:57:33.000000 atomrdf-0.8.1/tests/test_workflow.py
```

### Comparing `atomrdf-0.6.4/LICENSE` & `atomrdf-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/PKG-INFO` & `atomrdf-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.6.4
+Version: 0.8.1
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -15,14 +15,16 @@
 Requires-Dist: pyyaml
 Requires-Dist: graphviz
 Requires-Dist: networkx
 Requires-Dist: pyscal3
 Requires-Dist: spglib
 Requires-Dist: pandas
 Requires-Dist: owlready2
+Requires-Dist: atomman
+Requires-Dist: mp-api
 
 # atomRDF
 
 > [!NOTE]
 > `atomRDF` was previously called `pyscal-rdf`. 
 
 [![codecov](https://codecov.io/gh/pyscal/atomRDF/graph/badge.svg?token=X7S3TP2MP6)](https://codecov.io/gh/pyscal/atomRDF)
```

### Comparing `atomrdf-0.6.4/README.md` & `atomrdf-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/data/asmo.owl` & `atomrdf-0.8.1/atomrdf/data/asmo.owl`

 * *Files 17% similar despite different names*

#### Comparing `atomrdf-0.6.4/atomrdf/data/asmo.owl` & `atomrdf-0.8.1/atomrdf/data/asmo.owl`

```diff
@@ -1,23 +1,82 @@
 <?xml version="1.0" encoding="utf-8"?>
-<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/asmo/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:prov="http://www.w3.org/ns/prov#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/asmo/">
+<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/asmo/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:obo="http://purl.obolibrary.org/obo/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:prov="http://www.w3.org/ns/prov#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/asmo/">
   <owl:Ontology rdf:about="http://purls.helmholtz-metadaten.de/asmo/">
     <terms:contributor>https://orcid.org/0000-0002-6776-1213</terms:contributor>
     <terms:creator>https://orcid.org/0000-0001-7564-7990</terms:creator>
     <terms:description>ASMO is an ontology that aims to define the concepts needed to describe commonly used atomic scale simulation methods, i.e. density functional theory, molecular dynamics, Monte Carlo methods, etc. ASMO uses the Provenance Ontology (PROV-O) to describe the simulation process.</terms:description>
     <terms:title>Atomistic Simulation Methods Ontology (ASMO)</terms:title>
     <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">0.0.1</owl:versionInfo>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotation properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
+  <!-- http://purl.obolibrary.org/obo/IAO_0000111 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000111"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000112 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000112"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000114 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000114"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000115 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000115">
+    <obo:IAO_0000111 xml:lang="en">definition</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">The official definition, explaining the meaning of a class or property. Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions.</obo:IAO_0000115>
+    <obo:IAO_0000116 xml:lang="en">2012-04-05: 
+Barry Smith
+
+The official OBI definition, explaining the meaning of a class or property: 'Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions'  is terrible.
+
+Can you fix to something like:
+
+A statement of necessary and sufficient conditions explaining the meaning of an expression referring to a class or property.
+
+Alan Ruttenberg
+
+Your proposed definition is a reasonable candidate, except that it is very common that necessary and sufficient conditions are not given. Mostly they are necessary, occasionally they are necessary and sufficient or just sufficient. Often they use terms that are not themselves defined and so they effectively can't be evaluated by those criteria. 
+
+On the specifics of the proposed definition:
+
+We don't have definitions of 'meaning' or 'expression' or 'property'. For 'reference' in the intended sense I think we use the term 'denotation'. For 'expression', I think we you mean symbol, or identifier. For 'meaning' it differs for class and property. For class we want documentation that let's the intended reader determine whether an entity is instance of the class, or not. For property we want documentation that let's the intended reader determine, given a pair of potential relata, whether the assertion that the relation holds is true. The 'intended reader' part suggests that we also specify who, we expect, would be able to understand the definition, and also generalizes over human and computer reader to include textual and logical definition. 
+
+Personally, I am more comfortable weakening definition to documentation, with instructions as to what is desirable. 
+
+We also have the outstanding issue of how to aim different definitions to different audiences. A clinical audience reading chebi wants a different sort of definition documentation/definition from a chemistry trained audience, and similarly there is a need for a definition that is adequate for an ontologist to work with.</obo:IAO_0000116>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:isDefinedBy rdf:resource="http://purl.obolibrary.org/obo/iao.owl"/>
+    <rdfs:label xml:lang="en">definition</rdfs:label>
+  </owl:AnnotationProperty>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000116 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000116"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000117 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000117"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000119 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000119">
+    <obo:IAO_0000111 xml:lang="en">definition source</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">Formal citation, e.g. identifier in external database to indicate / attribute source(s) for the definition. Free text indicate / attribute source(s) for the definition. EXAMPLE: Author Name, URI, MeSH Term C04, PUBMED ID, Wiki uri on 31.01.2007</obo:IAO_0000115>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">Discussion on obo-discuss mailing-list, see http://bit.ly/hgm99w</obo:IAO_0000119>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:isDefinedBy rdf:resource="http://purl.obolibrary.org/obo/iao.owl"/>
+    <rdfs:label xml:lang="en">definition source</rdfs:label>
+  </owl:AnnotationProperty>
+  <!-- http://purl.obolibrary.org/obo/OBCS_0000221 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/OBCS_0000221">
+    <obo:IAO_0000112>A normal distribution probability density function has a formula of:
+f(x) = 1/(√(2 π) σ) e^-((x - μ)^2/(2 σ^2))</obo:IAO_0000112>
+    <obo:IAO_0000115>An annotation property that represents a mathematical formula.</obo:IAO_0000115>
+    <obo:IAO_0000117>Asiyah Yu Lin, Jie Zheng, Yongqun He</obo:IAO_0000117>
+    <rdfs:label xml:lang="en">mathematical formula</rdfs:label>
+  </owl:AnnotationProperty>
   <!-- http://purl.org/dc/elements/1.1/contributor -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/contributor"/>
   <!-- http://purl.org/dc/elements/1.1/creator -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/creator"/>
   <!-- http://purl.org/dc/elements/1.1/description -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/description"/>
   <!-- http://purl.org/dc/elements/1.1/title -->
@@ -127,58 +186,57 @@
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasComputationalMethod -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasComputationalMethod">
     <rdfs:domain rdf:resource="http://www.w3.org/ns/prov#Activity"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an activity and the type of computation method employed.</obo:IAO_0000115>
     <rdfs:label>has computational method</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasInputParameter -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasInputParameter">
-    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StructureOptimization"/>
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/asmo/EnergyCalculation"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InputParameter"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an Energy Calculation activity and the input parameters used.</obo:IAO_0000115>
     <rdfs:label>has input parameter</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasInteratomicPotential -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasInteratomicPotential">
-    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/asmo/MolecularDynamics"/>
+    <rdfs:domain rdf:resource="http://www.w3.org/ns/prov#Activity"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an activity and the interatomic potential used.</obo:IAO_0000115>
     <rdfs:label>has interatomic potential</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasRelaxationDOF -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasRelaxationDOF">
-    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StructureOptimization"/>
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/asmo/EnergyCalculation"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/asmo/RelaxationDOF"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an Energy Calculation activity and the relaxation degrees of freedom set as constraints in the calculation.</obo:IAO_0000115>
     <rdfs:label>has relaxation DOF</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasStatisticalEnsemble -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasStatisticalEnsemble">
-    <rdfs:domain>
-      <owl:Class>
-        <owl:unionOf rdf:parseType="Collection">
-          <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/asmo/AbInitioMolecularDynamics"/>
-          <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/asmo/MolecularDynamics"/>
-          <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/asmo/MonteCarloMethod"/>
-        </owl:unionOf>
-      </owl:Class>
-    </rdfs:domain>
+    <rdfs:domain rdf:resource="http://www.w3.org/ns/prov#Activity"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an activity and the statistical ensemble set in the simulation.</obo:IAO_0000115>
     <rdfs:label>has statistical ensemble</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasUnit -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasUnit">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InputParameter"/>
     <rdfs:range rdf:resource="http://qudt.org/schema/qudt/Unit"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between the input parameter set and the unit of the quantity. (e.g. eV for energy cutoff)</obo:IAO_0000115>
     <rdfs:label>has unit</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/asmo/wasCalculatedBy -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/wasCalculatedBy">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty"/>
     <rdfs:range rdf:resource="http://www.w3.org/ns/prov#Activity"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a calculated property and the activity through which it was obtained.</obo:IAO_0000115>
     <rdfs:label>was calculated by</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://www.w3.org/ns/prov#actedOnBehalfOf -->
   <owl:ObjectProperty rdf:about="http://www.w3.org/ns/prov#actedOnBehalfOf">
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/ns/prov#wasInfluencedBy"/>
     <rdfs:domain rdf:resource="http://www.w3.org/ns/prov#Agent"/>
     <rdfs:range rdf:resource="http://www.w3.org/ns/prov#Agent"/>
@@ -333,40 +391,40 @@
     <prov:inverse>influenced</prov:inverse>
     <prov:qualifiedForm rdf:resource="http://www.w3.org/ns/prov#Influence"/>
     <prov:qualifiedForm rdf:resource="http://www.w3.org/ns/prov#qualifiedInfluence"/>
     <prov:sharesDefinitionWith rdf:resource="http://www.w3.org/ns/prov#Influence"/>
   </owl:ObjectProperty>
   <owl:Axiom>
     <owl:annotatedSource rdf:resource="http://www.w3.org/ns/prov#wasInfluencedBy"/>
-    <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#domain"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#range"/>
     <owl:annotatedTarget>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://www.w3.org/ns/prov#Activity"/>
           <rdf:Description rdf:about="http://www.w3.org/ns/prov#Agent"/>
           <rdf:Description rdf:about="http://www.w3.org/ns/prov#Entity"/>
         </owl:unionOf>
       </owl:Class>
     </owl:annotatedTarget>
-    <prov:definition>influencee: an identifier (o2) for an entity, activity, or agent;</prov:definition>
+    <prov:definition>influencer: an identifier (o1) for an ancestor entity, activity, or agent that the former depends on;</prov:definition>
     <prov:dm>http://www.w3.org/TR/2013/REC-prov-dm-20130430/#term-influence</prov:dm>
   </owl:Axiom>
   <owl:Axiom>
     <owl:annotatedSource rdf:resource="http://www.w3.org/ns/prov#wasInfluencedBy"/>
-    <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#range"/>
+    <owl:annotatedProperty rdf:resource="http://www.w3.org/2000/01/rdf-schema#domain"/>
     <owl:annotatedTarget>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://www.w3.org/ns/prov#Activity"/>
           <rdf:Description rdf:about="http://www.w3.org/ns/prov#Agent"/>
           <rdf:Description rdf:about="http://www.w3.org/ns/prov#Entity"/>
         </owl:unionOf>
       </owl:Class>
     </owl:annotatedTarget>
-    <prov:definition>influencer: an identifier (o1) for an ancestor entity, activity, or agent that the former depends on;</prov:definition>
+    <prov:definition>influencee: an identifier (o2) for an entity, activity, or agent;</prov:definition>
     <prov:dm>http://www.w3.org/TR/2013/REC-prov-dm-20130430/#term-influence</prov:dm>
   </owl:Axiom>
   <!-- http://www.w3.org/ns/prov#wasInformedBy -->
   <owl:ObjectProperty rdf:about="http://www.w3.org/ns/prov#wasInformedBy">
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/ns/prov#wasInfluencedBy"/>
     <rdfs:domain rdf:resource="http://www.w3.org/ns/prov#Activity"/>
     <rdfs:range rdf:resource="http://www.w3.org/ns/prov#Activity"/>
@@ -392,14 +450,15 @@
     //
     // Data properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/asmo/hasValue -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/asmo/hasValue">
+    <obo:IAO_0000115>A data property linking an input parameter with the value set.</obo:IAO_0000115>
     <rdfs:label>has value</rdfs:label>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasReference -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasReference">
     <rdfs:domain rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
     <rdfs:range rdf:resource="http://www.w3.org/2000/01/rdf-schema#Literal"/>
     <rdfs:label>has reference</rdfs:label>
@@ -437,89 +496,150 @@
     // Classes
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/asmo/AbInitioMolecularDynamics -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/AbInitioMolecularDynamics">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Ab Initio Molecular Dynamics is a computational method where finite-temperature dynamical trajectories are generated by using forces obtained directly from electronic structure calculations performed ‘‘on the fly’’ as the simulation proceeds.</obo:IAO_0000115>
     <rdfs:label>Ab Initio Molecular Dynamics</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">AIMD</skos:altLabel>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Ab initio MD</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Computational method is a method used to numerically solve mathematical models and study the behaviour of physical systems.</obo:IAO_0000115>
     <rdfs:label>Computational Method</rdfs:label>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/DensityFunctionalTheory -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/DensityFunctionalTheory">
     <owl:equivalentClass rdf:resource="https://w3id.org/mdo/calculation/DensityFunctionalTheoryMethod"/>
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Density functional theory is a computational method used to study the electronic structure and ground state of atoms, molecules, and, solids. This technique determines the properties of a many-electron system thorugh functionals of the spatially dependent electron density.</obo:IAO_0000115>
     <rdfs:label>Density Functional Theory</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">DFT</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/EmbeddedAtomModel -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/EmbeddedAtomModel">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Embedded Atom Model is an many-body interatomic potential which contains two contributions to the potential energy: the embedding term, which describes the energy required to embed an atom into an electron cloud, and the pair-wise interaction.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1103/PhysRevLett.50.1285</obo:IAO_0000119>
+    <obo:OBCS_0000221 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">E(r) = \sum_i F_i (\rho_i(r_i)) + 1/2 \sum_{i,j} \varphi(r_{i,j})</obo:OBCS_0000221>
     <rdfs:label>Embedded Atom Model</rdfs:label>
     <skos:altLabel>EAM</skos:altLabel>
   </owl:Class>
+  <!-- http://purls.helmholtz-metadaten.de/asmo/EnergyCalculation -->
+  <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/EnergyCalculation">
+    <rdfs:subClassOf rdf:resource="http://www.w3.org/ns/prov#Activity"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Energy calculation is an activity where the energy of the system is computed within the given optimization constraints.</obo:IAO_0000115>
+    <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">This activity does not specify the way the energy is calculated, it can be used to refer to a rigid calculation or also to energy minimization or optimization. See RelaxationDOF class for specifics about the constraints.</rdfs:comment>
+    <rdfs:label>Energy Calculation</rdfs:label>
+  </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/EnergyDifferenceCalculation -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/EnergyDifferenceCalculation">
     <rdfs:subClassOf rdf:resource="http://www.w3.org/ns/prov#Activity"/>
     <rdfs:label>Energy Difference Calculation</rdfs:label>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/InputParameter -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/InputParameter">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Input Parameter are the parameters provided as input to the software tool performing the numerical calculations.</obo:IAO_0000115>
     <rdfs:label>Input Parameter</rdfs:label>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Interatomic potentials, in the context of computer simulations, are mathematical functions to calculate the potential energy of a system of atoms with given positions in space.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://en.wikipedia.org/wiki/Interatomic_potential</obo:IAO_0000119>
     <rdfs:label>Interatomic Potential</rdfs:label>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/KineticMonteCarloMethod -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/KineticMonteCarloMethod">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/MonteCarloMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Kinetic Monte Carlo Method is a variation of the Monte Carlo method, intended to simulate the time evolution of a process with known transition rates among states.</obo:IAO_0000115>
     <rdfs:label>Kinetic Monte Carlo Method</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">kMC</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/Lennard-JonesPotential -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/Lennard-JonesPotential">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Lennard-Jones Potential is a general two-body interatomic potential, which separates the interaction between atoms into a repulsive part, r^(–n), and attractive part, r^(–m), with (n &gt; m).</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1021/acs.jctc.4c00135</obo:IAO_0000119>
+    <obo:OBCS_0000221 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">E(r) = 4\epsilon[(\sigma/r)^{12}-(\sigma/r)^{6}]</obo:OBCS_0000221>
     <rdfs:label>Lennard-Jones Potential</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">12-6 potential</skos:altLabel>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">LJ potential</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/MachineLearningPotential -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/MachineLearningPotential">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Machine Learning Potential is an interatomic potential which maps the 3N-dimensional configurational space of the system onto its potential energy surface, represented by a discrete set of DFT energies included in the training dataset.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1016/j.actamat.2021.116980</obo:IAO_0000119>
+    <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Some of the most commonly used MLIP are: Atomic Cluster Expansion (ACE), Moment Tensor Potential (MTP) and Neural Network Potential (NNP)</rdfs:comment>
     <rdfs:label>Machine Learning Potential</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">MLIP</skos:altLabel>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">MLP</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/ModifiedEmbeddedAtomModel -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/ModifiedEmbeddedAtomModel">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Modified Embedded Atom Model is an interatomic potential which extends EAM to include angular forces.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1103/PhysRevB.46.2727</obo:IAO_0000119>
     <rdfs:label>Modified Embedded Atom Model</rdfs:label>
     <skos:altLabel>MEAM</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/MolecularDynamics -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/MolecularDynamics">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Molecular dynamics is a computational method for simulation of complex systems, modelled at the atomic level. The equations of motion are solved numerically to follow the time evolution of the system, allowing the derivation of kinetic and thermodynamic properties of interest by means of ‘computer experiments’.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1038/npg.els.0003048</obo:IAO_0000119>
     <rdfs:label>Molecular Dynamics</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">MD</skos:altLabel>
+  </owl:Class>
+  <!-- http://purls.helmholtz-metadaten.de/asmo/MolecularForceField -->
+  <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/MolecularForceField">
+    <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Molecular force field is a type of interatomic potential that contains the functional forms used to describe the intra- and inter-molecular potential energy of a collection of atoms, and the corresponding parameters that will determine the energy of a given configuration.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 9780192524706</obo:IAO_0000119>
+    <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Force Field</rdfs:label>
+    <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Molecular Force Field</rdfs:label>
+  </owl:Class>
+  <!-- http://purls.helmholtz-metadaten.de/asmo/MolecularStatics -->
+  <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/MolecularStatics">
+    <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Molecular statics is a computational method that uses a constrained optimization technique to minimize the energy of the system at the atomic level. It is usually employed within a Molecular Dynamics framework.</obo:IAO_0000115>
+    <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Molecular Statics</rdfs:label>
+    <rdfs:seeAlso rdf:resource="http://purls.helmholtz-metadaten.de/asmo/MolecularDynamics"/>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">MS</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/MonteCarloMethod -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/MonteCarloMethod">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/ComputationalMethod"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Monte Carlo Method is a computational method that models the probability of different outcomes. The system is evolved to a new state which is chosen from a randomly generated ensemble of possible future states. Then, using some criteria, this new state is accepted or rejected with a certain probability.</obo:IAO_0000115>
     <rdfs:label>Monte Carlo Method</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">MC</skos:altLabel>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Monte Carlo Simulation</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/RelaxationDOF -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/RelaxationDOF">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Relaxation Degrees of Freedom are the degrees of freedom allowed for the relaxation of the simulation cell in an atomistic simulation.</obo:IAO_0000115>
+    <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The instances of this class indicate the type of relaxation allowed, i.e. relaxation of the atomic positions, cell volume and cell shape.</rdfs:comment>
     <rdfs:label>Relaxation Degrees of Freedom</rdfs:label>
     <skos:altLabel>RelaxationDOF</skos:altLabel>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Statistical Ensemble is a collection of points in phase space. The points are distributed according to a probability density, which is determined by the chosen fixed macroscopic parameters (NPT, NVT, etc.). Each point represents a typical system at any particular instant of time.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 9780192524706</obo:IAO_0000119>
     <rdfs:label>Statistical Ensemble</rdfs:label>
   </owl:Class>
-  <!-- http://purls.helmholtz-metadaten.de/asmo/StructureOptimization -->
-  <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/StructureOptimization">
-    <rdfs:subClassOf rdf:resource="http://www.w3.org/ns/prov#Activity"/>
-    <rdfs:label>Structure Optimization</rdfs:label>
+  <!-- http://purls.helmholtz-metadaten.de/asmo/StillingerWeberPotential -->
+  <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/asmo/StillingerWeberPotential">
+    <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/asmo/InteratomicPotential"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Stillinger-Weber Potential is an interatomic potential comprising both two- and three-atom contributions to describe interactions in solid and liquid forms of Si (and other diamond structures).</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://doi.org/10.1103/PhysRevB.31.5262</obo:IAO_0000119>
+    <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Stillinger-Weber Potential</rdfs:label>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty">
     <rdfs:label>Calculated Property</rdfs:label>
     <skos:definition>A calculated property is a property of a material resulting from a calculation or simulation.</skos:definition>
   </owl:Class>
   <!-- http://qudt.org/schema/qudt/Unit -->
@@ -657,49 +777,67 @@
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Individuals
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
-  <!-- http://purls.helmholtz-metadaten.de/asmo/AtomicPosition -->
-  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/AtomicPosition">
+  <!-- http://purls.helmholtz-metadaten.de/asmo/AtomicPositionRelaxation -->
+  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/AtomicPositionRelaxation">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/RelaxationDOF"/>
-    <rdfs:label>Atomic Position</rdfs:label>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Atomic positions are allowed to change in the calculation.</obo:IAO_0000115>
+    <rdfs:label>Atomic Position Relaxation</rdfs:label>
   </owl:NamedIndividual>
   <!-- http://purls.helmholtz-metadaten.de/asmo/CanonicalEnsemble -->
   <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/CanonicalEnsemble">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">In the canonical ensemble the temperature, volume, and the number of particles of every species are kept constant.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 978-0323902922</obo:IAO_0000119>
     <rdfs:label>Canonical Ensemble</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">NVT ensemble</skos:altLabel>
   </owl:NamedIndividual>
-  <!-- http://purls.helmholtz-metadaten.de/asmo/CellShape -->
-  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/CellShape">
+  <!-- http://purls.helmholtz-metadaten.de/asmo/CellShapeRelaxation -->
+  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/CellShapeRelaxation">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/RelaxationDOF"/>
-    <rdfs:label>Cell Shape</rdfs:label>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Cell shape is allowed to change in the calculation.</obo:IAO_0000115>
+    <rdfs:label>Cell Shape Relaxation</rdfs:label>
   </owl:NamedIndividual>
-  <!-- http://purls.helmholtz-metadaten.de/asmo/CellVolume -->
-  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/CellVolume">
+  <!-- http://purls.helmholtz-metadaten.de/asmo/CellVolumeRelaxation -->
+  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/CellVolumeRelaxation">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/RelaxationDOF"/>
-    <rdfs:label>Cell Volume</rdfs:label>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Cell volume is allowed to change in the calculation.</obo:IAO_0000115>
+    <rdfs:label>Cell Volume Relaxation</rdfs:label>
   </owl:NamedIndividual>
   <!-- http://purls.helmholtz-metadaten.de/asmo/GrandCanonicalEnsemble -->
   <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/GrandCanonicalEnsemble">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">In the grand canonical ensemble the temperature, volume, and the chemical potential are kept constant.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 978-0323902922</obo:IAO_0000119>
     <rdfs:label>Grand Canonical Ensemble</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">µVT ensemble</skos:altLabel>
   </owl:NamedIndividual>
-  <!-- http://purls.helmholtz-metadaten.de/asmo/MicrocanonicalEnsemble -->
-  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/MicrocanonicalEnsemble">
+  <!-- http://purls.helmholtz-metadaten.de/asmo/IsoenthalpicIsobaricEnsemble -->
+  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/IsoenthalpicIsobaricEnsemble">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble"/>
-    <rdfs:label>Microcanonical Ensemble</rdfs:label>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">In the isoenthalpic-isobaric ensemble the enthalpy, pressure, and the number of particles of every species are kept constant.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 978-0323902922</obo:IAO_0000119>
+    <rdfs:label>Isoenthalpic–Isobaric Ensemble</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">NPH ensemble</skos:altLabel>
   </owl:NamedIndividual>
-  <!-- http://purls.helmholtz-metadaten.de/asmo/Isoenthalpic–isobaricEnsemble -->
-  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/Isoenthalpic–isobaricEnsemble">
+  <!-- http://purls.helmholtz-metadaten.de/asmo/IsothermalIsobaricEnsemble -->
+  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/IsothermalIsobaricEnsemble">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble"/>
-    <rdfs:label>Isoenthalpic–Isobaric Ensemble</rdfs:label>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">In the isothermal-isobaric ensemble the temperature, pressure, and the number of particles of every species are kept constant.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 978-0323902922</obo:IAO_0000119>
+    <rdfs:label>Isothermal–Isobaric Ensemble</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">NPT ensemble</skos:altLabel>
   </owl:NamedIndividual>
-  <!-- http://purls.helmholtz-metadaten.de/asmo/Isothermal–isobaricEnsemble -->
-  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/Isothermal–isobaricEnsemble">
+  <!-- http://purls.helmholtz-metadaten.de/asmo/MicrocanonicalEnsemble -->
+  <owl:NamedIndividual rdf:about="http://purls.helmholtz-metadaten.de/asmo/MicrocanonicalEnsemble">
     <rdf:type rdf:resource="http://purls.helmholtz-metadaten.de/asmo/StatisticalEnsemble"/>
-    <rdfs:label>Isothermal–isobaric Ensemble</rdfs:label>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">In the microcanonical ensemble the energy, volume, and the number of particles of every species are kept constant.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN-13: 978-0323902922</obo:IAO_0000119>
+    <rdfs:label>Microcanonical Ensemble</rdfs:label>
+    <skos:altLabel rdf:datatype="http://www.w3.org/2001/XMLSchema#string">NVE ensemble</skos:altLabel>
   </owl:NamedIndividual>
 </rdf:RDF>
 <!-- Generated by the OWL API (version 4.5.9.2019-02-01T07:24:44Z) https://github.com/owlcs/owlapi -->
```

### Comparing `atomrdf-0.6.4/atomrdf/data/cmso.owl` & `atomrdf-0.8.1/atomrdf/data/cmso.owl`

 * *Files 27% similar despite different names*

#### Comparing `atomrdf-0.6.4/atomrdf/data/cmso.owl` & `atomrdf-0.8.1/atomrdf/data/cmso.owl`

```diff
@@ -1,25 +1,73 @@
 <?xml version="1.0" encoding="utf-8"?>
-<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/cmso/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/cmso/">
+<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/cmso/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:obo="http://purl.obolibrary.org/obo/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/cmso/">
   <owl:Ontology rdf:about="http://purls.helmholtz-metadaten.de/cmso/">
     <terms:contributor>https://orcid.org/0000-0001-9560-4728</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0002-5149-603X</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0002-6776-1213</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0003-0698-4891</terms:contributor>
     <terms:creator>https://orcid.org/0000-0001-7564-7990</terms:creator>
     <terms:description>CMSO is an ontology that aims to describe computational materials science samples (or structures), including crystalline defects.</terms:description>
     <terms:title>Computational Material Sample Ontology (CMSO)</terms:title>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">0.0.1</owl:versionInfo>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotation properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
+  <!-- http://purl.obolibrary.org/obo/IAO_0000111 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000111"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000114 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000114"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000115 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000115">
+    <obo:IAO_0000111 xml:lang="en">definition</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">The official definition, explaining the meaning of a class or property. Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions.</obo:IAO_0000115>
+    <obo:IAO_0000116 xml:lang="en">2012-04-05: 
+Barry Smith
+
+The official OBI definition, explaining the meaning of a class or property: 'Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions'  is terrible.
+
+Can you fix to something like:
+
+A statement of necessary and sufficient conditions explaining the meaning of an expression referring to a class or property.
+
+Alan Ruttenberg
+
+Your proposed definition is a reasonable candidate, except that it is very common that necessary and sufficient conditions are not given. Mostly they are necessary, occasionally they are necessary and sufficient or just sufficient. Often they use terms that are not themselves defined and so they effectively can't be evaluated by those criteria. 
+
+On the specifics of the proposed definition:
+
+We don't have definitions of 'meaning' or 'expression' or 'property'. For 'reference' in the intended sense I think we use the term 'denotation'. For 'expression', I think we you mean symbol, or identifier. For 'meaning' it differs for class and property. For class we want documentation that let's the intended reader determine whether an entity is instance of the class, or not. For property we want documentation that let's the intended reader determine, given a pair of potential relata, whether the assertion that the relation holds is true. The 'intended reader' part suggests that we also specify who, we expect, would be able to understand the definition, and also generalizes over human and computer reader to include textual and logical definition. 
+
+Personally, I am more comfortable weakening definition to documentation, with instructions as to what is desirable. 
+
+We also have the outstanding issue of how to aim different definitions to different audiences. A clinical audience reading chebi wants a different sort of definition documentation/definition from a chemistry trained audience, and similarly there is a need for a definition that is adequate for an ontologist to work with.</obo:IAO_0000116>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:label xml:lang="en">definition</rdfs:label>
+  </owl:AnnotationProperty>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000116 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000116"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000117 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000117"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000119 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000119">
+    <obo:IAO_0000111 xml:lang="en">definition source</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">Formal citation, e.g. identifier in external database to indicate / attribute source(s) for the definition. Free text indicate / attribute source(s) for the definition. EXAMPLE: Author Name, URI, MeSH Term C04, PUBMED ID, Wiki uri on 31.01.2007</obo:IAO_0000115>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">Discussion on obo-discuss mailing-list, see http://bit.ly/hgm99w</obo:IAO_0000119>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:label xml:lang="en">definition source</rdfs:label>
+  </owl:AnnotationProperty>
   <!-- http://purl.org/dc/elements/1.1/contributor -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/contributor"/>
   <!-- http://purl.org/dc/elements/1.1/creator -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/creator"/>
   <!-- http://purl.org/dc/elements/1.1/description -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/description"/>
   <!-- http://purl.org/dc/elements/1.1/title -->
@@ -74,17 +122,14 @@
     <rdfs:label xml:lang="en">alternative label</rdfs:label>
     <skos:definition xml:lang="en">An alternative lexical label for a resource.</skos:definition>
     <skos:example xml:lang="en">Acronyms, abbreviations, spelling variants, and irregular plural/singular forms may be included among the alternative labels for a concept. Mis-spelled terms are normally included as hidden labels (see skos:hiddenLabel).</skos:example>
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2000/01/rdf-schema#label"/>
   </owl:AnnotationProperty>
   <!-- http://www.w3.org/2004/02/skos/core#definition -->
   <owl:AnnotationProperty rdf:about="http://www.w3.org/2004/02/skos/core#definition">
-    <rdfs:isDefinedBy rdf:resource="http://www.w3.org/2004/02/skos/core"/>
-    <rdfs:label xml:lang="en">definition</rdfs:label>
-    <skos:definition xml:lang="en">A statement or formal explanation of the meaning of a concept.</skos:definition>
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2004/02/skos/core#note"/>
   </owl:AnnotationProperty>
   <!-- http://www.w3.org/2004/02/skos/core#example -->
   <owl:AnnotationProperty rdf:about="http://www.w3.org/2004/02/skos/core#example">
     <rdfs:isDefinedBy rdf:resource="http://www.w3.org/2004/02/skos/core"/>
     <rdfs:label xml:lang="en">example</rdfs:label>
     <skos:definition xml:lang="en">An example of the use of a concept.</skos:definition>
@@ -128,96 +173,103 @@
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:domain>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a simulation or unit cell and its angle.</obo:IAO_0000115>
     <rdfs:label>has angle</rdfs:label>
-    <skos:definition>The relation between a simulation or unit cell and its angle.</skos:definition>
+  </owl:ObjectProperty>
+  <!-- http://purls.helmholtz-metadaten.de/cmso/hasAttribute -->
+  <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasAttribute">
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomicScaleSample"/>
+    <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a sample and a type of atom attribute, which refers to a per atom quantity of the atomic scale sample.</obo:IAO_0000115>
+    <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">has attribute</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasBasis -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasBasis">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Basis"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a unit cell and the basis of the crystal structure.</obo:IAO_0000115>
     <rdfs:label>has basis</rdfs:label>
-    <skos:definition>The relation between a unit cell and the basis of the crystal structure.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasCalculatedProperty -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasCalculatedProperty">
     <owl:inverseOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/isCalculatedPropertyOf"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a computational sample and the calculated property.</obo:IAO_0000115>
     <rdfs:label>has calculated property</rdfs:label>
-    <skos:definition>The relation between a computational sample and the calculated property.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasDefect -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasDefect">
     <owl:inverseOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/isDefectOf"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CrystallineMaterial"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CrystalDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between  a crystalline material and the crystal defects it contains.</obo:IAO_0000115>
     <rdfs:label>has defect</rdfs:label>
-    <skos:definition>The relation between  a crystalline material and the crystal defects it contains.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasElement -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasElement">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalSpecies"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalElement"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an atom and its chemical element.</obo:IAO_0000115>
     <rdfs:label>has element</rdfs:label>
-    <skos:definition>The relation between an atom and its chemical element.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasLatticeParameter -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasLatticeParameter">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/LatticeParameter"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a unit cell and its lattice parameters.</obo:IAO_0000115>
     <rdfs:label>has lattice parameter</rdfs:label>
-    <skos:definition>The relation between a unit cell and its lattice parameters.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasLength -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasLength">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Length"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a simulation cell and its length.</obo:IAO_0000115>
     <rdfs:label>has length</rdfs:label>
-    <skos:definition>The relation between a simulation cell and its length.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasMaterial -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasMaterial">
     <owl:inverseOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/isMaterialOf"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Material"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a computational sample and the material it represents.</obo:IAO_0000115>
     <rdfs:label>has material</rdfs:label>
-    <skos:definition>The relation between a computational sample and the material it represents.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasSimulationCell -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasSimulationCell">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomicScaleSample"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between an atomic scale sample and the simulation cell.</obo:IAO_0000115>
     <rdfs:label>has simulation cell</rdfs:label>
-    <skos:definition>The relation between an atomic scale sample and the simulation cell.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasSpaceGroup -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasSpaceGroup">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CrystalStructure"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SpaceGroup"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a crystal structure and the space group that describes the symmetry.</obo:IAO_0000115>
     <rdfs:label>has space group</rdfs:label>
-    <skos:definition>The relation between a crystal structure and the space group that describes the symmetry.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasSpecies -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasSpecies">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalSpecies"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a computational sample and the species that constitutes it.</obo:IAO_0000115>
     <rdfs:label>has species</rdfs:label>
-    <skos:definition>The relation between a computational sample and the species that constitutes it.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasStructure -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasStructure">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Material"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Structure"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a material and its structure.</obo:IAO_0000115>
     <rdfs:label>has structure</rdfs:label>
-    <skos:definition>The relation between a material and its structure.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasUnit -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasUnit">
     <rdfs:domain>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
@@ -225,37 +277,37 @@
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Length"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:domain>
     <rdfs:range rdf:resource="http://qudt.org/schema/qudt/Unit"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A relation indicating the unit.</obo:IAO_0000115>
     <rdfs:label>has unit</rdfs:label>
-    <skos:definition>A relation indicating the unit.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasUnitCell -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasUnitCell">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CrystalStructure"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a crystal structure and its unit cell.</obo:IAO_0000115>
     <rdfs:label>has unit cell</rdfs:label>
-    <skos:definition>The relation between a crystal structure and its unit cell.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasVector -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasVector">
     <rdfs:domain>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:domain>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a simulation or unit cell and its vectors.</obo:IAO_0000115>
     <rdfs:label>has vector</rdfs:label>
-    <skos:definition>The relation between a simulation or unit cell and its vectors.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/isCalculatedPropertyOf -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/isCalculatedPropertyOf">
     <rdfs:label>is calculated property of</rdfs:label>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/isDefectOf -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/isDefectOf">
@@ -273,475 +325,484 @@
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasAltName -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasAltName">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/hasName"/>
     <rdfs:domain rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an entity with alternative names.</obo:IAO_0000115>
     <rdfs:label>has alternative name</rdfs:label>
-    <skos:definition>A data property linking an entity with alternative names.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasAngle_alpha -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasAngle_alpha">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking the angle to the measurement in the x axis.</obo:IAO_0000115>
     <rdfs:label>has angle alpha</rdfs:label>
-    <skos:definition>A data property linking the angle to the measurement in the x axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasAngle_beta -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasAngle_beta">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking the angle to the measurement in the y axis.</obo:IAO_0000115>
     <rdfs:label>has angle beta</rdfs:label>
-    <skos:definition>A data property linking the angle to the measurement in the y axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasAngle_gamma -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasAngle_gamma">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking the angle to the measurement in the z axis.</obo:IAO_0000115>
     <rdfs:label>has angle gamma</rdfs:label>
-    <skos:definition>A data property linking the angle to the measurement in the z axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasAtomicPercent -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasAtomicPercent">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalElement"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a chemical element with atomic percentage present in the material.</obo:IAO_0000115>
     <rdfs:comment>abbreviated at.%</rdfs:comment>
     <rdfs:label>has atomic percent</rdfs:label>
-    <skos:definition>A data property linking a chemical element with atomic percentage present in the material.</skos:definition>
+  </owl:DatatypeProperty>
+  <!-- http://purls.helmholtz-metadaten.de/cmso/hasBravaisLattice -->
+  <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasBravaisLattice">
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking the crystal structure and the corresponding Bravais lattice.</obo:IAO_0000115>
+    <rdfs:label rdf:datatype="http://www.w3.org/2001/XMLSchema#string">has Bravais lattice</rdfs:label>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasChemicalSymbol -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasChemicalSymbol">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/hasSymbol"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalElement"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an element with its chemical symbol.</obo:IAO_0000115>
     <rdfs:label>has chemical symbol</rdfs:label>
-    <skos:definition>A data property linking an element with its chemical symbol.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasComponent_x -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasComponent_x">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a vector with its component on the x axis.</obo:IAO_0000115>
     <rdfs:label>has component x</rdfs:label>
-    <skos:definition>A data property linking a vector with its component on the x axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasComponent_y -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasComponent_y">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a vector with its component on the y axis.</obo:IAO_0000115>
     <rdfs:label>has component y</rdfs:label>
-    <skos:definition>A data property linking a vector with its component on the y axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasComponent_z -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasComponent_z">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a vector with its component on the z axis.</obo:IAO_0000115>
     <rdfs:label>has component z</rdfs:label>
-    <skos:definition>A data property linking a vector with its component on the z axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasElementRatio -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasElementRatio">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalElement"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a chemical element with the ratio or fraction of it in the material.</obo:IAO_0000115>
     <rdfs:comment>Indicated with a value from 0 to 1.</rdfs:comment>
     <rdfs:label>has element ratio</rdfs:label>
-    <skos:definition>A data property linking a chemical element with the ratio or fraction of it in the material.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasIdentifier -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasIdentifier">
     <rdfs:domain rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an entity with an identifier (internal or external) that represents the entity.</obo:IAO_0000115>
     <rdfs:label>has identifier</rdfs:label>
-    <skos:definition>A data property linking an entity with an identifier (internal or external) that represents the entity.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasLength_x -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasLength_x">
     <rdfs:domain>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/LatticeParameter"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Length"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:domain>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a length to the measurement in the x axis.</obo:IAO_0000115>
     <rdfs:label>has length x</rdfs:label>
-    <skos:definition>A data property linking a length to the measurement in the x axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasLength_y -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasLength_y">
     <rdfs:domain>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/LatticeParameter"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Length"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:domain>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a length to the measurement in the y axis.</obo:IAO_0000115>
     <rdfs:label>has length y</rdfs:label>
-    <skos:definition>A data property linking a length to the measurement in the y axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasLength_z -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasLength_z">
     <rdfs:domain>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/LatticeParameter"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Length"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:domain>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a length to the measurement in the z axis.</obo:IAO_0000115>
     <rdfs:label>has length z</rdfs:label>
-    <skos:definition>A data property linking a length to the measurement in the z axis.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasName -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasName">
     <rdfs:domain rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an entity with its name.</obo:IAO_0000115>
     <rdfs:label>has name</rdfs:label>
-    <skos:definition>A data property linking an entity with its name.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasNumberOfAtoms -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasNumberOfAtoms">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomicScaleSample"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an atomic scale sample with the number of atoms it contains.</obo:IAO_0000115>
     <rdfs:label>has number of atoms</rdfs:label>
-    <skos:definition>A data property linking an atomic scale sample with the number of atoms it contains.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasPath -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasPath">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an atom attribute (per atom quantity) with the path pointing to the file where the data is stored.</obo:IAO_0000115>
     <rdfs:label>has path</rdfs:label>
-    <skos:definition>A data property linking an atom attribute (per atom quantity) with the path pointing to the file where the data is stored.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasReference -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasReference">
     <rdfs:domain rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
-    <rdfs:range rdf:resource="http://www.w3.org/2000/01/rdf-schema#Literal"/>
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#anyURI"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an entity with a reference (e.g. bibliographic) to another resource.</obo:IAO_0000115>
+    <rdfs:comment rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The expected usage is to provide a Uniform Resource Identifier Reference (URI), which should point the referenced resource (e.g. a DOI for a publication)</rdfs:comment>
     <rdfs:label>has reference</rdfs:label>
-    <skos:definition>A data property linking an entity with a reference (e.g. bibliographic) to another resource.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasRepetition_x -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasRepetition_x">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a simulation cell with its number of repetitions in the x direction.</obo:IAO_0000115>
     <rdfs:label>has repetition x</rdfs:label>
-    <skos:definition>A data property linking a simulation cell with its number of repetitions in the x direction.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasRepetition_y -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasRepetition_y">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a simulation cell with its number of repetitions in the y direction.</obo:IAO_0000115>
     <rdfs:label>has repetition y</rdfs:label>
-    <skos:definition>A data property linking a simulation cell with its number of repetitions in the y direction.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasRepetition_z -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasRepetition_z">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a simulation cell with its number of repetitions in the z direction.</obo:IAO_0000115>
     <rdfs:label>has repetition z</rdfs:label>
-    <skos:definition>A data property linking a simulation cell with its number of repetitions in the z direction.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasSpaceGroupNumber -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasSpaceGroupNumber">
-    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SpaceGroup"/>
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CrystalStructure"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a crystal structure with its space group number.</obo:IAO_0000115>
     <rdfs:label>has space group number</rdfs:label>
-    <skos:definition>A data property linking a crystal structure with its space group number.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasSpaceGroupSymbol -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasSpaceGroupSymbol">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/hasSymbol"/>
-    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SpaceGroup"/>
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CrystalStructure"/>
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a crystal structure with its space group symbol.</obo:IAO_0000115>
     <rdfs:label>has space group symbol</rdfs:label>
-    <skos:definition>A data property linking a crystal structure with its space group symbol.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasSymbol -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasSymbol">
     <rdfs:domain rdf:resource="http://www.w3.org/2002/07/owl#Thing"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking an entity with its symbol.</obo:IAO_0000115>
     <rdfs:label>has symbol</rdfs:label>
-    <skos:definition>A data property linking an entity with its symbol.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasValue -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasValue">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty"/>
-    <rdfs:range rdf:resource="http://www.w3.org/2000/01/rdf-schema#Literal"/>
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a calculated property to its value.</obo:IAO_0000115>
     <rdfs:label>has value</rdfs:label>
-    <skos:definition>A data property linking a calculated property to its value.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasVolume -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasVolume">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/SimulationCell"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a simulation cell with its volume. Comment: the unit of the volume is indicated by the unit of the simulation cell length.</obo:IAO_0000115>
     <rdfs:label>has volume</rdfs:label>
-    <skos:definition>A data property linking a simulation cell with its volume. Comment: the unit of the volume is indicated by the unit of the simulation cell length.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/cmso/hasWeightPercent -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/cmso/hasWeightPercent">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalElement"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a chemical element with percentage by mass present in the material.</obo:IAO_0000115>
     <rdfs:comment>abbreviated wt.%</rdfs:comment>
     <rdfs:label>has weight percent</rdfs:label>
-    <skos:definition>A data property linking a chemical element with percentage by mass present in the material.</skos:definition>
   </owl:DatatypeProperty>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Classes
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/cmso/AmorphousMaterial -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/AmorphousMaterial">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Material"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An amorphous material or solid is a material which has no defined long-range order.</obo:IAO_0000115>
     <rdfs:label>Amorphous Material</rdfs:label>
     <skos:altLabel>Amorphous Solid</skos:altLabel>
     <skos:altLabel>Non-crystalline Solid</skos:altLabel>
-    <skos:definition>An amorphous material or solid is a material which has no defined long-range order.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Angle -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Angle">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An angle is a measure of the the space (usually in degrees) between two intersecting lines at the point where they meet or vertex.</obo:IAO_0000115>
     <rdfs:label>Angle</rdfs:label>
-    <skos:definition>An angle is a measure of the the space (usually in degrees) between two intersecting lines at the point where they meet or vertex.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Atom -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Atom">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalSpecies"/>
-    <rdfs:comment>Reference: https://goldbook.iupac.org/terms/view/A00493</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Smallest particle still characterizing a chemical element. It consists of a nucleus of a positive charge (Z is the proton number and e the elementary charge) carrying almost all its mass (more than 99.9%) and Z electrons determining its size.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://goldbook.iupac.org/terms/view/A00493</obo:IAO_0000119>
     <rdfs:label>Atom</rdfs:label>
-    <skos:definition>Smallest particle still characterizing a chemical element. It consists of a nucleus of a positive charge (Z is the proton number and e the elementary charge) carrying almost all its mass (more than 99.9%) and Z electrons determining its size.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/AtomAttribute -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Atom attribute refers to the features or quantities per atom of an atomic scale sample.</obo:IAO_0000115>
     <rdfs:label>Atom Attribute</rdfs:label>
-    <skos:definition>Atom attribute refers to the features or quantities per atom of an atomic scale sample.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/AtomicForce -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/AtomicForce">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Atomic force refers to the vector that represents the force of each atom.</obo:IAO_0000115>
     <rdfs:label>Atomic Force</rdfs:label>
-    <skos:definition>Atomic force refers to the vector that represents the force of each atom.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/AtomicPosition -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/AtomicPosition">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Atomic position refers to the vector that represents the position of each atom.</obo:IAO_0000115>
     <rdfs:comment>Cartesian coordinates are preferred over direct (or fractional) coordinates.</rdfs:comment>
     <rdfs:label>Atomic Position</rdfs:label>
-    <skos:definition>Atomic position refers to the vector that represents the position of each atom.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/AtomicScaleSample -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/AtomicScaleSample">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Atomic scale sample is a computational sample in the atomic length scale.</obo:IAO_0000115>
     <rdfs:label>Atomic Scale Sample</rdfs:label>
-    <skos:definition>Atomic scale sample is a computational sample in the atomic length scale.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/AtomicVelocity -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/AtomicVelocity">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Atomic velocity refers to the vector that represents the velocity of each atom.</obo:IAO_0000115>
     <rdfs:label>Atomic Velocity</rdfs:label>
-    <skos:definition>Atomic velocity refers to the vector that represents the velocity of each atom.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Basis -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Basis">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The basis of a crystal indicates the arrangement or position of atoms in the crystal lattice.</obo:IAO_0000115>
     <rdfs:label>Basis</rdfs:label>
-    <skos:definition>The basis of a crystal indicates the arrangement or position of atoms in the crystal lattice.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/CalculatedProperty">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A calculated property is a property of a material resulting from a calculation or simulation.</obo:IAO_0000115>
     <rdfs:label>Calculated Property</rdfs:label>
-    <skos:definition>A calculated property is a property of a material resulting from a calculation or simulation.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/ChemicalComposition -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/ChemicalComposition">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Chemical composition refers to the type, arrangement and ratio of the chemical elements of a compound (or material).</obo:IAO_0000115>
     <rdfs:label>Chemical Composition</rdfs:label>
-    <skos:definition>Chemical composition refers to the type, arrangement and ratio of the chemical elements of a compound (or material).</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/ChemicalElement -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/ChemicalElement">
-    <rdfs:comment>Reference: https://goldbook.iupac.org/terms/view/C01022</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A species of atoms; all atoms with the same number of protons in the atomic nucleus.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://goldbook.iupac.org/terms/view/C01022</obo:IAO_0000119>
     <rdfs:label>Chemical Element</rdfs:label>
-    <skos:definition>A species of atoms; all atoms with the same number of protons in the atomic nucleus.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/ChemicalSpecies -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/ChemicalSpecies">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A chemical species is an ensemble of chemically identical atomic or molecular structural units in a solid array. Comment: In this context, it refers to either an atom, ion or molecule.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://goldbook.iupac.org/terms/view/CT01038</obo:IAO_0000119>
     <rdfs:comment>In this context, it refers to either an atom, ion or molecule.</rdfs:comment>
-    <rdfs:comment>Reference: https://goldbook.iupac.org/terms/view/CT01038</rdfs:comment>
     <rdfs:label>Chemical Species</rdfs:label>
-    <skos:definition>A chemical species is an ensemble of chemically identical atomic or molecular structural units in a solid array. Comment: In this context, it refers to either an atom, ion or molecule.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/ComputationalSample -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A computational sample is a representative system of a material for analysis through computational methods in the context of materials science.</obo:IAO_0000115>
     <rdfs:label>Computational Sample</rdfs:label>
-    <skos:definition>A computational sample is a representative system of a material for analysis through computational methods in the context of materials science.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/CoordinationNumber -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/CoordinationNumber">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Coordination number refers to the number of neighbors of each atom.</obo:IAO_0000115>
     <rdfs:comment>In the case of molecules, it refers to the number of atoms, molecules or ions bonded to a central atom of the molecule. Also known as ligancy.</rdfs:comment>
     <rdfs:label>Coordination Number</rdfs:label>
-    <skos:definition>Coordination number refers to the number of neighbors of each atom.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/CrystalDefect -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/CrystalDefect">
+    <obo:IAO_0000115>A crystal defect is an imperfection or irregularity in the atomic arrangement of a crystalline solid.</obo:IAO_0000115>
     <rdfs:label>Crystal Defect</rdfs:label>
     <skos:altLabel>Crystallographic Defect</skos:altLabel>
-    <skos:definition>A crystal defect is an imperfection or irregularity in the atomic arrangement of a crystalline solid.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/CrystalStructure -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/CrystalStructure">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Structure"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Crystal structure is the arrangement of atoms or molecules in the solid state. Crystal structure also involves consideration of defects, or abnormalities, in the idealized atomic/molecular arrangements.</obo:IAO_0000115>
     <rdfs:comment>In this context, the crystal structure refers to the idealized state, while the defect information is represented elsewhere (see Crystal Defect).</rdfs:comment>
     <rdfs:label>Crystal Structure</rdfs:label>
-    <skos:definition>Crystal structure is the arrangement of atoms or molecules in the solid state. Crystal structure also involves consideration of defects, or abnormalities, in the idealized atomic/molecular arrangements.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/CrystallineMaterial -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/CrystallineMaterial">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Material"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A crystalline material or solid is a material in which atoms or molecules are arranged in a highly ordered and repeating pattern, forming a three-dimensional crystal lattice.</obo:IAO_0000115>
     <rdfs:label>Crystalline Material</rdfs:label>
     <skos:altLabel>Crystal</skos:altLabel>
     <skos:altLabel>Crystalline Solid</skos:altLabel>
-    <skos:definition>A crystalline material or solid is a material in which atoms or molecules are arranged in a highly ordered and repeating pattern, forming a three-dimensional crystal lattice.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/LatticeAngle -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/LatticeAngle">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The lattice angle refers to the angles between the crystallographic axes.</obo:IAO_0000115>
     <rdfs:label>Lattice Angle</rdfs:label>
-    <skos:definition>The lattice angle refers to the angles between the crystallographic axes.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/LatticeParameter -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/LatticeParameter">
     <rdfs:subClassOf>
       <owl:Class>
         <owl:unionOf rdf:parseType="Collection">
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/Length"/>
           <rdf:Description rdf:about="http://purls.helmholtz-metadaten.de/cmso/UnitCell"/>
         </owl:unionOf>
       </owl:Class>
     </rdfs:subClassOf>
-    <rdfs:comment>The lattice angles can also be considered lattice parameters (see Lattice Angles)</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The lattice parameter is the measurement of length of the unit cell of the crystal lattice.</obo:IAO_0000115>
+    <rdfs:comment>The lattice angles can also be considered lattice parameters (see Lattice Angle)</rdfs:comment>
     <rdfs:label>Lattice Parameter</rdfs:label>
     <skos:altLabel>Lattice Constant</skos:altLabel>
-    <skos:definition>The lattice parameter is the measurement of length of the unit cell of the crystal lattice.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/LatticeVector -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/LatticeVector">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A lattice vector is a vector that defines the lattice of the crystal structure.</obo:IAO_0000115>
     <rdfs:comment>Note that it differs from the simulation cell vector.</rdfs:comment>
     <rdfs:label>Lattice Vector</rdfs:label>
-    <skos:definition>A lattice vector is a vector that defines the lattice of the crystal structure.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Length -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Length">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Length is a measure of distance.</obo:IAO_0000115>
     <rdfs:label>Length</rdfs:label>
-    <skos:definition>Length is a measure of distance.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/MacroscaleSample -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/MacroscaleSample">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Macroscale sample is a computational sample in the macroscale.</obo:IAO_0000115>
     <rdfs:label>Macroscale Sample</rdfs:label>
     <skos:altLabel>Macro Scale Sample</skos:altLabel>
-    <skos:definition>Macroscale sample is a computational sample in the macroscale.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Material -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Material">
-    <rdfs:comment>Reference: https://web.archive.org/web/20100801234616/http://www.nature.com/nmat/authors/index.html</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Materials are substances in the condensed states (liquid, solid, colloidal) designed or manipulated for technological ends.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://web.archive.org/web/20100801234616/http://www.nature.com/nmat/authors/index.html</obo:IAO_0000119>
     <rdfs:label>Material</rdfs:label>
-    <skos:definition>Materials are substances in the condensed states (liquid, solid, colloidal) designed or manipulated for technological ends.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/MesoscaleSample -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/MesoscaleSample">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Mesoscale sample is a computational sample in the mesoscale.</obo:IAO_0000115>
     <rdfs:label>Mesoscale Sample</rdfs:label>
     <skos:altLabel>Meso Scale Sample</skos:altLabel>
-    <skos:definition>Mesoscale sample is a computational sample in the mesoscale.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/MicroscaleSample -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/MicroscaleSample">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Microscale sample is a computational sample in the microscale.</obo:IAO_0000115>
     <rdfs:label>Microscale Sample</rdfs:label>
     <skos:altLabel>Micro Scale Sample</skos:altLabel>
-    <skos:definition>Microscale sample is a computational sample in the microscale.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Microstructure -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Microstructure">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Structure"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The microstructure is the structure or arrangement of all components (atomic arrangement, defects, phases, etc.) of the material at the microscale.</obo:IAO_0000115>
     <rdfs:label>Microstructure</rdfs:label>
-    <skos:definition>The microstructure is the structure or arrangement of all components (atomic arrangement, defects, phases, etc.) of the material at the microscale.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Molecule -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Molecule">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ChemicalSpecies"/>
-    <rdfs:comment>Reference: https://goldbook.iupac.org/terms/view/M04002</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An electrically neutral entity consisting of more than one atom (n&gt;1). Rigorously, a molecule, in which n&gt;1 must correspond to a depression on the potential energy surface that is deep enough to confine at least one vibrational state.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://goldbook.iupac.org/terms/view/M04002</obo:IAO_0000119>
     <rdfs:label>Molecule</rdfs:label>
-    <skos:definition>An electrically neutral entity consisting of more than one atom (n&gt;1). Rigorously, a molecule, in which n&gt;1 must correspond to a depression on the potential energy surface that is deep enough to confine at least one vibrational state.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/NanoscaleSample -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/NanoscaleSample">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/ComputationalSample"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Nanoscale sample is a computational sample in the nanoscale.</obo:IAO_0000115>
     <rdfs:label>Nanoscale Sample</rdfs:label>
-    <skos:definition>Nanoscale sample is a computational sample in the nanoscale.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Occupancy -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Occupancy">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/AtomAttribute"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Occupancy refers to the atom type at each lattice site.</obo:IAO_0000115>
     <rdfs:comment>Note the difference from a total ratio or percentage of the occupancy of a site in the crystal structure (as defined in CIF)</rdfs:comment>
     <rdfs:label>Occupancy</rdfs:label>
-    <skos:definition>Occupancy refers to the atom type at each lattice site.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/SimulationCell -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/SimulationCell">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A simulation cell is a representation of the structure or system to be simulated. It is often a three-dimensional box (although not necessarily), where information about the crystal structure and material is contained.</obo:IAO_0000115>
     <rdfs:label>Simulation Cell</rdfs:label>
     <skos:altLabel>Box</skos:altLabel>
     <skos:altLabel>Supercell</skos:altLabel>
-    <skos:definition>A simulation cell is a representation of the structure or system to be simulated. It is often a three-dimensional box (although not necessarily), where information about the crystal structure and material is contained.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/SimulationCellAngle -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/SimulationCellAngle">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Angle"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The simulation cell angle refers to the angles of the simulation cell in each direction.</obo:IAO_0000115>
     <rdfs:label>Simulation Cell Angle</rdfs:label>
-    <skos:definition>The simulation cell angle refers to the angles of the simulation cell in each direction.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/SimulationCellLength -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/SimulationCellLength">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Length"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The simulation cell length refers to the length (dimension) of the simulation cell or box.</obo:IAO_0000115>
     <rdfs:label>Simulation Cell Length</rdfs:label>
     <skos:altLabel>Box length</skos:altLabel>
-    <skos:definition>The simulation cell length refers to the length (dimension) of the simulation cell or box.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/SimulationCellVector -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/SimulationCellVector">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/cmso/Vector"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The simulation cell vector is a vector that defines the simulation cell or box.</obo:IAO_0000115>
     <rdfs:comment>Note that it differs from the lattice vector.</rdfs:comment>
     <rdfs:label>Simulation Cell Vector</rdfs:label>
-    <skos:definition>The simulation cell vector is a vector that defines the simulation cell or box.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/SpaceGroup -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/SpaceGroup">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The space group represents the symmetry properties of the crystal. In three-dimensions, space groups are classified in 230 distinct groups.</obo:IAO_0000115>
     <rdfs:label>Space Group</rdfs:label>
-    <skos:definition>The space group represents the symmetry properties of the crystal. In three-dimensions, space groups are classified in 230 distinct groups.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Structure -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Structure">
-    <rdfs:comment>Reference: https://www.merriam-webster.com/dictionary/structure</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Structure is the the arrangement of particles or parts in a substance or body.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#anyURI">https://www.merriam-webster.com/dictionary/structure</obo:IAO_0000119>
     <rdfs:label>Structure</rdfs:label>
-    <skos:definition>Structure is the the arrangement of particles or parts in a substance or body.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/UnitCell -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/UnitCell">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The unit cell is the smallest repeating unit of the crystal structure which contains the overal symmetry of the crystal. The entire crystal lattice can be generated by repeating the unit cell in three dimensions.</obo:IAO_0000115>
     <rdfs:label>Unit Cell</rdfs:label>
-    <skos:definition>The unit cell is the smallest repeating unit of the crystal structure which contains the overal symmetry of the crystal. The entire crystal lattice can be generated by repeating the unit cell in three dimensions.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/cmso/Vector -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/cmso/Vector">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Vector is a quantity that has a magnitude and direction.</obo:IAO_0000115>
     <rdfs:label>Vector</rdfs:label>
-    <skos:definition>Vector is a quantity that has a magnitude and direction.</skos:definition>
   </owl:Class>
   <!-- http://qudt.org/schema/qudt/Unit -->
   <owl:Class rdf:about="http://qudt.org/schema/qudt/Unit">
     <terms:description rdf:datatype="http://qudt.org/schema/qudt/LatexString">A unit of measure, or unit, is a particular quantity value that has been chosen as a scale for measuring other quantities the same kind (more generally of equivalent dimension). For example, the meter is a quantity of length that has been rigorously defined and standardized by the BIPM (International Board of Weights and Measures). Any measurement of the length can be expressed as a number multiplied by the unit meter. More formally, the value of a physical quantity Q with respect to a unit (U) is expressed as the scalar multiple of a real number (n) and U, as  \(Q = nU\).</terms:description>
     <rdfs:isDefinedBy rdf:resource="http://qudt.org/2.1/schema/qudt"/>
     <rdfs:label>Unit</rdfs:label>
   </owl:Class>
```

### Comparing `atomrdf-0.6.4/atomrdf/data/element.yml` & `atomrdf-0.8.1/atomrdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/data/md_template.yml` & `atomrdf-0.8.1/atomrdf/data/md_template.yml`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/data/pldo.owl` & `atomrdf-0.8.1/atomrdf/data/pldo.owl`

 * *Files 13% similar despite different names*

#### Comparing `atomrdf-0.6.4/atomrdf/data/pldo.owl` & `atomrdf-0.8.1/atomrdf/data/pldo.owl`

```diff
@@ -1,25 +1,75 @@
 <?xml version="1.0" encoding="utf-8"?>
-<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/pldo/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/pldo/">
+<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/pldo/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:obo="http://purl.obolibrary.org/obo/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/pldo/">
   <owl:Ontology rdf:about="http://purls.helmholtz-metadaten.de/pldo/">
     <terms:contributor>https://orcid.org/0000-0001-9560-4728</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0002-5149-603X</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0002-6776-1213</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0003-0698-4891</terms:contributor>
     <terms:creator>https://orcid.org/0000-0001-7564-7990</terms:creator>
     <terms:description>PLDO focuses on the description of planar defects in crystalline materials.</terms:description>
     <terms:title>Planar Defects Ontology (PLDO)</terms:title>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">0.0.1</owl:versionInfo>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotation properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
+  <!-- http://purl.obolibrary.org/obo/IAO_0000111 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000111"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000114 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000114"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000115 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000115">
+    <obo:IAO_0000111 xml:lang="en">definition</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">The official definition, explaining the meaning of a class or property. Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions.</obo:IAO_0000115>
+    <obo:IAO_0000116 xml:lang="en">2012-04-05: 
+Barry Smith
+
+The official OBI definition, explaining the meaning of a class or property: 'Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions'  is terrible.
+
+Can you fix to something like:
+
+A statement of necessary and sufficient conditions explaining the meaning of an expression referring to a class or property.
+
+Alan Ruttenberg
+
+Your proposed definition is a reasonable candidate, except that it is very common that necessary and sufficient conditions are not given. Mostly they are necessary, occasionally they are necessary and sufficient or just sufficient. Often they use terms that are not themselves defined and so they effectively can't be evaluated by those criteria. 
+
+On the specifics of the proposed definition:
+
+We don't have definitions of 'meaning' or 'expression' or 'property'. For 'reference' in the intended sense I think we use the term 'denotation'. For 'expression', I think we you mean symbol, or identifier. For 'meaning' it differs for class and property. For class we want documentation that let's the intended reader determine whether an entity is instance of the class, or not. For property we want documentation that let's the intended reader determine, given a pair of potential relata, whether the assertion that the relation holds is true. The 'intended reader' part suggests that we also specify who, we expect, would be able to understand the definition, and also generalizes over human and computer reader to include textual and logical definition. 
+
+Personally, I am more comfortable weakening definition to documentation, with instructions as to what is desirable. 
+
+We also have the outstanding issue of how to aim different definitions to different audiences. A clinical audience reading chebi wants a different sort of definition documentation/definition from a chemistry trained audience, and similarly there is a need for a definition that is adequate for an ontologist to work with.</obo:IAO_0000116>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:isDefinedBy rdf:resource="http://purl.obolibrary.org/obo/iao.owl"/>
+    <rdfs:label xml:lang="en">definition</rdfs:label>
+  </owl:AnnotationProperty>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000116 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000116"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000117 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000117"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000119 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000119">
+    <obo:IAO_0000111 xml:lang="en">definition source</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">Formal citation, e.g. identifier in external database to indicate / attribute source(s) for the definition. Free text indicate / attribute source(s) for the definition. EXAMPLE: Author Name, URI, MeSH Term C04, PUBMED ID, Wiki uri on 31.01.2007</obo:IAO_0000115>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">Discussion on obo-discuss mailing-list, see http://bit.ly/hgm99w</obo:IAO_0000119>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:isDefinedBy rdf:resource="http://purl.obolibrary.org/obo/iao.owl"/>
+    <rdfs:label xml:lang="en">definition source</rdfs:label>
+  </owl:AnnotationProperty>
   <!-- http://purl.org/dc/elements/1.1/contributor -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/contributor"/>
   <!-- http://purl.org/dc/elements/1.1/creator -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/creator"/>
   <!-- http://purl.org/dc/elements/1.1/description -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/description"/>
   <!-- http://purl.org/dc/elements/1.1/title -->
@@ -75,17 +125,14 @@
     <rdfs:label xml:lang="en">alternative label</rdfs:label>
     <skos:definition xml:lang="en">An alternative lexical label for a resource.</skos:definition>
     <skos:example xml:lang="en">Acronyms, abbreviations, spelling variants, and irregular plural/singular forms may be included among the alternative labels for a concept. Mis-spelled terms are normally included as hidden labels (see skos:hiddenLabel).</skos:example>
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2000/01/rdf-schema#label"/>
   </owl:AnnotationProperty>
   <!-- http://www.w3.org/2004/02/skos/core#definition -->
   <owl:AnnotationProperty rdf:about="http://www.w3.org/2004/02/skos/core#definition">
-    <rdfs:isDefinedBy rdf:resource="http://www.w3.org/2004/02/skos/core"/>
-    <rdfs:label xml:lang="en">definition</rdfs:label>
-    <skos:definition xml:lang="en">A statement or formal explanation of the meaning of a concept.</skos:definition>
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2004/02/skos/core#note"/>
   </owl:AnnotationProperty>
   <!-- http://www.w3.org/2004/02/skos/core#example -->
   <owl:AnnotationProperty rdf:about="http://www.w3.org/2004/02/skos/core#example">
     <rdfs:isDefinedBy rdf:resource="http://www.w3.org/2004/02/skos/core"/>
     <rdfs:label xml:lang="en">example</rdfs:label>
     <skos:definition xml:lang="en">An example of the use of a concept.</skos:definition>
@@ -113,167 +160,167 @@
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/pldo/hasTiltComponent -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/hasTiltComponent">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/MixedGrainBoundary"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/pldo/TiltGrainBoundary"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a mixed grain boundary and the tilt grain boundary component.</obo:IAO_0000115>
     <rdfs:label>has tilt component</rdfs:label>
-    <skos:definition>The relation between a mixed grain boundary and the tilt grain boundary component.</skos:definition>
   </owl:ObjectProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/hasTwistComponent -->
   <owl:ObjectProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/hasTwistComponent">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/MixedGrainBoundary"/>
     <rdfs:range rdf:resource="http://purls.helmholtz-metadaten.de/pldo/TwistGrainBoundary"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The relation between a mixed grain boundary and the twist grain boundary component.</obo:IAO_0000115>
     <rdfs:label>has twist component</rdfs:label>
-    <skos:definition>The relation between a mixed grain boundary and the twist grain boundary component.</skos:definition>
   </owl:ObjectProperty>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Data properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/pldo/geometricalDegreesOfFreedom -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/geometricalDegreesOfFreedom">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The geometrical degrees of freedom are the parameters that are necessary to characterize a grain boundary.</obo:IAO_0000115>
     <rdfs:label>geometrical degrees of freedom</rdfs:label>
-    <skos:definition>The geometrical degrees of freedom are the parameters that are necessary to characterize a grain boundary.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/hasGBplane -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/hasGBplane">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/macroscopicDegreesOfFreedom"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indicating the grain boundary (GB) plane using Miller Indices.</obo:IAO_0000115>
     <rdfs:label>has GB plane</rdfs:label>
-    <skos:definition>A data property indicating the grain boundary (GB) plane using Miller Indices.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/hasMisorientationAngle -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/hasMisorientationAngle">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/macroscopicDegreesOfFreedom"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indicating the misorientation angle (θ) of the grains with respect to each other.</obo:IAO_0000115>
     <rdfs:label>has misorientation angle</rdfs:label>
-    <skos:definition>A data property indicating the misorientation angle (θ) of the grains with respect to each other.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/hasRotationAxis -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/hasRotationAxis">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/macroscopicDegreesOfFreedom"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indication the rotation axis [uvw].</obo:IAO_0000115>
     <rdfs:label>has rotation axis</rdfs:label>
-    <skos:definition>A data property indication the rotation axis [uvw].</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/hasSigmaValue -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/hasSigmaValue">
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
     <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property linking a GB with its sigma value.</obo:IAO_0000115>
     <rdfs:comment>Sigma value of a GB is the coincidence index, calculated as the coincidence unit cell volume by the crystal primitive unit cell volume. The coincidence index refers to the Coincidence Site Lattice (CSL).</rdfs:comment>
     <rdfs:label>has sigma value</rdfs:label>
-    <skos:definition>A data property linking a GB with its sigma value.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/macroscopicDegreesOfFreedom -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/macroscopicDegreesOfFreedom">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/geometricalDegreesOfFreedom"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">There are five macroscopic degrees of freedom (DOFs) that are sufficient to describe the thermodynamic description of the grain boundary.</obo:IAO_0000115>
     <rdfs:comment>In simulations of grain boundaries, the macroscopic DOFs are imposed on the structure.</rdfs:comment>
     <rdfs:label>macroscopic degrees of freedom</rdfs:label>
-    <skos:definition>There are five macroscopic degrees of freedom (DOFs) that are sufficient to describe the thermodynamic description of the grain boundary.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/pldo/microscopicDegreesOfFreedom -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/pldo/microscopicDegreesOfFreedom">
     <rdfs:subPropertyOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/geometricalDegreesOfFreedom"/>
     <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The microscopic degrees of freedom (DOFs) refer to the translation of one crystal with respect to the other at the microscopic scale. The microscopic parameters result from the relaxation process and are not independent of the macroscopic parameters.</obo:IAO_0000115>
     <rdfs:comment>In simulations of grain boundaries, the microscopic DOFs are obtained after the grain boundary energy minimization.</rdfs:comment>
     <rdfs:label>microscopic degrees of freedom</rdfs:label>
-    <skos:definition>The microscopic degrees of freedom (DOFs) refer to the translation of one crystal with respect to the other at the microscopic scale. The microscopic parameters result from the relaxation process and are not independent of the macroscopic parameters.</skos:definition>
   </owl:DatatypeProperty>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Classes
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/pldo/AntiphaseBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/AntiphaseBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/PlanarDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An antiphase boundary is a planar defect which occurs in ordered alloys. The boundary separates two domains of the same ordered phase.</obo:IAO_0000115>
     <rdfs:label>Antiphase Boundary</rdfs:label>
     <skos:altLabel>APB</skos:altLabel>
-    <skos:definition>An antiphase boundary is a planar defect which occurs in ordered alloys. The boundary separates two domains of the same ordered phase.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/GrainBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/PlanarDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A grain boundary is a planar defect that separates two crystals (or grains) of the same material.</obo:IAO_0000115>
     <rdfs:label>Grain Boundary</rdfs:label>
     <skos:altLabel>GB</skos:altLabel>
-    <skos:definition>A grain boundary is a planar defect that separates two crystals (or grains) of the same material.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/LowAngleGrainBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/LowAngleGrainBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
-    <rdfs:comment>Reference: ISBN 978-94-007-4968-9</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A low angle GB is a grain boundary with a misorientation angle lower than 15 degrees.</obo:IAO_0000115>
+    <obo:IAO_0000119>ISBN 978-94-007-4968-9</obo:IAO_0000119>
     <rdfs:label>Low Angle Grain Boundary</rdfs:label>
     <skos:altLabel>Low-Angle Grain Boundary</skos:altLabel>
-    <skos:definition>A low angle GB is a grain boundary with a misorientation angle lower than 15 degrees.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/MixedGrainBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/MixedGrainBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
-    <rdfs:comment>Reference: ISBN 978-94-007-4968-9</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A mixed grain boundary is a grain boundary where the [uvw] rotation axis has perpendicular and parallel components with respect to the boundary plane.</obo:IAO_0000115>
+    <obo:IAO_0000119>ISBN 978-94-007-4968-9</obo:IAO_0000119>
     <rdfs:label>Mixed Grain Boundary</rdfs:label>
-    <skos:definition>A mixed grain boundary is a grain boundary where the [uvw] rotation axis has perpendicular and parallel components with respect to the boundary plane.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/PlanarDefect -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/PlanarDefect">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A planar defect is a defect of the crystal structure across a plane. It is considered to be a two-dimensional defect, such as an internal interface or the surface.</obo:IAO_0000115>
     <rdfs:label>Planar Defect</rdfs:label>
     <skos:altLabel>Interface</skos:altLabel>
-    <skos:definition>A planar defect is a defect of the crystal structure across a plane. It is considered to be a two-dimensional defect, such as an internal interface or the surface.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/StackingFault -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/StackingFault">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/PlanarDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A stacking fault is a planar defect created by an error (fault) in the order of the sequential layering of crystallographic planes.</obo:IAO_0000115>
     <rdfs:label>Stacking Fault</rdfs:label>
-    <skos:definition>A stacking fault is a planar defect created by an error (fault) in the order of the sequential layering of crystallographic planes.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/Surface -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/Surface">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/PlanarDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">The free surface (or external surface) of the material is a planar defect where the surface atoms have no neighbours or cohesive bonds on the external side.</obo:IAO_0000115>
     <rdfs:label>Surface</rdfs:label>
-    <skos:definition>The free surface (or external surface) of the material is a planar defect where the surface atoms have no neighbours or cohesive bonds on the external side.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/SymmetricalTiltGrainBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/SymmetricalTiltGrainBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/TiltGrainBoundary"/>
-    <rdfs:comment>Reference: ISBN 978-94-007-4968-9</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A symmetrical tilt grain boundary is a tilt grain boundary where the two grains are symmetric. The boundary plane has the same Miller indices in crystals I and II: {hkl}_1 = {hkl}_2.</obo:IAO_0000115>
+    <obo:IAO_0000119>ISBN 978-94-007-4968-9</obo:IAO_0000119>
     <rdfs:label>Symmetrical Tilt Grain Boundary</rdfs:label>
-    <skos:definition>A symmetrical tilt grain boundary is a tilt grain boundary where the two grains are symmetric. The boundary plane has the same Miller indices in crystals I and II: {hkl}_1 = {hkl}_2.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/TiltGrainBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/TiltGrainBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
-    <rdfs:comment>Reference: ISBN 978-94-007-4968-9</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A twist boundary is a grain boundary with a [uvw] rotation axis perpendicular to the boundary plane.</obo:IAO_0000115>
+    <obo:IAO_0000119>ISBN 978-94-007-4968-9</obo:IAO_0000119>
     <rdfs:label>Tilt Grain Boundary</rdfs:label>
     <skos:altLabel>Tilt Boundary</skos:altLabel>
-    <skos:definition>A twist boundary is a grain boundary with a [uvw] rotation axis perpendicular to the boundary plane.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/TwinBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/TwinBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/PlanarDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A twin boundary is a planar defect that occurs between two separate crystals which are mirror images of each other, both crystals should have the same crystal structure.</obo:IAO_0000115>
     <rdfs:label>Twin Boundary</rdfs:label>
-    <skos:definition>A twin boundary is a planar defect that occurs between two separate crystals which are mirror images of each other, both crystals should have the same crystal structure.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/pldo/TwistGrainBoundary -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/pldo/TwistGrainBoundary">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/pldo/GrainBoundary"/>
-    <rdfs:comment>Reference: ISBN 978-94-007-4968-9</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A twist boundary is a grain boundary with a [uvw] rotation axis contained within the boundary plane.</obo:IAO_0000115>
+    <obo:IAO_0000119>ISBN 978-94-007-4968-9</obo:IAO_0000119>
     <rdfs:label>Twist Grain Boundary</rdfs:label>
     <skos:altLabel>Twist Boundary</skos:altLabel>
-    <skos:definition>A twist boundary is a grain boundary with a [uvw] rotation axis contained within the boundary plane.</skos:definition>
   </owl:Class>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotations
     //
     ///////////////////////////////////////////////////////////////////////////////////////
```

### Comparing `atomrdf-0.6.4/atomrdf/data/podo.owl` & `atomrdf-0.8.1/atomrdf/data/podo.owl`

 * *Files 18% similar despite different names*

#### Comparing `atomrdf-0.6.4/atomrdf/data/podo.owl` & `atomrdf-0.8.1/atomrdf/data/podo.owl`

```diff
@@ -1,25 +1,75 @@
 <?xml version="1.0" encoding="utf-8"?>
-<rdf:RDF xmlns="http://www.semanticweb.org/a.azocar.guzman/ontologies/2023/5/untitled-ontology-21#" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://www.semanticweb.org/a.azocar.guzman/ontologies/2023/5/untitled-ontology-21">
+<rdf:RDF xmlns="http://purls.helmholtz-metadaten.de/podo/" xmlns:dc="http://purl.org/dc/elements/1.1/" xmlns:obo="http://purl.obolibrary.org/obo/" xmlns:owl="http://www.w3.org/2002/07/owl#" xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#" xmlns:xml="http://www.w3.org/XML/1998/namespace" xmlns:xsd="http://www.w3.org/2001/XMLSchema#" xmlns:rdfs="http://www.w3.org/2000/01/rdf-schema#" xmlns:skos="http://www.w3.org/2004/02/skos/core#" xmlns:terms="http://purl.org/dc/terms/" xml:base="http://purls.helmholtz-metadaten.de/podo/">
   <owl:Ontology rdf:about="http://purls.helmholtz-metadaten.de/podo/">
     <terms:contributor>https://orcid.org/0000-0001-9560-4728</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0002-5149-603X</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0002-6776-1213</terms:contributor>
     <terms:contributor>https://orcid.org/0000-0003-0698-4891</terms:contributor>
     <terms:creator>https://orcid.org/0000-0001-7564-7990</terms:creator>
     <terms:description>PODO focuses on the description of point defects in crystalline materials.</terms:description>
     <terms:title>Point Defects Ontology (PODO)</terms:title>
+    <owl:versionInfo rdf:datatype="http://www.w3.org/2001/XMLSchema#string">0.0.1</owl:versionInfo>
   </owl:Ontology>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotation properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
+  <!-- http://purl.obolibrary.org/obo/IAO_0000111 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000111"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000114 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000114"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000115 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000115">
+    <obo:IAO_0000111 xml:lang="en">definition</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">The official definition, explaining the meaning of a class or property. Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions.</obo:IAO_0000115>
+    <obo:IAO_0000116 xml:lang="en">2012-04-05: 
+Barry Smith
+
+The official OBI definition, explaining the meaning of a class or property: 'Shall be Aristotelian, formalized and normalized. Can be augmented with colloquial definitions'  is terrible.
+
+Can you fix to something like:
+
+A statement of necessary and sufficient conditions explaining the meaning of an expression referring to a class or property.
+
+Alan Ruttenberg
+
+Your proposed definition is a reasonable candidate, except that it is very common that necessary and sufficient conditions are not given. Mostly they are necessary, occasionally they are necessary and sufficient or just sufficient. Often they use terms that are not themselves defined and so they effectively can't be evaluated by those criteria. 
+
+On the specifics of the proposed definition:
+
+We don't have definitions of 'meaning' or 'expression' or 'property'. For 'reference' in the intended sense I think we use the term 'denotation'. For 'expression', I think we you mean symbol, or identifier. For 'meaning' it differs for class and property. For class we want documentation that let's the intended reader determine whether an entity is instance of the class, or not. For property we want documentation that let's the intended reader determine, given a pair of potential relata, whether the assertion that the relation holds is true. The 'intended reader' part suggests that we also specify who, we expect, would be able to understand the definition, and also generalizes over human and computer reader to include textual and logical definition. 
+
+Personally, I am more comfortable weakening definition to documentation, with instructions as to what is desirable. 
+
+We also have the outstanding issue of how to aim different definitions to different audiences. A clinical audience reading chebi wants a different sort of definition documentation/definition from a chemistry trained audience, and similarly there is a need for a definition that is adequate for an ontologist to work with.</obo:IAO_0000116>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:isDefinedBy rdf:resource="http://purl.obolibrary.org/obo/iao.owl"/>
+    <rdfs:label xml:lang="en">definition</rdfs:label>
+  </owl:AnnotationProperty>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000116 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000116"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000117 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000117"/>
+  <!-- http://purl.obolibrary.org/obo/IAO_0000119 -->
+  <owl:AnnotationProperty rdf:about="http://purl.obolibrary.org/obo/IAO_0000119">
+    <obo:IAO_0000111 xml:lang="en">definition source</obo:IAO_0000111>
+    <obo:IAO_0000114 rdf:resource="http://purl.obolibrary.org/obo/IAO_0000122"/>
+    <obo:IAO_0000115 xml:lang="en">Formal citation, e.g. identifier in external database to indicate / attribute source(s) for the definition. Free text indicate / attribute source(s) for the definition. EXAMPLE: Author Name, URI, MeSH Term C04, PUBMED ID, Wiki uri on 31.01.2007</obo:IAO_0000115>
+    <obo:IAO_0000117 xml:lang="en">PERSON:Daniel Schober</obo:IAO_0000117>
+    <obo:IAO_0000119 xml:lang="en">Discussion on obo-discuss mailing-list, see http://bit.ly/hgm99w</obo:IAO_0000119>
+    <obo:IAO_0000119 xml:lang="en">GROUP:OBI:&lt;http://purl.obolibrary.org/obo/obi&gt;</obo:IAO_0000119>
+    <rdfs:isDefinedBy rdf:resource="http://purl.obolibrary.org/obo/iao.owl"/>
+    <rdfs:label xml:lang="en">definition source</rdfs:label>
+  </owl:AnnotationProperty>
   <!-- http://purl.org/dc/elements/1.1/contributor -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/contributor"/>
   <!-- http://purl.org/dc/elements/1.1/creator -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/creator"/>
   <!-- http://purl.org/dc/elements/1.1/description -->
   <owl:AnnotationProperty rdf:about="http://purl.org/dc/elements/1.1/description"/>
   <!-- http://purl.org/dc/elements/1.1/title -->
@@ -75,17 +125,14 @@
     <rdfs:label xml:lang="en">alternative label</rdfs:label>
     <skos:definition xml:lang="en">An alternative lexical label for a resource.</skos:definition>
     <skos:example xml:lang="en">Acronyms, abbreviations, spelling variants, and irregular plural/singular forms may be included among the alternative labels for a concept. Mis-spelled terms are normally included as hidden labels (see skos:hiddenLabel).</skos:example>
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2000/01/rdf-schema#label"/>
   </owl:AnnotationProperty>
   <!-- http://www.w3.org/2004/02/skos/core#definition -->
   <owl:AnnotationProperty rdf:about="http://www.w3.org/2004/02/skos/core#definition">
-    <rdfs:isDefinedBy rdf:resource="http://www.w3.org/2004/02/skos/core"/>
-    <rdfs:label xml:lang="en">definition</rdfs:label>
-    <skos:definition xml:lang="en">A statement or formal explanation of the meaning of a concept.</skos:definition>
     <rdfs:subPropertyOf rdf:resource="http://www.w3.org/2004/02/skos/core#note"/>
   </owl:AnnotationProperty>
   <!-- http://www.w3.org/2004/02/skos/core#example -->
   <owl:AnnotationProperty rdf:about="http://www.w3.org/2004/02/skos/core#example">
     <rdfs:isDefinedBy rdf:resource="http://www.w3.org/2004/02/skos/core"/>
     <rdfs:label xml:lang="en">example</rdfs:label>
     <skos:definition xml:lang="en">An example of the use of a concept.</skos:definition>
@@ -109,94 +156,118 @@
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Data properties
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
+  <!-- http://purls.helmholtz-metadaten.de/podo/hasImpurityConcentration -->
+  <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/podo/hasImpurityConcentration">
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indicating the impurity concentration.</obo:IAO_0000115>
+    <rdfs:comment>The domain of this property should correspond to a material sample (either computational or experimental).</rdfs:comment>
+    <rdfs:label>has impurity concentration</rdfs:label>
+  </owl:DatatypeProperty>
+  <!-- http://purls.helmholtz-metadaten.de/podo/hasNumberOfImpurityAtoms -->
+  <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/podo/hasNumberOfImpurityAtoms">
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indicating the total number of impurity atoms in the crystal structure.</obo:IAO_0000115>
+    <rdfs:comment>The domain of this property should correspond to a material sample (either computational or experimental).</rdfs:comment>
+    <rdfs:label>has number of impurity atoms</rdfs:label>
+  </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/podo/hasNumberOfVacancies -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/podo/hasNumberOfVacancies">
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#integer"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indicating the total number of vacancies in the crystal structure.</obo:IAO_0000115>
+    <rdfs:comment>The domain of this property should correspond to a material sample (either computational or experimental).</rdfs:comment>
     <rdfs:label>has number of vacancies</rdfs:label>
-    <skos:definition>A data property indicating the total number of vacancies in the crystal structure.</skos:definition>
   </owl:DatatypeProperty>
   <!-- http://purls.helmholtz-metadaten.de/podo/hasVacancyConcentration -->
   <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/podo/hasVacancyConcentration">
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#float"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A data property indicating the vacancy concentration.</obo:IAO_0000115>
     <rdfs:comment>Note that the vacancy concentration is given as a fraction, with a value from 0 to 1.</rdfs:comment>
+    <rdfs:comment>The domain of this property should correspond to a material sample (either computational or experimental).</rdfs:comment>
     <rdfs:label>has vacancy concentration</rdfs:label>
-    <skos:definition>A data property indicating the vacancy concentration.</skos:definition>
+  </owl:DatatypeProperty>
+  <!-- http://purls.helmholtz-metadaten.de/podo/occupiesInterstitialSite -->
+  <owl:DatatypeProperty rdf:about="http://purls.helmholtz-metadaten.de/podo/occupiesInterstitialSite">
+    <rdfs:domain rdf:resource="http://purls.helmholtz-metadaten.de/podo/Interstitial"/>
+    <rdfs:range rdf:resource="http://www.w3.org/2001/XMLSchema#string"/>
+    <rdfs:label>occupies interstitial site</rdfs:label>
   </owl:DatatypeProperty>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Classes
     //
     ///////////////////////////////////////////////////////////////////////////////////////
      -->
   <!-- http://purls.helmholtz-metadaten.de/podo/AntisiteDefect -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/AntisiteDefect">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/PointDefect"/>
-    <rdfs:comment>Reference: ISBN 978-1-119-45416-8</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">Antisite Defect is a point defect which occurs in ordered alloys or compounds when two atoms of different type switch positions.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN 978-1-119-45416-8</obo:IAO_0000119>
     <rdfs:label>Antisite Defect</rdfs:label>
-    <skos:definition>Antisite Defect is a point defect which occurs in ordered alloys or compounds when two atoms of different type switch positions.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/FrenkelDefect -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/FrenkelDefect">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/PointDefect"/>
-    <rdfs:comment>Reference: ISBN 978-1-119-45416-8</rdfs:comment>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A Frenkel defect is a point defect which occurs in ionic crystals when an ion is removed to an interstitial position, leaving a vacancy behind.</obo:IAO_0000115>
+    <obo:IAO_0000119 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">ISBN 978-1-119-45416-8</obo:IAO_0000119>
     <rdfs:label>Frenkel Defect</rdfs:label>
     <skos:altLabel>Frenkel Pair</skos:altLabel>
-    <skos:definition>A Frenkel defect is a point defect which occurs in ionic crystals when an ion is removed to an interstitial position, leaving a vacancy behind.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/Impurity -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/Impurity">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/PointDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An impurity is a point defect where foreign atoms (of different type as the host atom) enter the crystal lattice.</obo:IAO_0000115>
     <rdfs:label>Impurity</rdfs:label>
-    <skos:definition>An impurity is a point defect where foreign atoms (of different type as the host atom) enter the crystal lattice.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/Interstitial -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/Interstitial">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/PointDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">An interstitial is a point defect where an atom occupies an interstitial site. In crystallography, interstitial sites are the empty space between the atoms (assuming a hard-sphere model).</obo:IAO_0000115>
     <rdfs:label>Interstitial</rdfs:label>
-    <skos:definition>An interstitial is a point defect where an atom occupies an interstitial site. In crystallography, interstitial sites are the empty space between the atoms (assuming a hard-sphere model).</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/InterstitialImpurity -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/InterstitialImpurity">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/Impurity"/>
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/Interstitial"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A interstitial impurity is a point defect where the atom occupying the interstitial site is of a different type as the matrix.</obo:IAO_0000115>
     <rdfs:label>Interstitial Impurity</rdfs:label>
-    <skos:definition>A interstitial impurity is a point defect where the atom occupying the interstitial site is of a different type as the matrix.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/PointDefect -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/PointDefect">
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A point defect is a crystalline defect which is localized at or around a single lattice point. It is considered to be a zero-dimensional defect because it does not extend in any dimension in the lattice.</obo:IAO_0000115>
     <rdfs:label>Point Defect</rdfs:label>
-    <skos:definition>A point defect is a crystalline defect which is localized at or around a single lattice point. It is considered to be a zero-dimensional defect because it does not extend in any dimension in the lattice.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/SchottkyDefect -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/SchottkyDefect">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/PointDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A Schottky defect is a point defect which occurs in ionic crystals when oppositely charged ions create a vacancy in the interior of the lattice and go to the surface.</obo:IAO_0000115>
     <rdfs:label>Schottky Defect</rdfs:label>
-    <skos:definition>A Schottky defect is a point defect which occurs in ionic crystals when oppositely charged ions create a vacancy in the interior of the lattice and go to the surface.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/Self-interstitial -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/Self-interstitial">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/Interstitial"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A self-interstitial is an insterstitial defect where the atom occupying the interstitial site is of the same type as the matrix.</obo:IAO_0000115>
     <rdfs:label>Self-interstitial</rdfs:label>
-    <skos:definition>A self-interstitial is an insterstitial defect where the atom occupying the interstitial site is of the same type as the matrix.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/SubstitutionalImpurity -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/SubstitutionalImpurity">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/Impurity"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A substitutional impurity is an impurity where an atom of different type replaces a host or matrix atom.</obo:IAO_0000115>
     <rdfs:label>Substitutional Impurity</rdfs:label>
-    <skos:definition>A substitutional impurity is an impurity where an atom of different type replaces a host or matrix atom.</skos:definition>
   </owl:Class>
   <!-- http://purls.helmholtz-metadaten.de/podo/Vacancy -->
   <owl:Class rdf:about="http://purls.helmholtz-metadaten.de/podo/Vacancy">
     <rdfs:subClassOf rdf:resource="http://purls.helmholtz-metadaten.de/podo/PointDefect"/>
+    <obo:IAO_0000115 rdf:datatype="http://www.w3.org/2001/XMLSchema#string">A vacancy is a point defect in which an atom is missing from its original lattice site.</obo:IAO_0000115>
     <rdfs:label>Vacancy</rdfs:label>
-    <skos:definition>A vacancy is a point defect in which an atom is missing from its original lattice site.</skos:definition>
   </owl:Class>
   <!-- 
     ///////////////////////////////////////////////////////////////////////////////////////
     //
     // Annotations
     //
     ///////////////////////////////////////////////////////////////////////////////////////
```

### Comparing `atomrdf-0.6.4/atomrdf/graph.py` & `atomrdf-0.8.1/atomrdf/graph.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,27 +29,32 @@
 import yaml
 import uuid
 import json
 import shutil
 import tarfile
 import logging
 import warnings
+import re
+import pickle
 
 # from pyscal3.core import System
 from pyscal3.atoms import Atoms
 
-from atomrdf.visualize import visualize_graph
+from atomrdf.visualize import visualize_graph, visualize_provenance
 from atomrdf.network.network import OntologyNetwork
 from atomrdf.network.ontology import read_ontology
 from atomrdf.structure import System
 import atomrdf.properties as prp
 from atomrdf.stores import create_store
 import atomrdf.json_io as json_io
+from atomrdf.workflow.workflow import Workflow
+from atomrdf.sample import Sample
+import atomrdf.mp as amp 
 
-from atomrdf.namespace import Namespace, CMSO, PLDO, PODO, ASMO
+from atomrdf.namespace import Namespace, CMSO, PLDO, PODO, ASMO, PROV, MATH, UNSAFECMSO, UNSAFEASMO
 
 # read element data file
 file_location = os.path.dirname(__file__).split("/")
 file_location = "/".join(file_location[:-1])
 file_location = os.path.join(os.path.dirname(__file__), "data/element.yml")
 with open(file_location, "r") as fin:
     element_indetifiers = yaml.safe_load(fin)
@@ -76,29 +81,39 @@
         "shape": "parallelogram",
         "style": "filled",
         "fontsize": "8",
         "fontname": "Helvetica",
     },
 }
 
+def _clean_string(input_string):
+    input_string = re.sub(r'\W', '_', input_string)
+    if input_string[0].isdigit():
+        input_string = "s" + input_string
+    return input_string
 
 def _replace_keys(refdict, indict):
     for key, val in indict.items():
         if key in refdict.keys():
             if isinstance(val, dict):
                 _replace_keys(refdict[key], indict[key])
             else:
                 refdict[key] = val
     return refdict
 
 
 def _dummy_log(str):
     pass
 
-
+def _name(term):
+    try:
+        return str(term.toPython())
+    except:
+        return str(term)
+    
 def _prepare_log(file):
     logger = logging.getLogger(__name__)
     handler = logging.FileHandler(file)
     formatter = logging.Formatter("%(asctime)s %(name)-12s %(levelname)-8s %(message)s")
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     logger.setLevel(logging.DEBUG)
@@ -208,14 +223,15 @@
         if ontology is None:
             ontology = read_ontology()
         self.ontology = ontology
         self.terms = self.ontology.terms
         self.store = store
         self._n_triples = 0
         self._initialize_graph()
+        self.workflow = Workflow(self)
 
     def add_structure(self, structure):
         """
         Add a structure to the knowledge graph.
 
         Parameters
         ----------
@@ -522,15 +538,15 @@
         >>> graph = KnowledgeGraph()
         >>> graph.add(("Alice", "likes", "Bob"))
         >>> graph.remove(("Alice", "likes", "Bob"))
         """
         modified_triple = self._modify_triple(triple)
         return self.graph.remove(modified_triple)
 
-    def create_node(self, namestring, classtype):
+    def create_node(self, namestring, classtype, label=None):
         """
         Create a new node in the graph.
 
         Parameters
         ----------
         namestring : str
             The name of the node.
@@ -541,14 +557,16 @@
         -------
         URIRef
             The newly created node.
 
         """
         item = URIRef(namestring)
         self.add((item, RDF.type, classtype))
+        if label is not None:
+            self.add((item, RDFS.label, Literal(_clean_string(label))))
         return item
 
     def _initialize_graph(self):
         """
         Create the RDF Graph from the data stored
 
         Parameters
@@ -640,16 +658,15 @@
         composition = list(
             [
                 k[2].toPython()
                 for k in self.triples((material, CMSO.hasElementRatio, None))
             ]
         )
         crystalstructure = self.value(material, CMSO.hasStructure)
-        spacegroup = self.value(crystalstructure, CMSO.hasSpaceGroup)
-        spacegroupsymbol = self.value(spacegroup, CMSO.hasSpaceGroupSymbol).toPython()
+        spacegroupsymbol = self.value(crystalstructure, CMSO.hasSpaceGroupSymbol).toPython()
 
         lattice = self.value(sample, CMSO.hasNumberOfAtoms).toPython()
         defect_types = list([self.value(d, RDF.type).toPython() for d in defects])
         prop_nodes = list(
             [k[2] for k in self.triples((sample, CMSO.hasCalculatedProperty, None))]
         )
         props = list([self.value(prop_node, RDFS.label) for prop_node in prop_nodes])
@@ -693,14 +710,15 @@
 
     def visualise(
         self,
         styledict=None,
         rankdir="BT",
         hide_types=False,
         workflow_view=False,
+        sample_view=False,
         size=None,
         layout="neato",
     ):
         """
         Visualize the RDF tree of the Graph.
 
         Parameters
@@ -709,14 +727,16 @@
             If provided, allows customization of color and other properties.
         rankdir : str, optional
             The direction of the graph layout. Default is "BT" (bottom to top).
         hide_types : bool, optional
             Whether to hide the types in the visualization. Default is False.
         workflow_view : bool, optional
             Whether to enable the workflow view. Default is False.
+        sample_view : bool, optional
+            Whether to enable the sample view. Default is False.
         size : tuple, optional
             The size of the visualization. Default is None.
         layout : str, optional
             The name of the layout algorithm for the graph. Default is "neato".
 
         Returns
         -------
@@ -761,14 +781,15 @@
 
         return visualize_graph(
             self.graph,
             styledict=sdict,
             rankdir=rankdir,
             hide_types=hide_types,
             workflow_view=workflow_view,
+            sample_view=sample_view,
             size=size,
             layout=layout,
         )
 
     def write(self, filename, format="json-ld"):
         """
         Write the serialised version of the graph to a file
@@ -785,15 +806,30 @@
         -------
         None
         """
 
         with open(filename, "w") as fout:
             fout.write(self.graph.serialize(format=format))
 
-    def archive(self, package_name, format="turtle", compress=True):
+    def close(self, filename, format="json-ld"):
+        """
+        Close the graph and write to a file
+
+        Parameters
+        ----------
+        filename: string
+            name of output file
+
+        Returns
+        -------
+        None
+        """
+        self.write(filename, format=format)
+
+    def archive(self, package_name, format="turtle", compress=True, add_simulations=False):
         """
         Publish a dataset from graph including per atom quantities.
 
         Parameters:
         -----------
         package_name : str
             The name of the package to be created.
@@ -833,15 +869,15 @@
                 raise ValueError(f"{package_name} tarball already exists")
 
         os.mkdir(package_name)
         structure_store = f"{package_name}/rdf_structure_store"
         os.mkdir(structure_store)
 
         # now go through each sample, and copy the file, at the same time fix the paths
-        for sample in self.samples:
+        for sample in self.sample_ids:
             filepath = self.value(URIRef(f"{sample}_Position"), CMSO.hasPath).toPython()
             shutil.copy(filepath, structure_store)
 
             # now we have to remove the old path, and fix new
             for val in ["Position", "Species"]:
                 self.remove((URIRef(f"{sample}_{val}"), CMSO.hasPath, None))
 
@@ -850,14 +886,28 @@
                 self.add(
                     (
                         URIRef(f"{sample}_{val}"),
                         CMSO.hasPath,
                         Literal(new_relpath, datatype=XSD.string),
                     )
                 )
+        #copy simulation files if needed
+        if add_simulations:
+            sim_store = f"{package_name}/simulation_store"
+            os.mkdir(sim_store)
+            activities = self.activity_ids
+            for activity in activities:
+                path = self.value(activity, CMSO.hasPath)
+                if path is not None:
+                    newpath = "/".join([sim_store, activity.toPython()])
+                    shutil.copytree(path, newpath)
+
+                    #remove old path
+                    self.remove((activity, CMSO.hasPath, None))
+                    self.add((activity, CMSO.hasPath, Literal(newpath, datatype=XSD.string)))
 
         triple_file = os.path.join(package_name, "triples")
         self.write(triple_file, format=format)
 
         if compress:
             with tarfile.open(f"{package_name}.tar.gz", "w:gz") as tar:
                 tar.add(package_name, arcname=os.path.basename(package_name))
@@ -1036,21 +1086,53 @@
         """
         Number of samples in the Graph
         """
 
         return len([x for x in self.triples((None, RDF.type, CMSO.AtomicScaleSample))])
 
     @property
-    def samples(self):
+    def sample_ids(self):
         """
         Returns a list of all Samples in the graph
         """
 
         return [x[0] for x in self.triples((None, RDF.type, CMSO.AtomicScaleSample))]
 
+    @property
+    def sample_names(self):
+        """
+        Returns a list of all Sample names in the graph
+        """
+        samples = [x[0] for x in self.triples((None, RDF.type, CMSO.AtomicScaleSample))]
+        samples_names = []
+        for sample in samples:
+            sample_name = self.value(sample, RDFS.label)
+            if sample_name is not None:
+                samples_names.append(sample_name.toPython())
+            else:
+                samples_names.append(sample.toPython())
+        return samples_names
+
+    @property
+    def samples(self):
+        sample_ids = self.sample_ids
+        sample_names = self.sample_names
+        sample_objects = []
+        for ids, name in zip(sample_ids, sample_names):
+            sample_objects.append(Sample(name, ids, self))
+        return sample_objects
+
+    @property
+    def activity_ids(self):
+        """
+        Returns a list of all Samples in the graph
+        """
+
+        return [x[0] for x in self.triples((None, RDF.type, PROV.Activity))]
+    
     def iterate_graph(self, item, create_new_graph=False):
         """
         Iterate through the graph starting from the given item.
 
         Parameters
         ----------
         item : object
@@ -1092,15 +1174,28 @@
         """
 
         self.iterate_graph(sample, create_new_graph=True)
         if no_atoms:
             na = self.sgraph.value(sample, CMSO.hasNumberOfAtoms).toPython()
             return self.sgraph, na
         return self.sgraph
-
+    
+    def get_label(self, item):
+        label = self.graph.value(item, RDFS.label)
+        if label is not None:
+            return label.toPython()
+
+    def get_sample_label(self, sample):
+        label = self.get_label(sample)
+        return label
+    
+    def change_label(self, sample, label):
+        self.graph.remove((sample, RDFS.label, None))
+        self.graph.add((sample, RDFS.label, Literal(label, datatype=XSD.string)))
+    
     def get_system_from_sample(self, sample):
         """
         Get a pyscal :py:class:`atomrdf.structure.System` from the selected sample
 
         Parameters
         ----------
         sample: string
@@ -1139,42 +1234,260 @@
         at = Atoms()
         at.from_dict(atoms)
         sys = System()
         sys.box = cell_vectors
         sys.atoms = at
         sys.sample = sample
         sys.graph = self
+        sys._name = sample.toPython().split('sample:')[-1]
         return sys
 
-    def to_file(self, sample, filename=None, format="poscar"):
+    def to_file(self, sample, filename=None, format="poscar", add_sample_id=True,
+        input_data=None, pseudopotentials=None, 
+                kspacing=None, kpts=None, 
+                koffset=(0, 0, 0), 
+                crystal_coordinates=False):
         """
         Save a given sample to a file
 
         Parameters
         ----------
         sample
             ID of the sample
 
         filename: string
             name of output file
 
-        format: string, {"lammps-dump","lammps-data", "poscar"}
+        format: string, {"lammps-dump","lammps-data", "poscar", 'cif', 'quantum-espresso'}
             or any format supported by ase
 
+        input_data : str, optional
+            Additional input data to include in the output file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        pseudopotentials : str, optional
+            The path to the pseudopotentials file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        kspacing : float, optional
+            The k-spacing value to include in the output file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        kpts : list, optional
+            A list of k-points to include in the output file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        koffset : tuple, optional
+            The k-offset values to include in the output file. Defaults to (0, 0, 0).
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        crystal_coordinates : bool, optional
+            Whether to include crystal coordinates in the output file. Defaults to False.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+
         Returns
         -------
         None
         """
 
         if filename is None:
             filename = os.path.join(os.getcwd(), "out")
 
         sys = self.get_system_from_sample(sample)
+        sys.to_file(filename=filename, format=format, add_sample_id=add_sample_id, input_data=input_data, 
+                pseudopotentials=pseudopotentials, kspacing=kspacing, 
+                kpts=kpts, koffset=koffset, crystal_coordinates=crystal_coordinates)
+
+    def enable_workflow(self, workflow_object, workflow_environment=None, workflow_module=None):
+        self.workflow.inform_graph(workflow_object, 
+                        workflow_environment=workflow_environment, 
+                        workflow_module=workflow_module)
+        
+    def add_workflow(self, job, workflow_environment=None, workflow_module=None, job_dicts=None,
+                    add_intermediate_jobs=False):
+        self.workflow.to_graph(job, workflow_environment=workflow_environment, 
+                            workflow_module=workflow_module, 
+                            job_dicts=job_dicts,
+                            add_intermediate_jobs=add_intermediate_jobs)
+    
+    def find_property(self, label):
+        prop_list = list(self.graph.triples((None, RDFS.label, label)))
+        if len(prop_list) == 0:
+            raise RuntimeError(f'Property {label} not found in the graph')
+        prop = prop_list[0][0]
+        return prop        
+
+    def get_string_label(self, item):
+        label = self.get_label(item)
+
+        if label is None:
+            try:
+                label = str(item.toPython())
+            except:
+                label = str(item)
+        
+        if "activity" in label:
+            method = self.value(item, ASMO.hasComputationalMethod)
+            if method is not None:
+                method_name = self.value(method, RDF.type)
+                if method_name is not None:
+                    label = method_name.toPython().split("/")[-1]
+        return label
+
+    def _add_to_dict(self, prop, indict):
+        name = _name(prop)
+        if name not in indict.keys():
+            indict[name] = {}
+            indict[name]['found'] = False
+            indict[name]['label'] = self.get_string_label(prop)
+
+    def _get_ancestor(self, prop, prov):
+        #note that only one operation and parent are present!
+        if isinstance(prop, str):
+            prop = URIRef(prop)
+        propname = _name(prop)
+
+        operation = [x[1] for x in self.triples((prop, ASMO.wasCalculatedBy, None))]
+        if len(operation) > 0:
+            parent = [x[2] for x in self.triples((prop, ASMO.wasCalculatedBy, None))]
+            operation = operation[0]
+            parent = parent[0]        
+            prov[propname]['operation'] = 'output_parameter'
+            prov[propname]['inputs'] = {}
+            prov[propname]['inputs']['0'] = _name(parent)
+            self._add_to_dict(parent, prov)
+            prov[_name(parent)]['inputs'] = {}
+            associated_samples = [x[0] for x in self.triples((None, PROV.wasGeneratedBy, parent))]
+            for count, sample in enumerate(associated_samples):
+                prov[_name(parent)]['inputs'][str(count)] = _name(sample)
+                self._add_to_dict(sample, prov)
+            prov[_name(parent)]['found'] = True
+            prov[_name(parent)]['operation'] = 'sample_for_activity'
+                
+        else:
+            operation = [x[1] for x in self.triples((None, None, prop))]
+            parent = [list(self.triples((None, op, prop)))[0][0] for op in operation]
+            if len(operation) == 0:
+                prov[propname]['found'] = True
+                return prov
+            operation = operation[0]
+            parent = parent[0]
+
+            if operation.toPython() == "http://purls.helmholtz-metadaten.de/asmo/hasInputParameter":
+                #print(f'we ran 1 for {operation.toPython()}')
+                prov[propname]['operation'] = 'input_parameter'
+                prov[propname]['inputs'] = {}
+                prov[propname]['inputs']['0'] = _name(parent)
+                self._add_to_dict(parent, prov)
+                prov[_name(parent)]['inputs'] = {}
+                associated_samples = [x[0] for x in self.triples((None, PROV.wasGeneratedBy, parent))]
+                for count, sample in enumerate(associated_samples):
+                    prov[_name(parent)]['inputs'][str(count)] = _name(sample)
+                    self._add_to_dict(sample, prov)
+                prov[_name(parent)]['found'] = True
+                prov[_name(parent)]['operation'] = 'sample_for_activity'
+
+            elif operation.toPython() == "http://purls.helmholtz-metadaten.de/cmso/hasCalculatedProperty":
+                #print(f'we ran 2 for {operation.toPython()}')
+                prov[propname]['operation'] = 'output_parameter'
+                prov[propname]['inputs'] = {}
+                prov[propname]['inputs']['0'] = _name(parent)
+                self._add_to_dict(parent, prov)            
+                prov[_name(parent)]['found'] = True
+                prov[_name(parent)]['operation'] = 'sample_output'
+            
+            elif operation == MATH.hasSum:
+                addends = list(x[2] for x in self.triples((parent, MATH.hasAddend, None)))
+                prov[propname]['operation'] = 'addition'
+                prov[propname]['inputs'] = {}
+                for count, term in enumerate(addends):
+                    prov[propname]['inputs'][f'{count}'] = _name(term)
+                    self._add_to_dict(term, prov)
+            
+            elif operation == MATH.hasDifference:
+                minuend = self.value(parent, MATH.hasMinuend)
+                subtrahend = self.value(parent, MATH.hasSubtrahend)
+                prov[propname]['operation'] = 'subtraction'
+                prov[propname]['inputs'] = {}
+                prov[propname]['inputs']['0'] = _name(minuend)
+                prov[propname]['inputs']['1'] = _name(subtrahend)
+                self._add_to_dict(minuend, prov)
+                self._add_to_dict(subtrahend, prov)
+            
+            elif operation == MATH.hasProduct:
+                factors = list(x[2] for x in self.triples((parent, MATH.hasFactor, None)))
+                prov[propname]['operation'] = 'multiplication'
+                prov[propname]['inputs'] = {}
+                for count, term in enumerate(factors):
+                    prov[propname]['inputs'][f'{count}'] = _name(term)
+                    self._add_to_dict(term, prov)
+            
+            elif operation == MATH.hasQuotient:
+                divisor = self.value(parent, MATH.hasDivisor)
+                dividend = self.value(parent, MATH.hasDividend)
+                prov[propname]['operation'] = 'division'
+                prov[propname]['inputs'] = {}
+                prov[propname]['inputs']['0'] = _name(divisor)
+                prov[propname]['inputs']['1'] = _name(dividend)
+                self._add_to_dict(divisor, prov)
+                self._add_to_dict(dividend, prov)
+
+        prov[propname]['found'] = True
+        return prov
+    
+    def generate_provenance(self, prop=None, label=None, visualize=False):
+        if (prop is None) and (label is None):
+            raise ValueError('Either prop or label must be provided')
+        
+        if prop is None:
+            prop = self.find_property(label)
+        
+        name = _name(prop)
+        prov = {}
+        self._add_to_dict(prop, prov)
+
+        done = False
+        while not done:
+            done = True
+            keys = list(prov.keys()) 
+            for prop in keys:
+                if not prov[prop]['found']:
+                    prov = self._get_ancestor(prop, prov)
+                    done = False
+        
+        if visualize:
+            return visualize_provenance(prov)
+        
+        return prov
+    
 
-        if format == "ase":
-            return sys.write.ase()
-        elif format == "poscar":
-            asesys = sys.write.ase()
-            write(filename, asesys, format="vasp")
+    def query_structure_from_mp(self, api_key, chemical_system=None, material_ids=None, is_stable=True,
+                        conventional=True,
+                        add_to_graph=True):
+        docs = amp.query_mp(api_key, 
+                            chemical_system = chemical_system, 
+                            material_ids = material_ids, 
+                            is_stable = is_stable)
+        structures = []
+        for doc in docs:
+            struct = doc['structure']
+            if conventional:
+                aseatoms = struct.to_conventional().to_ase_atoms()
+            else:
+                aseatoms = struct.to_primitive().to_ase_atoms()
+            
+            sys = System.read.ase(aseatoms)
+            
+            symmetry = doc['symmetry']
+
+            if add_to_graph:
+                sys.graph = self
+                sys.to_graph()
+                
+                targets = [None, symmetry['symbol'], symmetry['number'], None, None, None]
+                sys._add_crystal_structure(targets=targets)
+
+                #add energy
+                self.add_calculated_quantity(sys.sample, 
+                                            'EnergyPerAtom', 
+                                            doc['energy_per_atom'], 
+                                            unit='EV')  
+                structures.append(sys)
+        if len(structures) == 1:
+            return structures[0]
         else:
-            asesys = sys.write.ase()
-            write(filename, asesys, format=format)
+            return structures
```

### Comparing `atomrdf-0.6.4/atomrdf/json_io.py` & `atomrdf-0.8.1/atomrdf/json_io.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/namespace.py` & `atomrdf-0.8.1/atomrdf/namespace.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,7 +67,12 @@
 file_location = os.path.dirname(__file__)
 
 CMSO = Namespace(os.path.join(file_location, "data/cmso.owl"))
 PLDO = Namespace(os.path.join(file_location, "data/pldo.owl"))
 PODO = Namespace(os.path.join(file_location, "data/podo.owl"))
 ASMO = Namespace(os.path.join(file_location, "data/asmo.owl"))
 PROV = RDFLibNamespace("http://www.w3.org/ns/prov#")
+MDO = RDFLibNamespace("https://w3id.org/mdo/calculation/")
+
+MATH = RDFLibNamespace("http://purls.helmholtz-metadaten.de/asmo/")
+UNSAFECMSO = RDFLibNamespace("http://purls.helmholtz-metadaten.de/cmso/")
+UNSAFEASMO = RDFLibNamespace("http://purls.helmholtz-metadaten.de/asmo/")
```

### Comparing `atomrdf-0.6.4/atomrdf/network/network.py` & `atomrdf-0.8.1/atomrdf/network/network.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/network/ontology.py` & `atomrdf-0.8.1/atomrdf/network/ontology.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+"""
+Documentation for the ontology module.
+
+Updates needed
+--------------
+ASMO module
+
+- Add math operations, see sample.py for the complete list of items - at the moment, 4 cardinal operations,
+but maybe more will be needed.
+
+- StructureOperation: StructureRotation and associated vectors, see structure.py
+"""
 import os
 from atomrdf.network.network import OntologyNetwork
 
 
 def read_ontology():
     """
     Read in ontologies and perform necessary operations.
@@ -10,18 +22,18 @@
     -------
     combo: OntologyNetwork, Combined ontology network.
     """
     # read in ontologies
     file_location = os.path.dirname(__file__).split("/")
     file_location = "/".join(file_location[:-1])
 
-    cmso = OntologyNetwork(os.path.join(file_location, "data/cmso.owl"))
-    pldo = OntologyNetwork(os.path.join(file_location, "data/pldo.owl"))
-    podo = OntologyNetwork(os.path.join(file_location, "data/podo.owl"))
-    asmo = OntologyNetwork(os.path.join(file_location, "data/asmo.owl"))
+    cmso = OntologyNetwork(os.path.join(file_location, "data/cmso.owl")) #eb8a58a60af1759afc4115ae395ad62ddffb6844
+    pldo = OntologyNetwork(os.path.join(file_location, "data/pldo.owl")) #d15d27712e3f64b405d75c70ad970c9d54ff0b51
+    podo = OntologyNetwork(os.path.join(file_location, "data/podo.owl")) #6a74d511c5b78042e1cb7a6e76e948fa56de598e
+    asmo = OntologyNetwork(os.path.join(file_location, "data/asmo.owl")) #c7e2da99b9126844f19f225c6a10cdb01aeb55e6
 
     # combine them
     combo = cmso + pldo + podo + asmo
 
     # add namespaces
     combo.add_namespace("prov", "http://www.w3.org/ns/prov#")
     combo.add_namespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
@@ -59,32 +71,40 @@
 
     # add paths
 
     # General fixes
     combo.add_path(("cmso:CrystalStructure", "cmso:hasAltName", "string"))
 
     # interontology paths
+    #CMSO -> PODO VACANCY
     combo.add_path(("cmso:Material", "cmso:hasDefect", "pldo:PlanarDefect"))
     combo.add_path(("cmso:Material", "cmso:hasDefect", "podo:Vacancy"))
-    combo.add_path(("cmso:SimulationCell", "podo:hasVacancyConcentration", "float"))
-    combo.add_path(("cmso:SimulationCell", "podo:hasNumberOfVacancies", "int"))
+    combo.add_path(("cmso:AtomicScaleSample", "podo:hasVacancyConcentration", "float"))
+    combo.add_path(("cmso:AtomicScaleSample", "podo:hasNumberOfVacancies", "int"))
+    
+    #CMSO -> PODO IMPURITY
+    combo.add_path(("cmso:Material", "cmso:hasDefect", "podo:SubstitutionalImpurity"))
+    combo.add_path(("cmso:Material", "cmso:hasDefect", "podo:InterstitialImpurity"))
+    combo.add_path(("cmso:AtomicScaleSample", "podo:hasNumberOfImpurityAtoms", "int"))
+    combo.add_path(("cmso:AtomicScaleSample", "podo:hasImpurityConcentration", "float"))
+    
     combo.add_path(
         ("cmso:ComputationalSample", "prov:wasDerivedFrom", "cmso:ComputationalSample")
     )
     combo.add_path(("cmso:ComputationalSample", "rdf:type", "prov:Entity"))
     combo.add_path(("cmso:AtomicScaleSample", "prov:wasGeneratedBy", "prov:Activity"))
-    combo.add_path(("asmo:StructureOptimization", "rdf:type", "prov:Activity"))
+    combo.add_path(("asmo:EnergyCalculation", "rdf:type", "prov:Activity"))
     combo.add_path(
-        ("asmo:StructureOptimization", "prov:wasAssociatedWith", "prov:SoftwareAgent")
+        ("asmo:EnergyCalculation", "prov:wasAssociatedWith", "prov:SoftwareAgent")
     )
     combo.add_path(
         (
             "cmso:ComputationalSample",
             "prov:wasGeneratedBy",
-            "asmo:StructureOptimization",
+            "asmo:EnergyCalculation",
         )
     )
     
     combo.add_path(("cmso:CalculatedProperty", "asmo:hasValue", "float"))
     combo.add_path(("cmso:CalculatedProperty", "rdfs:label", "string"))
     #how to handle units?
```

### Comparing `atomrdf-0.6.4/atomrdf/network/parser.py` & `atomrdf-0.8.1/atomrdf/network/parser.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/network/patch.py` & `atomrdf-0.8.1/atomrdf/network/patch.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/network/term.py` & `atomrdf-0.8.1/atomrdf/network/term.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/properties.py` & `atomrdf-0.8.1/atomrdf/properties.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/atomrdf/stores.py` & `atomrdf-0.8.1/atomrdf/stores.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from rdflib.store import NO_STORE, VALID_STORE
 from rdflib import plugin
 from rdflib import Graph, Literal
 
 import os
 
-# special methods; for supporting workflow envs
-from atomrdf.workflow import inform_graph
-
 
 def create_store(kg, store, identifier, store_file=None, structure_store=None):
     """
     Create a store based on the given parameters.
 
     Parameters:
     -----------
@@ -28,38 +25,30 @@
     Raises:
     -------
     ValueError
         If an unknown store type is provided.
 
     """
     kg.store_file = store_file
-    if store == "Memory":
+    if store in ["Memory", "memory"]:
         store_memory(
             kg,
             store,
             identifier,
             store_file=store_file,
             structure_store=structure_store,
         )
-    elif store == "SQLAlchemy":
+    elif store in ["SQLAlchemy", "db", "database", "sqlalchemy"]:
         store_alchemy(
             kg,
             store,
             identifier,
             store_file=store_file,
             structure_store=structure_store,
         )
-    elif type(store).__name__ == "Project":
-        store_pyiron(
-            kg,
-            store,
-            identifier,
-            store_file=store_file,
-            structure_store=structure_store,
-        )
     else:
         raise ValueError("Unknown store found!")
 
 
 def store_memory(kg, store, identifier, store_file=None, structure_store=None):
     """
     Store the knowledge graph in memory.
@@ -117,45 +106,14 @@
         raise ValueError("store file is needed if store is not memory")
 
     kg.graph = Graph(store="SQLAlchemy", identifier=identifier)
     uri = Literal(f"sqlite:///{store_file}")
     kg.graph.open(uri, create=True)
     kg.structure_store = _setup_structure_store(structure_store=structure_store)
 
-
-def store_pyiron(kg, store, identifier, store_file=None, structure_store=None):
-    """
-    Store the pyiron knowledge graph in a database.
-
-    Parameters
-    ----------
-    kg : pyiron.atomistics.structure.pyiron_atomistics.structure.AtomisticStructure
-        The pyiron knowledge graph to be stored.
-    store : pyiron.atomistics.structure.pyiron_atomistics.structure.AtomisticStructure
-        The store object where the knowledge graph will be stored.
-    identifier : str
-        The identifier for the knowledge graph.
-    store_file : str, optional
-        The path to the store file. If not provided, a default path will be used.
-    structure_store : str, optional
-        The path to the structure store. If not provided, a default path will be used.
-
-    Returns
-    -------
-    None
-
-    """
-    structure_store = os.path.join(store.path, "rdf_structure_store")
-    kg.structure_store = _setup_structure_store(structure_store=structure_store)
-    store_file = os.path.join(store.path, f"{store.name}.db")
-    store_alchemy(kg, store, identifier, store_file, structure_store=structure_store)
-    # finally update project object
-    inform_graph(store, kg)
-
-
 def _check_if_sqlalchemy_is_available():
     try:
         import sqlalchemy as sa
     except ImportError:
         raise RuntimeError("Please install the sqlalchemy package")
     try:
         import rdflib_sqlalchemy as rsa
```

### Comparing `atomrdf-0.6.4/atomrdf/structure.py` & `atomrdf-0.8.1/atomrdf/structure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 """
-This module provides functions for creating and manipulating atomic structures. It includes functions for creating crystals, 
-general lattices, dislocations, grain boundaries, and reading structures from files. The module also provides functionality for 
-adding interstitial impurities, substituting atoms, deleting atoms, and adding vacancies. 
-The structures can be converted to RDF graphs using the atomrdf library. 
+This module provides functions for creating and manipulating atomic structures. It includes functions for creating crystals,
+general lattices, dislocations, grain boundaries, and reading structures from files. The module also provides functionality for
+adding interstitial impurities, substituting atoms, deleting atoms, and adding vacancies.
+The structures can be converted to RDF graphs using the atomrdf library.
 The main object in this module is the System class, which extends the functionality of the pyscal3.core.System class and provides additional methods for working with atomic structures.
 """
 
 import numpy as np
 import copy
 from functools import partial, update_wrapper
 import os
 import yaml
 import uuid
 import json
 import shutil
 import tarfile
 import warnings
+from ase.io import write
 
 import pyscal3.structure_creator as pcs
 from pyscal3.grain_boundary import GrainBoundary
 from pyscal3.atoms import AttrSetter, Atoms
 import pyscal3.core as pc
 from pyscal3.core import structure_dict, element_dict
+import pyscal3.operations.input as inputmethods
+import pyscal3.operations.serialize as serialize
+from pyscal3.formats.ase import convert_snap
 
 import atomrdf.json_io as json_io
 import atomrdf.properties as prp
 
 from rdflib import Graph, Literal, Namespace, XSD, RDF, RDFS, BNode, URIRef
-from atomrdf.namespace import CMSO, PLDO, PODO
+from atomrdf.namespace import CMSO, PLDO, PODO, UNSAFEASMO, PROV
+
+from atomman.defect.Dislocation import Dislocation
+import atomman as am
+import atomman.unitconvert as uc
 
 # read element data file
 file_location = os.path.dirname(__file__).split("/")
 file_location = "/".join(file_location[:-1])
 file_location = os.path.join(os.path.dirname(__file__), "data/element.yml")
 with open(file_location, "r") as fin:
     element_indetifiers = yaml.safe_load(fin)
 
-
 def _make_crystal(
     structure,
     lattice_constant=1.00,
     repetitions=None,
     ca_ratio=1.633,
     noise=0,
     element=None,
     primitive=False,
     graph=None,
     names=False,
+    label=None,
 ):
     """
     Create a crystal structure using the specified parameters.
 
     Parameters:
     -----------
     structure : str
@@ -91,28 +99,30 @@
 
     s = System(graph=graph, names=names)
     s.box = box
     s.atoms = atoms
     s.atoms._lattice = structure
     s.atoms._lattice_constant = lattice_constant
     s._structure_dict = sdict
+    s.label = label
     s.to_graph()
     return s
 
 
 def _make_general_lattice(
     positions,
     types,
     box,
     lattice_constant=1.00,
     repetitions=None,
     noise=0,
     element=None,
     graph=None,
     names=False,
+    label=None,
 ):
     """
     Generate a general lattice structure.
 
     Parameters:
     -----------
     positions : array_like
@@ -153,14 +163,15 @@
     )
     s = System(graph=graph, names=names)
     s.box = box
     s.atoms = atoms
     s.atoms._lattice = "custom"
     s.atoms._lattice_constant = lattice_constant
     s._structure_dict = sdict
+    s.label = label
     s.to_graph()
 
     return s
 
 
 def _make_dislocation(
     burgers_vector,
@@ -173,14 +184,15 @@
     lattice_constant=1.00,
     repetitions=None,
     ca_ratio=1.633,
     noise=0,
     primitive=False,
     graph=None,
     names=False,
+    label=None,
 ):
     """
     Generate a dislocation structure. Wraps the atomman.defect.Dislocation class.
 
     Parameters
     ----------
     burgers_vector : numpy array of length 3
@@ -230,17 +242,14 @@
     following Voigt notation: "C11", "C12", "C13", "C14", "C15", "C16", "C22", "C23", "C24", "C25", "C26", "C33", "C34",
     "C35", "C36", "C44", "C45", "C46", "C55", "C56", "C66". The values should be given in GPa.
 
     The dislocation_type parameter can be set to "monopole" or "periodicarray". If set to "monopole", a single dislocation
     will be generated. If set to "periodicarray", a periodic array of dislocations will be generated.
 
     """
-    from atomman.defect.Dislocation import Dislocation
-    import atomman as am
-    import atomman.unitconvert as uc
 
     if structure is not None:
         # create a structure with the info
         input_structure = _make_crystal(
             structure,
             lattice_constant=lattice_constant,
             repetitions=repetitions,
@@ -311,28 +320,31 @@
     atom_dict = {"positions": positions, "types": types, "species": species}
     atom_obj = Atoms()
     atom_obj.from_dict(atom_dict)
     output_structure = System()
     output_structure.box = box
     output_structure.atoms = atom_obj
     output_structure = output_structure.modify.remap_to_box()
+    output_structure.label = label
+
     return output_structure
 
 
 def _make_grain_boundary(
     axis,
     sigma,
     gb_plane,
     structure=None,
     element=None,
     lattice_constant=1,
     repetitions=(1, 1, 1),
     overlap=0.0,
     graph=None,
     names=False,
+    label=None,
 ):
     """
     Create a grain boundary system.
 
     Parameters:
     -----------
     axis : tuple or list
@@ -379,14 +391,15 @@
         )
     s = System(graph=graph, names=names)
     s.box = box
     s.atoms = atoms
     s.atoms._lattice = structure
     s.atoms._lattice_constant = lattice_constant
     s._structure_dict = sdict
+    s.label = label
     s.to_graph()
     gb_dict = {
         "GBPlane": " ".join(np.array(gb_plane).astype(str)),
         "RotationAxis": axis,
         "MisorientationAngle": gb.theta,
         "GBType": gb.find_gb_character(),
         "sigma": gb.sigma,
@@ -401,14 +414,15 @@
     graph=None,
     names=False,
     species=None,
     lattice=None,
     lattice_constant=None,
     basis_box=None,
     basis_positions=None,
+    label=None,
 ):
     """
     Read in structure from file or ase object
 
     Parameters
     ----------
     filename: string
@@ -439,15 +453,15 @@
         specify the basis unit cell. Not required if lattice is provided
 
     basis_positions: nX3 list, optional
         specify the relative positions of atoms in the unit cell. Not required if lattice is provided
 
     Returns
     -------
-    atomrdf.System    
+    atomrdf.System
     """
     datadict = {}
     if lattice is not None:
         if lattice in structure_dict.keys():
             datadict = structure_dict[lattice]["conventional"]
         datadict["lattice"] = lattice
     if lattice_constant is not None:
@@ -462,14 +476,15 @@
         format=format,
         species=species,
         graph=graph,
         names=names,
         warn_read_in=False,
     )
     s.lattice_properties = datadict
+    s.label = label
     s.to_graph()
     return s
 
 
 class System(pc.System):
 
     create = AttrSetter()
@@ -531,23 +546,35 @@
             compressed=compressed,
             customkeys=customkeys,
             species=species,
         )
 
         # this is the sample which will be stored
         self.sample = None
+        self.label = None
         # the graph object should also be attached
         # for post-processing of structures
         self.graph = graph
         self.names = names
+        self._material = None
         self._atom_ids = None
         if source is not None:
             self.__dict__.update(source.__dict__)
 
-        # assign attributes
+        self.write = AttrSetter()
+        mapdict = {}
+        mapdict['ase'] = update_wrapper(partial(self.to_file, format='ase'), self.to_file)
+        mapdict['pyiron'] = update_wrapper(partial(self.to_file, format='pyiron'), self.to_file)
+        mapdict['file'] = self.to_file
+        mapdict['dict'] = update_wrapper(partial(serialize.serialize, self, return_type='dict'), serialize.serialize)
+        mapdict['json'] = update_wrapper(partial(serialize.serialize, self, return_type='json'), serialize.serialize)
+        mapdict['pydantic'] = update_wrapper(partial(serialize.serialize, self, return_type='model'), serialize.serialize)
+        mapdict['json_file'] = update_wrapper(partial(serialize.serialize, self, return_type='file'), serialize.serialize)
+        self.write._add_attribute(mapdict)
+
         self.schema = AttrSetter()
         mapdict = {
             "material": {
                 "element_ratio": partial(prp.get_chemical_composition, self),
                 "crystal_structure": {
                     "name": partial(prp.get_crystal_structure_name, self),
                     "spacegroup_symbol": partial(prp.get_spacegroup_symbol, self),
@@ -570,14 +597,24 @@
                 "position": partial(prp.get_position, self),
                 "species": partial(prp.get_species, self),
             },
         }
 
         self.schema._add_attribute(mapdict)
 
+    @property
+    def material(self):
+        if self._material is None:
+            self._material = self.graph.value(self.sample, CMSO.hasMaterial)
+        return self._material
+
+    @material.setter
+    def material(self, value):
+        self._material = value
+
     def delete(self, ids=None, indices=None, condition=None, selection=False):
         """
         Delete atoms from the structure.
 
         Parameters
         ----------
         ids : list, optional
@@ -648,15 +685,15 @@
                 for e, r in composition.items():
                     if e in element_indetifiers.keys():
                         element = self.graph.create_node(
                             element_indetifiers[e], CMSO.ChemicalElement
                         )
                         self.graph.add((chemical_species, CMSO.hasElement, element))
                         self.graph.add(
-                            (element, CMSO.hasSymbol, Literal(e, datatype=XSD.string))
+                            (element, CMSO.hasChemicalSymbol, Literal(e, datatype=XSD.string))
                         )
                         self.graph.add(
                             (
                                 element,
                                 CMSO.hasElementRatio,
                                 Literal(r, datatype=XSD.float),
                             )
@@ -685,14 +722,51 @@
                 },
             }
             outfile = os.path.join(
                 self.graph.structure_store, str(self._name).split(":")[-1]
             )
             json_io.write_file(outfile, datadict)
 
+    def add_vacancy(self, concentration, number=None):
+        """
+        Add Vacancy details which will be annotated by PODO
+
+        Parameters
+        ----------
+        concentration: float
+            vacancy concentration, value should be between 0-1
+
+        number: int
+            Number of atoms that were deleted, optional
+
+        Returns
+        -------
+        None
+        """
+        if self.graph is None:
+            return
+
+        vacancy = self.graph.create_node(f"{self._name}_Vacancy", PODO.Vacancy)
+        self.graph.add((self.material, CMSO.hasDefect, vacancy))
+        self.graph.add(
+            (
+                self.sample,
+                PODO.hasVacancyConcentration,
+                Literal(concentration, datatype=XSD.float),
+            )
+        )
+        if number is not None:
+            self.graph.add(
+                (
+                    self.sample,
+                    PODO.hasNumberOfVacancies,
+                    Literal(number, datatype=XSD.integer),
+                )
+            )
+
     def substitute_atoms(
         self,
         substitution_element,
         ids=None,
         indices=None,
         condition=None,
         selection=False,
@@ -741,14 +815,17 @@
             atomtype = rtype_dict[substitution_element]
         else:
             maxtype = max(self.atoms["types"]) + 1
 
         for x in delete_ids:
             self.atoms["species"][x] = substitution_element
             self.atoms["types"][x] = maxtype
+        #impurity metrics
+        no_of_impurities = len(delete_ids)
+        conc_of_impurities = no_of_impurities/self.natoms
 
         # operate on the graph
         if self.graph is not None:
             chemical_species = self.graph.value(self.sample, CMSO.hasSpecies)
             # start by cleanly removing elements
             for s in self.graph.triples((chemical_species, CMSO.hasElement, None)):
                 element = s[2]
@@ -772,15 +849,15 @@
                 for e, r in composition.items():
                     if e in element_indetifiers.keys():
                         element = self.graph.create_node(
                             element_indetifiers[e], CMSO.ChemicalElement
                         )
                         self.graph.add((chemical_species, CMSO.hasElement, element))
                         self.graph.add(
-                            (element, CMSO.hasSymbol, Literal(e, datatype=XSD.string))
+                            (element, CMSO.hasChemicalSymbol, Literal(e, datatype=XSD.string))
                         )
                         self.graph.add(
                             (
                                 element,
                                 CMSO.hasElementRatio,
                                 Literal(r, datatype=XSD.float),
                             )
@@ -808,31 +885,47 @@
                     "label": "species",
                 },
             }
             outfile = os.path.join(
                 self.graph.structure_store, str(self._name).split(":")[-1]
             )
             json_io.write_file(outfile, datadict)
+            self.add_triples_for_substitutional_impurities(conc_of_impurities, no_of_impurities=no_of_impurities)
+
+    def add_triples_for_substitutional_impurities(self, conc_of_impurities, no_of_impurities=None):
+        defect = self.graph.create_node(f"{self._name}_SubstitutionalImpurity", PODO.SubstitutionalImpurity)
+        self.graph.add((self.material, CMSO.hasDefect, defect))
+        self.graph.add((self.sample, PODO.hasImpurityConcentration, Literal(conc_of_impurities, datatype=XSD.float)))
+        if no_of_impurities is not None:
+            self.graph.add((self.sample, PODO.hasNumberOfImpurityAtoms, Literal(no_of_impurities, datatype=XSD.integer)))
 
     def add_interstitial_impurities(
-        self, element, void_type="tetrahedral", lattice_constant=None, threshold=0.01
+        self, element, void_type="tetrahedral",
+        lattice_constant=None,
+        threshold=0.01
     ):
         """
         Add interstitial impurities to the System
 
         Parameters
         ----------
         element: string or list
             Chemical symbol of the elements/elements to be added
             `element = 'Al'` will add one interstitial while `element = ['Al', 'Al']` or `element = ['Al', 'Li']` will add
             two impurities
 
         void_type: string
             type of void to be added.  {`tetrahedral`, `octahedral`}
 
+        lattice_constant: float, optional
+            lattice constant of the system. Required only for octahedral voids
+
+        threshold: float, optional
+            threshold for the distance from the lattice constant for octahedral voids to account for fluctuations in atomic positions
+
         Returns
         -------
         System:
             system with the added impurities
 
         Notes
         -----
@@ -845,14 +938,15 @@
         if void_type == "tetrahedral":
             element = np.atleast_1d(element)
             self.find.neighbors(method="voronoi", cutoff=0.1)
             verts = self.unique_vertices
             randindex = np.random.randint(0, len(verts), len(element))
             randpos = np.array(verts)[randindex]
 
+
         elif void_type == "octahedral":
             if lattice_constant is None:
                 if "lattice_constant" in self.lattice_properties.keys():
                     lattice_constant = self.lattice_properties["lattice_constant"]
                 else:
                     raise ValueError(
                         "lattice constant is needed for octahedral voids, please provide"
@@ -882,14 +976,17 @@
             if not len(randpos) == len(element):
                 raise ValueError("not enough octahedral positions found!")
 
         else:
             raise ValueError("void_type can only be tetrahedral/octahedral")
 
         # create new system with the atoms added
+        no_of_impurities = len(randpos)
+        conc_of_impurities = no_of_impurities/self.natoms
+
         sysn = System(source=self.add_atoms({"positions": randpos, "species": element}))
         # attach graphs
         sysn.sample = self.sample
         sysn.graph = self.graph
 
         # now we have to verify the triples correctly and add them in
         if self.graph is not None:
@@ -927,15 +1024,15 @@
                 for e, r in composition.items():
                     if e in element_indetifiers.keys():
                         element = self.graph.create_node(
                             element_indetifiers[e], CMSO.ChemicalElement
                         )
                         self.graph.add((chemical_species, CMSO.hasElement, element))
                         self.graph.add(
-                            (element, CMSO.hasSymbol, Literal(e, datatype=XSD.string))
+                            (element, CMSO.hasChemicalSymbol, Literal(e, datatype=XSD.string))
                         )
                         self.graph.add(
                             (
                                 element,
                                 CMSO.hasElementRatio,
                                 Literal(r, datatype=XSD.float),
                             )
@@ -964,16 +1061,25 @@
                 },
             }
             outfile = os.path.join(
                 self.graph.structure_store, str(self._name).split(":")[-1]
             )
             json_io.write_file(outfile, datadict)
 
+            self.add_triples_for_interstitial_impurities(conc_of_impurities, no_of_impurities=no_of_impurities)
         return sysn
 
+    def add_triples_for_interstitial_impurities(self, conc_of_impurities, no_of_impurities=None):
+        defect = self.graph.create_node(f"{self._name}_InterstitialImpurity", PODO.InterstitialImpurity)
+        self.graph.add((self.material, CMSO.hasDefect, defect))
+        self.graph.add((self.sample, PODO.hasImpurityConcentration, Literal(conc_of_impurities, datatype=XSD.float)))
+        if no_of_impurities is not None:
+            self.graph.add((self.sample, PODO.hasNumberOfImpurityAtoms, Literal(no_of_impurities, datatype=XSD.integer)))
+
+
     def __delitem__(self, val):
         """
         Delete item(s) from the structure.
 
         Parameters
         ----------
         val : int or list of int
@@ -986,14 +1092,134 @@
 
         """
         if isinstance(val, int):
             val = [val]
         # now the graph has to be updated accordingly
         self.delete(indices=list(val))
 
+    def write_poscar_id(self, outfile):
+        lines = []
+        with open(outfile, "r") as fin:
+            for line in fin:
+                lines.append(line)
+        lines[0] = self.sample.toPython() + "\n"
+        with open(outfile, "w") as fout:
+            for line in lines:
+                fout.write(line)
+
+    def write_quatum_espresso_id(self, outfile):
+        lines = []
+        lines.append(f"! {self.sample.toPython()}\n")
+        with open(outfile, "r") as fin:
+            for line in fin:
+                lines.append(line)
+        with open(outfile, "w") as fout:
+            for line in lines:
+                fout.write(line)
+
+    def to_file(self, filename=None, format='lammps-dump', customkeys=None, customvals=None,
+                compressed=False, timestep=0, species=None,  add_sample_id=True,
+                input_data=None, pseudopotentials=None,
+                kspacing=None, kpts=None,
+                koffset=(0, 0, 0),
+                crystal_coordinates=False):
+        """
+        Write the structure to a file in the specified format.
+
+        Parameters
+        ----------
+        outfile : str
+            The path to the output file.
+        format : str, optional
+            The format of the output file. Defaults to 'lammps-dump'.
+        customkeys : list, optional
+            A list of custom keys to include in the output file. Defaults to None.
+            Only valid if format is 'lammps-dump'.
+        customvals : list, optional
+            A list of custom values corresponding to the custom keys. Defaults to None.
+            Only valid if format is 'lammps-dump'.
+        compressed : bool, optional
+            Whether to compress the output file. Defaults to False.
+        timestep : int, optional
+            The timestep value to include in the output file. Defaults to 0.
+            Only valid if format is 'lammps-dump'.
+        species : list, optional
+            A list of species to include in the output file. Defaults to None.
+            Only valid for ASE, if species is not specified.
+        add_sample_id : bool, optional
+            Whether to add a sample ID to the output file. Defaults to True.
+            Only valid for poscar and quantum-espresso formats.
+        input_data : str, optional
+            Additional input data to include in the output file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        pseudopotentials : str, optional
+            The path to the pseudopotentials file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        kspacing : float, optional
+            The k-spacing value to include in the output file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        kpts : list, optional
+            A list of k-points to include in the output file. Defaults to None.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        koffset : tuple, optional
+            The k-offset values to include in the output file. Defaults to (0, 0, 0).
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+        crystal_coordinates : bool, optional
+            Whether to include crystal coordinates in the output file. Defaults to False.
+            Only valid for quantum-espresso format. See ASE write docs for more information.
+
+        Returns
+        -------
+        None
+        """
+        if filename is None:
+            outfile = f"structure.out"
+        else:
+            outfile = filename
+
+        if format == "ase":
+            asesys = convert_snap(self)
+            if self.sample is not None:
+                asesys.info["sample_id"] = self.sample
+            return asesys
+        
+        elif format == "pyiron":
+            from pyiron_atomistics.atomistics.structure.atoms import ase_to_pyiron
+            asesys = convert_snap(self)
+            pyironsys = ase_to_pyiron(asesys)
+            if self.sample is not None:
+                pyironsys.info["sample_id"] = self.sample            
+            return pyironsys
+
+        elif format == "poscar":
+            asesys = convert_snap(self)
+            write(outfile, asesys, format="vasp")
+            if add_sample_id and (self.sample is not None):
+                self.write_poscar_id(outfile)
+        
+        elif format == "lammps-dump":
+            inputmethods.to_file(self, outfile, format='lammps-dump', customkeys=customkeys, customvals=customvals,
+                compressed=compressed, timestep=timestep, species=species)
+        
+        elif format == "lammps-data":
+            asesys = convert_snap(self)
+            write(outfile, asesys, format='lammps-data', atom_style='atomic')
+        
+        elif format == "quantum-espresso":
+            asesys = convert_snap(self)
+            write(outfile, asesys, format='espresso-in', input_data=input_data,
+                pseudopotentials=pseudopotentials, kspacing=kspacing,
+                kpts=kpts, koffset=koffset, crystal_coordinates=crystal_coordinates)
+            if add_sample_id and (self.sample is not None):
+                self.write_quatum_espresso_id(outfile)
+        
+        else:
+            asesys = convert_snap(self)
+            write(outfile, asesys, format=format)
+
     def to_graph(self):
         """
         Converts the structure object to a graph representation.
 
         Returns
         -------
         None
@@ -1015,15 +1241,15 @@
             if name_index is None:
                 name_index = self.graph.n_samples + 1
             self._name = f"sample:{name_index}"
         else:
             self._name = f"sample:{str(uuid.uuid4())}"
 
     def _add_sample(self):
-        sample = self.graph.create_node(self._name, CMSO.AtomicScaleSample)
+        sample = self.graph.create_node(self._name, CMSO.AtomicScaleSample, label=self.label)
         self.sample = sample
 
     def _add_material(self):
         """
         Add a CMSO Material object
 
         Parameters
@@ -1293,15 +1519,15 @@
                 self.schema.material.crystal_structure.unit_cell.lattice_parameter(),
                 self.schema.material.crystal_structure.unit_cell.angle(),
             ]
 
         #fix for lattice angle of HCP
         if targets[0] == 'hcp':
             targets[5] = [90.0, 90.0, 120.0]
-            
+
         valid = self.graph._is_valid(targets)
 
         if valid:
             crystal_structure = self.graph.create_node(
                 f"{self._name}_CrystalStructure", CMSO.CrystalStructure
             )
             self.graph.add((self.material, CMSO.hasStructure, crystal_structure))
@@ -1334,26 +1560,26 @@
         ----------
         name
             if provided, the name will be used instead of random identifier
 
         Returns
         -------
         """
-        space_group = URIRef(f"{self._name}_SpaceGroup")
-        self.graph.add((self.crystal_structure, CMSO.hasSpaceGroup, space_group))
+        #space_group = URIRef(f"{self._name}_SpaceGroup")
+        #self.graph.add((self.crystal_structure, CMSO.hasSpaceGroup, space_group))
         self.graph.add(
             (
-                space_group,
+                self.crystal_structure,
                 CMSO.hasSpaceGroupSymbol,
                 Literal(spacegroup_symbol, datatype=XSD.string),
             )
         )
         self.graph.add(
             (
-                space_group,
+                self.crystal_structure,
                 CMSO.hasSpaceGroupNumber,
                 Literal(spacegroup_number, datatype=XSD.integer),
             )
         )
 
     def _add_unit_cell(self):
         """
@@ -1382,15 +1608,15 @@
         Returns:
             None
         """
         bv = URIRef(bv)
         self.graph.add(
             (
                 self.unit_cell,
-                Namespace("http://purls.helmholtz-metadaten.de/cmso/").hasBravaisLattice,
+                CMSO.hasBravaisLattice,
                 bv,
             )
         )
 
     def _add_lattice_properties(self, lattice_parameter_value, lattice_angle_value):
         """
         Add CMSO lattice properties such as Lattice Parameter,
@@ -1587,51 +1813,14 @@
         #    force = BNode(uname)
         #    self.add((self.sample, CMSO.hasAttribute, force))
         #    self.add((force, RDF.type, CMSO.AtomAttribute))
         #    self.add((force, CMSO.hasName, Literal('Force', data_type=XSD.string)))
         #    force_identifier = uuid.uuid4()
         #    self.add((force, CMSO.hasIdentifier, Literal(force_identifier, datatype=XSD.string)))
 
-    def add_vacancy(self, concentration, number=None):
-        """
-        Add Vacancy details which will be annotated by PODO
-
-        Parameters
-        ----------
-        concentration: float
-            vacancy concentration, value should be between 0-1
-
-        number: int
-            Number of atoms that were deleted, optional
-
-        Returns
-        -------
-        None
-        """
-        if self.graph is None:
-            return
-
-        vacancy = self.graph.create_node(f"{self._name}_Vacancy", PODO.Vacancy)
-        self.graph.add((self.material, CMSO.hasDefect, vacancy))
-        self.graph.add(
-            (
-                self.simulation_cell,
-                PODO.hasVacancyConcentration,
-                Literal(concentration, datatype=XSD.float),
-            )
-        )
-        if number is not None:
-            self.graph.add(
-                (
-                    self.simulation_cell,
-                    PODO.hasNumberOfVacancies,
-                    Literal(number, datatype=XSD.integer),
-                )
-            )
-
     def add_gb(self, gb_dict):
         """
         Add GB details which will be annotated using PLDO
 
         Parameters
         ----------
         gb_dict : dict
@@ -1705,7 +1894,139 @@
         self.graph.add(
             (
                 plane_defect,
                 PLDO.hasMisorientationAngle,
                 Literal(gb_dict["MisorientationAngle"], datatype=XSD.float),
             )
         )
+
+    
+    def rotate(self, rotation_vectors, graph=None, label=None):
+        box = am.Box(
+            avect=self.box[0],
+            bvect=self.box[1],
+            cvect=self.box[2],
+        )
+        
+        atoms = am.Atoms(
+            atype=self.atoms.types, pos=self.atoms.positions
+        )
+        
+        element = [val for key, val in self.atoms._type_dict.items()]
+
+        system = am.System(
+            atoms=atoms, 
+            box=box, 
+            pbc=[True, True, True], 
+            symbols=element, 
+            scale=False,
+        )
+
+        #now rotate with atomman
+        system = system.rotate(rotation_vectors)
+
+        #now convert back and return the system
+        box = [system.box.avect, 
+            system.box.bvect, 
+            system.box.cvect]
+        
+        atom_df = system.atoms_df()
+        types = [int(x) for x in atom_df.atype.values]
+        
+        species = []
+        for t in types:
+            species.append(element[int(t) - 1])
+
+        positions = np.column_stack(
+            (atom_df["pos[0]"].values, 
+            atom_df["pos[1]"].values, 
+            atom_df["pos[2]"].values)
+        )
+
+        atom_dict = {"positions": positions, "types": types, "species": species}
+        atom_obj = Atoms()
+        atom_obj.from_dict(atom_dict)
+        
+        output_structure = System()
+        output_structure.box = box
+        output_structure.atoms = atom_obj
+        #output_structure = output_structure.modify.remap_to_box()
+        if graph is not None:
+            output_structure.graph = graph
+        else:
+            output_structure.graph = self.graph
+        output_structure.atoms._lattice = self.atoms._lattice
+        output_structure.atoms._lattice_constant = self.atoms._lattice_constant
+        output_structure._structure_dict = self._structure_dict
+        if label is not None:
+            output_structure.label = label
+        else:
+            output_structure.label = self.label
+        output_structure.to_graph()
+        if output_structure.graph is not None:
+            self.add_rotation_triples(rotation_vectors, output_structure.sample)
+        return output_structure
+
+    def add_rotation_triples(self, rotation_vectors, child_sample_id):
+        activity_id = f"activity:{uuid.uuid4()}"
+        activity = self.graph.create_node(activity_id, UNSAFEASMO.StructureRotation)
+        self.graph.add((activity, RDF.type, PROV.Activity))
+        self.graph.add((child_sample_id, PROV.wasGeneratedBy, activity))
+        self.graph.add((child_sample_id, PROV.wasDerivedFrom, self.sample))
+
+        rot_vector_01 = self.graph.create_node(f"{activity_id}_RotationVector_1", CMSO.Vector)
+        self.graph.add((activity, CMSO.hasVector, rot_vector_01))
+        self.graph.add((rot_vector_01, CMSO.hasComponent_x, Literal(rotation_vectors[0][0], datatype=XSD.float),))
+        self.graph.add((rot_vector_01, CMSO.hasComponent_y, Literal(rotation_vectors[0][1], datatype=XSD.float),))
+        self.graph.add((rot_vector_01, CMSO.hasComponent_z, Literal(rotation_vectors[0][2], datatype=XSD.float),))
+
+        rot_vector_02 = self.graph.create_node(f"{activity_id}_RotationVector_2", CMSO.Vector)
+        self.graph.add((activity, CMSO.hasVector, rot_vector_02))
+        self.graph.add((rot_vector_02, CMSO.hasComponent_x, Literal(rotation_vectors[1][0], datatype=XSD.float),))
+        self.graph.add((rot_vector_02, CMSO.hasComponent_y, Literal(rotation_vectors[1][1], datatype=XSD.float),))
+        self.graph.add((rot_vector_02, CMSO.hasComponent_z, Literal(rotation_vectors[1][2], datatype=XSD.float),))
+
+        rot_vector_03 = self.graph.create_node(f"{activity_id}_RotationVector_3", CMSO.Vector)
+        self.graph.add((activity, CMSO.hasVector, rot_vector_03))
+        self.graph.add((rot_vector_03, CMSO.hasComponent_x, Literal(rotation_vectors[2][0], datatype=XSD.float),))
+        self.graph.add((rot_vector_03, CMSO.hasComponent_y, Literal(rotation_vectors[2][1], datatype=XSD.float),))
+        self.graph.add((rot_vector_03, CMSO.hasComponent_z, Literal(rotation_vectors[2][2], datatype=XSD.float),))
+
+    def _select_by_plane(self, plane, distance, reverse_orientation=False):
+        plane_norm = np.linalg.norm(plane)
+        selection = []
+        for pos in self.atoms.positions:
+            dist = np.dot(plane, pos)/plane_norm
+            
+            if dist < distance:
+                selection.append(True)
+            else:
+                selection.append(False)
+        if reverse_orientation:
+            selection = np.invert(selection)
+        return selection        
+
+    def select_by_plane(self, plane, distance, reverse_orientation=False):
+        selection = self._select_by_plane(plane, distance, 
+                        reverse_orientation=reverse_orientation)
+        self.apply_selection(condition=selection)
+        
+    def shear_system(self, shear, plane=None, distance=None, reverse_orientation=False):
+        if plane is not None:
+            if distance is None:
+                raise ValueError('distance needs to be provided')
+        
+        if plane is not None:
+            self.select_by_plane(plane, distance, reverse_orientation=reverse_orientation)
+
+        if not len(shear) == 3:
+            raise ValueError("shear vector must be of length 3")
+        
+        for x in range(len(self.atoms['positions'])):
+            if self.atoms['condition'][x]:
+                self.atoms['positions'][x] += np.array(shear)
+        
+        if plane is not None:
+            self.remove_selection()
+    
+    def add_shear_triples(self):
+        pass
```

### Comparing `atomrdf-0.6.4/atomrdf/visualize.py` & `atomrdf-0.8.1/atomrdf/visualize.py`

 * *Files 26% similar despite different names*

```diff
@@ -39,14 +39,29 @@
             return ".".join(rawsplit[-2:]), "URIRef"
 
     if "sample:" in raw:
         rawsplit = raw.split(":")
         if len(rawsplit) > 1:
             return "_".join(rawsplit), "BNode"
 
+    if "activity:" in raw:
+        rawsplit = raw.split(":")
+        if len(rawsplit) > 1:
+            return "_".join(rawsplit), "BNode"
+
+    if "operation:" in raw:
+        rawsplit = raw.split(":")
+        if len(rawsplit) > 1:
+            return "_".join(rawsplit), "BNode"
+
+    if "property:" in raw:
+        rawsplit = raw.split(":")
+        if len(rawsplit) > 1:
+            return "_".join(rawsplit), "BNode"
+
     # just a normal url split now
     rawsplit = raw.split("/")
     if len(rawsplit) > 1:
         return ".".join(rawsplit[-2:]), "URIRef"
 
     # none of the conditions worked, which means it's a hex string
     return raw, "BNode"
@@ -98,14 +113,15 @@
 
 def visualize_graph(
     g,
     styledict=styledict,
     rankdir="TB",
     hide_types=False,
     workflow_view=False,
+    sample_view=False,
     size=None,
     layout="dot",
 ):
     """
     Visualizes a graph using Graphviz.
 
     Parameters
@@ -116,14 +132,16 @@
         A dictionary containing styles for different types of nodes and edges. Default is `styledict`.
     rankdir : str, optional
         The direction of the graph layout. Default is "TB" (top to bottom).
     hide_types : bool, optional
         Whether to hide nodes with the "type" attribute. Default is False.
     workflow_view : bool, optional
         Whether to enable the workflow view. Default is False.
+    sample_view : bool, optional
+        Whether to enable the sample view. Default is False.
     size : str, optional
         The size of the graph. Default is None.
     layout : str, optional
         The layout algorithm to use. Default is "dot".
 
     Returns
     -------
@@ -169,14 +187,20 @@
                         shape=styledict[istype1]["shape"],
                         style=styledict[istype1]["style"],
                         color=styledict[istype1]["color"],
                         fontsize=styledict[istype1]["fontsize"],
                         fontname=styledict[istype1]["fontname"],
                     )
                     plot = False
+        
+        elif sample_view:
+            green_list = ['wasDerivedFrom', 'wasGeneratedBy']
+            if string3 not in green_list:
+                plot = False
+            
 
         if hide_types and (string3 == "type"):
             plot = False
 
         if not plot:
             continue
 
@@ -214,7 +238,87 @@
             color=styledict["edgecolor"],
             label=string3,
             fontsize=styledict[istype2]["fontsize"],
             fontname=styledict[istype2]["fontname"],
         )
 
     return dot
+
+def _id(item):
+    return str(item).replace(':', '_')
+
+def visualize_provenance(
+    prov,
+    rankdir="TB",
+    size=None,
+    layout="dot",
+):
+    dot = graphviz.Digraph()
+    dot.attr(
+        rankdir=rankdir,
+        style="filled",
+        size=size,
+        layout=layout,
+        overlap="false",
+    )
+    #add all nodes
+    for key in prov.keys():
+        nid = _id(key)
+        #if "activity" in key:
+        dot.node(nid, label=prov[key]['label'], 
+                shape='box', 
+                color="#C9DAF8", 
+                style="filled",
+                fontname='Helvetica',
+                fontsize='8')
+        #else:
+        #    dot.node(nid, label=prov[key]['label'], 
+        #            shape='parallelogram', 
+        #            color="#C9DAF8", 
+        #            style="filled",
+        #            fontname='Helvetica',
+        #            fontsize='8')
+    #add all edges
+    for key, val in prov.items():
+        if 'inputs' in val.keys():
+            if val['operation'] == 'input_parameter':
+                for subkey, subval in val['inputs'].items():
+                    dot.edge(_id(subval), _id(key), label='input_param', 
+                        color="#263238",
+                        fontname='Helvetica',
+                        fontsize='8')
+            if val['operation'] == 'output_parameter':
+                for subkey, subval in val['inputs'].items():
+                    dot.edge(_id(subval), _id(key), label='output_param', 
+                        color="#263238",
+                        fontname='Helvetica',
+                        fontsize='8')
+            elif val['operation'] == 'sample_for_activity':
+                for subkey, subval in val['inputs'].items():
+                    dot.edge(_id(subval), _id(key), label='input_sample', 
+                        color="#263238",
+                        fontname='Helvetica',
+                        fontsize='8')
+            elif val['operation'] == 'sample_output':
+                for subkey, subval in val['inputs'].items():
+                    dot.edge(_id(subval), _id(key), label='output_sample', 
+                        color="#263238",
+                        fontname='Helvetica',
+                        fontsize='8')
+            else:
+                operation_id = str(uuid.uuid4())
+                operation = dot.node(operation_id, label=val['operation'], 
+                                    color="#E6B8AF", 
+                                    shape='box', 
+                                    style='filled',
+                                    fontname='Helvetica',
+                                    fontsize='8')
+                for subkey, subval in val['inputs'].items():
+                    dot.edge(_id(subval), operation_id, label='input', 
+                        color="#263238",
+                        fontname='Helvetica',
+                        fontsize='8')
+                dot.edge(operation_id, _id(key), label='output', 
+                        color="#263238",
+                        fontname='Helvetica',
+                        fontsize='8')
+    return dot
```

### Comparing `atomrdf-0.6.4/atomrdf.egg-info/PKG-INFO` & `atomrdf-0.8.1/atomrdf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomrdf
-Version: 0.6.4
+Version: 0.8.1
 Summary: Ontology based structural manipulation and quering
 Home-page: https://pyscal.org
 Download-URL: https://github.com/pyscal/atomrdf
 Author: Abril Azocar Guzman, Sarath Menon
 Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -15,14 +15,16 @@
 Requires-Dist: pyyaml
 Requires-Dist: graphviz
 Requires-Dist: networkx
 Requires-Dist: pyscal3
 Requires-Dist: spglib
 Requires-Dist: pandas
 Requires-Dist: owlready2
+Requires-Dist: atomman
+Requires-Dist: mp-api
 
 # atomRDF
 
 > [!NOTE]
 > `atomRDF` was previously called `pyscal-rdf`. 
 
 [![codecov](https://codecov.io/gh/pyscal/atomRDF/graph/badge.svg?token=X7S3TP2MP6)](https://codecov.io/gh/pyscal/atomRDF)
```

### Comparing `atomrdf-0.6.4/atomrdf.egg-info/SOURCES.txt` & `atomrdf-0.8.1/atomrdf.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 MANIFEST.in
 README.md
 setup.py
 atomrdf/__init__.py
 atomrdf/encoder.py
 atomrdf/graph.py
 atomrdf/json_io.py
+atomrdf/mp.py
 atomrdf/namespace.py
 atomrdf/properties.py
+atomrdf/sample.py
 atomrdf/stores.py
 atomrdf/structure.py
 atomrdf/visualize.py
 atomrdf.egg-info/PKG-INFO
 atomrdf.egg-info/SOURCES.txt
 atomrdf.egg-info/dependency_links.txt
 atomrdf.egg-info/not-zip-safe
@@ -27,18 +29,23 @@
 atomrdf/network/__init__.py
 atomrdf/network/network.py
 atomrdf/network/ontology.py
 atomrdf/network/parser.py
 atomrdf/network/patch.py
 atomrdf/network/term.py
 atomrdf/workflow/__init__.py
-atomrdf/workflow/pyiron.py
 atomrdf/workflow/workflow.py
+atomrdf/workflow/pyiron/__init__.py
+atomrdf/workflow/pyiron/lammps.py
+atomrdf/workflow/pyiron/murnaghan.py
+atomrdf/workflow/pyiron/pyiron.py
+atomrdf/workflow/pyiron/vasp.py
 tests/test_encoder_and_write.py
 tests/test_graph.py
 tests/test_network.py
+tests/test_rotate.py
 tests/test_store.py
 tests/test_structure.py
 tests/test_structuregraph.py
 tests/test_term.py
 tests/test_visualise.py
 tests/test_workflow.py
```

### Comparing `atomrdf-0.6.4/setup.py` & `atomrdf-0.8.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,26 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='atomrdf',
-    version='0.6.4',
+    version='0.8.1',
     author='Abril Azocar Guzman, Sarath Menon',
     author_email='sarath.menon@pyscal.org',
     description='Ontology based structural manipulation and quering',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(include=['atomrdf', 'atomrdf.*']),
     zip_safe=False,
     download_url = 'https://github.com/pyscal/atomrdf',
     url = 'https://pyscal.org',
     install_requires=['numpy', 'ase', 'rdflib', 
     'pyyaml', 'graphviz', 'networkx', 
-    'pyscal3', 'spglib', 'pandas', 'owlready2'],
+    'pyscal3', 'spglib', 'pandas', 'owlready2',
+    'atomman', 'mp-api'],
     classifiers=[
         'Programming Language :: Python :: 3'
     ],
     include_package_data=True,
 )
```

### Comparing `atomrdf-0.6.4/tests/test_encoder_and_write.py` & `atomrdf-0.8.1/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/tests/test_graph.py` & `atomrdf-0.8.1/tests/test_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	s.log('testing-logger')
 	assert str(type(s.log).__name__) == "method"
  
 def test_add_structure():
 	s = KnowledgeGraph()
 	sys = System.create.element.Fe()
 	s.add_structure(sys)
-	assert sys.sample in s.samples
+	assert sys.sample in s.sample_ids
 
 def test_add_cross_triple():
 	
 	s = KnowledgeGraph(enable_log=True)
 	sys = System.create.element.Fe(graph=s)
 	status, _ = s._check_domain_if_uriref((sys.material, CMSO.hasDefect, PLDO.AntiphaseBoundary))
 	assert status == True
@@ -88,16 +88,15 @@
 	query = """
 	PREFIX cmso: <http://purls.helmholtz-metadaten.de/cmso/>
 	SELECT DISTINCT ?symbol
 	WHERE {
 	    ?sample cmso:hasNumberOfAtoms ?number .
 	    ?sample cmso:hasMaterial ?material .
 	    ?material cmso:hasStructure ?structure .
-	    ?structure cmso:hasSpaceGroup ?spgroup .
-	    ?spgroup cmso:hasSpaceGroupSymbol ?symbol .
+	    ?structure cmso:hasSpaceGroupSymbol ?symbol .
 	FILTER (?number="4"^^xsd:integer)
 	}"""
 	res = kg.query(query)
 	assert res.symbol.values[0].toPython() == 'Pm-3m'
 
 	res = kg.query_sample(kg.ontology.terms.cmso.hasAltName=='bcc')
 	assert res.hasAltNamevalue.values[0].toPython() == 'bcc'
@@ -107,15 +106,15 @@
 	assert res.hasAltNamevalue.values[0].toPython() == 'bcc'
 
 def test_extract_sample():
 	kg = KnowledgeGraph()
 	struct_Fe = System.create.element.Fe(graph=kg)
 	sample_graph, no_atoms = kg.get_sample(struct_Fe.sample, no_atoms=True)
 	assert no_atoms == 2
-	assert sample_graph.samples[0] == struct_Fe.sample
+	assert sample_graph.sample_ids[0] == struct_Fe.sample
 
 	struct = kg.get_system_from_sample(struct_Fe.sample)
 	assert len(struct.atoms.positions) == 2
 	assert struct.graph is not None
 
 	kg.to_file(struct_Fe.sample, filename='POSCAR')
 	assert os.path.exists('POSCAR')
```

### Comparing `atomrdf-0.6.4/tests/test_structure.py` & `atomrdf-0.8.1/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/tests/test_structuregraph.py` & `atomrdf-0.8.1/tests/test_structuregraph.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/tests/test_term.py` & `atomrdf-0.8.1/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `atomrdf-0.6.4/tests/test_visualise.py` & `atomrdf-0.8.1/tests/test_visualise.py`

 * *Files identical despite different names*

