# Comparing `tmp/wtlike-0.9.7.tar.gz` & `tmp/wtlike-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtlike-0.9.7.tar", last modified: Wed Apr  5 08:14:14 2023, max compression
+gzip compressed data, was "wtlike-0.9.8.tar", last modified: Fri May 12 14:21:51 2023, max compression
```

## Comparing `wtlike-0.9.7.tar` & `wtlike-0.9.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-04-05 13:48:04.666583 wtlike-0.9.7/
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2348 2020-12-26 22:01:34.000000 wtlike-0.9.7/CONTRIBUTING.md
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    11357 2020-12-26 22:01:34.000000 wtlike-0.9.7/LICENSE
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      111 2020-12-26 22:01:34.000000 wtlike-0.9.7/MANIFEST.in
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)   359169 2023-04-05 13:48:04.661584 wtlike-0.9.7/PKG-INFO
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)   358447 2022-11-06 19:03:12.000000 wtlike-0.9.7/README.md
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      902 2023-04-05 13:47:48.000000 wtlike-0.9.7/settings.ini
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)       38 2023-04-05 13:48:04.667583 wtlike-0.9.7/setup.cfg
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2541 2022-11-06 19:16:04.000000 wtlike-0.9.7/setup.py
-drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-04-05 13:48:03.371871 wtlike-0.9.7/utilities/
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      133 2021-09-18 16:36:21.000000 wtlike-0.9.7/utilities/__init__.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    12104 2023-04-01 15:27:55.000000 wtlike-0.9.7/utilities/catalogs.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2119 2023-02-10 14:38:15.000000 wtlike-0.9.7/utilities/clusterer.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     1814 2022-01-05 13:50:50.000000 wtlike-0.9.7/utilities/fermi_cat.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     3758 2020-12-27 15:12:10.000000 wtlike-0.9.7/utilities/ftp.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    25576 2022-07-12 17:44:44.000000 wtlike-0.9.7/utilities/healpix.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    24881 2023-03-03 23:30:07.000000 wtlike-0.9.7/utilities/ipynb_docgen.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      781 2023-02-18 13:58:41.000000 wtlike-0.9.7/utilities/navigation.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2022-02-13 00:25:42.000000 wtlike-0.9.7/utilities/power_spectrum_fft.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    24565 2023-02-28 14:04:46.000000 wtlike-0.9.7/utilities/process.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    22761 2023-03-10 17:01:27.000000 wtlike-0.9.7/utilities/simulation.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2046 2021-08-16 18:44:36.000000 wtlike-0.9.7/utilities/skydir.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6551 2023-02-08 13:48:28.000000 wtlike-0.9.7/utilities/spectral_functions.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      594 2021-09-18 16:36:15.000000 wtlike-0.9.7/utilities/timer.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2428 2023-03-13 22:55:40.000000 wtlike-0.9.7/utilities/uplots.py
-drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-04-05 13:48:04.192289 wtlike-0.9.7/wtlike/
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      549 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/__init__.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    73936 2023-04-05 13:47:50.000000 wtlike-0.9.7/wtlike/_modidx.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      277 2023-01-13 23:54:32.000000 wtlike-0.9.7/wtlike/_nbdev.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6896 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/bayesian.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    15593 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/cell_data.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    15601 2023-04-05 13:47:48.000000 wtlike-0.9.7/wtlike/config.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    36874 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/data_man.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     8580 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/effective_area.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    25474 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/energyflux.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    12742 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/exposure.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    31164 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/interface.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    19199 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/lightcurve.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    10474 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/load_data.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2374 2021-04-26 15:49:50.000000 wtlike-0.9.7/wtlike/load_gti.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    16362 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/loglike.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6225 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/main.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    17762 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/poisson.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    10948 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/simulation.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    17994 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/skymaps.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6716 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/source_data.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    14289 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/sources.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)    20097 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/time_series.py
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     8188 2023-04-05 13:47:49.000000 wtlike-0.9.7/wtlike/weights.py
-drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-04-05 13:48:04.418896 wtlike-0.9.7/wtlike.egg-info/
-drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-04-05 13:48:04.624030 wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)   359198 2022-09-05 19:22:48.000000 wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)      885 2022-09-05 19:22:48.000000 wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)       20 2022-09-05 19:22:48.000000 wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)       17 2022-09-05 19:22:48.000000 wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)   359169 2023-04-05 13:48:01.000000 wtlike-0.9.7/wtlike.egg-info/PKG-INFO
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)     1304 2023-04-05 13:48:02.000000 wtlike-0.9.7/wtlike.egg-info/SOURCES.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)        1 2023-04-05 13:48:01.000000 wtlike-0.9.7/wtlike.egg-info/dependency_links.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)       55 2023-04-05 13:48:01.000000 wtlike-0.9.7/wtlike.egg-info/entry_points.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)        1 2021-05-06 20:57:26.000000 wtlike-0.9.7/wtlike.egg-info/not-zip-safe
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)       73 2023-04-05 13:48:01.000000 wtlike-0.9.7/wtlike.egg-info/requires.txt
--rwxrwxrwx   0 burnett   (1000) burnett   (1000)       17 2023-04-05 13:48:01.000000 wtlike-0.9.7/wtlike.egg-info/top_level.txt
+drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-05-12 14:21:51.301265 wtlike-0.9.8/
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2348 2020-12-26 22:01:34.000000 wtlike-0.9.8/CONTRIBUTING.md
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    11357 2020-12-26 22:01:34.000000 wtlike-0.9.8/LICENSE
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      111 2020-12-26 22:01:34.000000 wtlike-0.9.8/MANIFEST.in
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)   359169 2023-05-12 14:21:51.295263 wtlike-0.9.8/PKG-INFO
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)   358447 2022-11-06 19:03:12.000000 wtlike-0.9.8/README.md
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      902 2023-05-12 12:22:44.000000 wtlike-0.9.8/settings.ini
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)       38 2023-05-12 14:21:51.303264 wtlike-0.9.8/setup.cfg
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2541 2022-11-06 19:16:04.000000 wtlike-0.9.8/setup.py
+drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-05-12 14:21:49.284353 wtlike-0.9.8/utilities/
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      133 2021-09-18 16:36:21.000000 wtlike-0.9.8/utilities/__init__.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    12653 2023-05-12 12:16:07.000000 wtlike-0.9.8/utilities/catalogs.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2119 2023-02-10 14:38:15.000000 wtlike-0.9.8/utilities/clusterer.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     1814 2022-01-05 13:50:50.000000 wtlike-0.9.8/utilities/fermi_cat.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     3758 2020-12-27 15:12:10.000000 wtlike-0.9.8/utilities/ftp.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    25576 2022-07-12 17:44:44.000000 wtlike-0.9.8/utilities/healpix.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    24881 2023-04-06 17:50:57.000000 wtlike-0.9.8/utilities/ipynb_docgen.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      781 2023-02-18 13:58:41.000000 wtlike-0.9.8/utilities/navigation.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2022-02-13 00:25:42.000000 wtlike-0.9.8/utilities/power_spectrum_fft.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    24565 2023-02-28 14:04:46.000000 wtlike-0.9.8/utilities/process.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    22761 2023-03-10 17:01:27.000000 wtlike-0.9.8/utilities/simulation.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2046 2021-08-16 18:44:36.000000 wtlike-0.9.8/utilities/skydir.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6551 2023-02-08 13:48:28.000000 wtlike-0.9.8/utilities/spectral_functions.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      594 2021-09-18 16:36:15.000000 wtlike-0.9.8/utilities/timer.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2428 2023-03-13 22:55:40.000000 wtlike-0.9.8/utilities/uplots.py
+drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-05-12 14:21:50.607493 wtlike-0.9.8/wtlike/
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      549 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/__init__.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    74047 2023-05-12 12:23:15.000000 wtlike-0.9.8/wtlike/_modidx.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      277 2023-01-13 23:54:32.000000 wtlike-0.9.8/wtlike/_nbdev.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6896 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/bayesian.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    15593 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/cell_data.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    15601 2023-05-12 12:23:13.000000 wtlike-0.9.8/wtlike/config.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    36874 2023-05-12 12:23:13.000000 wtlike-0.9.8/wtlike/data_man.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     8580 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/effective_area.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    25474 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/energyflux.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    12742 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/exposure.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    31671 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/interface.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    19333 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/lightcurve.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    10474 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/load_data.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     2374 2021-04-26 15:49:50.000000 wtlike-0.9.8/wtlike/load_gti.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    16362 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/loglike.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6225 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/main.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    17762 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/poisson.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    10948 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/simulation.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    17994 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/skymaps.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     6716 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/source_data.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    14301 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/sources.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)    20097 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/time_series.py
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     8188 2023-05-12 12:23:14.000000 wtlike-0.9.8/wtlike/weights.py
+drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-05-12 14:21:50.963632 wtlike-0.9.8/wtlike.egg-info/
+drwxrwxrwx   0 burnett   (1000) burnett   (1000)        0 2023-05-12 14:21:51.241378 wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)   359198 2022-09-05 19:22:48.000000 wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)      885 2022-09-05 19:22:48.000000 wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)       20 2022-09-05 19:22:48.000000 wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/entry_points-checkpoint.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)       17 2022-09-05 19:22:48.000000 wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)   359169 2023-05-12 14:21:47.000000 wtlike-0.9.8/wtlike.egg-info/PKG-INFO
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)     1304 2023-05-12 14:21:47.000000 wtlike-0.9.8/wtlike.egg-info/SOURCES.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)        1 2023-05-12 14:21:47.000000 wtlike-0.9.8/wtlike.egg-info/dependency_links.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)       55 2023-05-12 14:21:47.000000 wtlike-0.9.8/wtlike.egg-info/entry_points.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)        1 2021-05-06 20:57:26.000000 wtlike-0.9.8/wtlike.egg-info/not-zip-safe
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)       73 2023-05-12 14:21:47.000000 wtlike-0.9.8/wtlike.egg-info/requires.txt
+-rwxrwxrwx   0 burnett   (1000) burnett   (1000)       17 2023-05-12 14:21:47.000000 wtlike-0.9.8/wtlike.egg-info/top_level.txt
```

### Comparing `wtlike-0.9.7/CONTRIBUTING.md` & `wtlike-0.9.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/LICENSE` & `wtlike-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/PKG-INFO` & `wtlike-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtlike
-Version: 0.9.7
+Version: 0.9.8
 Summary: Time-dependent analysis of point sources in Fermi-LAT data
 Home-page: https://github.com/tburnett/wtlike/tree/master/
 Author: Toby Burnett
 Author-email: tburnett@uw.edu
 License: Apache Software License 2.0
 Keywords: fermi gamma-rays
 Platform: UNKNOWN
