# Comparing `tmp/symetrics-9.2.0.tar.gz` & `tmp/symetrics-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symetrics-9.2.0.tar", last modified: Sun May 12 17:24:27 2024, max compression
+gzip compressed data, was "symetrics-9.3.0.tar", last modified: Tue May 14 18:49:09 2024, max compression
```

## Comparing `symetrics-9.2.0.tar` & `symetrics-9.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 17:24:27.777605 symetrics-9.2.0/
--rw-rw-rw-   0        0        0     1151 2024-05-12 17:24:27.777605 symetrics-9.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-12 17:24:27.777605 symetrics-9.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1640 2024-05-12 17:24:11.000000 symetrics-9.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:24:27.760817 symetrics-9.2.0/symetrics/
--rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-9.2.0/symetrics/__init__.py
--rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-9.2.0/symetrics/dbcontext.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:24:27.777605 symetrics-9.2.0/symetrics/src/
--rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-9.2.0/symetrics/src/__init__.py
--rw-rw-rw-   0        0        0     1035 2024-04-30 06:51:43.000000 symetrics-9.2.0/symetrics/src/datastruct.py
--rw-rw-rw-   0        0        0    27457 2024-05-12 17:24:07.000000 symetrics-9.2.0/symetrics/symetrics_api.py
-drwxrwxrwx   0        0        0        0 2024-05-12 17:24:27.775126 symetrics-9.2.0/symetrics.egg-info/
--rw-rw-rw-   0        0        0     1151 2024-05-12 17:24:27.000000 symetrics-9.2.0/symetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-05-12 17:24:27.000000 symetrics-9.2.0/symetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 17:24:27.000000 symetrics-9.2.0/symetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-12 17:24:27.000000 symetrics-9.2.0/symetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-12 17:24:27.000000 symetrics-9.2.0/symetrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 18:49:09.504378 symetrics-9.3.0/
+-rw-rw-rw-   0        0        0     1151 2024-05-14 18:49:09.504378 symetrics-9.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:49:09.504378 symetrics-9.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1640 2024-05-14 18:48:08.000000 symetrics-9.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:49:09.463531 symetrics-9.3.0/symetrics/
+-rw-rw-rw-   0        0        0      101 2023-12-09 13:09:42.000000 symetrics-9.3.0/symetrics/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-12-09 13:09:33.000000 symetrics-9.3.0/symetrics/dbcontext.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:49:09.503379 symetrics-9.3.0/symetrics/src/
+-rw-rw-rw-   0        0        0       25 2023-10-25 09:08:07.000000 symetrics-9.3.0/symetrics/src/__init__.py
+-rw-rw-rw-   0        0        0     1035 2024-04-30 06:51:43.000000 symetrics-9.3.0/symetrics/src/datastruct.py
+-rw-rw-rw-   0        0        0    29353 2024-05-14 18:45:09.000000 symetrics-9.3.0/symetrics/symetrics_api.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:49:09.498686 symetrics-9.3.0/symetrics.egg-info/
+-rw-rw-rw-   0        0        0     1151 2024-05-14 18:49:09.000000 symetrics-9.3.0/symetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-05-14 18:49:09.000000 symetrics-9.3.0/symetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:49:09.000000 symetrics-9.3.0/symetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-14 18:49:09.000000 symetrics-9.3.0/symetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-14 18:49:09.000000 symetrics-9.3.0/symetrics.egg-info/top_level.txt
```

### Comparing `symetrics-9.2.0/PKG-INFO` & `symetrics-9.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 9.2.0
+Version: 9.3.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `symetrics-9.2.0/setup.py` & `symetrics-9.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '9.2.0' 
+VERSION = '9.3.0' 
 DESCRIPTION = 'Symetrics API'
 LONG_DESCRIPTION = '''A package to access SYMETRICS database. 
 SYMETRICS database is a consolidation of metrics for synonymous variants which were derived from a number of computational tools each of which contributing to 
 attribute specific metrics such as SYNVEP for general functional constraints, SpliceAI for splicing effect, SILVA for obtaining GERP++ (phylogenetic related constraints)
 CpG/CpG_Exon, dRSCU/RSCU for codon usage and SURF for rna stability. The package also includes a result of the analysis of the influence of each variants exceeding set threshold
 per metrics defined constituting to a score assigned to a gene'''
 REQUIRED_PACKAGES = [
```

### Comparing `symetrics-9.2.0/symetrics/dbcontext.py` & `symetrics-9.3.0/symetrics/dbcontext.py`

 * *Files identical despite different names*

### Comparing `symetrics-9.2.0/symetrics/src/datastruct.py` & `symetrics-9.3.0/symetrics/src/datastruct.py`

 * *Files identical despite different names*

### Comparing `symetrics-9.2.0/symetrics/symetrics_api.py` & `symetrics-9.3.0/symetrics/symetrics_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,72 @@
                     logging.error(e)
                     logging.error(f"Connection to {self._constraints} failed")
                 
                     
         else:
             logging.error(f'Group: {group} is not valid')       
     
+        return scores
+
+    def get_all_prop_score(self,group = MetricsGroup.SYNVEP.name):
+        
+        """
+        
+        Get the SYMETRICS score for  metrics group. The score was calculated from the pooled z proportion test of different
+        metrics group with their corresponding threhold:
+            - SYNVEP: 0.5
+            - GERP: 4
+            - CpG: 
+            - CpG_exon: 1
+            - RSCU:
+            - dRSCU:
+            - SpliceAI: 0.8
+            - SURF: 0.3
+        
+        Args:
+            group: A string representing the HGNC Symbol of a gene
+        
+        Returns:
+            scores: A dictionary returning the pvalues and fdr acquired from the test and the score before and after scaling.
+        
+        Examples:
+
+            >>> from symetrics import *
+            >>> symetrics = Symetrics('symetrics.db')
+            >>> score = symetrics.get_all_prop_score(group = 'SYNVEP')
+        
+        """
+
+        scores = (0,1)
+        scaler = StandardScaler()
+        
+
+        if group in MetricsGroup.__members__:
+            scores = None
+            try:
+                with self._constraints as dbhandler:
+                            
+                    cursor = dbhandler._conn.cursor()
+                            
+                    query = f"SELECT z as SYMETRIC_SCORE FROM GNOMADv4{group}"
+                            
+
+                    cursor.execute(query)
+                    rows = cursor.fetchall()
+                    rows = [r[0] for r in rows]
+                    scores = (np.mean(rows),np.std(rows))
+
+            except Error as e:
+                    logging.error(e)
+                    logging.error(f"Connection to {self._constraints} failed")
+                
+                    
+        else:
+            logging.error(f'Group: {group} is not valid')       
+    
         return scores    
     
     def get_gnomad_data(self, variant: VariantObject):
 
         """
         
         Get the gnomad information related to the alleles of the given variant (allele count, allele number and allele frequency)
```

### Comparing `symetrics-9.2.0/symetrics.egg-info/PKG-INFO` & `symetrics-9.3.0/symetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symetrics
-Version: 9.2.0
+Version: 9.3.0
 Summary: Symetrics API
 Home-page: https://lbundalian.github.io/symetrics/
 Author: Linnaeus Bundalian
 Author-email: linnaeusbundalian@gmail.com
 Keywords: python,synonymous variants
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

