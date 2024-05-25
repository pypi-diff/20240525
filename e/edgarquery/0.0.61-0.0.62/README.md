# Comparing `tmp/edgarquery-0.0.61.tar.gz` & `tmp/edgarquery-0.0.62.tar.gz`

## Comparing `edgarquery-0.0.61.tar` & `edgarquery-0.0.62.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rwxr-xr-x   0        0        0      621 2020-02-02 00:00:00.000000 edgarquery-0.0.61/genusage.sh
--rw-r--r--   0        0        0    10698 2020-02-02 00:00:00.000000 edgarquery-0.0.61/notes.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 edgarquery-0.0.61/requirements.txt
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.61/scripts/edgarquery.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.61/scripts/edgartickerstocsv.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/__about__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/concepts.sh
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/ebquery.py
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcikperson.py
--rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyconcepttocsv.py
--rw-r--r--   0        0        0     7504 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsshow.py
--rwxr-xr-x   0        0        0     6004 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyfactstocsv.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsziptocsv.py
--rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarlatest10K.py
--rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarlatestsubmission.py
--rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarlatestsubmissions.py
--rwxr-xr-x   0        0        0    15167 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarquery.py
--rw-r--r--   0        0        0    13998 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarsubmissions.py
--rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarsubmissionsziptocsv.py
--rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgartickerstocsv.py
--rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/edgarxbrlframestocsv.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/sedfile
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.61/src/edgarquery/tickerd.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/__init__.py
--rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/p.sh
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/s.sh
--rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/x.sh
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.61/tests/y.sh
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.61/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.61/LICENSE.txt
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 edgarquery-0.0.61/README.md
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 edgarquery-0.0.61/pyproject.toml
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 edgarquery-0.0.61/PKG-INFO
+-rwxr-xr-x   0        0        0      621 2020-02-02 00:00:00.000000 edgarquery-0.0.62/genusage.sh
+-rw-r--r--   0        0        0    11037 2020-02-02 00:00:00.000000 edgarquery-0.0.62/notes.txt
+-rw-r--r--   0        0        0  3628067 2020-02-02 00:00:00.000000 edgarquery-0.0.62/plotlyfig.html
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edgarquery-0.0.62/plotlyfig.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 edgarquery-0.0.62/requirements.txt
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 edgarquery-0.0.62/scripts/edgarquery.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 edgarquery-0.0.62/scripts/edgartickerstocsv.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/__about__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/__init__.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/concepts.sh
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/ebquery.py
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarcikperson.py
+-rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarcompanyconcepttocsv.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarcompanyfactsshow.py
+-rwxr-xr-x   0        0        0     6004 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarcompanyfactstocsv.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarcompanyfactsziptocsv.py
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarlatest10K.py
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarlatestsubmission.py
+-rw-r--r--   0        0        0     9269 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarlatestsubmissions.py
+-rwxr-xr-x   0        0        0    15167 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarquery.py
+-rw-r--r--   0        0        0    13998 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarsubmissions.py
+-rwxr-xr-x   0        0        0     5369 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarsubmissionsziptocsv.py
+-rwxr-xr-x   0        0        0     3865 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgartickerstocsv.py
+-rwxr-xr-x   0        0        0     4679 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/edgarxbrlframestocsv.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/sedfile
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 edgarquery-0.0.62/src/edgarquery/tickerd.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 edgarquery-0.0.62/tests/__init__.py
+-rwxr-xr-x   0        0        0     2760 2020-02-02 00:00:00.000000 edgarquery-0.0.62/tests/p.sh
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 edgarquery-0.0.62/tests/s.sh
+-rwxr-xr-x   0        0        0     2429 2020-02-02 00:00:00.000000 edgarquery-0.0.62/tests/x.sh
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 edgarquery-0.0.62/tests/y.sh
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 edgarquery-0.0.62/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 edgarquery-0.0.62/LICENSE.txt
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 edgarquery-0.0.62/README.md
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 edgarquery-0.0.62/pyproject.toml
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 edgarquery-0.0.62/PKG-INFO
```

### Comparing `edgarquery-0.0.61/genusage.sh` & `edgarquery-0.0.62/genusage.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/notes.txt` & `edgarquery-0.0.62/notes.txt`

 * *Files 5% similar despite different names*

```diff
@@ -251,8 +251,17 @@
   https://www.sec.gov/edgar/search/#/ciks=0000315090&
                 entityName=BUFFETT%2520WARREN%2520E%2520(CIK%25200000315090)
 
   tax 
   https://americansfortaxfairness.org/ultra-wealthys-8-5-trillion-untaxed-income/
   https://www.federalreserve.gov/econres/aboutscf.htm
 
+# plotly
+
+https://github.com/plotly/plotly.js
+fig.to_json()
+
+https://plotly.com/python/creating-and-updating-figures/
+https://stackoverflow.com/questions/39867224/plotly-js-only-one-plot-working-when-using-multiple-plots-on-same-page
+https://plnkr.co/edit/XluyqzOLOYAtdzp9EevX?p=preview&preview
+https://plotly.com/python/figure-structure/
```

### Comparing `edgarquery-0.0.61/scripts/edgarquery.py` & `edgarquery-0.0.62/scripts/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/ebquery.py` & `edgarquery-0.0.62/src/edgarquery/ebquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarcikperson.py` & `edgarquery-0.0.62/src/edgarquery/edgarcikperson.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarcompanyconcepttocsv.py` & `edgarquery-0.0.62/src/edgarquery/edgarcompanyconcepttocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsshow.py` & `edgarquery-0.0.62/src/edgarquery/edgarcompanyfactsshow.py`

 * *Files 23% similar despite different names*

```diff
@@ -73,49 +73,73 @@
         assert type(facts) == type({}), 'jsonfacts: facts not a dictionary'
         htmla = []
         htmla.append('<html>')
 
         cik = '%d' % (self.cik)
         ch = self.td.getrecforcik(self.cik)
         ttl = 'Company Facts: %s CIK%s' % (ch['title'], cik.zfill(10) )
