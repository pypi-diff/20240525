# Comparing `tmp/diart-0.9.0.tar.gz` & `tmp/diart-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diart-0.9.0.tar", last modified: Sun Nov 19 11:15:24 2023, max compression
+gzip compressed data, was "diart-0.9.1.tar", last modified: Sat May 25 18:51:23 2024, max compression
```

## Comparing `diart-0.9.0.tar` & `diart-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:24.119175 diart-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-11-19 11:15:15.000000 diart-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2023-11-19 11:15:24.119175 diart-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18709 2023-11-19 11:15:15.000000 diart-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-19 11:15:15.000000 diart-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2023-11-19 11:15:24.119175 diart-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-19 11:15:15.000000 diart-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:24.111175 diart-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:24.115175 diart-0.9.0/src/diart/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/argdoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/audio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:24.115175 diart-0.9.0/src/diart/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/diarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/blocks/vad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:24.119175 diart-0.9.0/src/diart/console/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/console/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/console/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/console/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/console/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/console/tune.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/features.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-11-19 11:15:15.000000 diart-0.9.0/src/diart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 11:15:24.115175 diart-0.9.0/src/diart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19958 2023-11-19 11:15:24.000000 diart-0.9.0/src/diart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-11-19 11:15:24.000000 diart-0.9.0/src/diart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-19 11:15:24.000000 diart-0.9.0/src/diart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-11-19 11:15:24.000000 diart-0.9.0/src/diart.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-19 11:15:24.000000 diart-0.9.0/src/diart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-19 11:15:24.000000 diart-0.9.0/src/diart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.911633 diart-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-25 18:51:19.000000 diart-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-05-25 18:51:23.911633 diart-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18709 2024-05-25 18:51:19.000000 diart-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-25 18:51:19.000000 diart-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-25 18:51:23.915634 diart-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 18:51:19.000000 diart-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.903633 diart-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.907633 diart-0.9.1/src/diart/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/argdoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/audio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.911633 diart-0.9.1/src/diart/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/blocks/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.911633 diart-0.9.1/src/diart/console/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/console/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/console/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/console/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/console/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/console/tune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-25 18:51:19.000000 diart-0.9.1/src/diart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.911633 diart-0.9.1/src/diart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-05-25 18:51:23.000000 diart-0.9.1/src/diart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-25 18:51:23.000000 diart-0.9.1/src/diart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:51:23.000000 diart-0.9.1/src/diart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-25 18:51:23.000000 diart-0.9.1/src/diart.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-25 18:51:23.000000 diart-0.9.1/src/diart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 18:51:23.000000 diart-0.9.1/src/diart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:51:23.911633 diart-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-25 18:51:19.000000 diart-0.9.1/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-25 18:51:19.000000 diart-0.9.1/tests/test_diarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-25 18:51:19.000000 diart-0.9.1/tests/test_end_to_end.py
```

### Comparing `diart-0.9.0/LICENSE` & `diart-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/PKG-INFO` & `diart-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: diart
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python framework to build AI for real-time speech
 Home-page: https://github.com/juanmc2005/diart
 Author: Juan Manuel Coria
 License: MIT
 Keywords: speaker diarization,streaming,online,real time,rxpy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.2
-Requires-Dist: matplotlib>=3.3.3
+Requires-Dist: matplotlib<3.6.0,>=3.3.3
 Requires-Dist: rx>=3.2.0
 Requires-Dist: scipy>=1.6.0
 Requires-Dist: sounddevice>=0.4.2
 Requires-Dist: einops>=0.3.0
 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: pandas>=1.4.2
 Requires-Dist: torch>=1.12.1
@@ -29,14 +29,17 @@
 Requires-Dist: pyannote.core>=4.5
 Requires-Dist: pyannote.database>=4.1.1
 Requires-Dist: pyannote.metrics>=3.2
 Requires-Dist: optuna>=2.10
 Requires-Dist: websocket-server>=0.6.4
 Requires-Dist: websocket-client>=0.58.0
 Requires-Dist: rich>=12.5.1
