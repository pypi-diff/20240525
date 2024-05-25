# Comparing `tmp/pyontoenv-0.1.7a3.tar.gz` & `tmp/pyontoenv-0.1.7a4.tar.gz`

## Comparing `pyontoenv-0.1.7a3.tar` & `pyontoenv-0.1.7a4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0     1001      127      776 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/Cargo.toml
--rw-r--r--   0     1001      127     5324 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/config.rs
--rw-r--r--   0     1001      127     2180 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/consts.rs
--rw-r--r--   0     1001      127     3267 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/doctor.rs
--rw-r--r--   0     1001      127      350 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/errors.rs
--rw-r--r--   0     1001      127    38873 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/lib.rs
--rw-r--r--   0     1001      127    13633 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/ontology.rs
--rw-r--r--   0     1001      127     3521 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/policy.rs
--rw-r--r--   0     1001      127     4646 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/transform.rs
--rw-r--r--   0     1001      127     6428 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/src/util.rs
--rw-r--r--   0     1001      127  1689944 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0     1001      127     1248 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/model
--rw-r--r--   0     1001      127      321 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/model.n3
--rw-r--r--   0     1001      127      537 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/model.nt
--rw-r--r--   0     1001      127     1248 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/model.ttl
--rw-r--r--   0     1001      127      789 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/model.xml
--rw-r--r--   0     1001      127      909 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   146214 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0     1001      127    30521 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   163975 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0     1001      127  1323794 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127    17472 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127  1456008 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127   104496 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0     1001      127  1255550 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0     1001      127    44502 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0     1001      127    81761 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/rec.ttl
--rw-r--r--   0     1001      127     4069 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/recimports.ttl
--rw-r--r--   0     1001      127    11876 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0     1001      127     1160 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data2/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data2/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data2/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/data2/ont4.ttl
--rw-r--r--   0     1001      127     1248 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/fileendings/model
--rw-r--r--   0     1001      127      321 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/fileendings/model.n3
--rw-r--r--   0     1001      127      537 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/fileendings/model.nt
--rw-r--r--   0     1001      127     1248 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/fileendings/model.ttl
--rw-r--r--   0     1001      127      789 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/fileendings/model.xml
--rw-r--r--   0     1001      127  1689944 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0     1001      127     1160 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0     1001      127     1135 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0     1001      127     1129 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a3/python/Cargo.toml
--rw-r--r--   0     1001      127     2886 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/.gitignore
--rw-r--r--   0     1001      127      731 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/README.md
--rw-r--r--   0     1001      127       71 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/build.rs
--rw-r--r--   0     1001      127     5241 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/poetry.lock
--rw-r--r--   0     1001      127       71 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/requirements.dev.txt
--rw-r--r--   0     1001      127    14284 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/src/lib.rs
--rw-r--r--   0     1001      127      694 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/python/test.py
--rw-r--r--   0     1001      127    73227 2024-05-23 03:10:53.000000 pyontoenv-0.1.7a3/Cargo.lock
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a3/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a3/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a3/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/Cargo.toml
+-rw-r--r--   0     1001      127     5324 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/errors.rs
+-rw-r--r--   0     1001      127    46611 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/lib.rs
+-rw-r--r--   0     1001      127    13820 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6477 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/src/util.rs
+-rw-r--r--   0     1001      127  1689944 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127  1689944 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/model
+-rw-r--r--   0     1001      127      321 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.xml
+-rw-r--r--   0     1001      127      909 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    81761 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/ref-schema.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/fileendings/model.xml
+-rw-r--r--   0     1001      127     1160 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/ont4.ttl
+-rw-r--r--   0     1001      127     1160 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a4/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/README.md
+-rw-r--r--   0     1001      127       71 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14319 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-05-25 05:37:57.000000 pyontoenv-0.1.7a4/python/test.py
+-rw-r--r--   0     1001      127    73227 2024-05-25 05:38:23.000000 pyontoenv-0.1.7a4/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a4/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a4/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a4/PKG-INFO
```

### Comparing `pyontoenv-0.1.7a3/lib/Cargo.toml` & `pyontoenv-0.1.7a4/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/src/config.rs` & `pyontoenv-0.1.7a4/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/src/consts.rs` & `pyontoenv-0.1.7a4/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/src/doctor.rs` & `pyontoenv-0.1.7a4/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/src/lib.rs` & `pyontoenv-0.1.7a4/lib/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     Dataset, Graph, GraphName, NamedNode, NamedNodeRef, NamedOrBlankNode, QuadRef, SubjectRef,
 };
 use oxigraph::store::Store;
 use petgraph::graph::{Graph as DiGraph, NodeIndex};
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::collections::{HashSet, VecDeque};
+use std::fs;
 use std::io::{BufReader, Write};
 use std::path::Path;
 
 // custom derive for ontologies field as vec of Ontology
 fn ontologies_ser<S>(
     ontologies: &HashMap<GraphIdentifier, Ontology>,
     s: S,
@@ -101,25 +102,14 @@
                 .map_err(|e| anyhow::anyhow!("Could not open store: {}", e));
         }
         Store::open(ontoenv_dir.join("store.db"))
             .or_else(|_| Store::open_read_only(ontoenv_dir.join("store.db")))
             .map_err(|e| anyhow::anyhow!("Could not open store: {}", e))
     }
 