```

### Comparing `wtlike-0.9.7/README.md` & `wtlike-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/settings.ini` & `wtlike-0.9.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 user = tburnett
 description = Time-dependent analysis of point sources in Fermi-LAT data
 keywords = fermi gamma-rays
 author = Toby Burnett
 author_email = tburnett@uw.edu
 copyright = T. Burnett
 branch = master
-version = 0.9.7
+version = 0.9.8
 min_python = 3.9
 audience = Developers
 language = English
 custom_sidebar = False
 license = apache2
 status = 4
 requirements = matplotlib>3.5 pandas scipy>=1.7.3 astropy>4.0 healpy ipython>7.0
```

### Comparing `wtlike-0.9.7/setup.py` & `wtlike-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/catalogs.py` & `wtlike-0.9.8/utilities/catalogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,60 +248,77 @@
         cvar = lambda a: data[a].astype(float)
         ivar = lambda a: data[a].astype(int)
         name = list(map(lambda x: x.strip() , data['Source_Name']))
 
         # calculate these first
         funcs = self.specfuncs(data)
 
-        super().__init__( dict(
+        cat_subset =  dict(
             ra          = cvar('RAJ2000'),
             dec         = cvar('DEJ2000'), 
             # fk5         = list(map(LonLat, cvar('RAJ2000'),cvar('DEJ2000'))),
             glat        = cvar('GLAT'),
             glon        = cvar('GLON'),
             # galactic    = list(map(LonLat, cvar('GLON'),cvar('GLAT'))),
             r95         = cvar('Conf_95_SemiMajor'),
             specfunc    = funcs,
             pivot       = cvar('Pivot_Energy'),
             eflux       = cvar('Energy_Flux100'), # erg cm-2 s-1
             significance= cvar('Signif_Avg'),
             variability = cvar('Variability_Index'),
-            assoc_prob  = cvar('ASSOC_PROB_BAY'), # for Bayesian, or _LR for likelihood ratio
-            assoc1_name = cname('ASSOC1'),
-            # assoc2_name = cname('ASSOC2'),
-            class1      = cname('CLASS1'),
+
             # class2      = cname('CLASS2'),
             flags       = list(map(self.FlagBits, ivar('FLAGS'))),
             # ....
-        ))
+        )
+        if 'ASSOC1' in data.columns.names:
+            # release format
+            cat_subset.update(dict(
+                assoc_prob  = cvar('ASSOC_PROB_BAY'), # for Bayesian, or _LR for likelihood ratio
+                assoc1_name = cname('ASSOC1'),
+                class1      = cname('CLASS1'),
+            ))
+        else:
+            # internal format 
+            cat_subset.update(dict(
+                assoc_prob  = cvar('Passoc'), 
+                assoc1_name = cname('assoc_new'),
+                class1      = cname('class_new'),
+            ))
+
+        super().__init__( cat_subset)
+
         print( f': {len(self)} entries' )
         self.__dict__.update(data=data, filename=filename.name, name='4FGL-DR3')
         self.index = name
         self.index.name = 'name'
         self.fitscols = data.columns
 
     def specfuncs(self, data):
         """ Return a list of spectral functions
         """
         # special version that
         specfun_dict = dict(
             PowerLaw=PowerLaw,
             LogParabola=LogParabola,
             PLSuperExpCutoff=PLSuperExpCutoff4,
+            PLSuperExpCutoff4=PLSuperExpCutoff4,
+
             )
         cvar = lambda a: data[a].astype(float)
         cname= lambda n : [s.strip() for s in data[n]]
         def par_array(colnames):
             # return a transposed table of the columns 
             return np.array(list(map(cvar, colnames))).T
 
         pardict = dict(
             LogParabola=par_array('LP_Flux_Density LP_Index LP_beta Pivot_Energy'.split()),
             PowerLaw    =par_array('PL_Flux_Density PL_Index'.split()),
-            PLSuperExpCutoff=par_array('PLEC_Flux_Density PLEC_IndexS PLEC_ExpfactorS PLEC_Exp_Index'.split())
+            PLSuperExpCutoff=par_array('PLEC_Flux_Density PLEC_IndexS PLEC_ExpfactorS PLEC_Exp_Index'.split()),
+            PLSuperExpCutoff4=par_array('PLEC_Flux_Density PLEC_IndexS PLEC_ExpfactorS PLEC_Exp_Index'.split())
                     )
 
         pivot = cvar('Pivot_Energy')
         spec = []                    
         for i,name in enumerate(cname('SpectrumType')):
             pars = pardict[name][i]
             spec.append( specfun_dict[name]( pars, e0=pivot[i]))
