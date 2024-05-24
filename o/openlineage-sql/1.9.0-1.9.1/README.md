# Comparing `tmp/openlineage_sql-1.9.0.tar.gz` & `tmp/openlineage_sql-1.9.1.tar.gz`

## Comparing `openlineage_sql-1.9.0.tar` & `openlineage_sql-1.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-rw-r--   0     1001     1002      590 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/Cargo.toml
--rw-rw-r--   0     1001     1002      704 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/bigquery.rs
--rw-rw-r--   0     1001     1002     1314 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/context/alias_table.rs
--rw-rw-r--   0     1001     1002    16362 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/context/mod.rs
--rw-rw-r--   0     1001     1002     1700 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/dialect.rs
--rw-rw-r--   0     1001     1002     3134 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/lib.rs
--rw-rw-r--   0     1001     1002     6817 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/lineage.rs
--rw-rw-r--   0     1001     1002    22232 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/src/visitor.rs
--rw-rw-r--   0     1001     1002      189 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/column_lineage/mod.rs
--rw-rw-r--   0     1001     1002     3999 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/column_lineage/tests_aliases.rs
--rw-rw-r--   0     1001     1002     1119 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/column_lineage/tests_cte.rs
--rw-rw-r--   0     1001     1002     2149 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/column_lineage/tests_select.rs
--rw-rw-r--   0     1001     1002     8992 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/column_lineage/tests_simple.rs
--rw-rw-r--   0     1001     1002      389 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/mod.rs
--rw-rw-r--   0     1001     1002     1140 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_alter.rs
--rw-rw-r--   0     1001     1002     3925 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_copy.rs
--rw-rw-r--   0     1001     1002     5193 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_create.rs
--rw-rw-r--   0     1001     1002     5547 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_cte.rs
--rw-rw-r--   0     1001     1002      909 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_delete.rs
--rw-rw-r--   0     1001     1002      431 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_drop.rs
--rw-rw-r--   0     1001     1002     1549 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_error_handling.rs
--rw-rw-r--   0     1001     1002    17700 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_insert.rs
--rw-rw-r--   0     1001     1002     2199 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_merge.rs
--rw-rw-r--   0     1001     1002     3448 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_select.rs
--rw-rw-r--   0     1001     1002    34761 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_tpcds.rs
--rw-rw-r--   0     1001     1002      392 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_truncate.rs
--rw-rw-r--   0     1001     1002     1530 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/table_lineage/tests_update.rs
--rw-rw-r--   0     1001     1002      918 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/test_utils/mod.rs
--rw-rw-r--   0     1001     1002      158 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/impl/tests/tests.rs
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 openlineage_sql-1.9.0/iface-py/Cargo.toml
--rw-rw-r--   0     1001     1002      174 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/build.rs
--rw-rw-r--   0     1001     1002     1855 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/openlineage_sql.pyi
--rw-rw-r--   0     1001     1002       13 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/requirements.txt
--rwxrwxr-x   0     1001     1002     1438 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/script/build-macos.sh
--rwxrwxr-x   0     1001     1002     1341 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/script/build.sh
--rwxrwxr-x   0     1001     1002     1142 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/script/setup-macos.sh
--rw-rw-r--   0     1001     1002    12911 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/src/lib.rs
--rw-rw-r--   0     1001     1002     2347 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/tests/python/sql_tester.py
--rw-rw-r--   0     1001     1002      280 2024-02-23 14:50:07.000000 openlineage_sql-1.9.0/iface-py/tests/python/test_small.py
--rw-r--r--   0        0        0    11866 2024-02-23 14:50:49.000000 openlineage_sql-1.9.0/Cargo.lock
--rw-r--r--   0        0        0       78 1970-01-01 00:00:00.000000 openlineage_sql-1.9.0/Cargo.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 openlineage_sql-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 openlineage_sql-1.9.0/PKG-INFO
+-rw-rw-r--   0     1001     1002      590 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/Cargo.toml
+-rw-rw-r--   0     1001     1002      704 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/bigquery.rs
+-rw-rw-r--   0     1001     1002     1314 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/context/alias_table.rs
+-rw-rw-r--   0     1001     1002    16362 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/context/mod.rs
+-rw-rw-r--   0     1001     1002     1700 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/dialect.rs
+-rw-rw-r--   0     1001     1002     3134 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/lib.rs
+-rw-rw-r--   0     1001     1002     6817 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/lineage.rs
+-rw-rw-r--   0     1001     1002    22232 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/src/visitor.rs
+-rw-rw-r--   0     1001     1002      189 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/column_lineage/mod.rs
+-rw-rw-r--   0     1001     1002     3999 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/column_lineage/tests_aliases.rs
+-rw-rw-r--   0     1001     1002     1119 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/column_lineage/tests_cte.rs
+-rw-rw-r--   0     1001     1002     2149 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/column_lineage/tests_select.rs
+-rw-rw-r--   0     1001     1002     8992 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/column_lineage/tests_simple.rs
+-rw-rw-r--   0     1001     1002      389 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/mod.rs
+-rw-rw-r--   0     1001     1002     1140 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_alter.rs
+-rw-rw-r--   0     1001     1002     3925 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_copy.rs
+-rw-rw-r--   0     1001     1002     5193 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_create.rs
+-rw-rw-r--   0     1001     1002     5547 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_cte.rs
+-rw-rw-r--   0     1001     1002      909 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_delete.rs
+-rw-rw-r--   0     1001     1002      431 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_drop.rs
+-rw-rw-r--   0     1001     1002     1549 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_error_handling.rs
+-rw-rw-r--   0     1001     1002    17700 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_insert.rs
+-rw-rw-r--   0     1001     1002     2199 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_merge.rs
+-rw-rw-r--   0     1001     1002     3448 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_select.rs
+-rw-rw-r--   0     1001     1002    34761 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_tpcds.rs
+-rw-rw-r--   0     1001     1002      392 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_truncate.rs
+-rw-rw-r--   0     1001     1002     1530 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/table_lineage/tests_update.rs
+-rw-rw-r--   0     1001     1002      918 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/test_utils/mod.rs
+-rw-rw-r--   0     1001     1002      158 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/impl/tests/tests.rs
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 openlineage_sql-1.9.1/iface-py/Cargo.toml
+-rw-rw-r--   0     1001     1002      174 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/build.rs
+-rw-rw-r--   0     1001     1002     1855 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/openlineage_sql.pyi
+-rw-rw-r--   0     1001     1002       13 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/requirements.txt
+-rwxrwxr-x   0     1001     1002     1438 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/script/build-macos.sh
+-rwxrwxr-x   0     1001     1002     1341 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/script/build.sh
+-rwxrwxr-x   0     1001     1002     1142 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/script/setup-macos.sh
+-rw-rw-r--   0     1001     1002    12911 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/src/lib.rs
+-rw-rw-r--   0     1001     1002     2347 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/tests/python/sql_tester.py
+-rw-rw-r--   0     1001     1002      280 2024-02-26 15:00:39.000000 openlineage_sql-1.9.1/iface-py/tests/python/test_small.py
+-rw-r--r--   0        0        0    11866 2024-02-26 15:01:29.000000 openlineage_sql-1.9.1/Cargo.lock
+-rw-r--r--   0        0        0       78 1970-01-01 00:00:00.000000 openlineage_sql-1.9.1/Cargo.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 openlineage_sql-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 openlineage_sql-1.9.1/PKG-INFO
```

### Comparing `openlineage_sql-1.9.0/impl/Cargo.toml` & `openlineage_sql-1.9.1/impl/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "openlineage_sql"
 description = "Library extracting source and destination tables from sql statements"
