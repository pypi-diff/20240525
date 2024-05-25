# Comparing `tmp/sil-thot-3.4.3.tar.gz` & `tmp/sil_thot-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sil-thot-3.4.3.tar", last modified: Thu Nov 30 21:38:02 2023, max compression
+gzip compressed data, was "sil_thot-3.4.4.tar", last modified: Fri May 24 23:56:50 2024, max compression
```

## Comparing `sil-thot-3.4.3.tar` & `sil_thot-3.4.4.tar`

### file list

```diff
@@ -1,431 +1,431 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.216681 sil-thot-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-11-30 21:37:53.000000 sil-thot-3.4.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2023-11-30 21:37:53.000000 sil-thot-3.4.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2023-11-30 21:37:53.000000 sil-thot-3.4.3/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-30 21:37:53.000000 sil-thot-3.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-11-30 21:38:02.216681 sil-thot-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-11-30 21:37:53.000000 sil-thot-3.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.148680 sil-thot-3.4.3/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-11-30 21:37:53.000000 sil-thot-3.4.3/cmake/FindGMP.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.144680 sil-thot-3.4.3/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.152680 sil-thot-3.4.3/include/hat_trie/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/array_growth_policy.h
--rw-r--r--   0 runner    (1001) docker     (127)    65286 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/array_hash.h
--rw-r--r--   0 runner    (1001) docker     (127)    31617 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/array_map.h
--rw-r--r--   0 runner    (1001) docker     (127)    24739 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)    80533 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/htrie_hash.h
--rw-r--r--   0 runner    (1001) docker     (127)    22544 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/htrie_map.h
--rw-r--r--   0 runner    (1001) docker     (127)    19656 2023-11-30 21:37:53.000000 sil-thot-3.4.3/include/hat_trie/htrie_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-11-30 21:37:53.000000 sil-thot-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 21:38:02.216681 sil-thot-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-11-30 21:37:53.000000 sil-thot-3.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.216681 sil-thot-3.4.3/sil_thot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2023-11-30 21:38:02.000000 sil-thot-3.4.3/sil_thot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13537 2023-11-30 21:38:02.000000 sil-thot-3.4.3/sil_thot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 21:38:02.000000 sil-thot-3.4.3/sil_thot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 21:38:02.000000 sil-thot-3.4.3/sil_thot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-30 21:38:02.000000 sil-thot-3.4.3/sil_thot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-30 21:38:02.000000 sil-thot-3.4.3/sil_thot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.152680 sil-thot-3.4.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.152680 sil-thot-3.4.3/src/downhill_simplex/
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/downhill_simplex/step_by_step_dhs.c
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/downhill_simplex/step_by_step_dhs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.156680 sil-thot-3.4.3/src/error_correction/
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/BaseEcModelForNbUcat.h
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/BaseEcmForWg.h
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/BaseEditDist.h
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/BaseErrorCorrectionModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/BaseErrorCorrectionModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/BaseWgProcessorForAnlp.h
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/EditDistForStr.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/EditDistForStr.h
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/EditDistForVec.h
--rw-r--r--   0 runner    (1001) docker     (127)    16788 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/EditDistForVecString.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/EditDistForVecString.h
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/HypStateIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NbSearchHighLevelHyp.h
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NbSearchHyp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NbSearchStack.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NbSearchStack.h
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NbestCorrections.h
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NonPbEcModelForNbUcat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/NonPbEcModelForNbUcat.h
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/PfsmEcm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/PfsmEcm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/PfsmEcmForWg.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/PfsmEcmForWg.h
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/PfsmEcmForWgEsi.h
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/PrefAlignInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/RejectedWordsSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WgHandler.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WgHandler.h
--rw-r--r--   0 runner    (1001) docker     (127)    55383 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WgProcessorForAnlp.h
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WordAndCharLevelOps.h
--rw-r--r--   0 runner    (1001) docker     (127)    45668 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WordGraph.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WordGraph.h
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WordGraphArc.h
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WordGraphArcId.h
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/WordGraphStateData.h
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/_editDist.h
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/_editDistBasedEcm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/error_correction/_editDistBasedEcm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.160680 sil-thot-3.4.3/src/incr_models/
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/BaseIncrCondProbModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/BaseIncrCondProbTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/BaseIncrEncCondProbModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/BaseIncrEncoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/BaseWordPenaltyModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    17917 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/IncrCondProbTable.h
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/IncrEncoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/IncrJelMerNgramLM.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/IncrJelMerNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/IncrNgramLM.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/IncrNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/WordPenaltyModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/WordPenaltyModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/WordPredictor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/WordPredictor.h
--rw-r--r--   0 runner    (1001) docker     (127)    27535 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/_incrEncCondProbModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    12128 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/_incrJelMerNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (127)    19692 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/_incrNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/im_pair.h
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/lm_ienc.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/lm_ienc.h
--rw-r--r--   0 runner    (1001) docker     (127)    19410 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/vecx_x_incr_cptable.h
--rw-r--r--   0 runner    (1001) docker     (127)     5346 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/vecx_x_incr_ecpm.h
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/incr_models/vecx_x_incr_enc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.168681 sil-thot-3.4.3/src/nlp_common/
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/AwkInputStream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/AwkInputStream.h
--rw-r--r--   0 runner    (1001) docker     (127)     9549 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/BaseIncrNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/BaseNgramLM.h
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/BidTrie.h
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Bitset.h
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Count.h
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/ErrorDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Exceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/LM_Defs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/LogCount.h
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/MathDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/MathFuncs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/MathFuncs.h
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/NbestTableNode.h
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/NbestTransTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/OrderedVector.h
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/PositionIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Prob.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Prob.h
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Score.h
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/SingleWordVocab.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/SingleWordVocab.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/SmtDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/StrProcUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/StrProcUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/TranslationData.h
--rw-r--r--   0 runner    (1001) docker     (127)    19128 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/Trie.h
--rw-r--r--   0 runner    (1001) docker     (127)    12708 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/TrieVecs.h
--rw-r--r--   0 runner    (1001) docker     (127)    13070 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/WordAlignmentMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/WordAlignmentMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/WordClasses.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/WordClasses.h
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/WordIndex.h
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/ctimer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/ctimer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/getdelim.c
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/getdelim.h
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/getline.c
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/getline.h
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/ins_op_pair.h
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/lt_op_vec.h
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/printAligFuncs.cc
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/printAligFuncs.h
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/uiHashF.h
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/nlp_common/uiPairHashF.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.176680 sil-thot-3.4.3/src/phrase_models/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/AligInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)    14190 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/AlignmentContainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/AlignmentContainer.h
--rw-r--r--   0 runner    (1001) docker     (127)    16515 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/AlignmentExtractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/AlignmentExtractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BaseCountPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BaseIncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BaseIncrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BasePhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BasePhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BasePhrasePairFilter.h
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BasePhraseTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BpSet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BpSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/BpSetInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/CategPhrasePairFilter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/CategPhrasePairFilter.h
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/CellAlignment.h
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/CellID.h
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/HatTriePhraseTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/HatTriePhraseTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/IncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/IncrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseExtractParameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseExtractUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseExtractUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseExtractionCell.h
--rw-r--r--   0 runner    (1001) docker     (127)    35713 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseExtractionTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4959 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseExtractionTable.h
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseId.h
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhrasePair.h
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhrasePairInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseSortCriterion.h
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/PhraseTransTableNodeData.h
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SegLenTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SegLenTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SentSegmentation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrcSegmLenTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrcSegmLenTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrfBisegm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrfNodeInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrfNodeInfoMap.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrfNodeInfoMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrfNodeKey.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/SrfNodeKey.h
--rw-r--r--   0 runner    (1001) docker     (127)    17251 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/StlPhraseTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/StlPhraseTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/StrictCategPhrasePairFilter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/StrictCategPhrasePairFilter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/TrgCutsTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/TrgCutsTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/TrgSegmLenTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/TrgSegmLenTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/VecUnsignedIntSortCriterion.h
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/WbaIncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/WbaIncrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    16505 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/_incrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/_incrPhraseModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/_wbaIncrPhraseModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/phrase_models/_wbaIncrPhraseModel.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.176680 sil-thot-3.4.3/src/python_module/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/python_module/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    44740 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/python_module/module.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.180681 sil-thot-3.4.3/src/shared_library/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/shared_library/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    37191 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/shared_library/thot.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/shared_library/thot.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.200681 sil-thot-3.4.3/src/stack_dec/
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseAssistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseHypState.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseHypState.h
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseHypothesis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseHypothesisRec.h
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseLogLinWeightUpdater.h
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseMiraScorer.h
--rw-r--r--   0 runner    (1001) docker     (127)    10597 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BasePbTransModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BasePbTransModelFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BasePbTransModelStats.h
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BasePhraseHypothesis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BasePhraseHypothesisRec.h
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseScorer.h
--rw-r--r--   0 runner    (1001) docker     (127)     8574 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseSmtModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseSmtMultiStack.h
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseSmtStack.h
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseStackDecoder.h
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/BaseTranslationMetadata.h
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/DictFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/DictFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/DirectPhraseModelFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/DirectPhraseModelFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/FeaturesInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/HypSortCriterion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/HypStateDict.h
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/HypStateDictData.h
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/InversePhraseModelFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/InversePhraseModelFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/KbMiraLlWu.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/KbMiraLlWu.h
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/LM_State.h
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/LangModelFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/LangModelFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/LangModelInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/LangModelPars.h
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraBleu.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraBleu.h
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraChrF.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraChrF.h
--rw-r--r--   0 runner    (1001) docker     (127)     7882 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraGtm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraGtm.h
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraWer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/MiraWer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/NbestTransCacheData.h
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/OnTheFlyDictFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/OnTheFlyDictFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/OnlineTrainingPars.h
--rw-r--r--   0 runner    (1001) docker     (127)    11540 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PbTransModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PbTransModelInputVars.h
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PbTransModelPars.h
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypData.h
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypDataStr.h
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypEqClassF.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypEqClassF.h
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumps01EqClassF.h
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumpsEqClassF.h
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypState.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrHypState.h
--rw-r--r--   0 runner    (1001) docker     (127)    48659 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrLocalSwLiTm.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrLocalSwLiTm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrLocalSwLiTmHypRec.h
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTable.h
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTablePref.h
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTablePrefKey.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTablePrefKey.h
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTableRef.h
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTableRefKey.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrNbestTransTableRefKey.h
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrScoreInfo.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrScoreInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhraseBasedTmHyp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhraseBasedTmHypRec.h
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhraseCacheTable.h
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhraseModelInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhraseModelPars.h
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/PhrasePairCacheTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/ScoreCompDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SmtModelUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SmtModelUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SmtMultiStackRec.h
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SmtStack.h
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SourceSegmentation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SrcPhraseLenFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SrcPhraseLenFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SrcPosJumpFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SrcPosJumpFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SwModelInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/SwModelPars.h
--rw-r--r--   0 runner    (1001) docker     (127)    17974 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/TranslationMetadata.h
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/TrgPhraseLenFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/TrgPhraseLenFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)    10269 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/WeightUpdateUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/WeightUpdateUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/WgUncoupledAssistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/WordPenaltyFeat.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/WordPenaltyFeat.h
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_assistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_nbUncoupledAssistedTrans.h
--rw-r--r--   0 runner    (1001) docker     (127)   105202 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_pbTransModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    21148 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_phrSwTransModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    99378 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_phraseBasedTransModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_phraseHypothesis.h
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_phraseHypothesisRec.h
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_smtModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_smtMultiStack.h
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_smtStack.h
--rw-r--r--   0 runner    (1001) docker     (127)    37194 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_stackDecoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_stackDecoderRec.h
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/_stack_decoder_statistics.h
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/bleu.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/bleu.h
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/chrf.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/chrf.h
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/stack_dec/multi_stack_decoder_rec.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/src/sw_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Aligner.h
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/AlignmentInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/AlignmentModelBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/AlignmentModelBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/AlignmentTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/AlignmentTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/CachedHmmAligLgProb.cc
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/CachedHmmAligLgProb.h
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/DiagonalAlignment.h
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/DistortionTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/DistortionTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/DoubleMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/DoubleMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    25734 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/FastAlignModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/FastAlignModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/FertilityTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/FertilityTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/HeadDistortionTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/HeadDistortionTable.h
--rw-r--r--   0 runner    (1001) docker     (127)    38778 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/HmmAlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/HmmAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/HmmAlignmentTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/HmmAlignmentTable.h
--rw-r--r--   0 runner    (1001) docker     (127)    17187 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm1AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm1AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    11461 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm2AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm2AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    35398 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm3AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm3AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    18602 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm4AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Ibm4AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    21402 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentTrainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentTrainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentTrainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentTrainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentTrainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentTrainer.h
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/LexCounts.h
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/LexTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/LightSentenceHandler.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/LightSentenceHandler.h
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/Md.h
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/MemoryLexTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/MemoryLexTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/NonheadDistortionTable.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/NonheadDistortionTable.h
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/NormalSentenceLengthModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/NormalSentenceLengthModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SentenceHandler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SentenceLengthModel.h
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SentenceLengthModelBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SentenceLengthModelBase.h
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/StepwiseAlignmentModel.h
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SwDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SymmetrizedAligner.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/SymmetrizedAligner.h
--rw-r--r--   0 runner    (1001) docker     (127)    13117 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/anjiMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/anjiMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/anjm1ip_anjiMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2023-11-30 21:37:53.000000 sil-thot-3.4.3/src/sw_models/anjm1ip_anjiMatrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/tests/nlp_common/
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/nlp_common/WordAlignmentMatrixTest.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/tests/phrase_models/
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/phrase_models/HatTriePhraseTableTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/phrase_models/StlPhraseTableTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18181 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/phrase_models/_phraseTableTest.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/tests/stack_dec/
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/stack_dec/KbMiraLlWuTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/stack_dec/MiraChrFTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/stack_dec/PhrLocalSwLiTmTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/stack_dec/TranslationMetadataTest.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/tests/sw_models/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/FastAlignModelTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/Ibm4AlignmentModelTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/IncrHmmAlignmentModelTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/LexTableTest.h
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/MemoryLexTableTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/TestUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/sw_models/TestUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2023-11-30 21:37:53.000000 sil-thot-3.4.3/tests/test_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/thot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/thot/alignment/
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2023-11-30 21:37:53.000000 sil-thot-3.4.3/thot/alignment/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.212681 sil-thot-3.4.3/thot/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2023-11-30 21:37:53.000000 sil-thot-3.4.3/thot/common/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 21:37:53.000000 sil-thot-3.4.3/thot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 21:38:02.216681 sil-thot-3.4.3/thot/translation/
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2023-11-30 21:37:53.000000 sil-thot-3.4.3/thot/translation/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-24 23:56:45.000000 sil_thot-3.4.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-24 23:56:45.000000 sil_thot-3.4.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-24 23:56:45.000000 sil_thot-3.4.4/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 23:56:45.000000 sil_thot-3.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-24 23:56:50.615701 sil_thot-3.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-24 23:56:45.000000 sil_thot-3.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.555701 sil_thot-3.4.4/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-24 23:56:45.000000 sil_thot-3.4.4/cmake/FindGMP.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.551701 sil_thot-3.4.4/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.555701 sil_thot-3.4.4/include/hat_trie/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/array_growth_policy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    65286 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/array_hash.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31617 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/array_map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24739 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80533 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/htrie_hash.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22544 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/htrie_map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19656 2024-05-24 23:56:45.000000 sil_thot-3.4.4/include/hat_trie/htrie_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-24 23:56:45.000000 sil_thot-3.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 23:56:50.615701 sil_thot-3.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-24 23:56:45.000000 sil_thot-3.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/sil_thot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-24 23:56:50.000000 sil_thot-3.4.4/sil_thot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13537 2024-05-24 23:56:50.000000 sil_thot-3.4.4/sil_thot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:56:50.000000 sil_thot-3.4.4/sil_thot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:56:50.000000 sil_thot-3.4.4/sil_thot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 23:56:50.000000 sil_thot-3.4.4/sil_thot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 23:56:50.000000 sil_thot-3.4.4/sil_thot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.555701 sil_thot-3.4.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.555701 sil_thot-3.4.4/src/downhill_simplex/
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/downhill_simplex/step_by_step_dhs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/downhill_simplex/step_by_step_dhs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.563701 sil_thot-3.4.4/src/error_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/BaseEcModelForNbUcat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/BaseEcmForWg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/BaseEditDist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/BaseErrorCorrectionModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/BaseErrorCorrectionModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/BaseWgProcessorForAnlp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/EditDistForStr.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/EditDistForStr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/EditDistForVec.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16788 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/EditDistForVecString.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/EditDistForVecString.h
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/HypStateIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NbSearchHighLevelHyp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NbSearchHyp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NbSearchStack.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NbSearchStack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NbestCorrections.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NonPbEcModelForNbUcat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/NonPbEcModelForNbUcat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/PfsmEcm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/PfsmEcm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/PfsmEcmForWg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/PfsmEcmForWg.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/PfsmEcmForWgEsi.h
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/PrefAlignInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/RejectedWordsSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WgHandler.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WgHandler.h
+-rw-r--r--   0 runner    (1001) docker     (127)    55383 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WgProcessorForAnlp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WordAndCharLevelOps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    45668 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WordGraph.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WordGraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WordGraphArc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WordGraphArcId.h
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/WordGraphStateData.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/_editDist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/_editDistBasedEcm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/error_correction/_editDistBasedEcm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.567701 sil_thot-3.4.4/src/incr_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/BaseIncrCondProbModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/BaseIncrCondProbTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/BaseIncrEncCondProbModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/BaseIncrEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/BaseWordPenaltyModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17917 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/IncrCondProbTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/IncrEncoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/IncrJelMerNgramLM.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/IncrJelMerNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/IncrNgramLM.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/IncrNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/WordPenaltyModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/WordPenaltyModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/WordPredictor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/WordPredictor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27535 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/_incrEncCondProbModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12128 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/_incrJelMerNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19692 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/_incrNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/im_pair.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/lm_ienc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/lm_ienc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19410 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/vecx_x_incr_cptable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/vecx_x_incr_ecpm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/incr_models/vecx_x_incr_enc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.575701 sil_thot-3.4.4/src/nlp_common/
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/AwkInputStream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/AwkInputStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/BaseIncrNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/BaseNgramLM.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/BidTrie.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Bitset.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Count.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/ErrorDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Exceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/LM_Defs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/LogCount.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/MathDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/MathFuncs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/MathFuncs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/NbestTableNode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/NbestTransTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/OrderedVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/PositionIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Prob.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Prob.h
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Score.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/SingleWordVocab.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/SingleWordVocab.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/SmtDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/StrProcUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/StrProcUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/TranslationData.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19128 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/Trie.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/TrieVecs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/WordAlignmentMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/WordAlignmentMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/WordClasses.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/WordClasses.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/WordIndex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/ctimer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/ctimer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/getdelim.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/getdelim.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/getline.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/getline.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/ins_op_pair.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/lt_op_vec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/printAligFuncs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/printAligFuncs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/uiHashF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/nlp_common/uiPairHashF.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.583701 sil_thot-3.4.4/src/phrase_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/AligInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/AlignmentContainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/AlignmentContainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16515 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/AlignmentExtractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/AlignmentExtractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BaseCountPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BaseIncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BaseIncrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BasePhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BasePhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BasePhrasePairFilter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BasePhraseTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BpSet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BpSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/BpSetInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/CategPhrasePairFilter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/CategPhrasePairFilter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/CellAlignment.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/CellID.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/HatTriePhraseTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/HatTriePhraseTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/IncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/IncrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseExtractParameters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseExtractUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseExtractUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseExtractionCell.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35713 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseExtractionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseExtractionTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseId.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhrasePair.h
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhrasePairInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseSortCriterion.h
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/PhraseTransTableNodeData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SegLenTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SegLenTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SentSegmentation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrcSegmLenTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrcSegmLenTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrfBisegm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrfNodeInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrfNodeInfoMap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrfNodeInfoMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrfNodeKey.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/SrfNodeKey.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/StlPhraseTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/StlPhraseTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/StrictCategPhrasePairFilter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/StrictCategPhrasePairFilter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/TrgCutsTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/TrgCutsTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/TrgSegmLenTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/TrgSegmLenTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/VecUnsignedIntSortCriterion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/WbaIncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/WbaIncrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16505 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/_incrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/_incrPhraseModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/_wbaIncrPhraseModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/phrase_models/_wbaIncrPhraseModel.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.583701 sil_thot-3.4.4/src/python_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/python_module/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    44637 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/python_module/module.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.583701 sil_thot-3.4.4/src/shared_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/shared_library/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    37191 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/shared_library/thot.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/shared_library/thot.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.599701 sil_thot-3.4.4/src/stack_dec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseAssistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseHypState.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseHypState.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseHypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseHypothesisRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseLogLinWeightUpdater.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseMiraScorer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10597 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BasePbTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BasePbTransModelFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BasePbTransModelStats.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BasePhraseHypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BasePhraseHypothesisRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseScorer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseSmtModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseSmtMultiStack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseSmtStack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseStackDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/BaseTranslationMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/DictFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/DictFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/DirectPhraseModelFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/DirectPhraseModelFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/FeaturesInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/HypSortCriterion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/HypStateDict.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/HypStateDictData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/InversePhraseModelFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/InversePhraseModelFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/KbMiraLlWu.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/KbMiraLlWu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/LM_State.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/LangModelFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/LangModelFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/LangModelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/LangModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraBleu.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraBleu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraChrF.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraChrF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7882 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraGtm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraGtm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraWer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/MiraWer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/NbestTransCacheData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/OnTheFlyDictFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/OnTheFlyDictFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/OnlineTrainingPars.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PbTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PbTransModelInputVars.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PbTransModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypDataStr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypEqClassF.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypEqClassF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumps01EqClassF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumpsEqClassF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypState.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrHypState.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48659 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrLocalSwLiTm.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrLocalSwLiTm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrLocalSwLiTmHypRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTablePref.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTablePrefKey.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTablePrefKey.h
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTableRef.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTableRefKey.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrNbestTransTableRefKey.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrScoreInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrScoreInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhraseBasedTmHyp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhraseBasedTmHypRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhraseCacheTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhraseModelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhraseModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/PhrasePairCacheTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/ScoreCompDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SmtModelUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SmtModelUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SmtMultiStackRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SmtStack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SourceSegmentation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SrcPhraseLenFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SrcPhraseLenFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SrcPosJumpFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SrcPosJumpFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SwModelInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/SwModelPars.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17974 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/TranslationMetadata.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/TrgPhraseLenFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/TrgPhraseLenFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10269 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/WeightUpdateUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/WeightUpdateUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/WgUncoupledAssistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/WordPenaltyFeat.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/WordPenaltyFeat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_assistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_nbUncoupledAssistedTrans.h
+-rw-r--r--   0 runner    (1001) docker     (127)   105202 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_pbTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21148 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_phrSwTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    99378 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_phraseBasedTransModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_phraseHypothesis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_phraseHypothesisRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_smtModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_smtMultiStack.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_smtStack.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37194 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_stackDecoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_stackDecoderRec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/_stack_decoder_statistics.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/bleu.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/bleu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/chrf.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/chrf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/stack_dec/multi_stack_decoder_rec.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.611701 sil_thot-3.4.4/src/sw_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Aligner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/AlignmentInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/AlignmentModelBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/AlignmentModelBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/AlignmentTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/AlignmentTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/CachedHmmAligLgProb.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/CachedHmmAligLgProb.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/DiagonalAlignment.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/DistortionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/DistortionTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/DoubleMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/DoubleMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25734 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/FastAlignModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/FastAlignModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/FertilityTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/FertilityTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/HeadDistortionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/HeadDistortionTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)    38778 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/HmmAlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/HmmAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/HmmAlignmentTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/HmmAlignmentTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17187 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm1AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm1AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11461 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm2AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm2AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35398 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm3AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm3AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18602 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm4AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Ibm4AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21402 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentTrainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentTrainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentTrainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentTrainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentTrainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentTrainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/LexCounts.h
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/LexTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/LightSentenceHandler.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/LightSentenceHandler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/Md.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/MemoryLexTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/MemoryLexTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/NonheadDistortionTable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/NonheadDistortionTable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7538 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/NormalSentenceLengthModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/NormalSentenceLengthModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SentenceHandler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SentenceLengthModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SentenceLengthModelBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SentenceLengthModelBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/StepwiseAlignmentModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SwDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SymmetrizedAligner.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/SymmetrizedAligner.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13117 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/anjiMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/anjiMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/anjm1ip_anjiMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-24 23:56:45.000000 sil_thot-3.4.4/src/sw_models/anjm1ip_anjiMatrix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.611701 sil_thot-3.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.611701 sil_thot-3.4.4/tests/nlp_common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/nlp_common/WordAlignmentMatrixTest.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.611701 sil_thot-3.4.4/tests/phrase_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/phrase_models/HatTriePhraseTableTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/phrase_models/StlPhraseTableTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18181 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/phrase_models/_phraseTableTest.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/tests/stack_dec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/stack_dec/KbMiraLlWuTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/stack_dec/MiraChrFTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/stack_dec/PhrLocalSwLiTmTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/stack_dec/TranslationMetadataTest.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/tests/sw_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/FastAlignModelTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/Ibm4AlignmentModelTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/IncrHmmAlignmentModelTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/LexTableTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/MemoryLexTableTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/TestUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/sw_models/TestUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-24 23:56:45.000000 sil_thot-3.4.4/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/thot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/thot/alignment/
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-24 23:56:45.000000 sil_thot-3.4.4/thot/alignment/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/thot/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-24 23:56:45.000000 sil_thot-3.4.4/thot/common/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:45.000000 sil_thot-3.4.4/thot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:56:50.615701 sil_thot-3.4.4/thot/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-05-24 23:56:45.000000 sil_thot-3.4.4/thot/translation/__init__.pyi
```

### Comparing `sil-thot-3.4.3/CMakeLists.txt` & `sil_thot-3.4.4/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     cmake_policy(SET CMP0135 OLD)
 endif()
 if(POLICY CMP0127)
     set(CMAKE_POLICY_DEFAULT_CMP0127 OLD)
 endif()
 set(CMAKE_POLICY_DEFAULT_CMP0077 NEW)
 # set(CMAKE_MSVC_RUNTIME_LIBRARY "MultiThreaded$<$<CONFIG:Debug>:Debug>")
