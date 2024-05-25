# Comparing `tmp/neurocaps-0.9.1.tar.gz` & `tmp/neurocaps-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.1.tar", last modified: Thu May 23 03:23:29 2024, max compression
+gzip compressed data, was "neurocaps-0.9.2.tar", last modified: Sat May 25 00:49:59 2024, max compression
```

## Comparing `neurocaps-0.9.1.tar` & `neurocaps-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.928774 neurocaps-0.9.1/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.1/LICENSE.md
--rw-rw-rw-   0        0        0    15499 2024-05-23 03:23:29.928774 neurocaps-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    14181 2024-05-23 03:16:14.000000 neurocaps-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.876917 neurocaps-0.9.1/neurocaps/
--rw-rw-rw-   0        0        0       78 2024-04-28 16:38:21.000000 neurocaps-0.9.1/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.903339 neurocaps-0.9.1/neurocaps/_utils/
--rw-rw-rw-   0        0        0      369 2024-05-23 03:16:17.000000 neurocaps-0.9.1/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.906845 neurocaps-0.9.1/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.1/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2591 2024-05-09 19:38:42.000000 neurocaps-0.9.1/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      186 2024-04-28 16:38:21.000000 neurocaps-0.9.1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.913324 neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2863 2024-05-23 03:16:17.000000 neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-23 03:16:17.000000 neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2701 2024-05-22 00:17:25.000000 neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.917605 neurocaps-0.9.1/neurocaps/analysis/
--rw-rw-rw-   0        0        0      143 2024-05-14 02:35:32.000000 neurocaps-0.9.1/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    60421 2024-05-23 03:18:30.000000 neurocaps-0.9.1/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4811 2024-05-14 02:35:32.000000 neurocaps-0.9.1/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1598 2024-05-14 02:35:32.000000 neurocaps-0.9.1/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.919922 neurocaps-0.9.1/neurocaps/extraction/
--rw-rw-rw-   0        0        0       89 2024-04-28 16:38:21.000000 neurocaps-0.9.1/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    30304 2024-05-23 03:16:17.000000 neurocaps-0.9.1/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.927775 neurocaps-0.9.1/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    15499 2024-05-23 03:23:29.000000 neurocaps-0.9.1/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-23 03:23:29.000000 neurocaps-0.9.1/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 03:23:29.000000 neurocaps-0.9.1/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-05-23 03:23:29.000000 neurocaps-0.9.1/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 03:23:29.000000 neurocaps-0.9.1/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1491 2024-05-23 03:18:30.000000 neurocaps-0.9.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 03:23:29.929987 neurocaps-0.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 03:23:29.925776 neurocaps-0.9.1/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.1/tests/test_CAP.py
--rw-rw-rw-   0        0        0     3767 2024-05-09 19:38:42.000000 neurocaps-0.9.1/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.1/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.1/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.1/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.144962 neurocaps-0.9.2/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.2/LICENSE.md
+-rw-rw-rw-   0        0        0    16232 2024-05-25 00:49:59.134579 neurocaps-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14914 2024-05-24 23:48:48.000000 neurocaps-0.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.038452 neurocaps-0.9.2/neurocaps/
+-rw-rw-rw-   0        0        0       78 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.095996 neurocaps-0.9.2/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      369 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.102977 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2591 2024-05-09 19:38:42.000000 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      186 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.114978 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2863 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2701 2024-05-22 00:17:25.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.118327 neurocaps-0.9.2/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      143 2024-05-14 02:35:32.000000 neurocaps-0.9.2/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    68833 2024-05-24 23:48:48.000000 neurocaps-0.9.2/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4811 2024-05-14 02:35:32.000000 neurocaps-0.9.2/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1598 2024-05-14 02:35:32.000000 neurocaps-0.9.2/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.128526 neurocaps-0.9.2/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       89 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    30437 2024-05-24 23:48:48.000000 neurocaps-0.9.2/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.134579 neurocaps-0.9.2/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    16232 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1491 2024-05-25 00:49:27.000000 neurocaps-0.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 00:49:59.145975 neurocaps-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.134579 neurocaps-0.9.2/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.2/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     3767 2024-05-09 19:38:42.000000 neurocaps-0.9.2/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.2/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.2/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.2/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.1/LICENSE.md` & `neurocaps-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/PKG-INFO` & `neurocaps-0.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: neurocaps
-Version: 0.9.1
-Summary: Co-activation patterns Python package
-Author-email: Donisha Smith <donishasmith@outlook.com>
-Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
-Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: kneed
-Requires-Dist: nibabel
-Requires-Dist: nilearn==0.10.2
-Requires-Dist: surfplot
-Requires-Dist: neuromaps
-Requires-Dist: pybids; platform_system != "Windows"
-
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
 **Still in beta but stable.**
 
 # Installation
 