```

### Comparing `wtlike-0.9.7/utilities/clusterer.py` & `wtlike-0.9.8/utilities/clusterer.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/fermi_cat.py` & `wtlike-0.9.8/utilities/fermi_cat.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/ftp.py` & `wtlike-0.9.8/utilities/ftp.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/healpix.py` & `wtlike-0.9.8/utilities/healpix.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/ipynb_docgen.py` & `wtlike-0.9.8/utilities/ipynb_docgen.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/navigation.py` & `wtlike-0.9.8/utilities/navigation.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/process.py` & `wtlike-0.9.8/utilities/process.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/simulation.py` & `wtlike-0.9.8/utilities/simulation.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/skydir.py` & `wtlike-0.9.8/utilities/skydir.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/spectral_functions.py` & `wtlike-0.9.8/utilities/spectral_functions.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/timer.py` & `wtlike-0.9.8/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/utilities/uplots.py` & `wtlike-0.9.8/utilities/uplots.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/__init__.py` & `wtlike-0.9.8/wtlike/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 # wtlike--make FermiLAT gamma-ray Light curves
 
 see https://tburnett.github.io/wtlike/tutorial
 """
 
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from pathlib import Path
 
 from .config import Config, UTC, MJD, Timer, FermiInterval
```

### Comparing `wtlike-0.9.7/wtlike/_modidx.py` & `wtlike-0.9.8/wtlike/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,14 +316,15 @@
                                   'wtlike.interface.SummaryInfo': ('interface.html#summaryinfo', 'wtlike/interface.py'),
                                   'wtlike.interface.SummaryInfo.__call__': ('interface.html#summaryinfo.__call__', 'wtlike/interface.py'),
                                   'wtlike.interface.SummaryInfo.run': ('interface.html#summaryinfo.run', 'wtlike/interface.py'),
                                   'wtlike.interface.WTSkyCoord': ('interface.html#wtskycoord', 'wtlike/interface.py'),
                                   'wtlike.interface.WTSkyCoord.__repr__': ('interface.html#wtskycoord.__repr__', 'wtlike/interface.py'),
                                   'wtlike.interface._float_format': ('interface.html#_float_format', 'wtlike/interface.py'),
                                   'wtlike.interface.examine_source': ('interface.html#examine_source', 'wtlike/interface.py'),
+                                  'wtlike.interface.get_SA': ('interface.html#get_sa', 'wtlike/interface.py'),
                                   'wtlike.interface.get_fermi_info': ('interface.html#get_fermi_info', 'wtlike/interface.py'),
                                   'wtlike.interface.harmonic_plots': ('interface.html#harmonic_plots', 'wtlike/interface.py'),
                                   'wtlike.interface.load_source_spreadsheet': ( 'interface.html#load_source_spreadsheet',
                                                                                 'wtlike/interface.py'),
                                   'wtlike.interface.phase_plots': ('interface.html#phase_plots', 'wtlike/interface.py'),
                                   'wtlike.interface.process_df': ('interface.html#process_df', 'wtlike/interface.py'),
                                   'wtlike.interface.process_excel': ('interface.html#process_excel', 'wtlike/interface.py'),
```

### Comparing `wtlike-0.9.7/wtlike/bayesian.py` & `wtlike-0.9.8/wtlike/bayesian.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/cell_data.py` & `wtlike-0.9.8/wtlike/cell_data.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/config.py` & `wtlike-0.9.8/wtlike/config.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/data_man.py` & `wtlike-0.9.8/wtlike/data_man.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/effective_area.py` & `wtlike-0.9.8/wtlike/effective_area.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/energyflux.py` & `wtlike-0.9.8/wtlike/energyflux.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/exposure.py` & `wtlike-0.9.8/wtlike/exposure.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/interface.py` & `wtlike-0.9.8/wtlike/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/91_interface.ipynb.
 
 # %% auto 0
-__all__ = ['src_finder', 'defaults', 'Summarize', 'SourceAnalyzer', 'SummaryInfo', 'phase_plots', 'harmonic_plots',
-           'examine_source', 'PhaseInfo', 'process_df', 'WTSkyCoord', 'load_source_spreadsheet', 'get_fermi_info',
-           'setup_excel', 'process_excel']
+__all__ = ['src_finder', 'defaults', 'proc', 'Summarize', 'SourceAnalyzer', 'SummaryInfo', 'phase_plots', 'harmonic_plots',
+           'get_SA', 'examine_source', 'PhaseInfo', 'process_df', 'WTSkyCoord', 'load_source_spreadsheet',
+           'get_fermi_info', 'setup_excel', 'process_excel']
 
 # %% ../nbs/91_interface.ipynb 2
 import os, sys, warnings
 import datetime
 
 from pathlib import Path
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 from utilities.ipynb_docgen import ( show, DataFrameWrapper, ipynb_doc, capture_hide, capture, monospace)
 from utilities.catalogs import (UWcat, Fermi4FGL)
-from . import (WtLike, PointSource, SourceFinder)
+from . import (WtLike, PointSource, SourceFinder, Config)
 from astropy.coordinates import SkyCoord
 
 # %% ../nbs/91_interface.ipynb 3
 """
 Analysis of the time behaviour of a source
 
 To run an individual source: examine_source(name)
