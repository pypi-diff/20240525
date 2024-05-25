# Comparing `tmp/BSTPP-0.1.2.tar.gz` & `tmp/BSTPP-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BSTPP-0.1.2.tar", last modified: Wed Apr 10 01:08:55 2024, max compression
+gzip compressed data, was "BSTPP-0.1.3.tar", last modified: Sat May 25 20:32:00 2024, max compression
```

## Comparing `BSTPP-0.1.2.tar` & `BSTPP-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-04-10 01:08:55.469574 BSTPP-0.1.2/
-drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-04-10 01:08:55.445573 BSTPP-0.1.2/BSTPP.egg-info/
--rw-r--r--   0 imanring  (1008) imanring  (1008)     1966 2024-04-10 01:08:55.000000 BSTPP-0.1.2/BSTPP.egg-info/PKG-INFO
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     1087 2024-04-10 01:08:55.000000 BSTPP-0.1.2/BSTPP.egg-info/SOURCES.txt
--rw-rw-r--   0 imanring  (1008) imanring  (1008)        1 2024-04-10 01:08:55.000000 BSTPP-0.1.2/BSTPP.egg-info/dependency_links.txt
--rw-rw-r--   0 imanring  (1008) imanring  (1008)      254 2024-04-10 01:08:55.000000 BSTPP-0.1.2/BSTPP.egg-info/requires.txt
--rw-rw-r--   0 imanring  (1008) imanring  (1008)        6 2024-04-10 01:08:55.000000 BSTPP-0.1.2/BSTPP.egg-info/top_level.txt
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    35120 2024-04-10 00:34:57.000000 BSTPP-0.1.2/LICENSE.txt
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     1966 2024-04-10 01:08:55.469574 BSTPP-0.1.2/PKG-INFO
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     1661 2024-03-20 20:41:02.000000 BSTPP-0.1.2/README.md
-drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-04-10 01:08:55.449573 BSTPP-0.1.2/bstpp/
--rw-rw-r--   0 imanring  (1008) imanring  (1008)        0 2023-11-02 20:04:44.000000 BSTPP-0.1.2/bstpp/__init__.py
-drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-04-10 01:08:55.457573 BSTPP-0.1.2/bstpp/data/
--rw-rw-r--   0 imanring  (1008) imanring  (1008)   109760 2024-01-27 15:46:59.000000 BSTPP-0.1.2/bstpp/data/BH_conflicts.csv
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    90315 2024-01-27 15:46:59.000000 BSTPP-0.1.2/bstpp/data/BH_cov.csv
--rw-rw-r--   0 imanring  (1008) imanring  (1008)   545580 2024-01-27 15:42:06.000000 BSTPP-0.1.2/bstpp/data/Boundaries - Community Areas (current).zip
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    94494 2024-01-27 15:42:56.000000 BSTPP-0.1.2/bstpp/data/Chicago_2022_xyt.csv
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    80653 2024-01-27 15:42:56.000000 BSTPP-0.1.2/bstpp/data/Chicago_2023_xyt.csv
--rw-rw-r--   0 imanring  (1008) imanring  (1008)   507884 2024-01-27 19:42:44.000000 BSTPP-0.1.2/bstpp/data/Chicago_cov.zip
--rw-rw-r--   0 imanring  (1008) imanring  (1008)        0 2024-01-27 15:51:18.000000 BSTPP-0.1.2/bstpp/data/__init__.py
-drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-04-10 01:08:55.469574 BSTPP-0.1.2/bstpp/decoders/
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    83861 2023-11-15 20:40:41.000000 BSTPP-0.1.2/bstpp/decoders/2d_decoder.pkl
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    86401 2023-11-17 14:15:33.000000 BSTPP-0.1.2/bstpp/decoders/2d_decoder_10_5.pkl
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    84561 2023-11-16 12:51:12.000000 BSTPP-0.1.2/bstpp/decoders/2d_decoder_12.pkl
--rw-rw-r--   0 imanring  (1008) imanring  (1008)   149341 2024-02-06 23:58:20.000000 BSTPP-0.1.2/bstpp/decoders/2d_decoder_15_5_large.pkl
--rw-rw-r--   0 imanring  (1008) imanring  (1008)   149504 2023-12-09 15:46:08.000000 BSTPP-0.1.2/bstpp/decoders/2d_decoder_15_5_large_device.pkl
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    86401 2023-11-20 20:48:39.000000 BSTPP-0.1.2/bstpp/decoders/2d_decoder_fixvar.pkl
--rw-rw-r--   0 imanring  (1008) imanring  (1008)        0 2023-11-03 15:09:39.000000 BSTPP-0.1.2/bstpp/decoders/__init__.py
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     9136 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_1d_T50_fixed_ls
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     9136 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_1d_T50_fixed_ls10
--rw-rw-r--   0 imanring  (1008) imanring  (1008)   131550 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_1d_T50_fixed_ls_n900
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    20779 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_1d_T80_fixed_ls10
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    59712 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_1d_n400_integral_n
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    55789 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_1d_n400_lgcp
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    83698 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoder_2d_n25_infer_hyperpars
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    59712 2023-11-01 16:09:00.000000 BSTPP-0.1.2/bstpp/decoders/decoders
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     9361 2024-03-02 03:26:45.000000 BSTPP-0.1.2/bstpp/inference_functions.py
--rw-rw-r--   0 imanring  (1008) imanring  (1008)    37883 2024-04-03 03:01:25.000000 BSTPP-0.1.2/bstpp/main.py
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     6094 2024-02-28 13:27:15.000000 BSTPP-0.1.2/bstpp/trigger.py
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     4898 2024-02-14 01:43:03.000000 BSTPP-0.1.2/bstpp/utils.py
--rw-rw-r--   0 imanring  (1008) imanring  (1008)     3118 2023-11-01 20:01:55.000000 BSTPP-0.1.2/bstpp/vae_functions.py
--rw-rw-r--   0 imanring  (1008) imanring  (1008)       84 2024-02-03 20:44:48.000000 BSTPP-0.1.2/pyproject.toml
--rw-rw-r--   0 imanring  (1008) imanring  (1008)       38 2024-04-10 01:08:55.469574 BSTPP-0.1.2/setup.cfg
--rw-rw-r--   0 imanring  (1008) imanring  (1008)      888 2024-04-10 01:08:49.000000 BSTPP-0.1.2/setup.py
+drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-05-25 20:32:00.656925 BSTPP-0.1.3/
+drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-05-25 20:32:00.648925 BSTPP-0.1.3/BSTPP.egg-info/
+-rw-r--r--   0 imanring  (1008) imanring  (1008)     1966 2024-05-25 20:32:00.000000 BSTPP-0.1.3/BSTPP.egg-info/PKG-INFO
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     1087 2024-05-25 20:32:00.000000 BSTPP-0.1.3/BSTPP.egg-info/SOURCES.txt
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)        1 2024-05-25 20:32:00.000000 BSTPP-0.1.3/BSTPP.egg-info/dependency_links.txt
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)      254 2024-05-25 20:32:00.000000 BSTPP-0.1.3/BSTPP.egg-info/requires.txt
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)        6 2024-05-25 20:32:00.000000 BSTPP-0.1.3/BSTPP.egg-info/top_level.txt
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    35120 2024-04-10 00:34:57.000000 BSTPP-0.1.3/LICENSE.txt
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     1966 2024-05-25 20:32:00.656925 BSTPP-0.1.3/PKG-INFO
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     1661 2024-03-20 20:41:02.000000 BSTPP-0.1.3/README.md
+drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-05-25 20:32:00.648925 BSTPP-0.1.3/bstpp/
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)        0 2023-11-02 20:04:44.000000 BSTPP-0.1.3/bstpp/__init__.py
+drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-05-25 20:32:00.652925 BSTPP-0.1.3/bstpp/data/
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)   109760 2024-01-27 15:46:59.000000 BSTPP-0.1.3/bstpp/data/BH_conflicts.csv
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    90315 2024-01-27 15:46:59.000000 BSTPP-0.1.3/bstpp/data/BH_cov.csv
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)   545580 2024-01-27 15:42:06.000000 BSTPP-0.1.3/bstpp/data/Boundaries - Community Areas (current).zip
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    94494 2024-01-27 15:42:56.000000 BSTPP-0.1.3/bstpp/data/Chicago_2022_xyt.csv
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    80653 2024-01-27 15:42:56.000000 BSTPP-0.1.3/bstpp/data/Chicago_2023_xyt.csv
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)   507884 2024-01-27 19:42:44.000000 BSTPP-0.1.3/bstpp/data/Chicago_cov.zip
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)        0 2024-01-27 15:51:18.000000 BSTPP-0.1.3/bstpp/data/__init__.py
+drwxrwxr-x   0 imanring  (1008) imanring  (1008)        0 2024-05-25 20:32:00.656925 BSTPP-0.1.3/bstpp/decoders/
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    83861 2023-11-15 20:40:41.000000 BSTPP-0.1.3/bstpp/decoders/2d_decoder.pkl
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    86401 2023-11-17 14:15:33.000000 BSTPP-0.1.3/bstpp/decoders/2d_decoder_10_5.pkl
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    84561 2023-11-16 12:51:12.000000 BSTPP-0.1.3/bstpp/decoders/2d_decoder_12.pkl
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)   149341 2024-02-06 23:58:20.000000 BSTPP-0.1.3/bstpp/decoders/2d_decoder_15_5_large.pkl
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)   149504 2023-12-09 15:46:08.000000 BSTPP-0.1.3/bstpp/decoders/2d_decoder_15_5_large_device.pkl
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    86401 2023-11-20 20:48:39.000000 BSTPP-0.1.3/bstpp/decoders/2d_decoder_fixvar.pkl
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)        0 2023-11-03 15:09:39.000000 BSTPP-0.1.3/bstpp/decoders/__init__.py
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     9136 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_1d_T50_fixed_ls
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     9136 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_1d_T50_fixed_ls10
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)   131550 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_1d_T50_fixed_ls_n900
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    20779 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_1d_T80_fixed_ls10
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    59712 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_1d_n400_integral_n
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    55789 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_1d_n400_lgcp
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    83698 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoder_2d_n25_infer_hyperpars
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    59712 2023-11-01 16:09:00.000000 BSTPP-0.1.3/bstpp/decoders/decoders
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     9481 2024-05-24 21:50:20.000000 BSTPP-0.1.3/bstpp/inference_functions.py
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)    37883 2024-04-03 03:01:25.000000 BSTPP-0.1.3/bstpp/main.py
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     6094 2024-02-28 13:27:15.000000 BSTPP-0.1.3/bstpp/trigger.py
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     4898 2024-02-14 01:43:03.000000 BSTPP-0.1.3/bstpp/utils.py
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)     3118 2023-11-01 20:01:55.000000 BSTPP-0.1.3/bstpp/vae_functions.py
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)       84 2024-02-03 20:44:48.000000 BSTPP-0.1.3/pyproject.toml
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)       38 2024-05-25 20:32:00.656925 BSTPP-0.1.3/setup.cfg
+-rw-rw-r--   0 imanring  (1008) imanring  (1008)      888 2024-05-25 20:31:11.000000 BSTPP-0.1.3/setup.py
```

### Comparing `BSTPP-0.1.2/BSTPP.egg-info/PKG-INFO` & `BSTPP-0.1.3/BSTPP.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BSTPP
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bayesian Spatiotemporal Point Process
 Home-page: https://github.com/imanring/BSTPP.git
 Author: Isaac Manring
 Author-email: isaacamanring@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BSTPP-0.1.2/BSTPP.egg-info/SOURCES.txt` & `BSTPP-0.1.3/BSTPP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/LICENSE.txt` & `BSTPP-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/PKG-INFO` & `BSTPP-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BSTPP
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bayesian Spatiotemporal Point Process
 Home-page: https://github.com/imanring/BSTPP.git
 Author: Isaac Manring
 Author-email: isaacamanring@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `BSTPP-0.1.2/README.md` & `BSTPP-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/data/BH_conflicts.csv` & `BSTPP-0.1.3/bstpp/data/BH_conflicts.csv`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/data/BH_cov.csv` & `BSTPP-0.1.3/bstpp/data/BH_cov.csv`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/data/Boundaries - Community Areas (current).zip` & `BSTPP-0.1.3/bstpp/data/Boundaries - Community Areas (current).zip`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/data/Chicago_2022_xyt.csv` & `BSTPP-0.1.3/bstpp/data/Chicago_2022_xyt.csv`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/data/Chicago_2023_xyt.csv` & `BSTPP-0.1.3/bstpp/data/Chicago_2023_xyt.csv`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/data/Chicago_cov.zip` & `BSTPP-0.1.3/bstpp/data/Chicago_cov.zip`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/2d_decoder.pkl` & `BSTPP-0.1.3/bstpp/decoders/2d_decoder.pkl`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/2d_decoder_10_5.pkl` & `BSTPP-0.1.3/bstpp/decoders/2d_decoder_10_5.pkl`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/2d_decoder_12.pkl` & `BSTPP-0.1.3/bstpp/decoders/2d_decoder_12.pkl`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/2d_decoder_15_5_large.pkl` & `BSTPP-0.1.3/bstpp/decoders/2d_decoder_15_5_large.pkl`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/2d_decoder_15_5_large_device.pkl` & `BSTPP-0.1.3/bstpp/decoders/2d_decoder_15_5_large_device.pkl`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/2d_decoder_fixvar.pkl` & `BSTPP-0.1.3/bstpp/decoders/2d_decoder_fixvar.pkl`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_1d_T50_fixed_ls` & `BSTPP-0.1.3/bstpp/decoders/decoder_1d_T50_fixed_ls`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_1d_T50_fixed_ls10` & `BSTPP-0.1.3/bstpp/decoders/decoder_1d_T50_fixed_ls10`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_1d_T50_fixed_ls_n900` & `BSTPP-0.1.3/bstpp/decoders/decoder_1d_T50_fixed_ls_n900`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_1d_T80_fixed_ls10` & `BSTPP-0.1.3/bstpp/decoders/decoder_1d_T80_fixed_ls10`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_1d_n400_integral_n` & `BSTPP-0.1.3/bstpp/decoders/decoder_1d_n400_integral_n`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_1d_n400_lgcp` & `BSTPP-0.1.3/bstpp/decoders/decoder_1d_n400_lgcp`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoder_2d_n25_infer_hyperpars` & `BSTPP-0.1.3/bstpp/decoders/decoder_2d_n25_infer_hyperpars`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/decoders/decoders` & `BSTPP-0.1.3/bstpp/decoders/decoders`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/inference_functions.py` & `BSTPP-0.1.3/bstpp/inference_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from numpyro.infer.autoguide import *
 from numpyro import optim
 from .utils import difference_matrix
 from .vae_functions import *
 
 
 def spatiotemporal_hawkes_model(args):
+    # Model for Hawkes and Cox Hawkes
+    
     t_events=args["t_events"]
     xy_events=args["xy_events"]
     N=t_events.shape[0]
 
     if args['model'] == 'hawkes':
       a_0 = numpyro.sample("a_0", args['priors']['a_0'])
       if 'spatial_cov' in args:
@@ -173,15 +175,14 @@
 
 
 def run_mcmc(rng_key, model_mcmc, args):
     start = time.time()
 
     init_strategy = init_to_median(num_samples=10)
     kernel = NUTS(model_mcmc, init_strategy=init_strategy)#, max_tree_depth=(7,9))
-    #kernel = SVI(model_mcmc, )
     mcmc = MCMC(
         kernel,
         num_warmup=args["num_warmup"],
         num_samples=args["num_samples"],
         num_chains=args["num_chains"],
         thinning=args["thinning"],
         progress_bar=False if "NUMPYRO_SPHINXBUILD" in os.environ else True,
@@ -190,15 +191,18 @@
     mcmc.print_summary()
     print("\nMCMC elapsed time:", time.time() - start)
     return mcmc
 
 def get_samples(rng_key,model,guide,svi_result,args,sites):
     predictive = Predictive(model, guide=guide, params=svi_result.params, 
                             return_sites = sites,
-                            num_samples=args["num_samples"])
+                            num_samples=args["num_samples"], 
+                            parallel = True
+                           )
+    print("Sampling Posterior...")
     posterior_samples = predictive(rng_key, args=args)
     return posterior_samples
 
 def run_SVI(rng_key, model, args, num_steps, lr, sites, auto_guide = AutoMultivariateNormal, init_strategy=init_to_median,init_state=None):
     start = time.time()
     optimizer = numpyro.optim.Adam(inverse_time_decay(lr,num_steps,4))
     #optimizer = numpyro.optim.Adam(exponential_decay(lr,num_steps,0.01))
```