@@ -98,16 +65,18 @@
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
 - Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
 
 **Main features for `CAP` includes:**
 
 - Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
 - Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
 - Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
 different CAPs across the entire run.
 
 **Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
@@ -192,21 +161,28 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
+# Create surface plots of CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
+```python
+# Create correlation matrix
+cap_analysis.caps2corr(annot=True)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
```

### Comparing `neurocaps-0.9.1/README.md` & `neurocaps-0.9.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: neurocaps
+Version: 0.9.2
+Summary: Co-activation patterns Python package
+Author-email: Donisha Smith <donishasmith@outlook.com>
+Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: kneed
+Requires-Dist: nibabel
+Requires-Dist: nilearn==0.10.2
+Requires-Dist: surfplot
+Requires-Dist: neuromaps
+Requires-Dist: pybids; platform_system != "Windows"
+
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
 **Still in beta but stable.**
 
 # Installation
 
@@ -65,16 +98,18 @@
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
 - Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
 
 **Main features for `CAP` includes:**
 
 - Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
 - Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
 - Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
 different CAPs across the entire run.
 
 **Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
@@ -159,21 +194,28 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
+# Create surface plots of CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
+```python
+# Create correlation matrix
+cap_analysis.caps2corr(annot=True)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
```

### Comparing `neurocaps-0.9.1/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.2/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/analysis/cap.py` & `neurocaps-0.9.2/neurocaps/analysis/cap.py`

 * *Files 13% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         self._optimal_n_clusters = {}
         self._kmeans = {}
 
         for group in self._groups.keys():
             self._silhouette_scores[group] = {}
             for n_cluster in self._n_clusters:
                 self._kmeans[group] = KMeans(n_clusters=n_cluster, random_state=random_state, init=init, n_init=n_init, max_iter=max_iter, tol=tol, algorithm=algorithm).fit(self._concatenated_timeseries[group])
-                cluster_labels = self._kmeans[group].predict(self._concatenated_timeseries[group])
+                cluster_labels = self._kmeans[group].labels_
                 self._silhouette_scores[group].update({n_cluster: silhouette_score(self._concatenated_timeseries[group], cluster_labels)})
             self._optimal_n_clusters[group] = max(self._silhouette_scores[group], key=self._silhouette_scores[group].get)
             if self._optimal_n_clusters[group] != self._n_clusters[-1]:
                 self._kmeans[group] = KMeans(n_clusters=self._optimal_n_clusters[group], random_state=random_state, init=init, n_init=n_init, max_iter=max_iter, tol=tol, algorithm=algorithm).fit(self._concatenated_timeseries[group]) 
             print(f"Optimal cluster size for {group} is {self._optimal_n_clusters[group]}.")
         
     
@@ -278,21 +278,55 @@
             Options are "regions" or "nodes".
         task_title: str, default=None
             Serves as the title of each plot as well as the name of the saved file if output_dir is given.
         show_figs: bool, default=True
             Display figures or not to display figures.
         subplots: bool, default=True
             Produce subplots for outer product plots.