@@ -48,36 +48,35 @@
 uwcat.loc[:,'glat'] = _sk.b.deg
 uwcat.loc[:,'glon'] = _sk.l.deg
 uwcat.loc[:, 'r95'] = np.sqrt( (uwcat.a * 2.64)**2 + (0.00791)**2) # 
 
 src_finder = SourceFinder()
 
 defaults = dict(neighbor=None, interval=30, nyquist=24, max_sep=0.5, tsmin=16, info_name='Other info',
-            fft_query='p1>25 & 10>f>0.01')
+            fft_query='p1>25 & 10>f>0.01', UTC=False)
 
 
 # %% ../nbs/91_interface.ipynb 5
 class Summarize():
     """ base class for call-back class"""
 
     def add(self, sa): 
         pass
 
 class SourceAnalyzer():
 
     def __init__(self, name, 
+            config=None,
             neighbor=None,  
-            # interval=30, 
-            # nyquist=24, 
-            # tsmin=16,
             make_figs=True,
             summarizer=Summarize(),
             **kwargs):
         """
         """
+        self.config = config if config is not None else Config()
         self.log=''
         self.wtl=None
         self.max_sep = kwargs.pop('max_sep', defaults['max_sep'])
         self.porb = float(kwargs.pop('porb', np.nan))
         self.fluxlim = kwargs.pop('fluxlim', None)
         interval = kwargs.pop('interval', defaults['interval'])
         nyquist  = kwargs.pop('nyquist', defaults['nyquist'])
