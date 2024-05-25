# Comparing `tmp/muttfuzz-0.6.7-py3-none-any.whl.zip` & `tmp/muttfuzz-0.6.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8115 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3761 b- defN 24-May-24 15:11 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     8226 b- defN 24-May-24 15:08 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     4296 b- defN 24-May-24 15:08 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-24 15:11 muttfuzz-0.6.7.dist-info/RECORD
-8 files, 21656 bytes uncompressed, 7031 bytes compressed:  67.5%
+Zip file size: 8221 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4064 b- defN 24-May-25 14:43 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     8277 b- defN 24-May-25 14:43 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     4648 b- defN 24-May-25 14:43 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-25 14:44 muttfuzz-0.6.8.dist-info/RECORD
+8 files, 22362 bytes uncompressed, 7137 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.7.dist-info/METADATA
+Filename: muttfuzz-0.6.8.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.7.dist-info/WHEEL
+Filename: muttfuzz-0.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.7.dist-info/entry_points.txt
+Filename: muttfuzz-0.6.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.7.dist-info/top_level.txt
+Filename: muttfuzz-0.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.7.dist-info/RECORD
+Filename: muttfuzz-0.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -13,16 +13,18 @@
                         help='executable to be fuzzer/mutated')
     parser.add_argument('--budget', type=int, default=3600,
                         help='total fuzzing budget in seconds (default 3600)')
     parser.add_argument('--time_per_mutant', type=int, default=300,
                         help='max time to fuzz each mutant in seconds (default 300)')
     parser.add_argument('--fraction_mutant', type=float, default=0.5,
                         help='portion of budget to devote to mutants (default 0.5)')
+    parser.add_argument('--only_mutate', type=str, default="",
+                        help='string with comma delimited list of functions patterns to mutate (match by simple inclusion)')
     parser.add_argument('--avoid_mutating', type=str, default="",
-                        help='string with comma delimited list of sections not to mutate inside')
+                        help='string with comma delimited list of function patterns not to mutate (match by simple inclusion)')
     parser.add_argument('--prune_mutant_cmd', type=str, default="",
                         help='command to check mutants for validity/interest')
     parser.add_argument('--prune_mutant_timeout', type=float, default=2.0,
                         help='timeout for mutant check')
     parser.add_argument('--initial_fuzz_cmd', type=str, default="",
                         help='command for initial fuzzing before mutants')
     parser.add_argument('--initial_budget', type=int, default=60,
@@ -58,14 +60,15 @@
     config = make_config(parsed_args)
     try:
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
+                                   config.only_mutate.replace(", ", ",").split(","),
                                    config.avoid_mutating.replace(", ", ",").split(","),
                                    config.prune_mutant_cmd,
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
```

## muttfuzz/fuzzutil.py

```diff
@@ -54,25 +54,26 @@
     finally:
         if P.poll() is None:
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
     return P.returncode
 
 
 def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
+                      only_mutate=[],
                       avoid_mutating=[],
                       prune_mutant_cmd="",
                       prune_mutant_timeout=1,
                       initial_fuzz_cmd="",
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
                       status_cmd="",
                       order=1):
     executable_code = mutate.get_code(executable)
-    executable_jumps = mutate.get_jumps(executable, avoid_mutating)
+    executable_jumps = mutate.get_jumps(executable, only_mutate, avoid_mutating)
     start_fuzz = time.time()
     mutant_no = 1
     try:
         if initial_fuzz_cmd != "":
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
```

## muttfuzz/mutate.py

```diff
@@ -7,15 +7,15 @@
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
 NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
 
-def get_jumps(filename, avoid_mutating=[]):
+def get_jumps(filename, only_mutate=[], avoid_mutating=[]):
     jumps = {}
 
     proc = subprocess.Popen(["objdump", "-d", "--file-offsets", filename],
                             stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     out, err = proc.communicate()
     output = str(out, encoding="utf-8")
 
@@ -25,14 +25,23 @@
         try:
             if "File Offset" in line and line[-1] == ":":
                 avoid = False
                 section_name = line.split()[1]
                 for s in avoid_mutating:
                     if s in section_name:
                         avoid = True
+                        break
+                if only_mutate != []:
+                    found = False
+                    for s in only_mutate:
+                        if s in section_name:
+                            found = True
+                            break
+                    if not found:
+                        avoid = True
                 section_base = int(line.split()[0], 16)
                 offset_hex = line.split("File Offset:")[1].split(")")[0]
                 section_offset = int(offset_hex, 16) - section_base
                 continue
             if avoid:
                 continue
             found_inst = False
```

## Comparing `muttfuzz-0.6.7.dist-info/METADATA` & `muttfuzz-0.6.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.7
+Version: 0.6.8
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.6.7.dist-info/RECORD` & `muttfuzz-0.6.8.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=RhCCkBsokDmyLRRPaX-36wbcd4jI15OfU-9ZP-gF8-I,3761
-muttfuzz/fuzzutil.py,sha256=2k0RL-XBbH3AxBZu2osL0eM9fg_zu6pAd7-m9PBahNY,8226
-muttfuzz/mutate.py,sha256=_rxsqBFHSfeoEEvn0Hkpx2T1UDaRm_WF_NzameVbsBQ,4296
-muttfuzz-0.6.7.dist-info/METADATA,sha256=Hs4p6UCHOdZySfMO4w5xZMgRR6Ir-7H0HrSTtzB1eaI,4589
-muttfuzz-0.6.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.6.7.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.6.7.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.6.7.dist-info/RECORD,,
+muttfuzz/fuzz.py,sha256=kXOW5-pXGneTVMqPYCikiPfWpEG6hSf1pbEbrmi00Xo,4064
+muttfuzz/fuzzutil.py,sha256=AKuqtH0UrquHjc998RHhgvdSEBgGrrAToFecnU9-Pb8,8277
+muttfuzz/mutate.py,sha256=wmQJ-PUCTK2rl_bp6H_8NHUxLDP5JjRYLQiwVmq3Nyc,4648
+muttfuzz-0.6.8.dist-info/METADATA,sha256=YnUCfXSaR5ET3g5v5wGqNUouVYaqFyOBX0own5e_VYs,4589
+muttfuzz-0.6.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.6.8.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.6.8.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.6.8.dist-info/RECORD,,
```

