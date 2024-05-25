# Comparing `tmp/tree_sitter_earthfile-0.4.3-cp38-abi3-win_amd64.whl.zip` & `tmp/tree_sitter_earthfile-0.5.0-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 98469 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 18:17 tree_sitter_earthfile/__init__.py
--rw-rw-rw-  2.0 fat       27 b- defN 24-May-20 18:17 tree_sitter_earthfile/__init__.pyi
--rw-rw-rw-  2.0 fat   481280 b- defN 24-May-20 18:19 tree_sitter_earthfile/_binding.pyd
--rw-rw-rw-  2.0 fat      642 b- defN 24-May-20 18:17 tree_sitter_earthfile/binding.c
--rw-rw-rw-  2.0 fat        0 b- defN 24-May-20 18:17 tree_sitter_earthfile/py.typed
--rw-rw-rw-  2.0 fat     1442 b- defN 24-May-20 18:17 tree_sitter_earthfile/queries/highlights.scm
--rw-rw-rw-  2.0 fat      271 b- defN 24-May-20 18:17 tree_sitter_earthfile/queries/injections.scm
--rw-rw-rw-  2.0 fat     1072 b- defN 24-May-20 18:19 tree_sitter_earthfile-0.4.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      987 b- defN 24-May-20 18:19 tree_sitter_earthfile-0.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-20 18:19 tree_sitter_earthfile-0.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       31 b- defN 24-May-20 18:19 tree_sitter_earthfile-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1098 b- defN 24-May-20 18:19 tree_sitter_earthfile-0.4.3.dist-info/RECORD
-12 files, 487042 bytes uncompressed, 96577 bytes compressed:  80.2%
+Zip file size: 89506 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 11:58 tree_sitter_earthfile/__init__.py
+-rw-rw-rw-  2.0 fat       27 b- defN 24-May-25 11:58 tree_sitter_earthfile/__init__.pyi
+-rw-rw-rw-  2.0 fat   463872 b- defN 24-May-25 12:00 tree_sitter_earthfile/_binding.pyd
+-rw-rw-rw-  2.0 fat      642 b- defN 24-May-25 11:58 tree_sitter_earthfile/binding.c
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-25 11:58 tree_sitter_earthfile/py.typed
+-rw-rw-rw-  2.0 fat     1397 b- defN 24-May-25 11:58 tree_sitter_earthfile/queries/highlights.scm
+-rw-rw-rw-  2.0 fat      271 b- defN 24-May-25 11:58 tree_sitter_earthfile/queries/injections.scm
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-May-25 12:00 tree_sitter_earthfile-0.5.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      987 b- defN 24-May-25 12:00 tree_sitter_earthfile-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-25 12:00 tree_sitter_earthfile-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       31 b- defN 24-May-25 12:00 tree_sitter_earthfile-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1098 b- defN 24-May-25 12:00 tree_sitter_earthfile-0.5.0.dist-info/RECORD
+12 files, 469589 bytes uncompressed, 87614 bytes compressed:  81.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tree_sitter_earthfile/queries/highlights.scm
 Comment: 
 
 Filename: tree_sitter_earthfile/queries/injections.scm
 Comment: 
 
-Filename: tree_sitter_earthfile-0.4.3.dist-info/LICENSE
+Filename: tree_sitter_earthfile-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: tree_sitter_earthfile-0.4.3.dist-info/METADATA
+Filename: tree_sitter_earthfile-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: tree_sitter_earthfile-0.4.3.dist-info/WHEEL
+Filename: tree_sitter_earthfile-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: tree_sitter_earthfile-0.4.3.dist-info/top_level.txt
+Filename: tree_sitter_earthfile-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: tree_sitter_earthfile-0.4.3.dist-info/RECORD
+Filename: tree_sitter_earthfile-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tree_sitter_earthfile/queries/highlights.scm