@@ -152,19 +151,19 @@
             self.pointlike_info = pi = uwcat.loc[pt_name]
             ts = pi.ts
             if ts < tsmin:
                 self.log = f'UW source has TS={ts:.1f} < {tsmin}'
                 self.wtl = None
                 return True
 
-            self.wtl = WtLike(PointSource(pt_name), time_bins=(tstart, tstop, interval)) 
+            self.wtl = WtLike(PointSource(pt_name, config=self.config), time_bins=(tstart, tstop, interval),) 
 
             if type(neighbor)==str and str(neighbor).strip():
                 print(f'Reweighting with {neighbor}')
-                self.neighbor_bb = WtLike(neighbor).bb_view()
+                self.neighbor_bb = WtLike(neighbor, config=self.config).bb_view()
                 self.wtl = self.wtl.reweighted_view(self.neighbor_bb)
             self.bb = self.wtl.view(interval).bb_view()
             
             self.px = self.wtl.periodogram( 1/(4*nyquist), tstart=tstart, tstop=tstop)
 
             if not(np.isnan(self.porb)) and self.porb is not None:
                 # generate orbial phase view to plot later (no periastron yet)
@@ -277,18 +276,18 @@
                     ['flux beta sig_beta'.split()]
             return pd.concat([df_bb, df_beta], axis=1)
 
         except Exception as e:
             print(f'SourceAnalyzer: bb 2-d fit failed: {e}', file=sys.stderr)
             return None
         
