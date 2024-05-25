# Comparing `tmp/genairr-0.1.0.tar.gz` & `tmp/genairr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genairr-0.1.0.tar", last modified: Sat May 25 09:50:01 2024, max compression
+gzip compressed data, was "genairr-0.1.1.tar", last modified: Sat May 25 10:03:09 2024, max compression
```

## Comparing `genairr-0.1.0.tar` & `genairr-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.212127 genairr-0.1.0/
--rw-rw-rw-   0        0        0    24500 2024-05-25 09:50:01.201978 genairr-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    23320 2024-03-10 10:42:31.000000 genairr-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 09:50:01.212127 genairr-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1688 2024-05-25 09:49:13.000000 genairr-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.072172 genairr-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.086013 genairr-0.1.0/src/GenAIRR/
--rw-rw-rw-   0        0        0      156 2024-03-07 11:37:33.000000 genairr-0.1.0/src/GenAIRR/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.092091 genairr-0.1.0/src/GenAIRR/alleles/
--rw-rw-rw-   0        0        0      120 2024-02-14 14:01:48.000000 genairr-0.1.0/src/GenAIRR/alleles/__init__.py
--rw-rw-rw-   0        0        0    12344 2024-03-31 06:06:28.000000 genairr-0.1.0/src/GenAIRR/alleles/allele.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.152081 genairr-0.1.0/src/GenAIRR/data/
--rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.0/src/GenAIRR/data/HH_S5F_60_META.pkl
--rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.0/src/GenAIRR/data/HH_S5F_META.pkl
--rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.0/src/GenAIRR/data/HH_S5F_Opposite_META.pkl
--rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.0/src/GenAIRR/data/HKL_S5F_META.pkl
--rw-rw-rw-   0        0        0  6375188 2024-02-29 08:18:48.000000 genairr-0.1.0/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl
--rw-rw-rw-   0        0        0  6375243 2024-03-31 06:09:57.000000 genairr-0.1.0/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl
--rw-rw-rw-   0        0        0   897136 2024-02-29 08:29:35.000000 genairr-0.1.0/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl
--rw-rw-rw-   0        0        0   897188 2024-04-04 07:14:45.000000 genairr-0.1.0/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl
--rw-rw-rw-   0        0        0  1258135 2024-02-29 08:24:14.000000 genairr-0.1.0/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl
--rw-rw-rw-   0        0        0  1258187 2024-04-04 07:14:45.000000 genairr-0.1.0/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl
--rw-rw-rw-   0        0        0      639 2024-05-22 15:26:12.000000 genairr-0.1.0/src/GenAIRR/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.152081 genairr-0.1.0/src/GenAIRR/generateDataConfig/
--rw-rw-rw-   0        0        0       82 2024-03-07 11:28:19.000000 genairr-0.1.0/src/GenAIRR/generateDataConfig/__init__.py
--rw-rw-rw-   0        0        0    42684 2024-03-24 09:12:04.000000 genairr-0.1.0/src/GenAIRR/generateDataConfig/make_dataconfig.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.165969 genairr-0.1.0/src/GenAIRR/mutation/
--rw-rw-rw-   0        0        0       95 2024-02-14 14:01:48.000000 genairr-0.1.0/src/GenAIRR/mutation/__init__.py
--rw-rw-rw-   0        0        0     1514 2024-02-29 15:28:44.000000 genairr-0.1.0/src/GenAIRR/mutation/config.py
--rw-rw-rw-   0        0        0     1081 2024-02-29 15:31:36.000000 genairr-0.1.0/src/GenAIRR/mutation/mutation_model.py
--rw-rw-rw-   0        0        0    18179 2024-03-31 06:06:28.000000 genairr-0.1.0/src/GenAIRR/mutation/s5f.py
--rw-rw-rw-   0        0        0     6789 2024-03-31 06:06:28.000000 genairr-0.1.0/src/GenAIRR/mutation/uniform.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.171989 genairr-0.1.0/src/GenAIRR/sequence/
--rw-rw-rw-   0        0        0      165 2024-03-06 08:37:25.000000 genairr-0.1.0/src/GenAIRR/sequence/__init__.py
--rw-rw-rw-   0        0        0     9859 2024-04-07 10:57:21.000000 genairr-0.1.0/src/GenAIRR/sequence/heavy_chain.py
--rw-rw-rw-   0        0        0     8878 2024-04-07 10:49:51.000000 genairr-0.1.0/src/GenAIRR/sequence/light_chain.py
--rw-rw-rw-   0        0        0     4948 2024-02-29 15:57:46.000000 genairr-0.1.0/src/GenAIRR/sequence/np_region.py
--rw-rw-rw-   0        0        0     4369 2024-03-06 08:37:25.000000 genairr-0.1.0/src/GenAIRR/sequence/sequence.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.182174 genairr-0.1.0/src/GenAIRR/simulation/
--rw-rw-rw-   0        0        0      339 2024-02-14 14:01:48.000000 genairr-0.1.0/src/GenAIRR/simulation/__init__.py
--rw-rw-rw-   0        0        0    21613 2024-05-22 15:09:43.000000 genairr-0.1.0/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py
--rw-rw-rw-   0        0        0    30282 2024-04-30 07:21:27.000000 genairr-0.1.0/src/GenAIRR/simulation/light_chain_sequence_augmentor.py
--rw-rw-rw-   0        0        0    36881 2024-04-18 15:01:19.000000 genairr-0.1.0/src/GenAIRR/simulation/sequence_augmentor_base.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.201978 genairr-0.1.0/src/GenAIRR/utilities/
--rw-rw-rw-   0        0        0     3286 2024-03-02 09:19:19.000000 genairr-0.1.0/src/GenAIRR/utilities/AlleleNComparer.py
--rw-rw-rw-   0        0        0      236 2024-02-29 09:29:41.000000 genairr-0.1.0/src/GenAIRR/utilities/__init__.py
--rw-rw-rw-   0        0        0    15686 2024-03-31 06:06:28.000000 genairr-0.1.0/src/GenAIRR/utilities/asc_utilities.py
--rw-rw-rw-   0        0        0     2288 2024-03-02 09:37:07.000000 genairr-0.1.0/src/GenAIRR/utilities/data_config.py
--rw-rw-rw-   0        0        0     3396 2024-03-31 06:06:28.000000 genairr-0.1.0/src/GenAIRR/utilities/data_utilities.py
--rw-rw-rw-   0        0        0      846 2024-03-02 09:38:08.000000 genairr-0.1.0/src/GenAIRR/utilities/file_utilities.py
--rw-rw-rw-   0        0        0     3335 2024-03-02 09:38:47.000000 genairr-0.1.0/src/GenAIRR/utilities/misc.py
--rw-rw-rw-   0        0        0     9495 2024-04-04 07:14:45.000000 genairr-0.1.0/src/GenAIRR/utilities/report.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:50:01.201978 genairr-0.1.0/src/GenAIRR.egg-info/
--rw-rw-rw-   0        0        0    24500 2024-05-25 09:50:00.000000 genairr-0.1.0/src/GenAIRR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1682 2024-05-25 09:50:00.000000 genairr-0.1.0/src/GenAIRR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 09:50:00.000000 genairr-0.1.0/src/GenAIRR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-25 09:50:00.000000 genairr-0.1.0/src/GenAIRR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-25 09:50:00.000000 genairr-0.1.0/src/GenAIRR.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.386337 genairr-0.1.1/
+-rw-rw-rw-   0        0        0    24500 2024-05-25 10:03:09.384084 genairr-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    23320 2024-03-10 10:42:31.000000 genairr-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 10:03:09.387527 genairr-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1688 2024-05-25 10:03:05.000000 genairr-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.269166 genairr-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.277856 genairr-0.1.1/src/GenAIRR/
+-rw-rw-rw-   0        0        0      156 2024-03-07 11:37:33.000000 genairr-0.1.1/src/GenAIRR/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.285458 genairr-0.1.1/src/GenAIRR/alleles/
+-rw-rw-rw-   0        0        0      120 2024-02-14 14:01:48.000000 genairr-0.1.1/src/GenAIRR/alleles/__init__.py
+-rw-rw-rw-   0        0        0    12344 2024-03-31 06:06:28.000000 genairr-0.1.1/src/GenAIRR/alleles/allele.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.342777 genairr-0.1.1/src/GenAIRR/data/
+-rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.1/src/GenAIRR/data/HH_S5F_60_META.pkl
+-rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.1/src/GenAIRR/data/HH_S5F_META.pkl
+-rw-rw-rw-   0        0        0   366369 2024-02-14 13:58:48.000000 genairr-0.1.1/src/GenAIRR/data/HH_S5F_Opposite_META.pkl
+-rw-rw-rw-   0        0        0   366378 2024-02-14 13:58:48.000000 genairr-0.1.1/src/GenAIRR/data/HKL_S5F_META.pkl
+-rw-rw-rw-   0        0        0  6375188 2024-02-29 08:18:48.000000 genairr-0.1.1/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl
+-rw-rw-rw-   0        0        0  6375243 2024-03-31 06:09:57.000000 genairr-0.1.1/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl
+-rw-rw-rw-   0        0        0   897136 2024-02-29 08:29:35.000000 genairr-0.1.1/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl
+-rw-rw-rw-   0        0        0   897188 2024-04-04 07:14:45.000000 genairr-0.1.1/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl
+-rw-rw-rw-   0        0        0  1258135 2024-02-29 08:24:14.000000 genairr-0.1.1/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl
+-rw-rw-rw-   0        0        0  1258187 2024-04-04 07:14:45.000000 genairr-0.1.1/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl
+-rw-rw-rw-   0        0        0      639 2024-05-22 15:26:12.000000 genairr-0.1.1/src/GenAIRR/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.344955 genairr-0.1.1/src/GenAIRR/generateDataConfig/
+-rw-rw-rw-   0        0        0       82 2024-03-07 11:28:19.000000 genairr-0.1.1/src/GenAIRR/generateDataConfig/__init__.py
+-rw-rw-rw-   0        0        0    42684 2024-03-24 09:12:04.000000 genairr-0.1.1/src/GenAIRR/generateDataConfig/make_dataconfig.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.351335 genairr-0.1.1/src/GenAIRR/mutation/
+-rw-rw-rw-   0        0        0       95 2024-02-14 14:01:48.000000 genairr-0.1.1/src/GenAIRR/mutation/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-02-29 15:28:44.000000 genairr-0.1.1/src/GenAIRR/mutation/config.py
+-rw-rw-rw-   0        0        0     1081 2024-02-29 15:31:36.000000 genairr-0.1.1/src/GenAIRR/mutation/mutation_model.py
+-rw-rw-rw-   0        0        0    18179 2024-03-31 06:06:28.000000 genairr-0.1.1/src/GenAIRR/mutation/s5f.py
+-rw-rw-rw-   0        0        0     6789 2024-03-31 06:06:28.000000 genairr-0.1.1/src/GenAIRR/mutation/uniform.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.358997 genairr-0.1.1/src/GenAIRR/sequence/
+-rw-rw-rw-   0        0        0      165 2024-03-06 08:37:25.000000 genairr-0.1.1/src/GenAIRR/sequence/__init__.py
+-rw-rw-rw-   0        0        0     9859 2024-04-07 10:57:21.000000 genairr-0.1.1/src/GenAIRR/sequence/heavy_chain.py
+-rw-rw-rw-   0        0        0     8878 2024-04-07 10:49:51.000000 genairr-0.1.1/src/GenAIRR/sequence/light_chain.py
+-rw-rw-rw-   0        0        0     4948 2024-02-29 15:57:46.000000 genairr-0.1.1/src/GenAIRR/sequence/np_region.py
+-rw-rw-rw-   0        0        0     4369 2024-03-06 08:37:25.000000 genairr-0.1.1/src/GenAIRR/sequence/sequence.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.365528 genairr-0.1.1/src/GenAIRR/simulation/
+-rw-rw-rw-   0        0        0      339 2024-02-14 14:01:48.000000 genairr-0.1.1/src/GenAIRR/simulation/__init__.py
+-rw-rw-rw-   0        0        0    21613 2024-05-22 15:09:43.000000 genairr-0.1.1/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py
+-rw-rw-rw-   0        0        0    30282 2024-04-30 07:21:27.000000 genairr-0.1.1/src/GenAIRR/simulation/light_chain_sequence_augmentor.py
+-rw-rw-rw-   0        0        0    36881 2024-04-18 15:01:19.000000 genairr-0.1.1/src/GenAIRR/simulation/sequence_augmentor_base.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.380738 genairr-0.1.1/src/GenAIRR/utilities/
+-rw-rw-rw-   0        0        0     3286 2024-03-02 09:19:19.000000 genairr-0.1.1/src/GenAIRR/utilities/AlleleNComparer.py
+-rw-rw-rw-   0        0        0      236 2024-02-29 09:29:41.000000 genairr-0.1.1/src/GenAIRR/utilities/__init__.py
+-rw-rw-rw-   0        0        0    15686 2024-03-31 06:06:28.000000 genairr-0.1.1/src/GenAIRR/utilities/asc_utilities.py
+-rw-rw-rw-   0        0        0     2288 2024-03-02 09:37:07.000000 genairr-0.1.1/src/GenAIRR/utilities/data_config.py
+-rw-rw-rw-   0        0        0     3396 2024-03-31 06:06:28.000000 genairr-0.1.1/src/GenAIRR/utilities/data_utilities.py
+-rw-rw-rw-   0        0        0      846 2024-03-02 09:38:08.000000 genairr-0.1.1/src/GenAIRR/utilities/file_utilities.py
+-rw-rw-rw-   0        0        0     3335 2024-03-02 09:38:47.000000 genairr-0.1.1/src/GenAIRR/utilities/misc.py
+-rw-rw-rw-   0        0        0     9495 2024-04-04 07:14:45.000000 genairr-0.1.1/src/GenAIRR/utilities/report.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:03:09.382999 genairr-0.1.1/src/GenAIRR.egg-info/
+-rw-rw-rw-   0        0        0    24500 2024-05-25 10:03:08.000000 genairr-0.1.1/src/GenAIRR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2024-05-25 10:03:09.000000 genairr-0.1.1/src/GenAIRR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 10:03:08.000000 genairr-0.1.1/src/GenAIRR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-25 10:03:08.000000 genairr-0.1.1/src/GenAIRR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 10:03:08.000000 genairr-0.1.1/src/GenAIRR.egg-info/top_level.txt
```

### Comparing `genairr-0.1.0/PKG-INFO` & `genairr-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: GenAIRR
-Version: 0.1.0
+Version: 0.1.1
 Summary: An advanced immunoglobulin sequence simulation suite for benchmarking alignment models and sequence analysis.
 Home-page: https://github.com/MuteJester/GenAIRR
-Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.1.tar.gz
 Author: Thomas Konstantinovsky & Ayelet Peres
 Author-email: thomaskon90@gmail.com
 Project-URL: Bug Tracker, https://github.com/MuteJester/GenAIRR/issues
 Keywords: immunogenetics,sequence simulation,bioinformatics,alignment benchmarking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: numpy~=1.24.3
 Requires-Dist: scipy~=1.11.1
 Requires-Dist: setuptools~=68.0.0
 
 # GenAIRR: AIRR Sequence Simulator
```

### Comparing `genairr-0.1.0/README.md` & `genairr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/setup.py` & `genairr-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='GenAIRR',
-    version='0.1.0',
+    version='0.1.1',
     author='Thomas Konstantinovsky & Ayelet Peres',
     author_email='thomaskon90@gmail.com',
     description='An advanced immunoglobulin sequence simulation suite for benchmarking alignment models and sequence analysis.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MuteJester/GenAIRR',
-    download_url='https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.0.tar.gz',
+    download_url='https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.1.tar.gz',
     project_urls={
         "Bug Tracker": "https://github.com/MuteJester/GenAIRR/issues"
     },
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     package_data={'GenAIRR': ['data/*.pkl', 'data/*.json']},  # Include any additional data files
     include_package_data=True,  # Include everything in source control