+Provides-Extra: tests
+Requires-Dist: pytest<8.0.0,>=7.4.0; extra == "tests"
+Requires-Dist: onnxruntime==1.18.0; extra == "tests"
 
 <p align="center">
 <img width="100%" src="https://github.com/juanmc2005/diart/blob/main/logo.jpg?raw=true" title="diart logo" />
 </p>
 
 <p align="center">
 <i>🌿 Build AI-powered real-time audio applications in a breeze 🌿</i>
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: diart Version: 0.9.0 Summary: A python framework to
+Metadata-Version: 2.1 Name: diart Version: 0.9.1 Summary: A python framework to
 build AI for real-time speech Home-page: https://github.com/juanmc2005/diart
 Author: Juan Manuel Coria License: MIT Keywords: speaker
 diarization,streaming,online,real time,rxpy Classifier: Development Status :: 4
 - Beta Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
 Multimedia :: Sound/Audio :: Analysis Classifier: Topic :: Multimedia :: Sound/
 Audio :: Speech Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: numpy>=1.20.2 Requires-Dist: matplotlib>=3.3.3 Requires-Dist:
-rx>=3.2.0 Requires-Dist: scipy>=1.6.0 Requires-Dist: sounddevice>=0.4.2
+Requires-Dist: numpy>=1.20.2 Requires-Dist: matplotlib<3.6.0,>=3.3.3 Requires-
+Dist: rx>=3.2.0 Requires-Dist: scipy>=1.6.0 Requires-Dist: sounddevice>=0.4.2
 Requires-Dist: einops>=0.3.0 Requires-Dist: tqdm>=4.64.0 Requires-Dist:
 pandas>=1.4.2 Requires-Dist: torch>=1.12.1 Requires-Dist: torchvision>=0.14.0
 Requires-Dist: torchaudio>=2.0.2 Requires-Dist: pyannote.audio>=2.1.1 Requires-
 Dist: requests>=2.31.0 Requires-Dist: pyannote.core>=4.5 Requires-Dist:
 pyannote.database>=4.1.1 Requires-Dist: pyannote.metrics>=3.2 Requires-Dist:
 optuna>=2.10 Requires-Dist: websocket-server>=0.6.4 Requires-Dist: websocket-
