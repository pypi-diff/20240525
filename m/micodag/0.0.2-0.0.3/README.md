# Comparing `tmp/micodag-0.0.2.tar.gz` & `tmp/micodag-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micodag-0.0.2.tar", last modified: Fri Nov 10 19:26:04 2023, max compression
+gzip compressed data, was "micodag-0.0.3.tar", last modified: Sat May 25 03:46:50 2024, max compression
```

## Comparing `micodag-0.0.2.tar` & `micodag-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-11-10 19:26:04.439665 micodag-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-11-10 19:01:55.000000 micodag-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2045 2023-11-10 19:26:04.439665 micodag-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-11-10 19:24:00.000000 micodag-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-11-10 19:26:04.433190 micodag-0.0.2/micodag/
--rw-rw-rw-   0        0        0       38 2023-11-10 19:01:55.000000 micodag-0.0.2/micodag/__init__.py
--rw-rw-rw-   0        0        0     6994 2023-11-10 19:01:55.000000 micodag-0.0.2/micodag/micpnid.py
-drwxrwxrwx   0        0        0        0 2023-11-10 19:26:04.438665 micodag-0.0.2/micodag.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-11-10 19:26:04.000000 micodag-0.0.2/micodag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-11-10 19:26:04.000000 micodag-0.0.2/micodag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-10 19:26:04.000000 micodag-0.0.2/micodag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-11-10 19:26:04.000000 micodag-0.0.2/micodag.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-11-10 19:26:04.000000 micodag-0.0.2/micodag.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-10 19:26:04.439665 micodag-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      965 2023-11-10 19:25:21.000000 micodag-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 03:46:50.790900 micodag-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-11-10 19:01:55.000000 micodag-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2045 2024-05-25 03:46:50.790900 micodag-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-11-10 19:24:00.000000 micodag-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 03:46:50.769633 micodag-0.0.3/micodag/
+-rw-rw-rw-   0        0        0       38 2023-11-10 19:01:55.000000 micodag-0.0.3/micodag/__init__.py
+-rw-rw-rw-   0        0        0     7056 2024-05-25 03:17:23.000000 micodag-0.0.3/micodag/micpnid.py
+drwxrwxrwx   0        0        0        0 2024-05-25 03:46:50.788898 micodag-0.0.3/micodag.egg-info/
+-rw-rw-rw-   0        0        0     2045 2024-05-25 03:46:50.000000 micodag-0.0.3/micodag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-25 03:46:50.000000 micodag-0.0.3/micodag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 03:46:50.000000 micodag-0.0.3/micodag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-25 03:46:50.000000 micodag-0.0.3/micodag.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-25 03:46:50.000000 micodag-0.0.3/micodag.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 03:46:50.790900 micodag-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      965 2024-05-25 03:27:53.000000 micodag-0.0.3/setup.py
```

### Comparing `micodag-0.0.2/LICENSE.txt` & `micodag-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `micodag-0.0.2/PKG-INFO` & `micodag-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micodag
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package of mixed integer convex programming for directed acyclic graphs.
 Author: Tong Xu
 Author-email: tongxu2027@u.northwestern.edu
 License: MIT
 Keywords: python,Bayesian network
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `micodag-0.0.2/README.md` & `micodag-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `micodag-0.0.2/micodag/micpnid.py` & `micodag-0.0.3/micodag/micpnid.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     ## Moral Graph
     G_moral = nx.Graph()
     for i in range(p):
         G_moral.add_node(i)
     G_moral.add_edges_from(list_edges)
 
     non_edges = list(set(E) - set(list_edges))
-    Sigma_hat = data.values.T @ data.values / n
+    # Sigma_hat = data.values.T @ data.values / n
+    Sigma_hat = np.cov(data.values.T)
 
     ############################## Find Delta and Mu ########################################
 
     # Find the smallest possible \mu such that Sigma_hat + \mu I be PD and stable.
     min_eig = np.min(scipy.linalg.eigh(Sigma_hat, eigvals_only=True))
     if min_eig < 0:
         pmu = np.abs(min_eig)  # due to numerical instability. This is the minimum value for \mu.
@@ -202,10 +203,10 @@
     Gamma_opt = np.reshape(Gamma_ij, (p, p))
     D_half = np.diag(np.diag(Gamma_opt))
     B = np.eye(p) - np.linalg.inv(D_half)@Gamma_opt.T
     B[abs(B) <= 1e-6] = 0
     run_time = end - start
     RGAP = m.MIPGAP
 
-    return RGAP, B, run_time
+    return RGAP, B, Gamma_opt, m.ObjVal, run_time
```

### Comparing `micodag-0.0.2/micodag.egg-info/PKG-INFO` & `micodag-0.0.3/micodag.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micodag
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python package of mixed integer convex programming for directed acyclic graphs.
 Author: Tong Xu
 Author-email: tongxu2027@u.northwestern.edu
 License: MIT
 Keywords: python,Bayesian network
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `micodag-0.0.2/setup.py` & `micodag-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 import os
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A Python package of mixed integer convex programming for directed acyclic graphs.'
 
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 # Setting up
```