```diff
@@ -63,13 +63,12 @@
     (double_quoted_string)
     (single_quoted_string)
 ] @string
 (unquoted_string) @string.special
 (escape_sequence) @constant.character.escape
 
 (variable) @variable
-(secret (identifier) @variable.other.member)
 (expansion ["$" "{" "}" "(" ")"] @punctuation.special)
 (build_arg) @variable
 (options (_) @variable.parameter)
 
 "=" @operator
```

## Comparing `tree_sitter_earthfile-0.4.3.dist-info/LICENSE` & `tree_sitter_earthfile-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tree_sitter_earthfile-0.4.3.dist-info/METADATA` & `tree_sitter_earthfile-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-earthfile
-Version: 0.4.3
+Version: 0.5.0
 Summary: Earthfile grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-earthfile
 Keywords: incremental,parsing,tree-sitter,earthfile
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

## Comparing `tree_sitter_earthfile-0.4.3.dist-info/RECORD` & `tree_sitter_earthfile-0.5.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 tree_sitter_earthfile/__init__.py,sha256=b49F9QXcBSzekYK6czZvmdtuGwDStmfTwwwbFGkS8H4,92
 tree_sitter_earthfile/__init__.pyi,sha256=8xf7bY1szgDY9HRJ7FJ326So4SFgMiSRfCB4LADkTpU,27
-tree_sitter_earthfile/_binding.pyd,sha256=4-Uo05SavEU_-NJK05QqAaYIAgId09AgVs4aPH-ezMg,481280
+tree_sitter_earthfile/_binding.pyd,sha256=5sCOHAllWgBKViV7uxDwpXNBCdggxOdsU6L4YITxnV0,463872
 tree_sitter_earthfile/binding.c,sha256=MKxNXwWUTomdXfVWUkzuE2I7Giioe_EcSNnz2Iw-P9Q,642
 tree_sitter_earthfile/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tree_sitter_earthfile/queries/highlights.scm,sha256=qhm-jq9Zne_rPb86soKpbPCF_8JR4jAjYULppHDYIRk,1442
+tree_sitter_earthfile/queries/highlights.scm,sha256=sHHDVqyppK76MTfeSHoaeKUgkEVjJ84jXchDcRWVREE,1397
 tree_sitter_earthfile/queries/injections.scm,sha256=-GVsiRO-9Cz_5wl71HXOXI7zbMv49V8I1sxJXrizujE,271
-tree_sitter_earthfile-0.4.3.dist-info/LICENSE,sha256=_VBuaug4WgiXJ36qNSlMQzxZZmW40iKiVm5SHHBDL3c,1072
-tree_sitter_earthfile-0.4.3.dist-info/METADATA,sha256=1-l1Fkch8fRt84-ZwMiqcpY0fJ738y_35bPIDel2ts4,987
-tree_sitter_earthfile-0.4.3.dist-info/WHEEL,sha256=UyMHzmWA0xVqVPKfTiLs2eN3OWWZUl-kQemNbpIqlKo,100
-tree_sitter_earthfile-0.4.3.dist-info/top_level.txt,sha256=Ddv97tXjIVquwTZTacOwi0oCQaBjxY52xeUX6Riy1vQ,31
-tree_sitter_earthfile-0.4.3.dist-info/RECORD,,
+tree_sitter_earthfile-0.5.0.dist-info/LICENSE,sha256=_VBuaug4WgiXJ36qNSlMQzxZZmW40iKiVm5SHHBDL3c,1072
+tree_sitter_earthfile-0.5.0.dist-info/METADATA,sha256=nnln8yKuQJ9Eilfnh8hYpjsLej1HRZuqy8wUIO3cRh4,987
+tree_sitter_earthfile-0.5.0.dist-info/WHEEL,sha256=UyMHzmWA0xVqVPKfTiLs2eN3OWWZUl-kQemNbpIqlKo,100
+tree_sitter_earthfile-0.5.0.dist-info/top_level.txt,sha256=Ddv97tXjIVquwTZTacOwi0oCQaBjxY52xeUX6Riy1vQ,31
+tree_sitter_earthfile-0.5.0.dist-info/RECORD,,
```

