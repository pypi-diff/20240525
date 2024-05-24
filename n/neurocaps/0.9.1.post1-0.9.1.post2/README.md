# Comparing `tmp/neurocaps-0.9.1.post1.tar.gz` & `tmp/neurocaps-0.9.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.1.post1.tar", last modified: Thu May 23 20:00:47 2024, max compression
+gzip compressed data, was "neurocaps-0.9.1.post2.tar", last modified: Fri May 24 22:47:16 2024, max compression
```

## Comparing `neurocaps-0.9.1.post1.tar` & `neurocaps-0.9.1.post2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.952728 neurocaps-0.9.1.post1/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post1/LICENSE.md
--rw-rw-rw-   0        0        0    15505 2024-05-23 20:00:47.952728 neurocaps-0.9.1.post1/PKG-INFO
--rw-rw-rw-   0        0        0    14181 2024-05-23 03:16:14.000000 neurocaps-0.9.1.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.910917 neurocaps-0.9.1.post1/neurocaps/
--rw-rw-rw-   0        0        0       78 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post1/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.931728 neurocaps-0.9.1.post1/neurocaps/_utils/
--rw-rw-rw-   0        0        0      369 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post1/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.931728 neurocaps-0.9.1.post1/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2591 2024-05-09 19:38:42.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      186 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.938749 neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2863 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2701 2024-05-22 00:17:25.000000 neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.945649 neurocaps-0.9.1.post1/neurocaps/analysis/
--rw-rw-rw-   0        0        0      143 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post1/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    64045 2024-05-23 19:59:12.000000 neurocaps-0.9.1.post1/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4811 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post1/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1598 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post1/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.945649 neurocaps-0.9.1.post1/neurocaps/extraction/
--rw-rw-rw-   0        0        0       89 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post1/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    30437 2024-05-23 19:59:12.000000 neurocaps-0.9.1.post1/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.952728 neurocaps-0.9.1.post1/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    15505 2024-05-23 20:00:47.000000 neurocaps-0.9.1.post1/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-23 20:00:47.000000 neurocaps-0.9.1.post1/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 20:00:47.000000 neurocaps-0.9.1.post1/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-05-23 20:00:47.000000 neurocaps-0.9.1.post1/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 20:00:47.000000 neurocaps-0.9.1.post1/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1496 2024-05-23 19:59:12.000000 neurocaps-0.9.1.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 20:00:47.952728 neurocaps-0.9.1.post1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 20:00:47.952728 neurocaps-0.9.1.post1/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.1.post1/tests/test_CAP.py
--rw-rw-rw-   0        0        0     3767 2024-05-09 19:38:42.000000 neurocaps-0.9.1.post1/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.1.post1/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.1.post1/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post1/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.332066 neurocaps-0.9.1.post2/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post2/LICENSE.md
+-rw-rw-rw-   0        0        0    15667 2024-05-24 22:47:16.327084 neurocaps-0.9.1.post2/PKG-INFO
+-rw-rw-rw-   0        0        0    14343 2024-05-24 22:46:10.000000 neurocaps-0.9.1.post2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.156637 neurocaps-0.9.1.post2/neurocaps/
+-rw-rw-rw-   0        0        0       78 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post2/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.220326 neurocaps-0.9.1.post2/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      369 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post2/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.232096 neurocaps-0.9.1.post2/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2591 2024-05-09 19:38:42.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      186 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.255422 neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2863 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-23 03:16:17.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2701 2024-05-22 00:17:25.000000 neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.272854 neurocaps-0.9.1.post2/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      143 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post2/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    68833 2024-05-24 22:32:17.000000 neurocaps-0.9.1.post2/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4811 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post2/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1598 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post2/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.301153 neurocaps-0.9.1.post2/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       89 2024-04-28 16:38:21.000000 neurocaps-0.9.1.post2/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    30437 2024-05-24 22:43:24.000000 neurocaps-0.9.1.post2/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.323929 neurocaps-0.9.1.post2/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    15667 2024-05-24 22:47:16.000000 neurocaps-0.9.1.post2/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-24 22:47:16.000000 neurocaps-0.9.1.post2/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 22:47:16.000000 neurocaps-0.9.1.post2/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-05-24 22:47:16.000000 neurocaps-0.9.1.post2/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 22:47:16.000000 neurocaps-0.9.1.post2/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1496 2024-05-24 22:41:53.000000 neurocaps-0.9.1.post2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 22:47:16.333222 neurocaps-0.9.1.post2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 22:47:16.319075 neurocaps-0.9.1.post2/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.1.post2/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     3767 2024-05-09 19:38:42.000000 neurocaps-0.9.1.post2/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.1.post2/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.1.post2/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.1.post2/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.1.post1/LICENSE.md` & `neurocaps-0.9.1.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/PKG-INFO` & `neurocaps-0.9.1.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.1.post1
+Version: 0.9.1.post2
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -197,14 +197,19 @@
 
 ```python
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
+```python
+cap_analysis.caps2corr(annot=True)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.9.1.post1/README.md` & `neurocaps-0.9.1.post2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,19 @@
 
 ```python
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
+```python
+cap_analysis.caps2corr(annot=True)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.9.1.post1/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.1.post2/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.1.post2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/analysis/cap.py` & `neurocaps-0.9.1.post2/neurocaps/analysis/cap.py`

 * *Files 2% similar despite different names*

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
         
     
@@ -821,15 +821,97 @@
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
```