-    pub fn new_readonly(config: Config) -> Result<Self> {
-        // create the store in the root/.ontoenv/store.db directory
-        let store = Store::open_secondary(config.root.join(".ontoenv/store.db"))?;
-        Ok(Self {
-            config,
-            ontologies: HashMap::new(),
-            dependency_graph: DiGraph::new(),
-            read_only: true,
-        })
-    }
-
     pub fn close(self) {}
 
     //TODO: add import_graph which imports a single graph into a given graph
 
     pub fn num_graphs(&self) -> usize {
         self.ontologies.len()
     }
@@ -161,18 +151,15 @@
             .find(|&ontology| ontology.location() == Some(location))
     }
 
     pub fn from_file(path: &Path, read_only: bool) -> Result<Self> {
         let file = std::fs::File::open(path)?;
         let reader = BufReader::new(file);
         let env: OntoEnv = serde_json::from_reader(reader)?;
-        Ok(Self {
-            read_only,
-            ..env
-        })
+        Ok(Self { read_only, ..env })
     }
 
     /// creates a new directory called .ontoenv in self.root and saves:
     /// - the configuration as ontoenv.json
     /// - all graphs in the environment as .ttl files
     /// - the dependency graph as a json file
     pub fn save_to_directory(&self) -> Result<()> {
@@ -473,14 +460,15 @@
                 }
             }
         }
         Ok(files)
     }
 
     pub fn add(&mut self, location: OntologyLocation) -> Result<GraphIdentifier> {
+        info!("Adding ontology from location: {:?}", location);
         self.add_or_update_ontology_from_location(location)
     }
 
     /// Add or update the ontology from the given location. Overwrites the ontology
     /// if it already exists in the environment.
     fn add_or_update_ontology_from_location(
         &mut self,
@@ -773,38 +761,74 @@
 #[cfg(test)]
 mod tests {
 
     use super::*;
     use std::path::PathBuf;
     use tempdir::TempDir;
 
-    fn copy_file(path: &PathBuf, dest: &PathBuf) -> Result<()> {
-        println!("Copying {:?} to {:?}", path, dest);
-        if path.is_file() {
-            std::fs::copy(path, dest)?;
-        } else {
-            std::fs::create_dir_all(dest)?;
-        }
-        Ok(())
+    // the tests directory contains a number of test files that are used to test the OntoEnv.
+    // Each has a unique name and they all exist in a flat folder.
+    // This is a macro which takes a list of strings describing the directory structure of a
+    // test directory and creates a temporary directory with the given structure. The strings
+    // in the test directory might be nested in different directories. The macro copies the
+    // files to the temporary directory and returns the temporary directory.
+    macro_rules! setup {
+        ($temp_dir:expr, { $($from:expr => $to:expr),* $(,)? }) => {{
+            use std::collections::HashSet;
+            use std::path::PathBuf;
+            use std::fs;
+
+            // Assign the temporary directory
+            let dir = $temp_dir;
+
+            // Create a HashSet of the destination files
+            let provided_files: HashSet<&str> = {
+                let mut set = HashSet::new();
+                $( set.insert($to); )*
+                set
+            };
+
+            // Copy each specified file to the temporary directory
+            $(
+                let source_path: PathBuf = PathBuf::from($from);
+                let dest_path: PathBuf = dir.path().join($to);
+                if !dest_path.exists() {
+                    // Ensure the parent directories exist
+                    if let Some(parent) = dest_path.parent() {
+                        if !parent.exists() {
+                            fs::create_dir_all(parent).expect("Failed to create parent directories");
+                        }
+                    }
+
+                    // 'copy_file' is assumed to be a custom function in the user's project
+                    // If not, consider using std::fs::copy for basic file copying
+                    copy_file(&source_path, &dest_path).expect(format!("Failed to copy file from {} to {}", source_path.display(), dest_path.display()).as_str());
+                }
+            )*
+
+            // Check the contents of the temporary directory
+            for entry in fs::read_dir(dir.path()).expect("Failed to read directory") {
+                let entry = entry.expect("Failed to read entry");
+                let file_name = entry.file_name().into_string().expect("Failed to convert filename to string");
+
+                if !provided_files.contains(file_name.as_str()) && entry.file_type().expect("Failed to get file type").is_file() {
+                    println!("Warning: extra file {} found in directory", file_name);
+                    // remove it
+                    fs::remove_file(entry.path()).expect("Failed to remove file");
+                }
+            }
+        }};
     }
 
-    fn setup(dir: &str) -> Result<TempDir> {
-        // copy all files from tests/ to a temp directory and return the temp directory
-        let test_dir = TempDir::new("ontoenv")?;
-        // where test files are located
-        let base_dir = Path::new("tests/").join(dir);
-        println!("Copying files from {:?} to {:?}", base_dir, test_dir.path());
-        // destination directory
-        for entry in walkdir::WalkDir::new(&base_dir) {
-            let entry = entry?;
-            let path = entry.path();
-            let dest = test_dir.path().join(path.strip_prefix(&base_dir)?);
-            copy_file(&path.into(), &dest)?;
+    fn copy_file(src_path: &PathBuf, dst_path: &PathBuf) -> Result<(), std::io::Error> {
+        if let Some(parent) = dst_path.parent() {
+            std::fs::create_dir_all(parent)?;
         }
-        Ok(test_dir)
+        std::fs::copy(src_path, dst_path)?;
+        Ok(())
     }
 
     fn default_config(dir: &TempDir) -> Config {
         Config::new(
             dir.path().into(),
             Some(vec![dir.path().into()]),
             &["*.ttl"],
@@ -834,26 +858,42 @@
     // we don't care about errors when cleaning up the TempDir so
     // we just drop the TempDir (looking at this doc:
     // https://docs.rs/tempdir/latest/tempdir/struct.TempDir.html#method.close)
     fn teardown(_dir: TempDir) {}
 
     #[test]
     fn test_ontoenv_scans() -> Result<()> {
-        let dir = setup("data2")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
+        // print the files in dir
+        println!("listing files");
+        for entry in std::fs::read_dir(dir.path())? {
+            let entry = entry?;
+            println!("inside> {:?}", entry.file_name());
+        }
+
         let cfg = default_config(&dir);
+        println!("config: {:?}", cfg);
         let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_scans_default() -> Result<()> {
-        let dir = setup("data2")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
         let cfg = Config::new_with_default_matches(
             dir.path().into(),
             Some([dir.path().into()]),
             false,
             false,
             true,
         )?;
@@ -862,15 +902,20 @@
         assert_eq!(env.num_graphs(), 4);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_num_triples() -> Result<()> {
-        let dir = setup("fileendings")?;
+        let dir = TempDir::new("fileendings")?;
+        setup!(&dir, {"tests/fileendings/model" => "model", 
+                      "tests/fileendings/model.n3" => "model.n3",
+                      "tests/fileendings/model.nt" => "model.nt",
+                      "tests/fileendings/model.ttl" => "model.ttl",
+                      "tests/fileendings/model.xml" => "model.xml"});
         let cfg1 = Config::new(
             dir.path().into(),
             Some(vec![dir.path().into()]),
             &["*.n3"],
             &[""],
             false,
             false,
@@ -883,45 +928,78 @@
         assert_eq!(env.num_triples()?, 5);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_update() -> Result<()> {
-        let dir = setup("data2")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
         let cfg = default_config(&dir);
         let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         let old_num_triples = env.num_triples()?;
         assert_eq!(env.num_graphs(), 4);
 
         // updating again shouldn't add anything
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         assert_eq!(env.num_triples()?, old_num_triples);
 
-        // remove file
-        std::fs::remove_file(dir.path().join("ont4.ttl"))?;
+        // remove ont4.ttl
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl"});
 
         env.update()?;
         assert_eq!(env.num_graphs(), 3);
 
         // copy ont4.ttl back
-        let base_dir = Path::new("tests/").join("data2");
-        std::fs::copy(base_dir.join("ont4.ttl"), dir.path().join("ont4.ttl"))?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         teardown(dir);
         Ok(())
     }
 
     #[test]
+    fn test_recreate() -> Result<()> {
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
+        let cfg = default_config(&dir);
+        let mut env = OntoEnv::new(cfg, false)?;
+        // create a new env, like above, but make sure it raises an error
+        let cfg = default_config(&dir);
+        let env = OntoEnv::new(cfg, false);
+        assert!(env.is_err());
+
+        let cfg = default_config(&dir);
+        let env = OntoEnv::new(cfg, true)?;
+
+        teardown(dir);
+        Ok(())
+    }
+
+    #[test]
     fn test_ontoenv_retrieval_by_name() -> Result<()> {
-        let dir = setup("data2")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
         let cfg = default_config(&dir);
         let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
 
         let ont1 = NamedNodeRef::new("urn:ont1")?;
         let ont = env
             .get_ontology_by_name(ont1)
@@ -930,15 +1008,19 @@
         assert!(ont.location().unwrap().is_file());
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_retrieval_by_location() -> Result<()> {
-        let dir = setup("data2")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
         let cfg = default_config(&dir);
         let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
 
         let ont1_path = dir.path().join("ont1.ttl");
         let loc = OntologyLocation::from_str(
             ont1_path
@@ -955,15 +1037,19 @@
             .is_file());
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_load() -> Result<()> {
-        let dir = setup("data2")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, { "tests/ont1.ttl" => "ont1.ttl", 
+                       "tests/ont2.ttl" => "ont2.ttl",
+                       "tests/ont3.ttl" => "ont3.ttl",
+                       "tests/ont4.ttl" => "ont4.ttl" });
         let cfg = default_config(&dir);
         let mut env = OntoEnv::new(cfg, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
         env.save_to_directory()?;
         // drop env
         env.close();
@@ -974,15 +1060,22 @@
         assert_eq!(env2.num_graphs(), 4);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_add() -> Result<()> {
-        let dir = setup("updates")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, {"tests/updates/v1/ont1.ttl" => "v1/ont1.ttl",
+                      "tests/updates/v1/ont2.ttl" => "v1/ont2.ttl",
+                      "tests/updates/v1/ont3.ttl" => "v1/ont3.ttl",
+                      "tests/updates/v1/ont4.ttl" => "v1/ont4.ttl",
+                      "tests/updates/v2/ont5.ttl" => "v2/ont5.ttl"
+        });
+
         let cfg1 = default_config_with_subdir(&dir, "v1");
         let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         let ont_path = dir.path().join("v2/ont5.ttl");
         let loc = OntologyLocation::from_str(
@@ -994,54 +1087,89 @@
         assert_eq!(env.num_graphs(), 5);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_ontoenv_detect_updates() -> Result<()> {
-        let dir = setup("updates")?;
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, {"tests/updates/v1/ont1.ttl" => "v1/ont1.ttl",
+                      "tests/updates/v1/ont2.ttl" => "v1/ont2.ttl",
+                      "tests/updates/v1/ont3.ttl" => "v1/ont3.ttl",
+                      "tests/updates/v1/ont4.ttl" => "v1/ont4.ttl",
+        });
         let cfg1 = default_config_with_subdir(&dir, "v1");
         let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         // copy files from dir/v2 to dir/v1
-        let base_dir = Path::new("tests/").join("updates").join("v2");
-        for entry in walkdir::WalkDir::new(&base_dir) {
-            let entry = entry?;
-            let path = entry.path();
-            let dest = dir.path().join("v1").join(path.strip_prefix(&base_dir)?);
-            println!("Copying {:?} without {:?} to {:?}", path, base_dir, dest);
-            copy_file(&path.to_path_buf(), &dest)?;
-        }
-
+        setup!(&dir, {"tests/updates/v1/ont1.ttl" => "v1/ont1.ttl",
+                      "tests/updates/v1/ont2.ttl" => "v1/ont2.ttl",
+                      "tests/updates/v1/ont4.ttl" => "v1/ont4.ttl",
+                      "tests/updates/v2/ont3.ttl" => "v1/ont3.ttl",
+                      "tests/updates/v2/ont5.ttl" => "v1/ont5.ttl",
+        });
         env.update()?;
 
         assert_eq!(env.num_graphs(), 5);
         teardown(dir);
         Ok(())
     }
 
     #[test]
     fn test_check_for_updates() -> Result<()> {
-        let dir = setup("updates")?;
+        let dir = TempDir::new("ontoenv")?;
         let cfg1 = default_config_with_subdir(&dir, "v1");
+        setup!(&dir, {"tests/updates/v1/ont1.ttl" => "v1/ont1.ttl",
+                      "tests/updates/v1/ont2.ttl" => "v1/ont2.ttl",
+                      "tests/updates/v1/ont3.ttl" => "v1/ont3.ttl",
+                      "tests/updates/v1/ont4.ttl" => "v1/ont4.ttl" });
         let mut env = OntoEnv::new(cfg1, false)?;
         env.update()?;
         assert_eq!(env.num_graphs(), 4);
 
         // copy files from dir/v2 to dir/v1
-        let base_dir = Path::new("tests/").join("updates").join("v2");
-        for entry in walkdir::WalkDir::new(&base_dir) {
-            let entry = entry?;
-            let path = entry.path();
-            let dest = dir.path().join("v1").join(path.strip_prefix(&base_dir)?);
-            println!("Copying {:?} without {:?} to {:?}", path, base_dir, dest);
-            copy_file(&path.to_path_buf(), &dest)?;
-        }
+        setup!(&dir, {"tests/updates/v1/ont1.ttl" => "v1/ont1.ttl",
+                      "tests/updates/v1/ont2.ttl" => "v1/ont2.ttl",
+                      "tests/updates/v1/ont4.ttl" => "v1/ont4.ttl",
+                      "tests/updates/v2/ont3.ttl" => "v1/ont3.ttl",
+                      "tests/updates/v2/ont5.ttl" => "v1/ont5.ttl",
+        });
 
         let updates = env.get_updated_files()?;
         assert_eq!(updates.len(), 1);
         teardown(dir);
         Ok(())
     }
+
+    #[test]
+    fn test_ontoenv_dependency_closure() -> Result<()> {
+        let dir = TempDir::new("ontoenv")?;
+        setup!(&dir, {"tests/brick-stuff/Brick-1.3.ttl" => "Brick-1.3.ttl",
+                      "tests/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl" => "support/SCHEMA-FACADE_QUDT-v2.1.ttl",
+                      "tests/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl" => "support/SCHEMA_QUDT_NoOWL-v2.1.ttl",
+                      "tests/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl" => "support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl" => "support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl" => "support/VOCAB_QUDT-PREFIX-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl" => "support/VOCAB_QUDT-PREFIXES-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl" => "support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl" => "support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl" => "support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl",
+                      "tests/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl" => "support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl",
+                      "tests/brick-stuff/support/bacnet.ttl" => "support/bacnet.ttl",
+                      "tests/brick-stuff/support/brickpatches.ttl" => "support/brickpatches.ttl",
+                      "tests/brick-stuff/support/rec.ttl" => "support/rec.ttl",
+                      "tests/brick-stuff/support/recimports.ttl" => "support/recimports.ttl",
+                      "tests/brick-stuff/support/ref-schema.ttl" => "support/ref-schema.ttl"});
+        let cfg = default_config(&dir);
+        let mut env = OntoEnv::new(cfg, false)?;
+        env.update()?;
+
+        let ont1 = NamedNodeRef::new("https://brickschema.org/schema/1.4-rc1/Brick")?;
+        let ont_graph = env.get_ontology_by_name(ont1).unwrap();
+        let closure = env.get_dependency_closure(&ont_graph.id()).unwrap();
+        assert_eq!(closure.len(), 14);
+        teardown(dir);
+        Ok(())
+    }
 }
```

### Comparing `pyontoenv-0.1.7a3/lib/src/ontology.rs` & `pyontoenv-0.1.7a4/lib/src/ontology.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 
     pub fn to_filename(&self) -> String {
         let name = self.name.as_str().replace(':', "+");
         let location = self.location.as_str().replace("file://", "");
         format!("{}-{}", name, location).replace('/', "_")
     }
     pub fn graphname(&self) -> Result<GraphName> {
+        // if self.name is a URL, use that as the graphname
+        if self.name.as_str().starts_with("http") {
+            return Ok(GraphName::NamedNode(self.name.clone()));
+        }
+
         // graphname is the self.name + URL-safe self.location
         let name = self.name.as_str().replace(':', "+");
         let location = self.location.as_str().replace("file://", "");
         Ok(GraphName::NamedNode(NamedNode::new(format!(
             "urn://{}-{}",
             name, location
         ))?))
```

### Comparing `pyontoenv-0.1.7a3/lib/src/policy.rs` & `pyontoenv-0.1.7a4/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/src/transform.rs` & `pyontoenv-0.1.7a4/lib/src/transform.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/src/util.rs` & `pyontoenv-0.1.7a4/lib/src/util.rs`

 * *Files 3% similar despite different names*

```diff
@@ -125,31 +125,31 @@
 mod tests {
     use super::*;
     use oxigraph::model::{Dataset, GraphNameRef, NamedNodeRef, QuadRef};
 
     #[test]
     fn test_read_file() {
         // testing turtle file
-        let graph = read_file(Path::new("tests/data/model.ttl")).unwrap();
+        let graph = read_file(Path::new("tests/fileendings/model.ttl")).unwrap();
         assert_eq!(graph.len(), 5);
 
         // testing ntriples file
-        let graph = read_file(Path::new("tests/data/model.nt")).unwrap();
+        let graph = read_file(Path::new("tests/fileendings/model.nt")).unwrap();
         assert_eq!(graph.len(), 5);
 
         // testing n3 file
-        let graph = read_file(Path::new("tests/data/model.n3")).unwrap();
+        let graph = read_file(Path::new("tests/fileendings/model.n3")).unwrap();
         assert_eq!(graph.len(), 5);
         //
         // testing xml file
-        let graph = read_file(Path::new("tests/data/model.xml")).unwrap();
+        let graph = read_file(Path::new("tests/fileendings/model.xml")).unwrap();
         assert_eq!(graph.len(), 5);
 
         // testing default turtle file
-        let graph = read_file(Path::new("tests/data/model")).unwrap();
+        let graph = read_file(Path::new("tests/fileendings/model")).unwrap();
         assert_eq!(graph.len(), 5);
 
         // reading non-existent file should return an error
         let result = read_file(Path::new("tests/data/non-existent.ttl"));
         assert!(result.is_err());
     }
 
@@ -165,18 +165,18 @@
         assert!(result.is_err());
     }
 
     #[test]
     fn test_write_dataset_to_file() {
         // create in-memory dataset
         let mut graph = Dataset::new();
-        let model = read_file(Path::new("tests/data/model.ttl")).unwrap();
+        let model = read_file(Path::new("tests/fileendings/model.ttl")).unwrap();
         let model_name =
             GraphNameRef::NamedNode(NamedNodeRef::new("http://example.org/model").unwrap());
-        let brick = read_file(Path::new("tests/data/Brick-1.3.ttl")).unwrap();
+        let brick = read_file(Path::new("tests/brick-stuff/Brick-1.3.ttl")).unwrap();
         let brick_name =
             GraphNameRef::NamedNode(NamedNodeRef::new("http://example.org/brick").unwrap());
         for quad in model.iter() {
             graph.insert(QuadRef::new(
                 quad.subject,
                 quad.predicate,
                 quad.object,
```

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.7a4/lib/tests/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/model` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/model.nt` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/model.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/model.xml` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.7a4/lib/tests/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.7a4/lib/tests/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.7a4/lib/tests/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.7a4/lib/tests/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/fileendings/model` & `pyontoenv-0.1.7a4/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.7a4/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.7a4/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.7a4/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.7a4/lib/tests/brick-stuff/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.7a4/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.7a4/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.7a4/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.7a4/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.7a4/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.7a4/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/python/Cargo.toml` & `pyontoenv-0.1.7a4/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/python/.github/workflows/CI.yml` & `pyontoenv-0.1.7a4/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/python/.gitignore` & `pyontoenv-0.1.7a4/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/python/README.md` & `pyontoenv-0.1.7a4/python/README.md`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/python/poetry.lock` & `pyontoenv-0.1.7a4/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/python/src/lib.rs` & `pyontoenv-0.1.7a4/python/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use ::ontoenv as ontoenvrs;
 use ::ontoenv::consts::{ONTOLOGY, TYPE};
 use ::ontoenv::ontology::OntologyLocation;
 use ::ontoenv::transform;
 use anyhow::Error;
-use std::sync::{Arc, Mutex, Once, OnceLock};
-use oxigraph::model::{BlankNode, Literal, NamedNode, Term, SubjectRef};
+use oxigraph::model::{BlankNode, Literal, NamedNode, SubjectRef, Term};
 use pyo3::{
     prelude::*,
-    types::{PyString, PyTuple, IntoPyDict},
+    types::{IntoPyDict, PyString, PyTuple},
 };
 use std::borrow::Borrow;
 use std::path::{Path, PathBuf};
+use std::sync::{Arc, Mutex, Once, OnceLock};
 
 static INIT: Once = Once::new();
 static ONTOENV_SINGLETON: OnceLock<Arc<Mutex<ontoenvrs::OntoEnv>>> = OnceLock::new();
 
 fn anyhow_to_pyerr(e: Error) -> PyErr {
     PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string())
 }
@@ -206,17 +206,15 @@
 
         {
             let mut env = env.lock().unwrap();
             env.update().map_err(anyhow_to_pyerr)?;
             env.save_to_directory().map_err(anyhow_to_pyerr)?;
         }
 
-        Ok(OntoEnv {
-            inner: env.clone(),
-        })
+        Ok(OntoEnv { inner: env.clone() })
     }
 
     fn update(&self) -> PyResult<()> {
         let mut inner = self.inner.lock().unwrap();
         inner.update().map_err(anyhow_to_pyerr)?;
         Ok(())
     }
@@ -228,15 +226,20 @@
             inner.num_graphs(),
             inner.num_triples().map_err(anyhow_to_pyerr)?
         ))
     }
 
     // The following methods will now access the inner OntoEnv in a thread-safe manner:
 
-    fn import_graph(&self, py: Python, destination_graph: &Bound<'_, PyAny>, uri: &str) -> PyResult<()> {
+    fn import_graph(
+        &self,
+        py: Python,
+        destination_graph: &Bound<'_, PyAny>,
+        uri: &str,
+    ) -> PyResult<()> {
         let inner = self.inner.lock().unwrap();
         let rdflib = py.import_bound("rdflib")?;
         let iri = NamedNode::new(uri)
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
         let ont = inner
             .get_ontology_by_name(iri.as_ref())
             .ok_or_else(|| PyErr::new::<pyo3::exceptions::PyValueError, _>("Ontology not found"))?;
@@ -244,15 +247,16 @@
 
         let uriref_constructor = rdflib.getattr("URIRef")?;
         let type_uri = uriref_constructor.call1((TYPE.as_str(),))?;
         let ontology_uri = uriref_constructor.call1((ONTOLOGY.as_str(),))?;
         let kwargs = [("predicate", type_uri), ("object", ontology_uri)].into_py_dict_bound(py);
         let result = destination_graph.call_method("value", (), Some(&kwargs))?;
         if !result.is_none() {
-            let ontology = NamedNode::new(result.extract::<String>()?).map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
+            let ontology = NamedNode::new(result.extract::<String>()?)
+                .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
             let base_ontology: SubjectRef = SubjectRef::NamedNode(ontology.as_ref());
 
             transform::rewrite_sh_prefixes_graph(&mut graph, base_ontology);
             transform::remove_ontology_declarations_graph(&mut graph, base_ontology);
         }
         transform::remove_owl_imports_graph(&mut graph);
```

### Comparing `pyontoenv-0.1.7a3/python/test.py` & `pyontoenv-0.1.7a4/python/test.py`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a3/Cargo.lock` & `pyontoenv-0.1.7a4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.7-a3"
+version = "0.1.7-a4"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1401,15 +1401,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.7-a3"
+version = "0.1.7-a4"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1719,15 +1719,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.7-a3"
+version = "0.1.7-a4"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.7a3/Cargo.toml` & `pyontoenv-0.1.7a4/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.7-a3"
+version = "0.1.7-a4"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
@@ -27,8 +27,8 @@
 glob = "0.3.1"
 chrono = { version = "0.4.33", features = ["serde"] }
 petgraph = { version = "0.6.4", features = ["serde-1"] }
 clap = { version = "4.4.18", features = ["derive"] }
 derive_builder = "0.13.0"
 oxigraph = "0.3.22"
 
-ontoenv = { version = "0.1.7-a3", path = "lib" }
+ontoenv = { version = "0.1.7-a4", path = "lib" }
```

### Comparing `pyontoenv-0.1.7a3/pyproject.toml` & `pyontoenv-0.1.7a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.7a3"
+version = "0.1.7a4"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pyontoenv-0.1.7a3/PKG-INFO` & `pyontoenv-0.1.7a4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.7a3
+Version: 0.1.7a4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```