@@ -30,9 +30,9 @@
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='immunogenetics, sequence simulation, bioinformatics, alignment benchmarking',
-    python_requires='>=3.7',
+    python_requires='>=3.9',
 )
```

### Comparing `genairr-0.1.0/src/GenAIRR/alleles/allele.py` & `genairr-0.1.1/src/GenAIRR/alleles/allele.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/HH_S5F_60_META.pkl` & `genairr-0.1.1/src/GenAIRR/data/HH_S5F_60_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/HH_S5F_META.pkl` & `genairr-0.1.1/src/GenAIRR/data/HH_S5F_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/HH_S5F_Opposite_META.pkl` & `genairr-0.1.1/src/GenAIRR/data/HH_S5F_Opposite_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/HKL_S5F_META.pkl` & `genairr-0.1.1/src/GenAIRR/data/HKL_S5F_META.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl` & `genairr-0.1.1/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V2.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl` & `genairr-0.1.1/src/GenAIRR/data/HeavyChain_DataConfig_OGRDB_V3.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl` & `genairr-0.1.1/src/GenAIRR/data/LightChain_KAPPA_DataConfigV2.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl` & `genairr-0.1.1/src/GenAIRR/data/LightChain_KAPPA_DataConfigV3.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl` & `genairr-0.1.1/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV2.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl` & `genairr-0.1.1/src/GenAIRR/data/LightChain_LAMBDA_DataConfigV3.pkl`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/data/__init__.py` & `genairr-0.1.1/src/GenAIRR/data/__init__.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/generateDataConfig/make_dataconfig.py` & `genairr-0.1.1/src/GenAIRR/generateDataConfig/make_dataconfig.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/mutation/config.py` & `genairr-0.1.1/src/GenAIRR/mutation/config.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/mutation/mutation_model.py` & `genairr-0.1.1/src/GenAIRR/mutation/mutation_model.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/mutation/s5f.py` & `genairr-0.1.1/src/GenAIRR/mutation/s5f.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/mutation/uniform.py` & `genairr-0.1.1/src/GenAIRR/mutation/uniform.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/sequence/heavy_chain.py` & `genairr-0.1.1/src/GenAIRR/sequence/heavy_chain.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/sequence/light_chain.py` & `genairr-0.1.1/src/GenAIRR/sequence/light_chain.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/sequence/np_region.py` & `genairr-0.1.1/src/GenAIRR/sequence/np_region.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/sequence/sequence.py` & `genairr-0.1.1/src/GenAIRR/sequence/sequence.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py` & `genairr-0.1.1/src/GenAIRR/simulation/heavy_chain_sequence_augmentor.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/simulation/light_chain_sequence_augmentor.py` & `genairr-0.1.1/src/GenAIRR/simulation/light_chain_sequence_augmentor.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/simulation/sequence_augmentor_base.py` & `genairr-0.1.1/src/GenAIRR/simulation/sequence_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/AlleleNComparer.py` & `genairr-0.1.1/src/GenAIRR/utilities/AlleleNComparer.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/asc_utilities.py` & `genairr-0.1.1/src/GenAIRR/utilities/asc_utilities.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/data_config.py` & `genairr-0.1.1/src/GenAIRR/utilities/data_config.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/data_utilities.py` & `genairr-0.1.1/src/GenAIRR/utilities/data_utilities.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/file_utilities.py` & `genairr-0.1.1/src/GenAIRR/utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/misc.py` & `genairr-0.1.1/src/GenAIRR/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR/utilities/report.py` & `genairr-0.1.1/src/GenAIRR/utilities/report.py`

 * *Files identical despite different names*

### Comparing `genairr-0.1.0/src/GenAIRR.egg-info/PKG-INFO` & `genairr-0.1.1/src/GenAIRR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: GenAIRR
-Version: 0.1.0
+Version: 0.1.1
 Summary: An advanced immunoglobulin sequence simulation suite for benchmarking alignment models and sequence analysis.
 Home-page: https://github.com/MuteJester/GenAIRR
-Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.0.tar.gz
+Download-URL: https://github.com/MuteJester/GenAIRR/archive/refs/tags/0.1.1.tar.gz
 Author: Thomas Konstantinovsky & Ayelet Peres
 Author-email: thomaskon90@gmail.com
 Project-URL: Bug Tracker, https://github.com/MuteJester/GenAIRR/issues
 Keywords: immunogenetics,sequence simulation,bioinformatics,alignment benchmarking
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: pandas~=1.5.3
 Requires-Dist: numpy~=1.24.3
 Requires-Dist: scipy~=1.11.1
 Requires-Dist: setuptools~=68.0.0
 
 # GenAIRR: AIRR Sequence Simulator
```

### Comparing `genairr-0.1.0/src/GenAIRR.egg-info/SOURCES.txt` & `genairr-0.1.1/src/GenAIRR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

