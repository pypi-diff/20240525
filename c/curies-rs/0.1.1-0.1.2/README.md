# Comparing `tmp/curies_rs-0.1.1-cp39-cp39-musllinux_1_1_x86_64.whl.zip` & `tmp/curies_rs-0.1.2-pp39-pypy39_pp73-macosx_10_12_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,8 @@
-Zip file size: 3824427 bytes, number of entries: 9
--rw-r--r--  4.6 unx     2796 b- defN 24-Jan-02 17:31 curies_rs-0.1.1.dist-info/METADATA
--rw-r--r--  4.6 unx      105 b- defN 24-Jan-02 17:31 curies_rs-0.1.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     1076 b- defN 24-Jan-02 17:31 curies_rs-0.1.1.dist-info/license_files/LICENSE
--rwxr-xr-x  4.6 unx   568065 b- defN 24-Jan-02 17:31 curies_rs.libs/libssl-5babfe3f.so.1.1
--rwxr-xr-x  4.6 unx    81257 b- defN 24-Jan-02 17:31 curies_rs.libs/libgcc_s-a04fdf82.so.1
--rwxr-xr-x  4.6 unx  2730009 b- defN 24-Jan-02 17:31 curies_rs.libs/libcrypto-f4bea926.so.1.1
--rw-r--r--  4.6 unx      119 b- defN 24-Jan-02 17:31 curies_rs/__init__.py
--rwxr-xr-x  4.6 unx  6787065 b- defN 24-Jan-02 17:31 curies_rs/curies_rs.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      795 b- defN 24-Jan-02 17:31 curies_rs-0.1.1.dist-info/RECORD
-9 files, 10171287 bytes uncompressed, 3823063 bytes compressed:  62.4%
+Zip file size: 2324053 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     3364 b- defN 24-May-25 08:44 curies_rs-0.1.2.dist-info/METADATA
+-rw-r--r--  4.6 unx      111 b- defN 24-May-25 08:44 curies_rs-0.1.2.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1076 b- defN 24-May-25 08:44 curies_rs-0.1.2.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      119 b- defN 24-May-25 08:44 curies_rs/__init__.py
+-rwxr-xr-x  4.6 unx  5518768 b- defN 24-May-25 08:44 curies_rs/curies_rs.pypy39-pp73-darwin.so
+-rw-r--r--  4.6 unx      495 b- defN 24-May-25 08:44 curies_rs-0.1.2.dist-info/RECORD
+6 files, 5523933 bytes uncompressed, 2323163 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -1,28 +1,19 @@
-Filename: curies_rs-0.1.1.dist-info/METADATA
+Filename: curies_rs-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: curies_rs-0.1.1.dist-info/WHEEL
+Filename: curies_rs-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: curies_rs-0.1.1.dist-info/license_files/LICENSE
-Comment: 
-
-Filename: curies_rs.libs/libssl-5babfe3f.so.1.1
-Comment: 
-
-Filename: curies_rs.libs/libgcc_s-a04fdf82.so.1
-Comment: 
-
-Filename: curies_rs.libs/libcrypto-f4bea926.so.1.1
+Filename: curies_rs-0.1.2.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: curies_rs/__init__.py
 Comment: 
 
-Filename: curies_rs/curies_rs.cpython-39-x86_64-linux-gnu.so
+Filename: curies_rs/curies_rs.pypy39-pp73-darwin.so
 Comment: 
 
-Filename: curies_rs-0.1.1.dist-info/RECORD
+Filename: curies_rs-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `curies_rs-0.1.1.dist-info/METADATA` & `curies_rs-0.1.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies-rs
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,20 +27,35 @@
 Project-URL: Tracker, https://github.com/biopragmatics/curies.rs/issues
 
 <h1 align="center">
   🦀 curies.rs
 </h1>
 
 <p align="center">
+    <a href="https://crates.io/crates/curies">
+        <img alt="crates.io" src="https://img.shields.io/crates/v/curies.svg" />
+    </a>
+    <a href="https://www.npmjs.com/package/@biopragmatics/curies">
+        <img alt="npm" src="https://img.shields.io/npm/v/@biopragmatics/curies" />
+    </a>
+    <a href="https://pypi.org/project/curies-rs">
+        <img alt="PyPI" src="https://img.shields.io/pypi/v/curies-rs" />
+    </a>
+</p>
+
+<p align="center">
     <a href="https://github.com/biopragmatics/curies.rs/actions/workflows/test.yml">
         <img alt="Test" src="https://github.com/biopragmatics/curies.rs/actions/workflows/test.yml/badge.svg" />
     </a>
     <a href="https://github.com/biopragmatics/curies.rs/actions/workflows/build.yml">
         <img alt="Build" src="https://github.com/biopragmatics/curies.rs/actions/workflows/build.yml/badge.svg" />
     </a>
+    <a href="https://docs.rs/curies">
+        <img alt="crates" src="https://docs.rs/curies/badge.svg" />
+    </a>
     <a href="https://deps.rs/repo/github/biopragmatics/curies.rs">
         <img src="https://deps.rs/repo/github/biopragmatics/curies.rs/status.svg" alt="Dependency status" />
     </a>
     <a href="https://github.com/biopragmatics/curies.rs/blob/main/LICENSE">
         <img alt="MIT license" src="https://img.shields.io/badge/License-MIT-brightgreen.svg" />
     </a>
     <a href="https://codecov.io/gh/biopragmatics/curies.rs/branch/main">
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies-rs Version: 0.1.1 Classifier: Development
+Metadata-Version: 2.1 Name: curies-rs Version: 0.1.2 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Rust Classifier: Topic :: Software Development :: Libraries ::
@@ -16,13 +16,14 @@
 charset=UTF-8; variant=GFM Project-URL: Changelog, https://github.com/
 biopragmatics/curies.rs/blob/main/CHANGELOG.md Project-URL: Documentation,
 https://biopragmatics.github.io/curies.rs Project-URL: Homepage, https://
 biopragmatics.github.io/curies.rs Project-URL: Source, https://github.com/
 biopragmatics/curies.rs/tree/main/python Project-URL: Tracker, https://
 github.com/biopragmatics/curies.rs/issues
                          ************ ?ð??¦? ccuurriieess..rrss ************
-         _[_T_e_s_t_]_[_B_u_i_l_d_]_[_D_e_p_e_n_d_e_n_c_y_ _s_t_a_t_u_s_]_[_M_I_T_ _l_i_c_e_n_s_e_]_[_C_o_d_e_c_o_v_ _s_t_a_t_u_s_]
+                            _[_c_r_a_t_e_s_._i_o_]_[_n_p_m_]_[_P_y_P_I_]
+     _[_T_e_s_t_]_[_B_u_i_l_d_]_[_c_r_a_t_e_s_]_[_D_e_p_e_n_d_e_n_c_y_ _s_t_a_t_u_s_]_[_M_I_T_ _l_i_c_e_n_s_e_]_[_C_o_d_e_c_o_v_ _s_t_a_t_u_s_]
 Idiomatic conversion between URIs and compact URIs (CURIEs) in Rust, with
 bindings to Python, and JavaScript compiled to WebAssembly. ## ð
 Documentation Checkout the **[biopragmatics.github.io/curies.rs](https://
 biopragmatics.github.io/curies.rs)** for more details on how to install and use
 it.
```

## Comparing `curies_rs-0.1.1.dist-info/license_files/LICENSE` & `curies_rs-0.1.2.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