-project(Thot VERSION 3.4.3 LANGUAGES CXX C)
+project(Thot VERSION 3.4.4 LANGUAGES CXX C)
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
 
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 
@@ -63,16 +63,16 @@
 option(BUILD_TESTS "Build unit tests" ON)
 
 if(WIN32)
     add_compile_options(/D_ITERATOR_DEBUG_LEVEL=0)
 endif()
 
 if(APPLE)
-    add_compile_options(-mmacosx-version-min=10.13 -Werror=partial-availability)
-    add_link_options(-mmacosx-version-min=10.13 -Wl,-no_weak_imports)
+    add_compile_options(-mmacosx-version-min=10.9 -Werror=partial-availability)
+    add_link_options(-mmacosx-version-min=10.9 -Wl,-no_weak_imports)
 endif()
 
 if(CMAKE_COMPILER_IS_GNUCC AND CMAKE_CXX_COMPILER_VERSION VERSION_LESS 9.5)
     set(CMAKE_INTERPROCEDURAL_OPTIMIZATION FALSE)
 endif()
 
 include(FetchContent)
```

### Comparing `sil-thot-3.4.3/COPYING.LESSER` & `sil_thot-3.4.4/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/PKG-INFO` & `sil_thot-3.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sil-thot
-Version: 3.4.3
+Version: 3.4.4
 Summary: A toolkit for statistical word alignment and machine translation
 Home-page: https://github.com/sillsdev/thot
 Author: SIL International
 Maintainer: Damien Daspit
 Maintainer-email: damien_daspit@sil.org
 License: LGPL-3.0
 Project-URL: Repository, https://github.com/sillsdev/thot
