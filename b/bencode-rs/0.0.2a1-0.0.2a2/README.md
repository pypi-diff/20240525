# Comparing `tmp/bencode_rs-0.0.2a1.tar.gz` & `tmp/bencode_rs-0.0.2a2.tar.gz`

## Comparing `bencode_rs-0.0.2a1.tar` & `bencode_rs-0.0.2a2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a1/Cargo.toml
--rw-r--r--   0     1001      127      120 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.coveragerc
--rw-r--r--   0     1001      127       13 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.gitattributes
--rw-r--r--   0     1001      127      124 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.github/renovate.json
--rw-r--r--   0     1001      127     3345 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.github/workflows/_build_wheels.yaml
--rw-r--r--   0     1001      127      643 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.github/workflows/build.yaml
--rw-r--r--   0     1001      127      538 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.github/workflows/release.yaml
--rw-r--r--   0     1001      127      889 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.github/workflows/tests.yaml
--rw-r--r--   0     1001      127     4828 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/.gitignore
--rw-r--r--   0     1001      127     1085 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/LICENSE
--rw-r--r--   0     1001      127     1081 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/bench.py
--rw-r--r--   0     1001      127      184 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/bencode_rs/__init__.py
--rw-r--r--   0     1001      127      188 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/bencode_rs/__init__.pyi
--rw-r--r--   0     1001      127      732 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/leak.py
--rw-r--r--   0     1001      127      380 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/readme.md
--rw-r--r--   0     1001      127      301 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/rustfmt.toml
--rw-r--r--   0     1001      127     7905 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/src/decode.rs
--rw-r--r--   0     1001      127     5612 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/src/encode.rs
--rw-r--r--   0     1001      127      557 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/src/lib.rs
--rw-r--r--   0     1001      127     5713 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/tests/fixtures/56507.torrent.bin
--rw-r--r--   0     1001      127   376318 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin
--rw-r--r--   0     1001      127     4397 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/tests/test_1_encode.py
--rw-r--r--   0     1001      127     3419 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/tests/test_2_decode.py
--rw-r--r--   0     1001      127     8499 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/Cargo.lock
--rw-r--r--   0     1001      127      807 2024-05-25 18:49:33.000000 bencode_rs-0.0.2a1/pyproject.toml
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a1/PKG-INFO
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a2/Cargo.toml
+-rw-r--r--   0     1001      127      120 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.coveragerc
+-rw-r--r--   0     1001      127       13 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.gitattributes
+-rw-r--r--   0     1001      127      124 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.github/renovate.json
+-rw-r--r--   0     1001      127     3345 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.github/workflows/_build_wheels.yaml
+-rw-r--r--   0     1001      127      643 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.github/workflows/build.yaml
+-rw-r--r--   0     1001      127      538 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.github/workflows/release.yaml
+-rw-r--r--   0     1001      127      921 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.github/workflows/tests.yaml
+-rw-r--r--   0     1001      127     4828 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/.gitignore
+-rw-r--r--   0     1001      127     1085 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/LICENSE
+-rw-r--r--   0     1001      127     1081 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/bench.py
+-rw-r--r--   0     1001      127      184 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/bencode_rs/__init__.py
+-rw-r--r--   0     1001      127      188 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/bencode_rs/__init__.pyi
+-rw-r--r--   0     1001      127      732 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/leak.py
+-rw-r--r--   0     1001      127      380 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/readme.md
+-rw-r--r--   0     1001      127      301 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/rustfmt.toml
+-rw-r--r--   0     1001      127     7905 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/src/decode.rs
+-rw-r--r--   0     1001      127     5612 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/src/encode.rs
+-rw-r--r--   0     1001      127      557 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/src/lib.rs
+-rw-r--r--   0     1001      127     5713 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/tests/fixtures/56507.torrent.bin
+-rw-r--r--   0     1001      127   376318 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin
+-rw-r--r--   0     1001      127     4397 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/tests/test_1_encode.py
+-rw-r--r--   0     1001      127     3419 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/tests/test_2_decode.py
+-rw-r--r--   0     1001      127     8499 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/Cargo.lock
+-rw-r--r--   0     1001      127      802 2024-05-25 18:56:35.000000 bencode_rs-0.0.2a2/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 bencode_rs-0.0.2a2/PKG-INFO
```

### Comparing `bencode_rs-0.0.2a1/Cargo.toml` & `bencode_rs-0.0.2a2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/.github/workflows/_build_wheels.yaml` & `bencode_rs-0.0.2a2/.github/workflows/_build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/.github/workflows/build.yaml` & `bencode_rs-0.0.2a2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/.github/workflows/release.yaml` & `bencode_rs-0.0.2a2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/.github/workflows/tests.yaml` & `bencode_rs-0.0.2a2/.github/workflows/tests.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -32,13 +32,14 @@
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           cache: "pip" # caching pip dependencies
 
+      - run: pip install -U pip
       - run: pip install -e '.[dev]'
 
       - name: Run pytest
         run: python -m pytest -sv
         env:
           RUST_BACKTRACE: 'full'
```

### Comparing `bencode_rs-0.0.2a1/.gitignore` & `bencode_rs-0.0.2a2/.gitignore`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/LICENSE` & `bencode_rs-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/bench.py` & `bencode_rs-0.0.2a2/bench.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/leak.py` & `bencode_rs-0.0.2a2/leak.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/src/decode.rs` & `bencode_rs-0.0.2a2/src/decode.rs`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/src/encode.rs` & `bencode_rs-0.0.2a2/src/encode.rs`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/src/lib.rs` & `bencode_rs-0.0.2a2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/tests/fixtures/56507.torrent.bin` & `bencode_rs-0.0.2a2/tests/fixtures/56507.torrent.bin`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin` & `bencode_rs-0.0.2a2/tests/fixtures/ubuntu-22.04.2-desktop-amd64.iso.torrent.bin`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/tests/test_1_encode.py` & `bencode_rs-0.0.2a2/tests/test_1_encode.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/tests/test_2_decode.py` & `bencode_rs-0.0.2a2/tests/test_2_decode.py`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/Cargo.lock` & `bencode_rs-0.0.2a2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bencode_rs-0.0.2a1/pyproject.toml` & `bencode_rs-0.0.2a2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "bencode-rs"
-version = "0.0.2a1"
+version = "0.0.2a2"
 requires-python = ">=3.8,<4.0"
 description = "a bencode parser binding build with pyo3"
 readme = "readme.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+]
+keywords = [
+    "bittorrent",
+    "bencode",
+    "p2p",
 ]
 
 [project.optional-dependencies]
 dev = [
     # lint
     "pre-commit",
     # testing
```

### Comparing `bencode_rs-0.0.2a1/PKG-INFO` & `bencode_rs-0.0.2a2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.3
 Name: bencode-rs
-Version: 0.0.2a1
+Version: 0.0.2a2
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pre-commit ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-github-actions-annotate-failures ==0.2.0 ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Summary: a bencode parser binding build with pyo3
+Keywords: bittorrent,bencode,p2p
 Requires-Python: >=3.8, <4.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # A bencode serialize/deserialize library based on cython
 
 ## install
```