### Comparing `BSTPP-0.1.2/bstpp/main.py` & `BSTPP-0.1.3/bstpp/main.py`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/trigger.py` & `BSTPP-0.1.3/bstpp/trigger.py`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/utils.py` & `BSTPP-0.1.3/bstpp/utils.py`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/bstpp/vae_functions.py` & `BSTPP-0.1.3/bstpp/vae_functions.py`

 * *Files identical despite different names*

### Comparing `BSTPP-0.1.2/setup.py` & `BSTPP-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 modules = ['dill>=0.3.5.1','geopandas>=0.14.0','importlib-resources','jax==0.4.23',
            'jaxlib==0.4.23','matplotlib>=3.5.2','multipledispatch>=0.6.0','numpy>=1.24.1',
            'numpyro>=0.10.0','opt-einsum>=3.3.0','packaging>=21.3','pandas>=1.4.3',
            'pyparsing>=3.0.9','scipy>=1.9.0','six>=1.16.0','tqdm>=4.64.0']
 
 setup(
     name='BSTPP',
-    version='0.1.2',
+    version='0.1.3',
 
     url='https://github.com/imanring/BSTPP.git',
     author='Isaac Manring',
     author_email='isaacamanring@gmail.com',
     
     install_requires=modules,
     packages=['bstpp'],
```