-        kwargs: dict
-            Keyword arguments used when saving figures. Valid keywords include "dpi", "format", "figsize", "fontsize", "hspace", "wspace", "xticklabels_size", "yticklabels_size", "shrink", "nrow", "ncol", "suptitle_fontsize", "tight_layout", "rect", "sharey", "xlabel_rotation", "ylabel_rotation", "annot". 
-            If `output_dir` is not None and no inputs for dpi and format are given, dpi defaults to 300 and format defaults to "png". If no keywords, "figsize" defaults to (8,6), "fontsize", which adjusts the title size of the individual plots or subplots, defaults to 14, "hspace", which adjusts spacing for subplots, defaults to 0.4, 
-            "wspace", which adjusts spacing between subplots, defaults to 0.4, "xticklabels_size" defaults to 8, "yticklabels_size" defaults to 8, shrink, which adjusts the cbar size, defaults to 0.8, "nrow", which is the number of rows for subplot and varies, and "ncol", which is the number of columns for subplot, default varies but max is 5, "suptitle_fontsize", 
-            size of the main title when subplot is True, defaults to 0.7, "tight_layout", use tight layout for subplot, defaults to True, "rect", input for the `rect` parameter in tight layout when subplots is True to fix whitespace issues, default is [0, 0.03, 1, 0.95], "sharey", which shares y axis labela for subplots, defaults to True, 
-            "xlabel_rotation", which rotates the labels on the x-axis, defaults to 0, "ylabel_rotation", which rotates the labels on the y-axis, defaults to 0, "annot", which adds values to cells on the outer product heatmap at the region level only, defaults to False, "linewidths", which specifies the padding between each cell, defaults to 0,
-            and "cmap", which specifies the color pattern of the cells in the plot, defaults to "coolwarm".
+        **kwargs: dict
+            Keyword arguments used when saving figures. Valid keywords include:
+
+            - "dpi": int, default=300
+                Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
+            - "figsize": tuple, default=(8, 6)
+                Size of the figure in inches.
+            - "fontsize": int, default=14
+                Font size for the title of individual plots or subplots.
+            - "hspace": float, default=0.4
+                Height space between subplots.
+            - "wspace": float, default=0.4
+                Width space between subplots.
+            - "xticklabels_size": int, default=8
+                Font size for x-axis tick labels.
+            - "yticklabels_size": int, default=8
+                Font size for y-axis tick labels.
+            - "shrink": float, default=0.8
+                Fraction by which to shrink the colorbar.
+            - "nrow": int, varies;
+                Number of rows for subplots. Default varies.
+            - "ncol": int, default varies (max 5)
+                Number of columns for subplots. Default varies but the maximum is 5.
+            - "suptitle_fontsize": float, default=0.7
+                Font size for the main title when subplot is True.
+            - "tight_layout": bool, default=True
+                Use tight layout for subplots.
+            - "rect": list, default=[0, 0.03, 1, 0.95]
+                Rectangle parameter for tight layout when subplots are True to fix whitespace issues.
+            - "sharey": bool, default=True
+                Share y-axis labels for subplots.
+            - "xlabel_rotation": int, default=0
+                Rotation angle for x-axis labels.
+            - "ylabel_rotation": int, default=0
+                Rotation angle for y-axis labels.
+            - "annot": bool, default=False
+                Add values to cells on the outer product heatmap at the region level only.
+            - "linewidths": float, default=0
+                Padding between each cell in the plot.
+            - "cmap": str, default="coolwarm"
+                Color map for the cells in the plot.
     
          Notes
         -----
         If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
         the zero index should correspond the first id that is not zero.
 
         Custom Key Structure:
@@ -341,15 +375,14 @@
         if not any(["regions" in visual_scope, "nodes" in visual_scope]):
             raise ValueError("Valid inputs for `visual_scope` are 'regions' and 'nodes'.")
 
         if "regions" in visual_scope: self._create_regions()
 
         # Create plot dictionary
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
-                        format = kwargs["format"] if kwargs and "format" in kwargs.keys() else "png",
                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6),
                         fontsize = kwargs["fontsize"] if kwargs and "fontsize" in kwargs.keys() else 14,
                         hspace = kwargs["hspace"] if kwargs and "hspace" in kwargs.keys() else 0.2,
                         wspace = kwargs["wspace"] if kwargs and "wspace" in kwargs.keys() else 0.2,
                         xticklabels_size = kwargs["xticklabels_size"] if kwargs and "xticklabels_size" in kwargs.keys() else 8,
                         yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
                         shrink = kwargs["shrink"] if kwargs and "shrink" in kwargs.keys() else 0.8,