-    def plot_bb(self, ax):
+    def plot_bb(self, ax, UTC=False):
         if self.fluxlim is not None:
             ax.set(ylim=self.fluxlim) ###
-        self.bb.plot(ax=ax, source_name=self.wtl.source.name, UTC=True)
+        self.bb.plot(ax=ax, source_name=self.wtl.source.name, UTC=UTC)
         self.bb_table = self.get_bb_info()
 
     def display_bb_table(self):
         """ return (hidden) markdown string"""
         bt = self.bb_table
         if bt is None or len(bt)==0 or not 'beta' in bt : return ''
         test = np.max(bt.beta/bt.sig_beta)
@@ -317,15 +316,15 @@
         self.px.power_plot(ax=ax3, pmax=50)
         hist_peak_power(self.px, ax=ax4, title='Peak distribution', xlabel='')
 
     def get_fft_peaks(self):
         if not hasattr(self, 'px'):
             return pd.DataFrame()
         query = defaults['fft_query']
-        df = self.px.find_peaks('p1').query(query)
+        df = self.px.find_peaks('p1').query(query).copy()
         if len(df)>0: 
             df['period'] = 1/df.f
         return df
     
     def display_fft_peaks(self, show=False):
         try:
             df = self.get_fft_peaks()
@@ -435,32 +434,40 @@
 
 # %% ../nbs/91_interface.ipynb 6
 class SummaryInfo:  
     """Batch process a list of sources,
         returning a dict of summary info for each one
     """  
     