-client>=0.58.0 Requires-Dist: rich>=12.5.1
+client>=0.58.0 Requires-Dist: rich>=12.5.1 Provides-Extra: tests Requires-Dist:
+pytest<8.0.0,>=7.4.0; extra == "tests" Requires-Dist: onnxruntime==1.18.0;
+extra == "tests"
        [https://github.com/juanmc2005/diart/blob/main/logo.jpg?raw=true]
       ð¿ Build AI-powered real-time audio applications in a breeze ð¿
  [PyPI Version][PyPI Downloads][Python Versions][Code size in bytes][License]
   _[_h_t_t_p_s_:_/_/_j_o_s_s_._t_h_e_o_j_._o_r_g_/_p_a_p_e_r_s_/_c_c_9_8_0_7_c_6_d_e_7_5_e_a_4_c_2_9_0_2_5_c_7_b_d_0_d_3_1_9_9_6_/_s_t_a_t_u_s_._s_v_g_]
           ****** _?ð_?_?_?¾_ _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn_ || _?ð_?_?_?_?ï_?¸_?_ _SS_tt_rr_ee_aa_mm_ _aa_uu_dd_ii_oo_ || _?ð_?_?§_? _ _MM_oo_dd_ee_ll_ss_ 
     _?ð_?_?_?_ _TT_uu_nn_ii_nn_gg_ || _?ð_?_?§_? _?ð_?_?_?_ _PP_ii_pp_ee_ll_ii_nn_ee_ss_ || _?ð_?_?_?_ _WW_ee_bb_SS_oo_cc_kk_ee_tt_ss_ || _?ð_?_?_?¬_ _RR_ee_ss_ee_aa_rr_cc_hh ******
```

### Comparing `diart-0.9.0/README.md` & `diart-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/setup.cfg` & `diart-0.9.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = diart
-version = 0.9.0
+version = 0.9.1
 author = Juan Manuel Coria
 description = A python framework to build AI for real-time speech
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = speaker diarization, streaming, online, real time, rxpy
 url = https://github.com/juanmc2005/diart
 license = MIT
@@ -17,15 +17,15 @@
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	numpy>=1.20.2
-	matplotlib>=3.3.3
+	matplotlib>=3.3.3,<3.6.0
 	rx>=3.2.0
 	scipy>=1.6.0
 	sounddevice>=0.4.2
 	einops>=0.3.0
 	tqdm>=4.64.0
 	pandas>=1.4.2
 	torch>=1.12.1
@@ -37,14 +37,19 @@
 	pyannote.database>=4.1.1
 	pyannote.metrics>=3.2
 	optuna>=2.10
 	websocket-server>=0.6.4
 	websocket-client>=0.58.0
 	rich>=12.5.1
 
+[options.extras_require]
+tests = 
+	pytest>=7.4.0,<8.0.0
+	onnxruntime==1.18.0
+
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	diart.stream=diart.console.stream:run
 	diart.benchmark=diart.console.benchmark:run
```

### Comparing `diart-0.9.0/src/diart/argdoc.py` & `diart-0.9.1/src/diart/argdoc.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/audio.py` & `diart-0.9.1/src/diart/audio.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/__init__.py` & `diart-0.9.1/src/diart/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/aggregation.py` & `diart-0.9.1/src/diart/blocks/aggregation.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/base.py` & `diart-0.9.1/src/diart/blocks/base.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/clustering.py` & `diart-0.9.1/src/diart/blocks/clustering.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/diarization.py` & `diart-0.9.1/src/diart/blocks/diarization.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/embedding.py` & `diart-0.9.1/src/diart/blocks/embedding.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/segmentation.py` & `diart-0.9.1/src/diart/blocks/segmentation.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/utils.py` & `diart-0.9.1/src/diart/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/blocks/vad.py` & `diart-0.9.1/src/diart/blocks/vad.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/console/benchmark.py` & `diart-0.9.1/src/diart/console/benchmark.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/console/client.py` & `diart-0.9.1/src/diart/console/client.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/console/serve.py` & `diart-0.9.1/src/diart/console/serve.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/console/stream.py` & `diart-0.9.1/src/diart/console/stream.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/console/tune.py` & `diart-0.9.1/src/diart/console/tune.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/features.py` & `diart-0.9.1/src/diart/features.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/functional.py` & `diart-0.9.1/src/diart/functional.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/inference.py` & `diart-0.9.1/src/diart/inference.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/mapping.py` & `diart-0.9.1/src/diart/mapping.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/models.py` & `diart-0.9.1/src/diart/models.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/operators.py` & `diart-0.9.1/src/diart/operators.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/optim.py` & `diart-0.9.1/src/diart/optim.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/progress.py` & `diart-0.9.1/src/diart/progress.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/sinks.py` & `diart-0.9.1/src/diart/sinks.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/sources.py` & `diart-0.9.1/src/diart/sources.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart/utils.py` & `diart-0.9.1/src/diart/utils.py`

 * *Files identical despite different names*

### Comparing `diart-0.9.0/src/diart.egg-info/PKG-INFO` & `diart-0.9.1/src/diart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: diart
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python framework to build AI for real-time speech
 Home-page: https://github.com/juanmc2005/diart
 Author: Juan Manuel Coria
 License: MIT
 Keywords: speaker diarization,streaming,online,real time,rxpy
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.2
-Requires-Dist: matplotlib>=3.3.3
+Requires-Dist: matplotlib<3.6.0,>=3.3.3
 Requires-Dist: rx>=3.2.0
 Requires-Dist: scipy>=1.6.0
 Requires-Dist: sounddevice>=0.4.2
 Requires-Dist: einops>=0.3.0
 Requires-Dist: tqdm>=4.64.0
 Requires-Dist: pandas>=1.4.2
 Requires-Dist: torch>=1.12.1
@@ -29,14 +29,17 @@
 Requires-Dist: pyannote.core>=4.5
 Requires-Dist: pyannote.database>=4.1.1
 Requires-Dist: pyannote.metrics>=3.2
 Requires-Dist: optuna>=2.10
 Requires-Dist: websocket-server>=0.6.4
 Requires-Dist: websocket-client>=0.58.0
 Requires-Dist: rich>=12.5.1
+Provides-Extra: tests
+Requires-Dist: pytest<8.0.0,>=7.4.0; extra == "tests"
+Requires-Dist: onnxruntime==1.18.0; extra == "tests"
 
 <p align="center">
 <img width="100%" src="https://github.com/juanmc2005/diart/blob/main/logo.jpg?raw=true" title="diart logo" />
 </p>
 
 <p align="center">
 <i>🌿 Build AI-powered real-time audio applications in a breeze 🌿</i>
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: diart Version: 0.9.0 Summary: A python framework to
+Metadata-Version: 2.1 Name: diart Version: 0.9.1 Summary: A python framework to
 build AI for real-time speech Home-page: https://github.com/juanmc2005/diart
 Author: Juan Manuel Coria License: MIT Keywords: speaker
 diarization,streaming,online,real time,rxpy Classifier: Development Status :: 4
 - Beta Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
 Multimedia :: Sound/Audio :: Analysis Classifier: Topic :: Multimedia :: Sound/
 Audio :: Speech Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: numpy>=1.20.2 Requires-Dist: matplotlib>=3.3.3 Requires-Dist:
-rx>=3.2.0 Requires-Dist: scipy>=1.6.0 Requires-Dist: sounddevice>=0.4.2
+Requires-Dist: numpy>=1.20.2 Requires-Dist: matplotlib<3.6.0,>=3.3.3 Requires-
+Dist: rx>=3.2.0 Requires-Dist: scipy>=1.6.0 Requires-Dist: sounddevice>=0.4.2
 Requires-Dist: einops>=0.3.0 Requires-Dist: tqdm>=4.64.0 Requires-Dist:
 pandas>=1.4.2 Requires-Dist: torch>=1.12.1 Requires-Dist: torchvision>=0.14.0
 Requires-Dist: torchaudio>=2.0.2 Requires-Dist: pyannote.audio>=2.1.1 Requires-
 Dist: requests>=2.31.0 Requires-Dist: pyannote.core>=4.5 Requires-Dist:
 pyannote.database>=4.1.1 Requires-Dist: pyannote.metrics>=3.2 Requires-Dist:
 optuna>=2.10 Requires-Dist: websocket-server>=0.6.4 Requires-Dist: websocket-
-client>=0.58.0 Requires-Dist: rich>=12.5.1
+client>=0.58.0 Requires-Dist: rich>=12.5.1 Provides-Extra: tests Requires-Dist:
+pytest<8.0.0,>=7.4.0; extra == "tests" Requires-Dist: onnxruntime==1.18.0;
+extra == "tests"
        [https://github.com/juanmc2005/diart/blob/main/logo.jpg?raw=true]
       ð¿ Build AI-powered real-time audio applications in a breeze ð¿
  [PyPI Version][PyPI Downloads][Python Versions][Code size in bytes][License]
   _[_h_t_t_p_s_:_/_/_j_o_s_s_._t_h_e_o_j_._o_r_g_/_p_a_p_e_r_s_/_c_c_9_8_0_7_c_6_d_e_7_5_e_a_4_c_2_9_0_2_5_c_7_b_d_0_d_3_1_9_9_6_/_s_t_a_t_u_s_._s_v_g_]
           ****** _?ð_?_?_?¾_ _II_nn_ss_tt_aa_ll_ll_aa_tt_ii_oo_nn_ || _?ð_?_?_?_?ï_?¸_?_ _SS_tt_rr_ee_aa_mm_ _aa_uu_dd_ii_oo_ || _?ð_?_?§_? _ _MM_oo_dd_ee_ll_ss_ 
     _?ð_?_?_?_ _TT_uu_nn_ii_nn_gg_ || _?ð_?_?§_? _?ð_?_?_?_ _PP_ii_pp_ee_ll_ii_nn_ee_ss_ || _?ð_?_?_?_ _WW_ee_bb_SS_oo_cc_kk_ee_tt_ss_ || _?ð_?_?_?¬_ _RR_ee_ss_ee_aa_rr_cc_hh ******
```

### Comparing `diart-0.9.0/src/diart.egg-info/SOURCES.txt` & `diart-0.9.1/src/diart.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,8 +33,11 @@
 src/diart/blocks/utils.py
 src/diart/blocks/vad.py
 src/diart/console/__init__.py
 src/diart/console/benchmark.py
 src/diart/console/client.py
 src/diart/console/serve.py
 src/diart/console/stream.py
-src/diart/console/tune.py
+src/diart/console/tune.py
+tests/test_aggregation.py
+tests/test_diarization.py
+tests/test_end_to_end.py
```