@@ -538,24 +571,24 @@
                 # Modify label sizes
                 display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
                 display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
                 # Save individual plots
                 if output_dir:
                     partial_filename = f"{group}_{cap}_{task_title}" if task_title else f"{group}_{cap}"
-                    full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
+                    full_filename = f"{partial_filename}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.png"
                     display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
         
         # Remove subplots with no data
         if subplots: [fig.delaxes(ax) for ax in axes.flatten() if not ax.has_data()]
 
         # Save subplot
         if subplots and output_dir: 
             partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
+            full_filename = f"{partial_filename}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.png"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
         
         # Display figures
         if not show_figs: plt.close()
 
     def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
         import matplotlib.pyplot as plt, os, pandas as pd
@@ -604,15 +637,15 @@
         # Set plot name
         plot_title = f"{group} CAPS {task_title}" if task_title else f"{group} CAPS" 
         display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
         # Save plots
         if output_dir:
             partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_heatmap-nodes.{plot_dict['format']}"
+            full_filename = f"{partial_filename}_heatmap-regions.png" if scope == "regions" else f"{partial_filename}_heatmap-nodes.png"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
    
         # Display figures
         if not show_figs: plt.close()
 
     def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, output_dir: str=None, file_name: str=None) -> dict:
         """Get CAP metrics
@@ -788,15 +821,97 @@
         if output_dir:
             for metric in df_dict.keys():
                 filename = file_name + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
                 df_dict[f"{metric}"].to_csv(path_or_buf=os.path.join(output_dir,filename + ".csv"), sep=",", index=False)
 
         if return_df:
             return df_dict
+
+    def caps2corr(self, output_dir: str=None, show_figs: bool=True, **kwargs):
+        """ Generate Correlation Matrix
+
+        This function produces the correlation matrix of all CAPs. If groups were given when the CAP class was initialized, a correlation matrix will be generated for each group. 
+
+        Parameters
+        ----------
+        output_dir: str, default=None
+            Directory to save plots in. If None, plots will not be saved.
+        show_figs: bool, default=True
+            Display figures or not to display figures.
+        **kwargs: dict
+            Keyword arguments used when saving figures. Valid keywords include:
+
+            - "dpi": int, default=300
+                Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
+            - "figsize": tuple, default=(8, 6)
+                Size of the figure in inches.
+            - "fontsize": int, default=14
+                Font size for the title of individual plots or subplots.
+            - "xticklabels_size": int, default=8
+                Font size for x-axis tick labels.
+            - "yticklabels_size": int, default=8
+                Font size for y-axis tick labels.
+            - "shrink": float, default=0.8
+                Fraction by which to shrink the colorbar.
+            - "xlabel_rotation": int, default=0
+                Rotation angle for x-axis labels.
+            - "ylabel_rotation": int, default=0
+                Rotation angle for y-axis labels.
+            - "annot": bool, default=False
+                Add values to each cell.
+            - "linewidths": float, default=0
+                Padding between each cell in the plot.
+            - "cmap": str, default="coolwarm"
+                Color map for the cells in the plot.
+        """
+        import matplotlib.pyplot as plt, os, pandas as pd
+        from seaborn import heatmap
         
+        # Initialize new grid
+        
+        # Create plot dictionary
+        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
+                        figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6),
+                        fontsize = kwargs["fontsize"] if kwargs and "fontsize" in kwargs.keys() else 14,
+                        xticklabels_size = kwargs["xticklabels_size"] if kwargs and "xticklabels_size" in kwargs.keys() else 8,
+                        yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
+                        shrink = kwargs["shrink"] if kwargs and "shrink" in kwargs.keys() else 0.8,
+                        xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
+                        ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
+                        annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
+                        linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
+                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
+                        )
+        
+        if kwargs:
+            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
+            if len(invalid_kwargs.keys()) > 0:
+                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
+
+        for group in self.caps.keys():
+            # Refresh grid for each iteration
+            plt.figure(figsize=plot_dict["figsize"])
+
+            df = pd.DataFrame(self.caps[group])
+            display = heatmap(df.corr(), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], 
+                              cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"]) 
+            # Modify label sizes
+            display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
+            display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
+            # Set plot name
+            plot_title = f"{group} - CAPS Correlation Matrix" 
+            display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
+
+            # Display figures
+            if not show_figs: plt.close()
+            # Save figure
+            if output_dir:
+                full_filename = f"{group.replace(' ', '_')}_correlation_matrix.png"
+                display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
+
     def caps2surf(self, output_dir: str=None, show_figs: bool = True, fwhm: float=None, 
                   fslr_density: str="32k", method: str="linear", return_stat_map: bool = False, **kwargs):
         """Project CAPs back onto atlas used for spatial dimensionality reduction for visualization
         
         Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
         This function uses surfplot for surface plotting.
 