-    def __call__(self, info):
+    def __call__(self, info, config=None):
         if type(info)==str:  name, info = info, {}
         else: name = info.name
-        print(name)
+
         # run the analyzer without making figures
-        sa = SourceAnalyzer(name, make_figs=False, tsmin=20,
-                            **info )
+        try:
+            sa = SourceAnalyzer(name, make_figs=False, tsmin=20, config=config)
+        except Exception as e:
+            return name, dict(error=str(e))
+        if sa.name=='(not found)':
+            return name, dict(error='source name not found')
+        if sa is None:
+            return name, dict(error='SourceAnalyzer failure')
+        
         ret =  dict(
             light_curve = sa.get_bb_info(),
             fft_peaks = sa.get_fft_peaks(),
+            nearby = sa.get_nearby(), 
             porb = sa.porb,)
         if not pd.isna(sa.porb):
             # items computed only porb is specified.
             ret.update(
                 phase_lc = sa.orbital_phase.fits,
                 harmonics = sa.get_harmonics(num=10) 
             )
-        return ret
+        return name, ret
     
     def run(self, df):
         if isinstance(df, pd.DataFrame):
             # a data frame: column info passed to the analyzer
             return dict(df.apply(self, axis=1))
         elif hasattr(df, '__len__'):
             # a list of names
@@ -514,14 +521,19 @@
         ax.grid(alpha=0.5)
 
     for ax in axf[len(ldf): len(axf)]: ax.set_visible(False)
     fig.suptitle('HMXB H-test', fontsize=18)
     return fig
 
 # %% ../nbs/91_interface.ipynb 7
