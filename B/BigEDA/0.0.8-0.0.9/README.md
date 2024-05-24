# Comparing `tmp/bigeda-0.0.8.tar.gz` & `tmp/bigeda-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeda-0.0.8.tar", last modified: Fri May 17 15:05:19 2024, max compression
+gzip compressed data, was "bigeda-0.0.9.tar", last modified: Sat May 18 09:05:50 2024, max compression
```

## Comparing `bigeda-0.0.8.tar` & `bigeda-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:05:19.134920 bigeda-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-05-17 15:05:19.092647 bigeda-0.0.8/BigEDA/
--rw-rw-rw-   0        0        0      783 2024-03-31 16:22:20.000000 bigeda-0.0.8/BigEDA/__init__.py
--rw-rw-rw-   0        0        0    26812 2024-05-17 15:04:09.000000 bigeda-0.0.8/BigEDA/descriptive.py
--rw-rw-rw-   0        0        0    78541 2024-05-13 23:16:09.000000 bigeda-0.0.8/BigEDA/plots.py
--rw-rw-rw-   0        0        0    11707 2024-04-14 01:24:57.000000 bigeda-0.0.8/BigEDA/preprocessing.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:05:19.131989 bigeda-0.0.8/BigEDA.egg-info/
--rw-rw-rw-   0        0        0      870 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 15:05:18.000000 bigeda-0.0.8/BigEDA.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 bigeda-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      870 2024-05-17 15:05:19.133916 bigeda-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-12-09 16:15:51.000000 bigeda-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 15:05:19.134920 bigeda-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      838 2024-05-17 15:04:39.000000 bigeda-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:05:50.387570 bigeda-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-05-18 09:05:50.342742 bigeda-0.0.9/BigEDA/
+-rw-rw-rw-   0        0        0      783 2024-03-31 16:22:20.000000 bigeda-0.0.9/BigEDA/__init__.py
+-rw-rw-rw-   0        0        0    26812 2024-05-17 15:04:09.000000 bigeda-0.0.9/BigEDA/descriptive.py
+-rw-rw-rw-   0        0        0    78777 2024-05-18 09:03:33.000000 bigeda-0.0.9/BigEDA/plots.py
+-rw-rw-rw-   0        0        0    11707 2024-04-14 01:24:57.000000 bigeda-0.0.9/BigEDA/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-18 09:05:50.387166 bigeda-0.0.9/BigEDA.egg-info/
+-rw-rw-rw-   0        0        0     1043 2024-05-18 09:05:50.000000 bigeda-0.0.9/BigEDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-05-18 09:05:50.000000 bigeda-0.0.9/BigEDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 09:05:50.000000 bigeda-0.0.9/BigEDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-05-18 09:05:50.000000 bigeda-0.0.9/BigEDA.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 09:05:50.000000 bigeda-0.0.9/BigEDA.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 bigeda-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1043 2024-05-18 09:05:50.387570 bigeda-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-12-09 16:15:51.000000 bigeda-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 09:05:50.387570 bigeda-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      944 2024-05-18 09:05:43.000000 bigeda-0.0.9/setup.py
```

### Comparing `bigeda-0.0.8/BigEDA/__init__.py` & `bigeda-0.0.9/BigEDA/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.8/BigEDA/descriptive.py` & `bigeda-0.0.9/BigEDA/descriptive.py`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.8/BigEDA/plots.py` & `bigeda-0.0.9/BigEDA/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,20 +180,20 @@
     plt.show()  
 
 ######################################################################################################################
     
 def boxplot(X, color, figsize=(9,5), n_xticks=15, x_rotation=0, statistics=None, 
             random=False, n=None, fraction=None, seed=123, save=False, file_name=None,
             style='whitegrid', lines_width=0.55, bbox_to_anchor=(0.5,-0.5), legend_size=10,
-              color_stats=None) :
+            color_stats=None) :
 
     """
     Parameters (inputs)
     ----------
-    X: a pandas series or a numpy array (the variable).
+    X: a polars series (the variable).
     bins: number of intervals used to create the histogram (number of bars).
     color: name of the color to be use for the histogram bars.
     figsize: dimensions of the plot. Must be a pair of numbers (a,b), where a indicates the plot width, and b the length.
     rotation: a integer positive number. Indicates the rotation degree of the sticks from the axis.
     get_intervals:If True, the intervals used to create the histogram will be return. If False, not.
     sep: a parameter used for creating the sticks of the x-axis. We recommend using the default value.
    
@@ -522,24 +522,25 @@
     if save == True :         
         fig.savefig(file_name + '.jpg', format='jpg', dpi=500)
 
     plt.show()
 
 ######################################################################################################################
 
-def barplot(X, color, categories_order=None, figsize=(9,5), xticks_rotation=0, random=False, 
+def barplot(X, color, orientation='vertical', bar_width=0.5, order=None, figsize=(9,5), xticks_rotation=0, random=False, 
             n=None, fraction=None, seed=123, fontsize=10, y_up_limit=1, 
-            y_low_limit=0, xticks_fontsize=11, yticks_fontsize=11, xlabel_size=11, 
-            ylabel_size=11, ylabel='Relative Frequency', xlabel='',
-            title_size=14, title_weight='bold') :
+            y_low_limit=0, xticks_fontsize=11, yticks_fontsize=11, 
+            ylabel_size=11, ylabel='Relative Frequency', 
+            xlabel_size=11, xlabel='', 
+            title_size=14, title_weight='bold'):
 
     """
     Parameters (inputs)
     ----------
-    X: a pandas series or a numpy array (the variable).
+    X: a polars series.
     color: name of the color to be use for the histogram bars.
     categories_order: a list with X categories order as they will appear in the plot.
     figsize: dimensions of the plot. Must be a pair of numbers (a,b), where a indicates the plot width, and b the length.
     rotation: a integer positive number. Indicates the rotation degree of the sticks from the axis.
     sep: a parameter used for creating the sticks of the x-axis. We recommend using the default value.
    
     Returns (outputs)
@@ -556,29 +557,33 @@
 
     if isinstance(X, pl.Series):
         X = X.to_pandas()
 
     # Setting the figure size.
     fig, axs = plt.subplots(figsize=figsize)
 
-    # Computing the barplot.
-    value_counts = X.value_counts(normalize=True).reindex(categories_order)
-    ax = value_counts.plot(kind='bar', color=color)
+    X = X.drop_nulls().to_numpy()
+    unique_values, rel_freq = get_frequencies(X)
+    unique_values = [str(x) for x in unique_values] 
+    if orientation == 'vertical':
+        ax = sns.barplot(x=unique_values, y=rel_freq, color=color, width=bar_width, order=order)
+    elif orientation == 'horizontal':
+        ax = sns.barplot(x=rel_freq, y=unique_values, color=color, width=bar_width, order=order)
 
     ax.set_ylabel(ylabel, size=ylabel_size)
     ax.set_xlabel(xlabel, size=xlabel_size)
     plt.xticks(fontsize=xticks_fontsize, rotation=xticks_rotation)
     plt.yticks(fontsize=yticks_fontsize)
 
     # Setting the title of the plot.
     plt.title(label = 'Bar-plot' + '  ' + X.name, fontsize=title_size, weight=title_weight)
     ax.set_ylim(y_low_limit, y_up_limit)  
 
     # Add text annotations to each bar
-    for i, v in enumerate(value_counts):
+    for i, v in enumerate(rel_freq):
         plt.text(i, v, f"{v:.2f}", color='black', ha='center', va='bottom', fontsize=fontsize, fontweight='bold')
 
     plt.show()
 
 
 ######################################################################################################################
```