@@ -812,19 +927,61 @@
             Density of the fslr surface when converting from mni 152 space to fslr surface. Options are 
             "32k" or "164k".
         method: str, default="linear"
             Interpolation method to use when converting from mni152 space to fslr surface. Options are "linear"
             or "nearest".
         return_stat_map: bool, default=FAlse
             Returns the atlas as a stat map.
-        **kwargs: dict
-            Additional parameters to pass to modify certain plot parameters. Options include "dpi", defaults to 300, "title_pad", defaults to -3,
-            "cmap", defaults to "cold_hot", "cbar_location", defaults to "bottom", "cbar_draw_border", defaults to False, "cbar_aspect", defaults to 10, "cbar_shrink", defaults 
-            to 0.2, "cbar_decimals", defaults to 0, and "cbar_pad", defaults to 0.
-            
+        **kwargs : dict
+            Additional parameters to pass to modify certain plot parameters. Options include:
+
+            - "dpi": int, default=300
+                Dots per inch for the plot.
+            - "title_pad": int, default=-3
+                Padding for the plot title.
+            - "cmap": str, default="cold_hot"
+                Colormap to be used for the plot.
+            - "cbar_location": str, default="bottom"
+                Location of the colorbar.
+            - "cbar_draw_border": bool, default=False
+                Whether to draw a border around the colorbar.
+            - "cbar_aspect": int, default=20
+                Aspect ratio of the colorbar.
+            - "cbar_shrink": float, default=0.2
+                Fraction by which to shrink the colorbar.
+            - "cbar_decimals": int, default=2
+                Number of decimals for colorbar values.
+            - "cbar_pad": float, default=0
+                Padding between the colorbars.
+            - "cbar_fraction": float, default=0.05
+                Fraction of the original axes to use for the colorbar.
+            - "cbar_n_ticks": int, default=3
+                Number of ticks on the colorbar.
+            - "cbar_fontsize": int, default=10
+                Font size for the colorbar labels.
+            - "cbar_alpha": float, default=1
+                Transparency level of the colorbar.
+            - "size": tuple, default=(500, 400)
+                Size of the plot in pixels.
+            - "layout": str, default="grid";
+                Layout of the plot.
+            - "zoom": float, default=1.5
+                Zoom level for the plot.
+            - "views": list of str, default=["lateral", "medial"]
+                Views to be displayed in the plot.
+            - "brightness": float, default=0.5
+                Brightness level of the plot.
+            - "figsize": tuple or None, default=None
+                Size of the figure.
+            - "scale": tuple, default=(2, 2)
+                Scale factors for the plot.
+
+            Please refer to surfplot's documentation for specifics: 
+            https://surfplot.readthedocs.io/en/latest/generated/surfplot.plotting.Plot.html#surfplot.plotting.Plot.
+
         Returns
         -------
         Nifti Stat map
 
         Notes
         -----
         Assumes that atlas background label is zero and atlas is in MNI space. Also assumes that the indices from the cluster centroids are related
@@ -843,18 +1000,30 @@
         from surfplot import Plot
 
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
                          title_pad = kwargs["title_pad"] if kwargs and "title_pad" in kwargs.keys() else -3,
                          cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "cold_hot",
                          cbar_location = kwargs["cbar_location"] if kwargs and "cbar_location" in kwargs.keys() else "bottom",
                          cbar_draw_border = kwargs["cbar_draw_border"] if kwargs and "cbar_draw_border" in kwargs.keys() else False,