+proc = None
+def get_SA():
+    """ access to the most recent SourceAnalyzer object"""
+    return proc
+
 @ipynb_doc
 def examine_source(name, info=None, text='',  **kwargs): 
 
     """### {name}
     {other_info}
     {text}
     {log}
```

### Comparing `wtlike-0.9.7/wtlike/lightcurve.py` & `wtlike-0.9.8/wtlike/lightcurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,48 +247,50 @@
                    ) * flux_factor
 
     # do the limits first (only for poisson rep)
     if len(lim)>0:
         t = lim.t-tzero
         tw = lim.tw
         color = colors[2 if step else 1]
+        if color!= 'none':
 
-        y = allflux[limit]
-        # set any inf's to zero 
-        y = np.where(np.isinf(y),0,y)
-        if limit_fmt is None:
-
-            # try to draw an error bar, hard to determine size
-            yerr = error_size(ax, t, y) #0.2*(1 if kw['yscale']=='linear' else y)#*flux_factor
-
-            ax.errorbar(x=t, y=y, xerr=tw/2,
-                    yerr=yerr,  color=color ,
-                    uplims=True, ls='',
-                    ms=ms, lw=error_lw, capsize=2*error_lw, capthick=0,
-                    zorder=zorder, label='  95% limit', **errorbar_args)
-        else:
-            # just a symbol, like 'v'
-            ax.errorbar(x=t,xerr=tw/2, y=y, fmt=limit_fmt, color=color,
-                       zorder=zorder, label='  95% limit', **errorbar_args)
+            y = allflux[limit]
+            # set any inf's to zero 
+            y = np.where(np.isinf(y),0,y)
+            if limit_fmt is None:
+
+                # try to draw an error bar, hard to determine size
+                yerr = error_size(ax, t, y) #0.2*(1 if kw['yscale']=='linear' else y)#*flux_factor
+
+                ax.errorbar(x=t, y=y, xerr=tw/2,
+                        yerr=yerr,  color=color ,
+                        uplims=True, ls='',
+                        ms=ms, lw=error_lw, capsize=2*error_lw, capthick=0,
+                        zorder=zorder, label='  95% limit', **errorbar_args)
+            else:
+                # just a symbol, like 'v'
+                ax.errorbar(x=t,xerr=tw/2, y=y, fmt=limit_fmt, color=color,
+                        zorder=zorder, label='  95% limit', **errorbar_args)
 
     # then the points with error bars
     t = bar.t.values-tzero
     tw = bar.tw.values.astype(float)
     fluxmeas = allflux[~limit]
     upper = bar.fit.apply(lambda f: f.errors[1]).values * flux_factor
     lower = bar.fit.apply(lambda f: f.errors[0]).values * flux_factor
     error = np.array([upper-fluxmeas, fluxmeas-lower])
 #     if label is None:
 #         label = f'{bin_size_name(round(tw.mean(),4))} bins' if np.std(tw)<1e-6 else ''
-    ax.errorbar(
-        x=t, xerr=tw/2, ms=ms,
-                y=fluxmeas, yerr=error, lw=2, fmt=fmt,
-                color=colors[0],
-                label=label, zorder=zorder+1,
-                **errorbar_args)
+    if colors[0]!='none':
+        ax.errorbar(
+            x=t, xerr=tw/2, ms=ms,
+                    y=fluxmeas, yerr=error, lw=2, fmt=fmt,
+                    color=colors[0],
+                    label=label, zorder=zorder+1,
+                    **errorbar_args)
 
     # finally overlay the step if requested
     if step:
         t = df.t.values-tzero
         xerr = df.tw.values/2;
         x = np.append(t-xerr, [t[-1]+xerr[-1]]);
         y = np.append(allflux, [allflux[-1]])
```

### Comparing `wtlike-0.9.7/wtlike/load_data.py` & `wtlike-0.9.8/wtlike/load_data.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/load_gti.py` & `wtlike-0.9.8/wtlike/load_gti.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/loglike.py` & `wtlike-0.9.8/wtlike/loglike.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/main.py` & `wtlike-0.9.8/wtlike/main.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/poisson.py` & `wtlike-0.9.8/wtlike/poisson.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/simulation.py` & `wtlike-0.9.8/wtlike/simulation.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/skymaps.py` & `wtlike-0.9.8/wtlike/skymaps.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/source_data.py` & `wtlike-0.9.8/wtlike/source_data.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/sources.py` & `wtlike-0.9.8/wtlike/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     """
 
     max_sep = 0.1
 
     def __init__(self, config=None):
         from astropy.io import fits
         import pandas as pd
-        self.config=Config() if config is None else config
+        config=self.config=Config() if config is None else config
         self.log = ''
 
-        zip_index = get_wtzip_index(config)
+        zip_index = get_wtzip_index(self.config)
         if zip_index is None:
             raise Exception('Expected zip file weight_files.zip')
 
         self.pt_dirs=zip_index['coord']
         self.pt_names = zip_index['name']
 
         catalog_file = Path(config.catalog_file).expanduser()
```

### Comparing `wtlike-0.9.7/wtlike/time_series.py` & `wtlike-0.9.8/wtlike/time_series.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike/weights.py` & `wtlike-0.9.8/wtlike/weights.py`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt` & `wtlike-0.9.8/wtlike.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `wtlike-0.9.7/wtlike.egg-info/PKG-INFO` & `wtlike-0.9.8/wtlike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtlike
-Version: 0.9.7
+Version: 0.9.8
 Summary: Time-dependent analysis of point sources in Fermi-LAT data
 Home-page: https://github.com/tburnett/wtlike/tree/master/
 Author: Toby Burnett
 Author-email: tburnett@uw.edu
 License: Apache Software License 2.0
 Keywords: fermi gamma-rays
 Platform: UNKNOWN
```

### Comparing `wtlike-0.9.7/wtlike.egg-info/SOURCES.txt` & `wtlike-0.9.8/wtlike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

