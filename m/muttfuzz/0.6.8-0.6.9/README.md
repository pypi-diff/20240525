# Comparing `tmp/muttfuzz-0.6.8-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8221 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4064 b- defN 24-May-25 14:43 muttfuzz/fuzz.py
+Zip file size: 8237 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4102 b- defN 24-May-25 14:56 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     8277 b- defN 24-May-25 14:43 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     4648 b- defN 24-May-25 14:43 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/RECORD
-8 files, 22362 bytes uncompressed, 7137 bytes compressed:  68.1%
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/RECORD
+8 files, 22400 bytes uncompressed, 7153 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.8.dist-info/METADATA
+Filename: muttfuzz-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.8.dist-info/WHEEL
+Filename: muttfuzz-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.8.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.8.dist-info/top_level.txt
+Filename: muttfuzz-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.8.dist-info/RECORD
+Filename: muttfuzz-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -60,16 +60,16 @@
     config = make_config(parsed_args)
     try:
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
-                                   config.only_mutate.replace(", ", ",").split(","),
-                                   config.avoid_mutating.replace(", ", ",").split(","),
+                                   list(filter(None, config.only_mutate.replace(", ", ",").split(",")),
+                                   list(filter(None, config.avoid_mutating.replace(", ", ",").split(",")),
                                    config.prune_mutant_cmd,
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.status_cmd,
```

## Comparing `muttfuzz-0.6.8.dist-info/METADATA` & `muttfuzz-0.6.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.8
+Version: 0.6.9
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.6.8.dist-info/RECORD` & `muttfuzz-0.6.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=kXOW5-pXGneTVMqPYCikiPfWpEG6hSf1pbEbrmi00Xo,4064
+muttfuzz/fuzz.py,sha256=IAJqVAOdeFRkU3RAXq5t6ARnrghAxH3OqPOZk0otshU,4102
 muttfuzz/fuzzutil.py,sha256=AKuqtH0UrquHjc998RHhgvdSEBgGrrAToFecnU9-Pb8,8277
 muttfuzz/mutate.py,sha256=wmQJ-PUCTK2rl_bp6H_8NHUxLDP5JjRYLQiwVmq3Nyc,4648
-muttfuzz-0.6.8.dist-info/METADATA,sha256=YnUCfXSaR5ET3g5v5wGqNUouVYaqFyOBX0own5e_VYs,4589
-muttfuzz-0.6.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.6.8.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.6.8.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.6.8.dist-info/RECORD,,
+muttfuzz-0.6.9.dist-info/METADATA,sha256=0hkR5GmPdg2KeXBHeUTiVq55foOfyIeYUVloVk7hlzs,4589
+muttfuzz-0.6.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.6.9.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.6.9.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.6.9.dist-info/RECORD,,
```