```

### Comparing `sil-thot-3.4.3/cmake/FindGMP.cmake` & `sil_thot-3.4.4/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/LICENSE` & `sil_thot-3.4.4/include/hat_trie/LICENSE`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/array_growth_policy.h` & `sil_thot-3.4.4/include/hat_trie/array_growth_policy.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/array_hash.h` & `sil_thot-3.4.4/include/hat_trie/array_hash.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/array_map.h` & `sil_thot-3.4.4/include/hat_trie/array_map.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/array_set.h` & `sil_thot-3.4.4/include/hat_trie/array_set.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/htrie_hash.h` & `sil_thot-3.4.4/include/hat_trie/htrie_hash.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/htrie_map.h` & `sil_thot-3.4.4/include/hat_trie/htrie_map.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/include/hat_trie/htrie_set.h` & `sil_thot-3.4.4/include/hat_trie/htrie_set.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/setup.py` & `sil_thot-3.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="sil-thot",
-    version="3.4.3",
+    version="3.4.4",
     author="SIL International",
     maintainer="Damien Daspit",
     maintainer_email="damien_daspit@sil.org",
     description="A toolkit for statistical word alignment and machine translation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="LGPL-3.0",
```

### Comparing `sil-thot-3.4.3/sil_thot.egg-info/PKG-INFO` & `sil_thot-3.4.4/sil_thot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sil-thot
-Version: 3.4.3
+Version: 3.4.4
 Summary: A toolkit for statistical word alignment and machine translation
 Home-page: https://github.com/sillsdev/thot
 Author: SIL International
 Maintainer: Damien Daspit
 Maintainer-email: damien_daspit@sil.org
 License: LGPL-3.0
 Project-URL: Repository, https://github.com/sillsdev/thot
