# Comparing `tmp/muttfuzz-0.6.6-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8116 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3761 b- defN 24-May-24 15:08 muttfuzz/fuzz.py
+Zip file size: 8115 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-24 15:11 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     8226 b- defN 24-May-24 15:08 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     4296 b- defN 24-May-24 15:08 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 15:08 muttfuzz-0.6.6.dist-info/RECORD
-8 files, 21656 bytes uncompressed, 7032 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/RECORD
+8 files, 21656 bytes uncompressed, 7031 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.6.dist-info/METADATA
+Filename: muttfuzz-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.6.dist-info/WHEEL
+Filename: muttfuzz-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.6.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.6.dist-info/top_level.txt
+Filename: muttfuzz-0.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.6.dist-info/RECORD
+Filename: muttfuzz-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -58,15 +58,15 @@
     config = make_config(parsed_args)
     try:
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
-                                   config.avoid_mutating.replace(", ", ",").split(",").
+                                   config.avoid_mutating.replace(", ", ",").split(","),
                                    config.prune_mutant_cmd,
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.status_cmd,
```

## Comparing `muttfuzz-0.6.6.dist-info/METADATA` & `muttfuzz-0.6.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.6
+Version: 0.6.7
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.6.6.dist-info/RECORD` & `muttfuzz-0.6.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=wjktN6N2_nXYKmHsbV9-DWobuSLpU4o3o4gzJPw1vVE,3761
+muttfuzz/fuzz.py,sha256=RhCCkBsokDmyLRRPaX-36wbcd4jI15OfU-9ZP-gF8-I,3761
 muttfuzz/fuzzutil.py,sha256=2k0RL-XBbH3AxBZu2osL0eM9fg_zu6pAd7-m9PBahNY,8226
 muttfuzz/mutate.py,sha256=_rxsqBFHSfeoEEvn0Hkpx2T1UDaRm_WF_NzameVbsBQ,4296
-muttfuzz-0.6.6.dist-info/METADATA,sha256=xTlkrN5EsGNFjxzSaHiIrAIYJ-8GmtcX0ELMpf38tWI,4589
-muttfuzz-0.6.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.6.6.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.6.6.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.6.6.dist-info/RECORD,,
+muttfuzz-0.6.7.dist-info/METADATA,sha256=Hs4p6UCHOdZySfMO4w5xZMgRR6Ir-7H0HrSTtzB1eaI,4589
+muttfuzz-0.6.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.6.7.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.6.7.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.6.7.dist-info/RECORD,,
```