-                         cbar_aspect = kwargs["cbar_aspect"] if kwargs and "cbar_aspect" in kwargs.keys() else 10,
+                         cbar_aspect = kwargs["cbar_aspect"] if kwargs and "cbar_aspect" in kwargs.keys() else 20,
                          cbar_shrink = kwargs["cbar_shrink"] if kwargs and "cbar_shrink" in kwargs.keys() else 0.2,
-                         cbar_decimals = kwargs["cbar_decimals"] if kwargs and "cbar_decimals" in kwargs.keys() else 0,
-                         cbar_pad = kwargs["cbar_pad"] if kwargs and "cbar_pad" in kwargs.keys() else 0)
+                         cbar_decimals = kwargs["cbar_decimals"] if kwargs and "cbar_decimals" in kwargs.keys() else 2,
+                         cbar_pad = kwargs["cbar_pad"] if kwargs and "cbar_pad" in kwargs.keys() else 0,
+                         cbar_fraction = kwargs["cbar_fraction"] if kwargs and "cbar_fraction" in kwargs.keys() else 0.05,
+                         cbar_n_ticks = kwargs["cbar_n_ticks"] if kwargs and "cbar_n_ticks" in kwargs.keys() else 3,
+                         cbar_fontsize = kwargs["cbar_fontsize"] if kwargs and "cbar_fontsize" in kwargs.keys() else 10,
+                         cbar_alpha = kwargs["cbar_alpha"] if kwargs and "cbar_alpha" in kwargs.keys() else 1,
+                         size = kwargs["size"] if kwargs and "size" in kwargs.keys() else (500,400),
+                         layout = kwargs["layout"] if kwargs and "layout" in kwargs.keys() else "grid",
+                         zoom = kwargs["zoom"] if kwargs and "zoom" in kwargs.keys() else 1.5,
+                         views = kwargs["views"] if kwargs and "views" in kwargs.keys() else ["lateral", "medial"],
+                         brightness = kwargs["brightness"] if kwargs and "brightness" in kwargs.keys() else 0.5,
+                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else None,
+                         scale = kwargs["scale"] if kwargs and "scale" in kwargs.keys() else (2,2),
+                         )
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
                 print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
 
         for group in self._caps.keys():
@@ -876,35 +1045,37 @@
                 surfaces = fetch_fslr()
                 lh, rh = surfaces['inflated']
                 lh = str(lh) if not isinstance(lh, str) else lh
                 rh = str(rh) if not isinstance(rh, str) else rh
                 sulc_lh, sulc_rh = surfaces['sulc']
                 sulc_lh = str(sulc_lh) if not isinstance(sulc_lh, str) else sulc_lh
                 sulc_rh = str(sulc_rh) if not isinstance(sulc_rh, str) else sulc_rh
-                p = Plot(lh, rh)
+                p = Plot(lh, rh, size=plot_dict["size"], layout=plot_dict["layout"], zoom=plot_dict["zoom"],
+                         views=plot_dict["views"], brightness=plot_dict["brightness"])
 
                 # Add base layer
                 p.add_layer({"left": sulc_lh, "right": sulc_rh}, cmap="binary_r", cbar=False)
 
                 plot_min = -1 if round(atlas_fdata.min()) == 0 else round(atlas_fdata.min())
                 plot_max = 1 if round(atlas_fdata.max()) == 0 else round(atlas_fdata.max())
 
                 # Add stat map layer
                 p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=_cmap_d[plot_dict["cmap"]], 
-                            color_range=(plot_min,plot_max))
+                            alpha=plot_dict["cbar_alpha"], color_range=(plot_min,plot_max))
 
                 # Color bar
                 kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