### Comparing `neurocaps-0.9.1.post1/neurocaps/analysis/merge.py` & `neurocaps-0.9.1.post2/neurocaps/analysis/merge.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/analysis/standardize.py` & `neurocaps-0.9.1.post2/neurocaps/analysis/standardize.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.1.post2/neurocaps/extraction/timeseriesextractor.py`

 * *Files 0% similar despite different names*

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
```

### Comparing `neurocaps-0.9.1.post1/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.1.post2/neurocaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.1.post1
+Version: 0.9.1.post2
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -197,14 +197,19 @@
 
 ```python
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
+```python
+cap_analysis.caps2corr(annot=True)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
 
 
 # References
```

### Comparing `neurocaps-0.9.1.post1/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.1.post2/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/pyproject.toml` & `neurocaps-0.9.1.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
 00000080: 7273 696f 6e20 3d20 2230 2e39 2e31 706f  rsion = "0.9.1po
-00000090: 7374 3122 0d0a 6175 7468 6f72 7320 3d20  st1"..authors = 
+00000090: 7374 3222 0d0a 6175 7468 6f72 7320 3d20  st2"..authors = 
 000000a0: 5b7b 6e61 6d65 203d 2022 446f 6e69 7368  [{name = "Donish
 000000b0: 6120 536d 6974 6822 2c20 656d 6169 6c20  a Smith", email 
 000000c0: 3d20 2264 6f6e 6973 6861 736d 6974 6840  = "donishasmith@
 000000d0: 6f75 746c 6f6f 6b2e 636f 6d22 7d5d 0d0a  outlook.com"}]..
 000000e0: 6465 7363 7269 7074 696f 6e20 3d20 2243  description = "C
 000000f0: 6f2d 6163 7469 7661 7469 6f6e 2070 6174  o-activation pat
 00000100: 7465 726e 7320 5079 7468 6f6e 2070 6163  terns Python pac
```

### Comparing `neurocaps-0.9.1.post1/tests/test_CAP.py` & `neurocaps-0.9.1.post2/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.1.post2/tests/test_TimeseriesExtractor.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.1.post2/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/tests/test_merge_dicts.py` & `neurocaps-0.9.1.post2/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.1.post1/tests/test_standardize.py` & `neurocaps-0.9.1.post2/tests/test_standardize.py`

 * *Files identical despite different names*