-version = "1.9.0"
+version = "1.9.1"
 edition = "2021"
 authors = ["Maciej Obuchowski <obuchowski.maciej@gmail.com>", "Piotr Wojtczak <piotr.m.wojtczak@gmail.com"]
 keywords = ["sql", "lineage", "openlineage"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "openlineage_sql"
```

### Comparing `openlineage_sql-1.9.0/impl/src/bigquery.rs` & `openlineage_sql-1.9.1/impl/src/bigquery.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/src/context/alias_table.rs` & `openlineage_sql-1.9.1/impl/src/context/alias_table.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/src/context/mod.rs` & `openlineage_sql-1.9.1/impl/src/context/mod.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/src/dialect.rs` & `openlineage_sql-1.9.1/impl/src/dialect.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/src/lib.rs` & `openlineage_sql-1.9.1/impl/src/lib.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/src/lineage.rs` & `openlineage_sql-1.9.1/impl/src/lineage.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/src/visitor.rs` & `openlineage_sql-1.9.1/impl/src/visitor.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/column_lineage/tests_aliases.rs` & `openlineage_sql-1.9.1/impl/tests/column_lineage/tests_aliases.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/column_lineage/tests_cte.rs` & `openlineage_sql-1.9.1/impl/tests/column_lineage/tests_cte.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/column_lineage/tests_select.rs` & `openlineage_sql-1.9.1/impl/tests/column_lineage/tests_select.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/column_lineage/tests_simple.rs` & `openlineage_sql-1.9.1/impl/tests/column_lineage/tests_simple.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_alter.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_alter.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_copy.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_copy.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_create.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_create.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_cte.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_cte.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_delete.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_delete.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_error_handling.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_error_handling.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_insert.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_insert.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_merge.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_merge.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_select.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_select.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_tpcds.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_tpcds.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/table_lineage/tests_update.rs` & `openlineage_sql-1.9.1/impl/tests/table_lineage/tests_update.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/impl/tests/test_utils/mod.rs` & `openlineage_sql-1.9.1/impl/tests/test_utils/mod.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/iface-py/Cargo.toml` & `openlineage_sql-1.9.1/iface-py/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "openlineage_sql_python"
 description = "Python interface for the Rust OpenLineage lineage extraction library"
-version = "1.9.0"
+version = "1.9.1"
 edition = "2021"
 authors = ["Maciej Obuchowski <obuchowski.maciej@gmail.com>"]
 keywords = ["sql", "lineage", "openlineage", "python"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "openlineage_sql"
```

### Comparing `openlineage_sql-1.9.0/iface-py/openlineage_sql.pyi` & `openlineage_sql-1.9.1/iface-py/openlineage_sql.pyi`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/iface-py/script/build-macos.sh` & `openlineage_sql-1.9.1/iface-py/script/build-macos.sh`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/iface-py/script/build.sh` & `openlineage_sql-1.9.1/iface-py/script/build.sh`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/iface-py/script/setup-macos.sh` & `openlineage_sql-1.9.1/iface-py/script/setup-macos.sh`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/iface-py/src/lib.rs` & `openlineage_sql-1.9.1/iface-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/iface-py/tests/python/sql_tester.py` & `openlineage_sql-1.9.1/iface-py/tests/python/sql_tester.py`

 * *Files identical despite different names*

### Comparing `openlineage_sql-1.9.0/Cargo.lock` & `openlineage_sql-1.9.1/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -121,32 +121,32 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "openlineage_sql"
-version = "1.9.0"
+version = "1.9.1"
 dependencies = [
  "anyhow",
  "sqlparser",
 ]
 
 [[package]]
 name = "openlineage_sql_java"
-version = "1.9.0"
+version = "1.9.1"
 dependencies = [
  "anyhow",
  "jni",
  "openlineage_sql",
 ]
 
 [[package]]
 name = "openlineage_sql_python"
-version = "1.9.0"
+version = "1.9.1"
 dependencies = [
  "anyhow",
  "openlineage_sql",
  "pyo3",
  "pyo3-build-config",
 ]
 
@@ -297,17 +297,17 @@
 source = "git+https://github.com/OpenLineage/sqlparser-rs/?branch=release#411fef2550ebe47ede2c5ac81ccfede495e7d135"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.50"
+version = "2.0.51"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74f1bdc9872430ce9b75da68329d1c1746faf50ffac5f19e02b71e37ff881ffb"
+checksum = "6ab617d94515e94ae53b8406c628598680aa0c9587474ecbe58188f7b345d66c"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