-        htmla.append('<head><h1>%s</h1></head>' % (ttl) )
+
+        htmla.append('<head>')
+        htmla.append('<h1>%s</h1>' % (ttl) )
+        htmla.append('<script src="https://cdn.plot.ly/plotly-2.32.0.min.js" charset="utf-8"></script>')
+        htmla.append('</head>')
 
         fka = [k for k in facts.keys()]
-        for k in fka:
+        for fi in range(len(fka) ):
+            k = fka[fi]
             self.facttype = k           # dei or us-gaap
             assert type(facts[k]) == type({}), \
                 'jsonfacts: %s not a dictionary' % self.k
 
+            #htmla.append('<div id="%s">' % (k) )
             htmla.append('<p>fact type: %s</p><br/>' % (self.facttype) )
 
-            fka = [ft for ft in facts[k].keys()]
-            for t in fka:
-                #htmla.append('<h3> Fact Name: %s</h3>' % (t) )
+            fta = [ft for ft in facts[k].keys()]
+            #for t in fta:
+            for ti in range(len(fta) ):
+                t = fta[ti]
 
                 label = facts[k][t]['label']
-                #htmla.append('<h4>Fact Label: %s</h4>' % (label) )
 
                 descr = facts[k][t]['description']
                 if not descr:
                     descr = 'No description'
+                #htmla.append('<div id="%s%s">' % (k,t) )
                 htmla.append('<h3>Description: %s</h3>' % (descr) )
 
                 units = facts[k][t]['units']
                 assert type(units) == type({}), \
                     'jsonfacts: units not a dictionary'
-                uka = (u for u in units.keys() )
-                for uk in uka:
+                uka = [u for u in units.keys() ]
+                #for uk in uka:
+                for ui in range(len(uka) ):
+                    uk = uka[ui]
                     self.units = uk
+                    #htmla.append('<div id="%s%s%s">' % (k, t, uk) )
                     assert type(units[uk]) == type([]), \
                         'jasonfacts %s is not an array'
                     fig = self.jsonfactplot(units[uk], label)
-                    fightml = fig.to_html()
-                    htmla.append(fightml)
+
+                    figjs = fig.to_json()
+
+                    htmla.append('<div id="fig%s%s%s">' % (fi, ti, ui) )
+                    htmla.append('<script>')
+                    htmla.append('var figobj = %s;\n' % figjs)
+                    htmla.append('Plotly.newPlot("fig%s%s%s", figobj.data, figobj.layout, {});' % (fi,ti,ui) )
+                    htmla.append('</script>')
+                    htmla.append('</div>')
+
+                    #fightml = fig.to_html()
+                    #htmla.append(fightml)
+
                     tbl = self.jsonfacttable(units[uk], label)
                     htmla.extend(tbl)
+                    #htmla.append('</div>')
+                #htmla.append('</div>')
+            #htmla.append('</div>')
         self.htmla.extend(htmla)
 
 
     def jsonfactplot(self, recs, label):
         """ jsonfactplot(self, recs, label)
 
         plot the first two columns of the fact array
```

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarcompanyfactstocsv.py` & `edgarquery-0.0.62/src/edgarquery/edgarcompanyfactstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarcompanyfactsziptocsv.py` & `edgarquery-0.0.62/src/edgarquery/edgarcompanyfactsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarlatest10K.py` & `edgarquery-0.0.62/src/edgarquery/edgarlatest10K.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarlatestsubmission.py` & `edgarquery-0.0.62/src/edgarquery/edgarlatestsubmission.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarlatestsubmissions.py` & `edgarquery-0.0.62/src/edgarquery/edgarlatestsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarquery.py` & `edgarquery-0.0.62/src/edgarquery/edgarquery.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarsubmissions.py` & `edgarquery-0.0.62/src/edgarquery/edgarsubmissions.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarsubmissionsziptocsv.py` & `edgarquery-0.0.62/src/edgarquery/edgarsubmissionsziptocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgartickerstocsv.py` & `edgarquery-0.0.62/src/edgarquery/edgartickerstocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/edgarxbrlframestocsv.py` & `edgarquery-0.0.62/src/edgarquery/edgarxbrlframestocsv.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/src/edgarquery/tickerd.py` & `edgarquery-0.0.62/src/edgarquery/tickerd.py`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/tests/p.sh` & `edgarquery-0.0.62/tests/p.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/tests/x.sh` & `edgarquery-0.0.62/tests/x.sh`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/LICENSE.txt` & `edgarquery-0.0.62/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/README.md` & `edgarquery-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/pyproject.toml` & `edgarquery-0.0.62/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edgarquery-0.0.61/PKG-INFO` & `edgarquery-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgarquery
-Version: 0.0.61
+Version: 0.0.62
 Summary: Downloads various SEC EDGAR files by CIK or ticker.  companyfactsshow displays company facts in your browser
 Project-URL: Documentation, https://github.com/dfwcnj/edgarquery#readme
 Project-URL: Issues, https://github.com/dfwcnj/edgarquery/issues
 Project-URL: Source, https://github.com/dfwcnj/edgarquery
 Author-email: Don Caldwell <dfwcnj@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