### Comparing `bigeda-0.0.8/BigEDA/preprocessing.py` & `bigeda-0.0.9/BigEDA/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.8/BigEDA.egg-info/PKG-INFO` & `bigeda-0.0.9/BigEDA.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: BigEDA
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.
 Home-page: https://github.com/FabioScielzoOrtiz/EDA_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: polars
+Requires-Dist: scipy
+Requires-Dist: itertools
+Requires-Dist: collections
+Requires-Dist: seaborn
+Requires-Dist: matplotlib
+Requires-Dist: random
 
 This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.
 
 We are currently working to develop the package.
 
 Usage:
```

### Comparing `bigeda-0.0.8/LICENSE` & `bigeda-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeda-0.0.8/PKG-INFO` & `bigeda-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: BigEDA
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is a package to carry out Exploratory Data Analysis, allowing to work with Big Data.
 Home-page: https://github.com/FabioScielzoOrtiz/EDA_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: polars
+Requires-Dist: scipy
+Requires-Dist: itertools
+Requires-Dist: collections
+Requires-Dist: seaborn
+Requires-Dist: matplotlib
+Requires-Dist: random
 
 This is a package to carry out Exploratory Data Analysis, allowing to work on Big Data.
 
 We are currently working to develop the package.
 
 Usage:
```

