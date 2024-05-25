# Comparing `tmp/fredquery-0.0.52.tar.gz` & `tmp/fredquery-0.0.54.tar.gz`

## Comparing `fredquery-0.0.52.tar` & `fredquery-0.0.54.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0  4117566 2020-02-02 00:00:00.000000 fredquery-0.0.52/Ploteg0.ipynb
--rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 fredquery-0.0.52/Ploteg1.ipynb
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 fredquery-0.0.52/genusage.sh
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fredquery-0.0.52/notes.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fredquery-0.0.52/requirements.txt
--rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.52/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb
--rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 fredquery-0.0.52/.ipynb_checkpoints/Ploteg1-checkpoint.ipynb
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/__about__.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/__init__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/aa2csv.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/aa2html.py
--rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredcategories.py
--rw-r--r--   0        0        0     4295 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredplot.py
--rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredplotseries.py
--rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredreleases.py
--rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredseries.py
--rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredsources.py
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/fredtags.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/query.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fredquery-0.0.52/src/fredquery/xmlstr2aa.py
--rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 fredquery-0.0.52/tests/p.sh
--rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 fredquery-0.0.52/tests/plot.sh
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 fredquery-0.0.52/tests/s.sh
--rwxr-xr-x   0        0        0     2228 2020-02-02 00:00:00.000000 fredquery-0.0.52/tests/x.sh
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fredquery-0.0.52/LICENSE.txt
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 fredquery-0.0.52/README.md
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fredquery-0.0.52/pyproject.toml
--rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 fredquery-0.0.52/PKG-INFO
+-rw-r--r--   0        0        0  4117566 2020-02-02 00:00:00.000000 fredquery-0.0.54/Ploteg0.ipynb
+-rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 fredquery-0.0.54/Ploteg1.ipynb
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 fredquery-0.0.54/genusage.sh
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fredquery-0.0.54/notes.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fredquery-0.0.54/requirements.txt
+-rw-r--r--   0        0        0  4120769 2020-02-02 00:00:00.000000 fredquery-0.0.54/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb
+-rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 fredquery-0.0.54/.ipynb_checkpoints/Ploteg1-checkpoint.ipynb
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/__about__.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/__init__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/aa2csv.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/aa2html.py
+-rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredcategories.py
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredplot.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredplotseries.py
+-rw-r--r--   0        0        0    10143 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredreleases.py
+-rw-r--r--   0        0        0    11104 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredseries.py
+-rw-r--r--   0        0        0    12113 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredsources.py
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/fredtags.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/query.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fredquery-0.0.54/src/fredquery/xmlstr2aa.py
+-rwxr-xr-x   0        0        0     2546 2020-02-02 00:00:00.000000 fredquery-0.0.54/tests/p.sh
+-rwxr-xr-x   0        0        0      341 2020-02-02 00:00:00.000000 fredquery-0.0.54/tests/plot.sh
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 fredquery-0.0.54/tests/s.sh
+-rwxr-xr-x   0        0        0     2228 2020-02-02 00:00:00.000000 fredquery-0.0.54/tests/x.sh
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fredquery-0.0.54/LICENSE.txt
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 fredquery-0.0.54/README.md
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 fredquery-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 fredquery-0.0.54/PKG-INFO
```

### Comparing `fredquery-0.0.52/Ploteg0.ipynb` & `fredquery-0.0.54/Ploteg0.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/Ploteg1.ipynb` & `fredquery-0.0.54/Ploteg1.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/notes.txt` & `fredquery-0.0.54/notes.txt`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb` & `fredquery-0.0.54/.ipynb_checkpoints/Ploteg0-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/.ipynb_checkpoints/Ploteg1-checkpoint.ipynb` & `fredquery-0.0.54/.ipynb_checkpoints/Ploteg1-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/aa2html.py` & `fredquery-0.0.54/src/fredquery/aa2html.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/fredcategories.py` & `fredquery-0.0.54/src/fredquery/fredcategories.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/fredplot.py` & `fredquery-0.0.54/src/fredquery/fredplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         fp = fredplotseries.FREDPlotSeries()
 
         ida = [aa[i][0] for i in range(1, len(aa))]
         idc = ','.join(ida)
         fp.getserieslist(idc)
         fp.getobservationlist(idc)
 
-        #fp.composeunitseriesplotwnotes(title)
         fp.composeunitfreqseriesplotwnotes(title)
 
         fp.saveplothtml(hfn)
         fp.showplothtml(hfn)
 
     def plotcategoryid(self, catid, directory):
         """ plotcategoryid(catid, directory)
```

### Comparing `fredquery-0.0.52/src/fredquery/fredreleases.py` & `fredquery-0.0.54/src/fredquery/fredreleases.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/fredseries.py` & `fredquery-0.0.54/src/fredquery/fredseries.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/fredsources.py` & `fredquery-0.0.54/src/fredquery/fredsources.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/fredtags.py` & `fredquery-0.0.54/src/fredquery/fredtags.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/query.py` & `fredquery-0.0.54/src/fredquery/query.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/src/fredquery/xmlstr2aa.py` & `fredquery-0.0.54/src/fredquery/xmlstr2aa.py`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/tests/p.sh` & `fredquery-0.0.54/tests/p.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/tests/s.sh` & `fredquery-0.0.54/tests/s.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/tests/x.sh` & `fredquery-0.0.54/tests/x.sh`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/LICENSE.txt` & `fredquery-0.0.54/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/README.md` & `fredquery-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/pyproject.toml` & `fredquery-0.0.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fredquery-0.0.52/PKG-INFO` & `fredquery-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fredquery
-Version: 0.0.52
+Version: 0.0.54
 Summary: Downloads various stlouisfed.org FRED files to CSV files and creates plots based on category, release, series, source, or tag
 Project-URL: Documentation, https://github.com/dfwcnj/fredquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/fredquery/issues
 Project-URL: Source, https://github.com/dfwcnj/fredquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