-                        decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"])
-                fig = p.build(cbar_kws=kws)
+                        decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"], fraction=plot_dict["cbar_fraction"], n_ticks=plot_dict["cbar_n_ticks"], 
+                        fontsize=plot_dict["cbar_fontsize"])
+                fig = p.build(cbar_kws=kws, figsize=plot_dict["figsize"], scale=plot_dict["scale"])
                 fig_name = f"{group} - {cap}"
                 fig.axes[0].set_title(fig_name, pad=plot_dict["title_pad"])      
                 
                 if show_figs:
                     fig.show()
                 
                 if output_dir:
-                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}"
+                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}.png"
                     fig.savefig(os.path.join(output_dir, save_name), dpi=plot_dict["dpi"])
 
         if return_stat_map:
             return stat_map
```

### Comparing `neurocaps-0.9.1/neurocaps/analysis/merge.py` & `neurocaps-0.9.2/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/analysis/standardize.py` & `neurocaps-0.9.2/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.2/neurocaps/extraction/timeseriesextractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         use_confounds : bool, default=True
             To use confounds when extracting timeseries.
         confound_names : List[str], default=None
             Names of confounds to use in confound files. If None, default confounds are used.
         fwhm : float, default=None
             Parameter for spatial smoothing.
         fd_threshold : float, default=None
-            Threshold criteria to remove volume after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
+            Threshold criteria to remove frames after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
             in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
         n_acompcor_separate : int, default = None
             The number of seperate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
             then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
             used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
             masks. To use the acompcor components derived from the combined masks (WM & CSF) leave this parameter as 'None' and list the specific acompcors of interest in the 
             `confound_names` parameter.
@@ -329,17 +329,22 @@
             for valid regions names.
         show_figs: bool, defaults=True
             Whether to show figires or not to show figures
         output_dir : str
             Directory to save the file to.
         file_name : str
             Name of the file with the extension to signify the file type.
-        kwargs: dict
-            Keyword arguments used when saving figures. Valid keywords include "dpi" and "figsize". If output_dir is not None and no inputs for dpi and format are given,
-            dpi defaults to 300. If "figsize" has no input, figure sizes defaults to (11,5).
+        **kwargs: dict
+            Keyword arguments used when saving figures. Valid keywords include:
+        
+            - "dpi": int, default=300
+                Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
+            - "figsize": tuple, default=(11, 5)
+                Size of the figure in inches. Default is (11, 5) if "figsize" is not specified.
+
 
         Raises
         ------
         ValueError
             If both `roi_indx` and `region` are specified.
         AssertionError
             If `file_name` does not contain an extension to signify the file type.
```

### Comparing `neurocaps-0.9.1/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.2/neurocaps.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.1
+Version: 0.9.2
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -98,16 +98,18 @@
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
 - Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
 
 **Main features for `CAP` includes:**
 
 - Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
 - Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
 - Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
 different CAPs across the entire run.
 
 **Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
@@ -192,21 +194,28 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
+# Create surface plots of CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
+```python
+# Create correlation matrix
+cap_analysis.caps2corr(annot=True)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+
 # Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
 [^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
```

### Comparing `neurocaps-0.9.1/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.2/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/pyproject.toml` & `neurocaps-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e31 220d  rsion = "0.9.1".
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e32 220d  rsion = "0.9.2".
 00000090: 0a61 7574 686f 7273 203d 205b 7b6e 616d  .authors = [{nam
 000000a0: 6520 3d20 2244 6f6e 6973 6861 2053 6d69  e = "Donisha Smi
 000000b0: 7468 222c 2065 6d61 696c 203d 2022 646f  th", email = "do
 000000c0: 6e69 7368 6173 6d69 7468 406f 7574 6c6f  nishasmith@outlo
 000000d0: 6f6b 2e63 6f6d 227d 5d0d 0a64 6573 6372  ok.com"}]..descr
 000000e0: 6970 7469 6f6e 203d 2022 436f 2d61 6374  iption = "Co-act
 000000f0: 6976 6174 696f 6e20 7061 7474 6572 6e73  ivation patterns
```

### Comparing `neurocaps-0.9.1/tests/test_CAP.py` & `neurocaps-0.9.2/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.2/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.2/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/tests/test_merge_dicts.py` & `neurocaps-0.9.2/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1/tests/test_standardize.py` & `neurocaps-0.9.2/tests/test_standardize.py`

 * *Files identical despite different names*

