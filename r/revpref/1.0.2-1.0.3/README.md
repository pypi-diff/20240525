# Comparing `tmp/revpref-1.0.2.tar.gz` & `tmp/revpref-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revpref-1.0.2.tar", last modified: Wed Apr 24 02:08:50 2024, max compression
+gzip compressed data, was "revpref-1.0.3.tar", last modified: Sat May 25 15:25:28 2024, max compression
```

## Comparing `revpref-1.0.2.tar` & `revpref-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-24 02:08:50.981217 revpref-1.0.2/
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5461 2024-04-24 02:08:50.980991 revpref-1.0.2/PKG-INFO
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     4879 2024-04-24 02:02:41.000000 revpref-1.0.2/README.md
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      601 2024-04-23 13:35:18.000000 revpref-1.0.2/pyproject.toml
-drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-24 02:08:50.970466 revpref-1.0.2/revpref/
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      113 2024-04-21 16:08:26.000000 revpref-1.0.2/revpref/__init__.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     1534 2024-04-23 06:18:25.000000 revpref-1.0.2/revpref/_legacy.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     1836 2024-04-23 08:28:55.000000 revpref-1.0.2/revpref/_utils.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     1955 2024-04-23 06:28:47.000000 revpref-1.0.2/revpref/avi.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     3001 2024-04-23 11:59:47.000000 revpref-1.0.2/revpref/ccei.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5481 2024-04-24 02:07:45.000000 revpref-1.0.2/revpref/garp.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     6302 2024-04-24 01:55:53.000000 revpref-1.0.2/revpref/hmi.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     4409 2024-04-24 01:33:26.000000 revpref-1.0.2/revpref/mci.py
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     2334 2024-04-23 13:40:32.000000 revpref-1.0.2/revpref/mpi.py
-drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-04-24 02:08:50.980719 revpref-1.0.2/revpref.egg-info/
--rw-r--r--   0 aliebcxiang   (501) staff       (20)     5461 2024-04-24 02:08:50.000000 revpref-1.0.2/revpref.egg-info/PKG-INFO
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      336 2024-04-24 02:08:50.000000 revpref-1.0.2/revpref.egg-info/SOURCES.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)        1 2024-04-24 02:08:50.000000 revpref-1.0.2/revpref.egg-info/dependency_links.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)       49 2024-04-24 02:08:50.000000 revpref-1.0.2/revpref.egg-info/requires.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)        8 2024-04-24 02:08:50.000000 revpref-1.0.2/revpref.egg-info/top_level.txt
--rw-r--r--   0 aliebcxiang   (501) staff       (20)       38 2024-04-24 02:08:50.981267 revpref-1.0.2/setup.cfg
--rw-r--r--   0 aliebcxiang   (501) staff       (20)      473 2024-04-23 07:01:08.000000 revpref-1.0.2/setup.py
+drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-05-25 15:25:28.218176 revpref-1.0.3/
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5461 2024-05-25 15:25:28.217949 revpref-1.0.3/PKG-INFO
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     4879 2024-04-24 02:02:41.000000 revpref-1.0.3/README.md
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      601 2024-05-14 05:38:54.000000 revpref-1.0.3/pyproject.toml
+drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-05-25 15:25:28.216454 revpref-1.0.3/revpref/
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      113 2024-04-21 16:08:26.000000 revpref-1.0.3/revpref/__init__.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     1534 2024-04-23 06:18:25.000000 revpref-1.0.3/revpref/_legacy.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     1836 2024-04-23 08:28:55.000000 revpref-1.0.3/revpref/_utils.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     1955 2024-04-23 06:28:47.000000 revpref-1.0.3/revpref/avi.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     3001 2024-04-23 11:59:47.000000 revpref-1.0.3/revpref/ccei.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5481 2024-05-14 05:39:06.000000 revpref-1.0.3/revpref/garp.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     6310 2024-05-14 13:28:08.000000 revpref-1.0.3/revpref/hmi.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     4602 2024-05-14 07:13:38.000000 revpref-1.0.3/revpref/mci.py
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     2334 2024-04-23 13:40:32.000000 revpref-1.0.3/revpref/mpi.py
+drwxr-xr-x   0 aliebcxiang   (501) staff       (20)        0 2024-05-25 15:25:28.217682 revpref-1.0.3/revpref.egg-info/
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)     5461 2024-05-25 15:25:28.000000 revpref-1.0.3/revpref.egg-info/PKG-INFO
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      336 2024-05-25 15:25:28.000000 revpref-1.0.3/revpref.egg-info/SOURCES.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)        1 2024-05-25 15:25:28.000000 revpref-1.0.3/revpref.egg-info/dependency_links.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)       49 2024-05-25 15:25:28.000000 revpref-1.0.3/revpref.egg-info/requires.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)        8 2024-05-25 15:25:28.000000 revpref-1.0.3/revpref.egg-info/top_level.txt
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)       38 2024-05-25 15:25:28.218219 revpref-1.0.3/setup.cfg
+-rw-r--r--   0 aliebcxiang   (501) staff       (20)      473 2024-04-23 07:01:08.000000 revpref-1.0.3/setup.py
```

### Comparing `revpref-1.0.2/PKG-INFO` & `revpref-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revpref
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Tools for Computational Revealed Preference Analysis
 Home-page: https://github.com/Aliebc/revpref
 Author: Yi Xiang
 Author-email: Yi Xiang <xiangy.i@outlook.com>
 Project-URL: Homepage, https://github.com/Aliebc/revpref
 Project-URL: Bug Tracker, https://github.com/Aliebc/revpref
 Classifier: Programming Language :: Python :: 3