```

### Comparing `sil-thot-3.4.3/sil_thot.egg-info/SOURCES.txt` & `sil_thot-3.4.4/sil_thot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/CMakeLists.txt` & `sil_thot-3.4.4/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/downhill_simplex/step_by_step_dhs.c` & `sil_thot-3.4.4/src/downhill_simplex/step_by_step_dhs.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/downhill_simplex/step_by_step_dhs.h` & `sil_thot-3.4.4/src/downhill_simplex/step_by_step_dhs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/BaseEcModelForNbUcat.h` & `sil_thot-3.4.4/src/error_correction/BaseEcModelForNbUcat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/BaseEcmForWg.h` & `sil_thot-3.4.4/src/error_correction/BaseEcmForWg.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/BaseEditDist.h` & `sil_thot-3.4.4/src/error_correction/BaseEditDist.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/BaseErrorCorrectionModel.cc` & `sil_thot-3.4.4/src/error_correction/BaseErrorCorrectionModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/BaseErrorCorrectionModel.h` & `sil_thot-3.4.4/src/error_correction/BaseErrorCorrectionModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/BaseWgProcessorForAnlp.h` & `sil_thot-3.4.4/src/error_correction/BaseWgProcessorForAnlp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/EditDistForStr.cc` & `sil_thot-3.4.4/src/error_correction/EditDistForStr.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/EditDistForStr.h` & `sil_thot-3.4.4/src/error_correction/EditDistForStr.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/EditDistForVec.h` & `sil_thot-3.4.4/src/error_correction/EditDistForVec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/EditDistForVecString.cc` & `sil_thot-3.4.4/src/error_correction/EditDistForVecString.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/EditDistForVecString.h` & `sil_thot-3.4.4/src/error_correction/EditDistForVecString.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/HypStateIndex.h` & `sil_thot-3.4.4/src/error_correction/HypStateIndex.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NbSearchHighLevelHyp.h` & `sil_thot-3.4.4/src/error_correction/NbSearchHighLevelHyp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NbSearchHyp.h` & `sil_thot-3.4.4/src/error_correction/NbSearchHyp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NbSearchStack.cc` & `sil_thot-3.4.4/src/error_correction/NbSearchStack.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NbSearchStack.h` & `sil_thot-3.4.4/src/error_correction/NbSearchStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NbestCorrections.h` & `sil_thot-3.4.4/src/error_correction/NbestCorrections.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NonPbEcModelForNbUcat.cc` & `sil_thot-3.4.4/src/error_correction/NonPbEcModelForNbUcat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/NonPbEcModelForNbUcat.h` & `sil_thot-3.4.4/src/error_correction/NonPbEcModelForNbUcat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/PfsmEcm.cc` & `sil_thot-3.4.4/src/error_correction/PfsmEcm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/PfsmEcm.h` & `sil_thot-3.4.4/src/error_correction/PfsmEcm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/PfsmEcmForWg.cc` & `sil_thot-3.4.4/src/error_correction/PfsmEcmForWg.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/PfsmEcmForWg.h` & `sil_thot-3.4.4/src/error_correction/PfsmEcmForWg.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/PfsmEcmForWgEsi.h` & `sil_thot-3.4.4/src/error_correction/PfsmEcmForWgEsi.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/PrefAlignInfo.h` & `sil_thot-3.4.4/src/error_correction/PrefAlignInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/RejectedWordsSet.h` & `sil_thot-3.4.4/src/error_correction/RejectedWordsSet.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WgHandler.cc` & `sil_thot-3.4.4/src/error_correction/WgHandler.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WgHandler.h` & `sil_thot-3.4.4/src/error_correction/WgHandler.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WgProcessorForAnlp.h` & `sil_thot-3.4.4/src/error_correction/WgProcessorForAnlp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WordAndCharLevelOps.h` & `sil_thot-3.4.4/src/error_correction/WordAndCharLevelOps.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WordGraph.cc` & `sil_thot-3.4.4/src/error_correction/WordGraph.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WordGraph.h` & `sil_thot-3.4.4/src/error_correction/WordGraph.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WordGraphArc.h` & `sil_thot-3.4.4/src/error_correction/WordGraphArc.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WordGraphArcId.h` & `sil_thot-3.4.4/src/error_correction/WordGraphArcId.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/WordGraphStateData.h` & `sil_thot-3.4.4/src/error_correction/WordGraphStateData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/_editDist.h` & `sil_thot-3.4.4/src/error_correction/_editDist.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/_editDistBasedEcm.cc` & `sil_thot-3.4.4/src/error_correction/_editDistBasedEcm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/error_correction/_editDistBasedEcm.h` & `sil_thot-3.4.4/src/error_correction/_editDistBasedEcm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/BaseIncrCondProbModel.h` & `sil_thot-3.4.4/src/incr_models/BaseIncrCondProbModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/BaseIncrCondProbTable.h` & `sil_thot-3.4.4/src/incr_models/BaseIncrCondProbTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/BaseIncrEncCondProbModel.h` & `sil_thot-3.4.4/src/incr_models/BaseIncrEncCondProbModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/BaseIncrEncoder.h` & `sil_thot-3.4.4/src/incr_models/BaseIncrEncoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/BaseWordPenaltyModel.h` & `sil_thot-3.4.4/src/incr_models/BaseWordPenaltyModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/IncrCondProbTable.h` & `sil_thot-3.4.4/src/incr_models/IncrCondProbTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/IncrEncoder.h` & `sil_thot-3.4.4/src/incr_models/IncrEncoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/IncrJelMerNgramLM.cc` & `sil_thot-3.4.4/src/incr_models/IncrJelMerNgramLM.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/IncrJelMerNgramLM.h` & `sil_thot-3.4.4/src/incr_models/IncrJelMerNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/IncrNgramLM.cc` & `sil_thot-3.4.4/src/incr_models/IncrNgramLM.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/IncrNgramLM.h` & `sil_thot-3.4.4/src/incr_models/IncrNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/WordPenaltyModel.cc` & `sil_thot-3.4.4/src/incr_models/WordPenaltyModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/WordPenaltyModel.h` & `sil_thot-3.4.4/src/incr_models/WordPenaltyModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/WordPredictor.cc` & `sil_thot-3.4.4/src/incr_models/WordPredictor.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/WordPredictor.h` & `sil_thot-3.4.4/src/incr_models/WordPredictor.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/_incrEncCondProbModel.h` & `sil_thot-3.4.4/src/incr_models/_incrEncCondProbModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/_incrJelMerNgramLM.h` & `sil_thot-3.4.4/src/incr_models/_incrJelMerNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/_incrNgramLM.h` & `sil_thot-3.4.4/src/incr_models/_incrNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/im_pair.h` & `sil_thot-3.4.4/src/incr_models/im_pair.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/lm_ienc.cc` & `sil_thot-3.4.4/src/incr_models/lm_ienc.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/lm_ienc.h` & `sil_thot-3.4.4/src/incr_models/lm_ienc.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/vecx_x_incr_cptable.h` & `sil_thot-3.4.4/src/incr_models/vecx_x_incr_cptable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/vecx_x_incr_ecpm.h` & `sil_thot-3.4.4/src/incr_models/vecx_x_incr_ecpm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/incr_models/vecx_x_incr_enc.h` & `sil_thot-3.4.4/src/incr_models/vecx_x_incr_enc.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/AwkInputStream.cc` & `sil_thot-3.4.4/src/nlp_common/AwkInputStream.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/AwkInputStream.h` & `sil_thot-3.4.4/src/nlp_common/AwkInputStream.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/BaseIncrNgramLM.h` & `sil_thot-3.4.4/src/nlp_common/BaseIncrNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/BaseNgramLM.h` & `sil_thot-3.4.4/src/nlp_common/BaseNgramLM.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/BidTrie.h` & `sil_thot-3.4.4/src/nlp_common/BidTrie.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Bitset.h` & `sil_thot-3.4.4/src/nlp_common/Bitset.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Count.h` & `sil_thot-3.4.4/src/nlp_common/Count.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/ErrorDefs.h` & `sil_thot-3.4.4/src/nlp_common/ErrorDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/LM_Defs.h` & `sil_thot-3.4.4/src/nlp_common/LM_Defs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/LogCount.h` & `sil_thot-3.4.4/src/nlp_common/LogCount.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/MathDefs.h` & `sil_thot-3.4.4/src/nlp_common/MathDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/MathFuncs.cc` & `sil_thot-3.4.4/src/nlp_common/MathFuncs.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/MathFuncs.h` & `sil_thot-3.4.4/src/nlp_common/MathFuncs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Matrix.h` & `sil_thot-3.4.4/src/nlp_common/Matrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/NbestTableNode.h` & `sil_thot-3.4.4/src/nlp_common/NbestTableNode.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/NbestTransTable.h` & `sil_thot-3.4.4/src/nlp_common/NbestTransTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/OrderedVector.h` & `sil_thot-3.4.4/src/nlp_common/OrderedVector.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/PositionIndex.h` & `sil_thot-3.4.4/src/nlp_common/PositionIndex.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Prob.cc` & `sil_thot-3.4.4/src/nlp_common/Prob.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Prob.h` & `sil_thot-3.4.4/src/nlp_common/Prob.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Score.h` & `sil_thot-3.4.4/src/nlp_common/Score.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/SingleWordVocab.cc` & `sil_thot-3.4.4/src/nlp_common/SingleWordVocab.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/SingleWordVocab.h` & `sil_thot-3.4.4/src/nlp_common/SingleWordVocab.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/SmtDefs.h` & `sil_thot-3.4.4/src/nlp_common/SmtDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/StrProcUtils.cc` & `sil_thot-3.4.4/src/nlp_common/StrProcUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/StrProcUtils.h` & `sil_thot-3.4.4/src/nlp_common/StrProcUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/TranslationData.h` & `sil_thot-3.4.4/src/nlp_common/TranslationData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/Trie.h` & `sil_thot-3.4.4/src/nlp_common/Trie.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/TrieVecs.h` & `sil_thot-3.4.4/src/nlp_common/TrieVecs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/WordAlignmentMatrix.cc` & `sil_thot-3.4.4/src/nlp_common/WordAlignmentMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/WordAlignmentMatrix.h` & `sil_thot-3.4.4/src/nlp_common/WordAlignmentMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/WordClasses.cc` & `sil_thot-3.4.4/src/nlp_common/WordClasses.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/WordClasses.h` & `sil_thot-3.4.4/src/nlp_common/WordClasses.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/WordIndex.h` & `sil_thot-3.4.4/src/nlp_common/WordIndex.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/ctimer.c` & `sil_thot-3.4.4/src/nlp_common/ctimer.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/ctimer.h` & `sil_thot-3.4.4/src/nlp_common/ctimer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/getdelim.c` & `sil_thot-3.4.4/src/nlp_common/getdelim.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/getdelim.h` & `sil_thot-3.4.4/src/nlp_common/getdelim.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/getline.c` & `sil_thot-3.4.4/src/nlp_common/getline.c`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/getline.h` & `sil_thot-3.4.4/src/nlp_common/getline.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/ins_op_pair.h` & `sil_thot-3.4.4/src/nlp_common/ins_op_pair.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/lt_op_vec.h` & `sil_thot-3.4.4/src/nlp_common/lt_op_vec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/printAligFuncs.cc` & `sil_thot-3.4.4/src/nlp_common/printAligFuncs.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/printAligFuncs.h` & `sil_thot-3.4.4/src/nlp_common/printAligFuncs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/uiHashF.h` & `sil_thot-3.4.4/src/nlp_common/uiHashF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/nlp_common/uiPairHashF.h` & `sil_thot-3.4.4/src/nlp_common/uiPairHashF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/AlignmentContainer.cc` & `sil_thot-3.4.4/src/phrase_models/AlignmentContainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/AlignmentContainer.h` & `sil_thot-3.4.4/src/phrase_models/AlignmentContainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/AlignmentExtractor.cc` & `sil_thot-3.4.4/src/phrase_models/AlignmentExtractor.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/AlignmentExtractor.h` & `sil_thot-3.4.4/src/phrase_models/AlignmentExtractor.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BaseCountPhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/BaseCountPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BaseIncrPhraseModel.cc` & `sil_thot-3.4.4/src/phrase_models/BaseIncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BaseIncrPhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/BaseIncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BasePhraseModel.cc` & `sil_thot-3.4.4/src/phrase_models/BasePhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BasePhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/BasePhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BasePhrasePairFilter.h` & `sil_thot-3.4.4/src/phrase_models/BasePhrasePairFilter.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BasePhraseTable.h` & `sil_thot-3.4.4/src/phrase_models/BasePhraseTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BpSet.cc` & `sil_thot-3.4.4/src/phrase_models/BpSet.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BpSet.h` & `sil_thot-3.4.4/src/phrase_models/BpSet.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/BpSetInfo.h` & `sil_thot-3.4.4/src/phrase_models/BpSetInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/CategPhrasePairFilter.cc` & `sil_thot-3.4.4/src/phrase_models/CategPhrasePairFilter.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/CategPhrasePairFilter.h` & `sil_thot-3.4.4/src/phrase_models/CategPhrasePairFilter.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/CellAlignment.h` & `sil_thot-3.4.4/src/phrase_models/CellAlignment.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/CellID.h` & `sil_thot-3.4.4/src/phrase_models/CellID.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/HatTriePhraseTable.cc` & `sil_thot-3.4.4/src/phrase_models/HatTriePhraseTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/HatTriePhraseTable.h` & `sil_thot-3.4.4/src/phrase_models/HatTriePhraseTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/IncrPhraseModel.cc` & `sil_thot-3.4.4/src/phrase_models/IncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/IncrPhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/IncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseDefs.h` & `sil_thot-3.4.4/src/phrase_models/PhraseDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseExtractParameters.h` & `sil_thot-3.4.4/src/phrase_models/PhraseExtractParameters.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseExtractUtils.cc` & `sil_thot-3.4.4/src/phrase_models/PhraseExtractUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseExtractUtils.h` & `sil_thot-3.4.4/src/phrase_models/PhraseExtractUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseExtractionCell.h` & `sil_thot-3.4.4/src/phrase_models/PhraseExtractionCell.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseExtractionTable.cc` & `sil_thot-3.4.4/src/phrase_models/PhraseExtractionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseExtractionTable.h` & `sil_thot-3.4.4/src/phrase_models/PhraseExtractionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseId.h` & `sil_thot-3.4.4/src/phrase_models/PhraseId.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhrasePair.h` & `sil_thot-3.4.4/src/phrase_models/PhrasePair.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhrasePairInfo.h` & `sil_thot-3.4.4/src/phrase_models/PhrasePairInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseSortCriterion.h` & `sil_thot-3.4.4/src/phrase_models/PhraseSortCriterion.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/PhraseTransTableNodeData.h` & `sil_thot-3.4.4/src/phrase_models/PhraseTransTableNodeData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SegLenTable.cc` & `sil_thot-3.4.4/src/phrase_models/SegLenTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SegLenTable.h` & `sil_thot-3.4.4/src/phrase_models/SegLenTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SentSegmentation.h` & `sil_thot-3.4.4/src/phrase_models/SentSegmentation.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrcSegmLenTable.cc` & `sil_thot-3.4.4/src/phrase_models/SrcSegmLenTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrcSegmLenTable.h` & `sil_thot-3.4.4/src/phrase_models/SrcSegmLenTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrfBisegm.h` & `sil_thot-3.4.4/src/phrase_models/SrfBisegm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrfNodeInfo.h` & `sil_thot-3.4.4/src/phrase_models/SrfNodeInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrfNodeInfoMap.cc` & `sil_thot-3.4.4/src/phrase_models/SrfNodeInfoMap.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrfNodeInfoMap.h` & `sil_thot-3.4.4/src/phrase_models/SrfNodeInfoMap.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrfNodeKey.cc` & `sil_thot-3.4.4/src/phrase_models/SrfNodeKey.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/SrfNodeKey.h` & `sil_thot-3.4.4/src/phrase_models/SrfNodeKey.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/StlPhraseTable.cc` & `sil_thot-3.4.4/src/phrase_models/StlPhraseTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/StlPhraseTable.h` & `sil_thot-3.4.4/src/phrase_models/StlPhraseTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/StrictCategPhrasePairFilter.cc` & `sil_thot-3.4.4/src/phrase_models/StrictCategPhrasePairFilter.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/StrictCategPhrasePairFilter.h` & `sil_thot-3.4.4/src/phrase_models/StrictCategPhrasePairFilter.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/TrgCutsTable.cc` & `sil_thot-3.4.4/src/phrase_models/TrgCutsTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/TrgCutsTable.h` & `sil_thot-3.4.4/src/phrase_models/TrgCutsTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/TrgSegmLenTable.cc` & `sil_thot-3.4.4/src/phrase_models/TrgSegmLenTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/TrgSegmLenTable.h` & `sil_thot-3.4.4/src/phrase_models/TrgSegmLenTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/VecUnsignedIntSortCriterion.h` & `sil_thot-3.4.4/src/phrase_models/VecUnsignedIntSortCriterion.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/WbaIncrPhraseModel.cc` & `sil_thot-3.4.4/src/phrase_models/WbaIncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/WbaIncrPhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/WbaIncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/_incrPhraseModel.cc` & `sil_thot-3.4.4/src/phrase_models/_incrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/_incrPhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/_incrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/_wbaIncrPhraseModel.cc` & `sil_thot-3.4.4/src/phrase_models/_wbaIncrPhraseModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/phrase_models/_wbaIncrPhraseModel.h` & `sil_thot-3.4.4/src/phrase_models/_wbaIncrPhraseModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/python_module/CMakeLists.txt` & `sil_thot-3.4.4/src/python_module/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/python_module/module.cc` & `sil_thot-3.4.4/src/python_module/module.cc`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 #include "sw_models/SymmetrizedAligner.h"
 
 #include <memory>
 #include <pybind11/numpy.h>
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 
-#define NUM_TRANSLATE_THREADS 3
-
 namespace py = pybind11;
 
 std::vector<WordIndex> getSrcWordIndices(Aligner& aligner, const char* srcSentence)
 {
   std::vector<WordIndex> wordIndices;
   size_t i = 0;
   std::string s;
@@ -755,15 +753,15 @@
             return translate(decoder, sentence);
           },
           py::arg("sentence"))
       .def(
           "translate_batch",
           [](multi_stack_decoder_rec<PhrLocalSwLiTm>& decoder, const std::vector<std::string>& sentences) {
             std::vector<TranslationData> results(sentences.size());
-#pragma omp parallel num_threads(NUM_TRANSLATE_THREADS)
+#pragma omp parallel
             {
               multi_stack_decoder_rec<PhrLocalSwLiTm> threadDecoder;
               threadDecoder.setParentSmtModel(decoder.getParentSmtModel());
               auto smtModel = dynamic_cast<PhrLocalSwLiTm*>(decoder.getParentSmtModel()->clone());
               smtModel->setTranslationMetadata(new TranslationMetadata<PhrScoreInfo>);
               threadDecoder.setSmtModel(smtModel);
               threadDecoder.useBestScorePruning(true);
@@ -786,15 +784,15 @@
             return translateN(decoder, sentence, n);
           },
           py::arg("sentence"), py::arg("n"))
       .def(
           "translate_n_batch",
           [](multi_stack_decoder_rec<PhrLocalSwLiTm>& decoder, const std::vector<std::string>& sentences, int n) {
             std::vector<std::vector<TranslationData>> results(sentences.size());
-#pragma omp parallel num_threads(NUM_TRANSLATE_THREADS)
+#pragma omp parallel
             {
               multi_stack_decoder_rec<PhrLocalSwLiTm> threadDecoder;
               threadDecoder.setParentSmtModel(decoder.getParentSmtModel());
               auto smtModel = dynamic_cast<PhrLocalSwLiTm*>(decoder.getParentSmtModel()->clone());
               smtModel->setTranslationMetadata(new TranslationMetadata<PhrScoreInfo>);
               threadDecoder.setSmtModel(smtModel);
               threadDecoder.useBestScorePruning(true);
```

### Comparing `sil-thot-3.4.3/src/shared_library/thot.cc` & `sil_thot-3.4.4/src/shared_library/thot.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/shared_library/thot.h` & `sil_thot-3.4.4/src/shared_library/thot.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseAssistedTrans.h` & `sil_thot-3.4.4/src/stack_dec/BaseAssistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseHypState.cc` & `sil_thot-3.4.4/src/stack_dec/BaseHypState.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseHypState.h` & `sil_thot-3.4.4/src/stack_dec/BaseHypState.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseHypothesis.h` & `sil_thot-3.4.4/src/stack_dec/BaseHypothesis.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseHypothesisRec.h` & `sil_thot-3.4.4/src/stack_dec/BaseHypothesisRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseLogLinWeightUpdater.h` & `sil_thot-3.4.4/src/stack_dec/BaseLogLinWeightUpdater.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseMiraScorer.h` & `sil_thot-3.4.4/src/stack_dec/BaseMiraScorer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BasePbTransModel.h` & `sil_thot-3.4.4/src/stack_dec/BasePbTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BasePbTransModelFeature.h` & `sil_thot-3.4.4/src/stack_dec/BasePbTransModelFeature.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BasePbTransModelStats.h` & `sil_thot-3.4.4/src/stack_dec/BasePbTransModelStats.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BasePhraseHypothesis.h` & `sil_thot-3.4.4/src/stack_dec/BasePhraseHypothesis.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BasePhraseHypothesisRec.h` & `sil_thot-3.4.4/src/stack_dec/BasePhraseHypothesisRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseScorer.h` & `sil_thot-3.4.4/src/stack_dec/BaseScorer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseSmtModel.h` & `sil_thot-3.4.4/src/stack_dec/BaseSmtModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseSmtMultiStack.h` & `sil_thot-3.4.4/src/stack_dec/BaseSmtMultiStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseSmtStack.h` & `sil_thot-3.4.4/src/stack_dec/BaseSmtStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseStackDecoder.h` & `sil_thot-3.4.4/src/stack_dec/BaseStackDecoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/BaseTranslationMetadata.h` & `sil_thot-3.4.4/src/stack_dec/BaseTranslationMetadata.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/DictFeat.cc` & `sil_thot-3.4.4/src/stack_dec/DictFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/DictFeat.h` & `sil_thot-3.4.4/src/stack_dec/DictFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/DirectPhraseModelFeat.cc` & `sil_thot-3.4.4/src/stack_dec/DirectPhraseModelFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/DirectPhraseModelFeat.h` & `sil_thot-3.4.4/src/stack_dec/DirectPhraseModelFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/FeaturesInfo.h` & `sil_thot-3.4.4/src/stack_dec/FeaturesInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/HypSortCriterion.h` & `sil_thot-3.4.4/src/stack_dec/HypSortCriterion.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/HypStateDict.h` & `sil_thot-3.4.4/src/stack_dec/HypStateDict.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/HypStateDictData.h` & `sil_thot-3.4.4/src/stack_dec/HypStateDictData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/InversePhraseModelFeat.cc` & `sil_thot-3.4.4/src/stack_dec/InversePhraseModelFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/InversePhraseModelFeat.h` & `sil_thot-3.4.4/src/stack_dec/InversePhraseModelFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/KbMiraLlWu.cc` & `sil_thot-3.4.4/src/stack_dec/KbMiraLlWu.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/KbMiraLlWu.h` & `sil_thot-3.4.4/src/stack_dec/KbMiraLlWu.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/LM_State.h` & `sil_thot-3.4.4/src/stack_dec/LM_State.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/LangModelFeat.cc` & `sil_thot-3.4.4/src/stack_dec/LangModelFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/LangModelFeat.h` & `sil_thot-3.4.4/src/stack_dec/LangModelFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/LangModelInfo.h` & `sil_thot-3.4.4/src/stack_dec/LangModelInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/LangModelPars.h` & `sil_thot-3.4.4/src/stack_dec/LangModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraBleu.cc` & `sil_thot-3.4.4/src/stack_dec/MiraBleu.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraBleu.h` & `sil_thot-3.4.4/src/stack_dec/MiraBleu.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraChrF.cc` & `sil_thot-3.4.4/src/stack_dec/MiraChrF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraChrF.h` & `sil_thot-3.4.4/src/stack_dec/MiraChrF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraGtm.cc` & `sil_thot-3.4.4/src/stack_dec/MiraGtm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraGtm.h` & `sil_thot-3.4.4/src/stack_dec/MiraGtm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraWer.cc` & `sil_thot-3.4.4/src/stack_dec/MiraWer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/MiraWer.h` & `sil_thot-3.4.4/src/stack_dec/MiraWer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/NbestTransCacheData.h` & `sil_thot-3.4.4/src/stack_dec/NbestTransCacheData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/OnTheFlyDictFeat.cc` & `sil_thot-3.4.4/src/stack_dec/OnTheFlyDictFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/OnTheFlyDictFeat.h` & `sil_thot-3.4.4/src/stack_dec/OnTheFlyDictFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/OnlineTrainingPars.h` & `sil_thot-3.4.4/src/stack_dec/OnlineTrainingPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PbTransModel.h` & `sil_thot-3.4.4/src/stack_dec/PbTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PbTransModelInputVars.h` & `sil_thot-3.4.4/src/stack_dec/PbTransModelInputVars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PbTransModelPars.h` & `sil_thot-3.4.4/src/stack_dec/PbTransModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypData.h` & `sil_thot-3.4.4/src/stack_dec/PhrHypData.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypDataStr.h` & `sil_thot-3.4.4/src/stack_dec/PhrHypDataStr.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypEqClassF.cc` & `sil_thot-3.4.4/src/stack_dec/PhrHypEqClassF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypEqClassF.h` & `sil_thot-3.4.4/src/stack_dec/PhrHypEqClassF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc` & `sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumps01EqClassF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumps01EqClassF.h` & `sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumps01EqClassF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc` & `sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumpsEqClassF.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypNumcovJumpsEqClassF.h` & `sil_thot-3.4.4/src/stack_dec/PhrHypNumcovJumpsEqClassF.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypState.cc` & `sil_thot-3.4.4/src/stack_dec/PhrHypState.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrHypState.h` & `sil_thot-3.4.4/src/stack_dec/PhrHypState.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrLocalSwLiTm.cc` & `sil_thot-3.4.4/src/stack_dec/PhrLocalSwLiTm.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrLocalSwLiTm.h` & `sil_thot-3.4.4/src/stack_dec/PhrLocalSwLiTm.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrLocalSwLiTmHypRec.h` & `sil_thot-3.4.4/src/stack_dec/PhrLocalSwLiTmHypRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTable.h` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTablePref.h` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTablePref.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTablePrefKey.cc` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTablePrefKey.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTablePrefKey.h` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTablePrefKey.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTableRef.h` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTableRef.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTableRefKey.cc` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTableRefKey.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrNbestTransTableRefKey.h` & `sil_thot-3.4.4/src/stack_dec/PhrNbestTransTableRefKey.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrScoreInfo.cc` & `sil_thot-3.4.4/src/stack_dec/PhrScoreInfo.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrScoreInfo.h` & `sil_thot-3.4.4/src/stack_dec/PhrScoreInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhraseBasedTmHyp.h` & `sil_thot-3.4.4/src/stack_dec/PhraseBasedTmHyp.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhraseBasedTmHypRec.h` & `sil_thot-3.4.4/src/stack_dec/PhraseBasedTmHypRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhraseCacheTable.h` & `sil_thot-3.4.4/src/stack_dec/PhraseCacheTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhraseModelInfo.h` & `sil_thot-3.4.4/src/stack_dec/PhraseModelInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhraseModelPars.h` & `sil_thot-3.4.4/src/stack_dec/PhraseModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/PhrasePairCacheTable.h` & `sil_thot-3.4.4/src/stack_dec/PhrasePairCacheTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/ScoreCompDefs.h` & `sil_thot-3.4.4/src/stack_dec/ScoreCompDefs.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SmtModelUtils.cc` & `sil_thot-3.4.4/src/stack_dec/SmtModelUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SmtModelUtils.h` & `sil_thot-3.4.4/src/stack_dec/SmtModelUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SmtMultiStackRec.h` & `sil_thot-3.4.4/src/stack_dec/SmtMultiStackRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SmtStack.h` & `sil_thot-3.4.4/src/stack_dec/SmtStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SourceSegmentation.h` & `sil_thot-3.4.4/src/stack_dec/SourceSegmentation.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SrcPhraseLenFeat.cc` & `sil_thot-3.4.4/src/stack_dec/SrcPhraseLenFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SrcPhraseLenFeat.h` & `sil_thot-3.4.4/src/stack_dec/SrcPhraseLenFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SrcPosJumpFeat.cc` & `sil_thot-3.4.4/src/stack_dec/SrcPosJumpFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SrcPosJumpFeat.h` & `sil_thot-3.4.4/src/stack_dec/SrcPosJumpFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SwModelInfo.h` & `sil_thot-3.4.4/src/stack_dec/SwModelInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/SwModelPars.h` & `sil_thot-3.4.4/src/stack_dec/SwModelPars.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/TranslationMetadata.h` & `sil_thot-3.4.4/src/stack_dec/TranslationMetadata.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/TrgPhraseLenFeat.cc` & `sil_thot-3.4.4/src/stack_dec/TrgPhraseLenFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/TrgPhraseLenFeat.h` & `sil_thot-3.4.4/src/stack_dec/TrgPhraseLenFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/WeightUpdateUtils.cc` & `sil_thot-3.4.4/src/stack_dec/WeightUpdateUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/WeightUpdateUtils.h` & `sil_thot-3.4.4/src/stack_dec/WeightUpdateUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/WgUncoupledAssistedTrans.h` & `sil_thot-3.4.4/src/stack_dec/WgUncoupledAssistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/WordPenaltyFeat.cc` & `sil_thot-3.4.4/src/stack_dec/WordPenaltyFeat.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/WordPenaltyFeat.h` & `sil_thot-3.4.4/src/stack_dec/WordPenaltyFeat.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_assistedTrans.h` & `sil_thot-3.4.4/src/stack_dec/_assistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_nbUncoupledAssistedTrans.h` & `sil_thot-3.4.4/src/stack_dec/_nbUncoupledAssistedTrans.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_pbTransModel.h` & `sil_thot-3.4.4/src/stack_dec/_pbTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_phrSwTransModel.h` & `sil_thot-3.4.4/src/stack_dec/_phrSwTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_phraseBasedTransModel.h` & `sil_thot-3.4.4/src/stack_dec/_phraseBasedTransModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_phraseHypothesis.h` & `sil_thot-3.4.4/src/stack_dec/_phraseHypothesis.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_phraseHypothesisRec.h` & `sil_thot-3.4.4/src/stack_dec/_phraseHypothesisRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_smtModel.h` & `sil_thot-3.4.4/src/stack_dec/_smtModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_smtMultiStack.h` & `sil_thot-3.4.4/src/stack_dec/_smtMultiStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_smtStack.h` & `sil_thot-3.4.4/src/stack_dec/_smtStack.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_stackDecoder.h` & `sil_thot-3.4.4/src/stack_dec/_stackDecoder.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_stackDecoderRec.h` & `sil_thot-3.4.4/src/stack_dec/_stackDecoderRec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/_stack_decoder_statistics.h` & `sil_thot-3.4.4/src/stack_dec/_stack_decoder_statistics.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/bleu.cc` & `sil_thot-3.4.4/src/stack_dec/bleu.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/bleu.h` & `sil_thot-3.4.4/src/stack_dec/bleu.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/chrf.cc` & `sil_thot-3.4.4/src/stack_dec/chrf.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/chrf.h` & `sil_thot-3.4.4/src/stack_dec/chrf.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/stack_dec/multi_stack_decoder_rec.h` & `sil_thot-3.4.4/src/stack_dec/multi_stack_decoder_rec.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Aligner.h` & `sil_thot-3.4.4/src/sw_models/Aligner.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/AlignmentInfo.h` & `sil_thot-3.4.4/src/sw_models/AlignmentInfo.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/AlignmentModelBase.cc` & `sil_thot-3.4.4/src/sw_models/AlignmentModelBase.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/AlignmentModelBase.h` & `sil_thot-3.4.4/src/sw_models/AlignmentModelBase.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/AlignmentTable.cc` & `sil_thot-3.4.4/src/sw_models/AlignmentTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/AlignmentTable.h` & `sil_thot-3.4.4/src/sw_models/AlignmentTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/CachedHmmAligLgProb.cc` & `sil_thot-3.4.4/src/sw_models/CachedHmmAligLgProb.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/CachedHmmAligLgProb.h` & `sil_thot-3.4.4/src/sw_models/CachedHmmAligLgProb.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/DiagonalAlignment.h` & `sil_thot-3.4.4/src/sw_models/DiagonalAlignment.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/DistortionTable.cc` & `sil_thot-3.4.4/src/sw_models/DistortionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/DistortionTable.h` & `sil_thot-3.4.4/src/sw_models/DistortionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/DoubleMatrix.cc` & `sil_thot-3.4.4/src/sw_models/DoubleMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/DoubleMatrix.h` & `sil_thot-3.4.4/src/sw_models/DoubleMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/FastAlignModel.cc` & `sil_thot-3.4.4/src/sw_models/FastAlignModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/FastAlignModel.h` & `sil_thot-3.4.4/src/sw_models/FastAlignModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/FertilityTable.cc` & `sil_thot-3.4.4/src/sw_models/FertilityTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/FertilityTable.h` & `sil_thot-3.4.4/src/sw_models/FertilityTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/HeadDistortionTable.cc` & `sil_thot-3.4.4/src/sw_models/HeadDistortionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/HeadDistortionTable.h` & `sil_thot-3.4.4/src/sw_models/HeadDistortionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/HmmAlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/HmmAlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/HmmAlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/HmmAlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/HmmAlignmentTable.cc` & `sil_thot-3.4.4/src/sw_models/HmmAlignmentTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/HmmAlignmentTable.h` & `sil_thot-3.4.4/src/sw_models/HmmAlignmentTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm1AlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/Ibm1AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm1AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/Ibm1AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm2AlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/Ibm2AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm2AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/Ibm2AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm3AlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/Ibm3AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm3AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/Ibm3AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm4AlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/Ibm4AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Ibm4AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/Ibm4AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrAlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/IncrAlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentTrainer.cc` & `sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentTrainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrHmmAlignmentTrainer.h` & `sil_thot-3.4.4/src/sw_models/IncrHmmAlignmentTrainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentTrainer.cc` & `sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentTrainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm1AlignmentTrainer.h` & `sil_thot-3.4.4/src/sw_models/IncrIbm1AlignmentTrainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentModel.cc` & `sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentModel.h` & `sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentTrainer.cc` & `sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentTrainer.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/IncrIbm2AlignmentTrainer.h` & `sil_thot-3.4.4/src/sw_models/IncrIbm2AlignmentTrainer.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/LexCounts.h` & `sil_thot-3.4.4/src/sw_models/LexCounts.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/LexTable.h` & `sil_thot-3.4.4/src/sw_models/LexTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/LightSentenceHandler.cc` & `sil_thot-3.4.4/src/sw_models/LightSentenceHandler.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/LightSentenceHandler.h` & `sil_thot-3.4.4/src/sw_models/LightSentenceHandler.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/Md.h` & `sil_thot-3.4.4/src/sw_models/Md.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/MemoryLexTable.cc` & `sil_thot-3.4.4/src/sw_models/MemoryLexTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/MemoryLexTable.h` & `sil_thot-3.4.4/src/sw_models/MemoryLexTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/NonheadDistortionTable.cc` & `sil_thot-3.4.4/src/sw_models/NonheadDistortionTable.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/NonheadDistortionTable.h` & `sil_thot-3.4.4/src/sw_models/NonheadDistortionTable.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/NormalSentenceLengthModel.cc` & `sil_thot-3.4.4/src/sw_models/NormalSentenceLengthModel.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/NormalSentenceLengthModel.h` & `sil_thot-3.4.4/src/sw_models/NormalSentenceLengthModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/SentenceHandler.h` & `sil_thot-3.4.4/src/sw_models/SentenceHandler.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/SentenceLengthModel.h` & `sil_thot-3.4.4/src/sw_models/SentenceLengthModel.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/SentenceLengthModelBase.cc` & `sil_thot-3.4.4/src/sw_models/SentenceLengthModelBase.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/SentenceLengthModelBase.h` & `sil_thot-3.4.4/src/sw_models/SentenceLengthModelBase.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/SymmetrizedAligner.cc` & `sil_thot-3.4.4/src/sw_models/SymmetrizedAligner.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/SymmetrizedAligner.h` & `sil_thot-3.4.4/src/sw_models/SymmetrizedAligner.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/anjiMatrix.cc` & `sil_thot-3.4.4/src/sw_models/anjiMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/anjiMatrix.h` & `sil_thot-3.4.4/src/sw_models/anjiMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/anjm1ip_anjiMatrix.cc` & `sil_thot-3.4.4/src/sw_models/anjm1ip_anjiMatrix.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/src/sw_models/anjm1ip_anjiMatrix.h` & `sil_thot-3.4.4/src/sw_models/anjm1ip_anjiMatrix.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/CMakeLists.txt` & `sil_thot-3.4.4/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/nlp_common/WordAlignmentMatrixTest.cc` & `sil_thot-3.4.4/tests/nlp_common/WordAlignmentMatrixTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/phrase_models/HatTriePhraseTableTest.cc` & `sil_thot-3.4.4/tests/phrase_models/HatTriePhraseTableTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/phrase_models/StlPhraseTableTest.cc` & `sil_thot-3.4.4/tests/phrase_models/StlPhraseTableTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/phrase_models/_phraseTableTest.h` & `sil_thot-3.4.4/tests/phrase_models/_phraseTableTest.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/stack_dec/KbMiraLlWuTest.cc` & `sil_thot-3.4.4/tests/stack_dec/KbMiraLlWuTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/stack_dec/MiraChrFTest.cc` & `sil_thot-3.4.4/tests/stack_dec/MiraChrFTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/stack_dec/PhrLocalSwLiTmTest.cc` & `sil_thot-3.4.4/tests/stack_dec/PhrLocalSwLiTmTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/stack_dec/TranslationMetadataTest.cc` & `sil_thot-3.4.4/tests/stack_dec/TranslationMetadataTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/sw_models/FastAlignModelTest.cc` & `sil_thot-3.4.4/tests/sw_models/FastAlignModelTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/sw_models/Ibm4AlignmentModelTest.cc` & `sil_thot-3.4.4/tests/sw_models/Ibm4AlignmentModelTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/sw_models/IncrHmmAlignmentModelTest.cc` & `sil_thot-3.4.4/tests/sw_models/IncrHmmAlignmentModelTest.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/sw_models/LexTableTest.h` & `sil_thot-3.4.4/tests/sw_models/LexTableTest.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/sw_models/TestUtils.cc` & `sil_thot-3.4.4/tests/sw_models/TestUtils.cc`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/sw_models/TestUtils.h` & `sil_thot-3.4.4/tests/sw_models/TestUtils.h`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/tests/test_module.py` & `sil_thot-3.4.4/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/thot/alignment/__init__.pyi` & `sil_thot-3.4.4/thot/alignment/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/thot/common/__init__.pyi` & `sil_thot-3.4.4/thot/common/__init__.pyi`

 * *Files identical despite different names*

### Comparing `sil-thot-3.4.3/thot/translation/__init__.pyi` & `sil_thot-3.4.4/thot/translation/__init__.pyi`

 * *Files identical despite different names*