```

### Comparing `revpref-1.0.2/README.md` & `revpref-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `revpref-1.0.2/pyproject.toml` & `revpref-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "revpref"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     {"name" = "Yi Xiang", "email" = "xiangy.i@outlook.com"}
 ]
 description = "Python Tools for Computational Revealed Preference Analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `revpref-1.0.2/revpref/_legacy.py` & `revpref-1.0.3/revpref/_legacy.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.2/revpref/_utils.py` & `revpref-1.0.3/revpref/_utils.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.2/revpref/avi.py` & `revpref-1.0.3/revpref/avi.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.2/revpref/ccei.py` & `revpref-1.0.3/revpref/ccei.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.2/revpref/garp.py` & `revpref-1.0.3/revpref/garp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 __author__ = 'Yi Xiang'
 
 import networkx as nx
 import numpy as np
 from typing import Literal
 from matplotlib import pyplot as plt
```

### Comparing `revpref-1.0.2/revpref/hmi.py` & `revpref-1.0.3/revpref/hmi.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 def _mtz_hmi(p:np.ndarray, q:np.ndarray, solver = 'PULP_CBC_CMD'):
     sl = pl.getSolver(solver, msg = 0)
     edges = list(_generate_graph(p, q).edges())
     T = q.shape[0]
     PQT = p @ q.T
     
     EXP = np.diag(PQT).reshape(T, 1) @ np.ones((1, T))
-    Cs = np.clip(PQT - EXP, 0, None)
+    
+    Cs = np.clip(PQT - EXP, 1e-7, None)
     Cmin = np.min(Cs[np.nonzero(Cs)])
     Dmin = np.min(PQT[np.nonzero(PQT)])
     
     DELTA = min(Cmin, Dmin) / 2
     EPSILON = 1/(2 * T)
     ALPHA = np.max(PQT) + 1
```

### Comparing `revpref-1.0.2/revpref/mci.py` & `revpref-1.0.3/revpref/mci.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,23 +67,26 @@
             else:
                 min_cost = mci_lp.fun
                 return min_cost / sum_cost
         else:
             raise RuntimeError("MILP Failed!")
     pass
 
-def _mtz_mci(p:np.ndarray, q:np.ndarray, solver = 'PULP_CBC_CMD'):
+def _mtz_mci(p:np.ndarray, q:np.ndarray, solver = 'PULP_CBC_CMD', err = False):
     sl = pl.getSolver(solver, msg = 0)
     edges = list(_generate_graph(p, q).edges())
     T = q.shape[0]
     PQT = p @ q.T
     
     EXP = np.diag(PQT).reshape(T, 1) @ np.ones((1, T))
-    Cs = np.clip(PQT - EXP, 0, None)
-    Cmin = np.min(Cs[np.nonzero(Cs)])
+    
+    Cs = np.clip(PQT - EXP, 1e-6, None)
+    Csz = Cs[np.nonzero(Cs)]
+    Cmin = np.min(Csz)
+    
     Dmin = np.min(PQT[np.nonzero(PQT)])
     
     cons_delta = min(Cmin, Dmin) / 2
     cons_epsilon = 1/(1.5 * T)
     cons_alpha = np.max(PQT) * 2
     cons_beta = np.max(PQT) * 2
     
@@ -126,16 +129,22 @@
         
         prob += -cons_delta + cons_alpha * (vU[t][v] +  vB[t][v]) >= PQT[t][t] - PQT[t][v]
         prob += cons_alpha * (vU[v][t] - 1 - vB[t][v]) <= PQT[t][v] - PQT[t][t]
         prob += cons_beta * (vB[t][v] - 1) <=  PQT[t][t] - PQT[t][v]
     
     prob += pl.lpDot(vB2, vw)
     prob.solve(solver = sl)
-    e = pl.value(prob.objective) / sum_cost
     
+    if pl.LpStatus[prob.status] != "Optimal":
+        if err:
+            raise RuntimeError("Optimization Failed")
+        else:
+            return -1
+
+    e = pl.value(prob.objective) / sum_cost
     return e
     
 def _milp_mci(p:np.ndarray, q:np.ndarray, solver = 'PULP_CBC_CMD'):
     raise NotImplementedError("MILP not implemented")
 
 ####################################
 mci_mtz = _mtz_mci
```

### Comparing `revpref-1.0.2/revpref/mpi.py` & `revpref-1.0.3/revpref/mpi.py`

 * *Files identical despite different names*

### Comparing `revpref-1.0.2/revpref.egg-info/PKG-INFO` & `revpref-1.0.3/revpref.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revpref
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Tools for Computational Revealed Preference Analysis
 Home-page: https://github.com/Aliebc/revpref
 Author: Yi Xiang
 Author-email: Yi Xiang <xiangy.i@outlook.com>
 Project-URL: Homepage, https://github.com/Aliebc/revpref
 Project-URL: Bug Tracker, https://github.com/Aliebc/revpref
 Classifier: Programming Language :: Python :: 3
```

