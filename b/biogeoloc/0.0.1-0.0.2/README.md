# Comparing `tmp/biogeoloc-0.0.1.tar.gz` & `tmp/biogeoloc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biogeoloc-0.0.1.tar", last modified: Mon May 20 16:16:04 2024, max compression
+gzip compressed data, was "biogeoloc-0.0.2.tar", last modified: Sat May 25 16:50:20 2024, max compression
```

## Comparing `biogeoloc-0.0.1.tar` & `biogeoloc-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-09 23:42:35.000000 biogeoloc-0.0.1/LICENSE
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     2857 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/PKG-INFO
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2476 2024-05-11 19:39:17.000000 biogeoloc-0.0.1/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/biogeoloc/
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)       86 2024-05-11 19:35:20.000000 biogeoloc-0.0.1/biogeoloc/__init__.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    15498 2024-05-11 15:40:07.000000 biogeoloc-0.0.1/biogeoloc/cls.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    12257 2024-05-11 19:42:17.000000 biogeoloc-0.0.1/biogeoloc/genesys.py
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      176 2024-05-11 03:22:53.000000 biogeoloc-0.0.1/biogeoloc/versions.py
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/biogeoloc.egg-info/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     2857 2024-05-20 16:16:03.000000 biogeoloc-0.0.1/biogeoloc.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      272 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/biogeoloc.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-20 16:16:03.000000 biogeoloc-0.0.1/biogeoloc.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/biogeoloc.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/biogeoloc.egg-info/top_level.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-20 16:16:04.000000 biogeoloc-0.0.1/setup.cfg
--rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      837 2024-05-11 03:29:08.000000 biogeoloc-0.0.1/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-25 16:50:20.000000 biogeoloc-0.0.2/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2024-05-09 23:42:35.000000 biogeoloc-0.0.2/LICENSE
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2914 2024-05-25 16:50:20.000000 biogeoloc-0.0.2/PKG-INFO
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2476 2024-05-11 19:39:17.000000 biogeoloc-0.0.2/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-25 16:50:20.000000 biogeoloc-0.0.2/biogeoloc/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      108 2024-05-23 19:38:34.000000 biogeoloc-0.0.2/biogeoloc/__init__.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    30867 2024-05-25 16:48:46.000000 biogeoloc-0.0.2/biogeoloc/cls.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)    12609 2024-05-23 21:23:02.000000 biogeoloc-0.0.2/biogeoloc/genesys.py
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      289 2024-05-22 18:44:40.000000 biogeoloc-0.0.2/biogeoloc/versions.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2024-05-25 16:50:20.000000 biogeoloc-0.0.2/biogeoloc.egg-info/
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)     2914 2024-05-25 16:50:19.000000 biogeoloc-0.0.2/biogeoloc.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      272 2024-05-25 16:50:19.000000 biogeoloc-0.0.2/biogeoloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2024-05-25 16:50:19.000000 biogeoloc-0.0.2/biogeoloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       49 2024-05-25 16:50:19.000000 biogeoloc-0.0.2/biogeoloc.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       10 2024-05-25 16:50:19.000000 biogeoloc-0.0.2/biogeoloc.egg-info/top_level.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2024-05-25 16:50:20.000000 biogeoloc-0.0.2/setup.cfg
+-rw-r--r--   0 xuyuxing  (1003) xuyuxing  (1003)      837 2024-05-11 03:29:08.000000 biogeoloc-0.0.2/setup.py
```

### Comparing `biogeoloc-0.0.1/LICENSE` & `biogeoloc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biogeoloc-0.0.1/PKG-INFO` & `biogeoloc-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: biogeoloc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for plotting correlations between variants and environmental factors.
 Home-page: https://github.com/SouthernCD/GeoGenoPlot
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: toolbiox>=0.0.46
+Requires-Dist: plotbiox>=0.0.2
+Requires-Dist: cyvcf2>=0.30.28
 
 # biogeoloc
 A python object package for storing and managing geographic information about biological samples
 
 ## Installation
 ```
 pip install biogeoloc
@@ -80,9 +81,7 @@
 
 q_id = 'PI207841'
 u_id = sorghumGS.search(q_id)
 acc = sorghumGS.get(u_id)
 ```
 
 
-
-
```

### Comparing `biogeoloc-0.0.1/README.md` & `biogeoloc-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `biogeoloc-0.0.1/biogeoloc/genesys.py` & `biogeoloc-0.0.2/biogeoloc/genesys.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,41 +39,45 @@
         georefed_genesys_df = non_dup_df[non_dup_df.lat.notnull(
         ) | non_dup_df.lon.notnull()]
 
         print("There are %d samples in Genesys, in which %d samples are non-duplicated (%d data have conflicted coord information) and %d samples have georeference information." %
               (len(genesys_df), len(non_dup_df), len(coord_contradictory_list), len(georefed_genesys_df)))
 
         # 生成Accession对象, 并添加到AccessionSet中
-        uniq_num = 0
-        uniq_id_format = "u%%0%dd" % len(str(len(non_dup_df)))
+        # uniq_num = 0
+        # uniq_id_format = "u%%0%dd" % len(str(len(non_dup_df)))
         for i in range(len(non_dup_df)):
             row = non_dup_df.iloc[i]
             pi_id_list = row.pi_id.split(",") if len(row.pi_id) > 0 else []
             is_id_list = row.is_id.split(",") if len(row.is_id) > 0 else []
             gs_id_list = row.gs_id.split(",") if len(row.gs_id) > 0 else []
 
-            uniq_id = uniq_id_format % uniq_num
-            s = Accession(uniq_id,
+            # uniq_id = uniq_id_format % uniq_num
+            # s = Accession(uniq_id,
+            s = Accession(           
                           lat=row.lat,
                           lon=row.lon,
                           passport={"local_adapted": row.local_adapted},
                           sources=['Genesys'],
                           pi_id_list=pi_id_list,
                           is_id_list=is_id_list,
                           genesys_id_list=gs_id_list,
                           )
-            uniq_num += 1
+            # uniq_num += 1
 
             self.add(s)
 
 
 # PI_ID_format = r'PI ?\d+[A-Z]?'
-# IS_ID_format = r'IS ?\d+[A-Z]?'
-PI_ID_format = r'PI ?\d+'
-IS_ID_format = r'IS ?\d+'
+# IS_ID_format = r'^IS ?\d+[A-Z]?$'
+# PI_ID_format = r'^PI ?\d+$'
+# IS_ID_format = r'IS ?\d+'
+# IS_ID_format = re.compile(r'IS ?\d+[A-Z]?')
+IS_ID_format = re.compile(r'^IS ?\d+[A-Z]?$')
+PI_ID_format = re.compile(r'^(PI ?\d+)$|^Duplicate of (PI ?\d+)$')
 
 
 def load_genesys_dir(genesys_metadata_dir):
 
     genesys_core_file = genesys_metadata_dir + "/core.csv"
     genesys_names_file = genesys_metadata_dir + "/names.csv"
     cmd_string = "sed '1s/$/,/' geo.csv > geo_new.csv"
@@ -181,25 +185,30 @@
         name_list = acceNumb + names
 
         pi_id_list = []
         is_id_list = []
 
         for name in name_list:
             # PI ID
-            refinder = re.findall(PI_ID_format, name)
-            for pi_id in refinder:
-                pi_id = pi_id.replace(" ", "")
-                pi_id_list.append(pi_id)
+            refinder = PI_ID_format.match(name)
+            if refinder:
+                for pi_id in refinder.groups():
+                    if pi_id is None:
+                        continue
+                    pi_id = pi_id.replace(" ", "")
+                    pi_id_list.append(pi_id)
 
             # IS ID
-            refinder = re.findall(IS_ID_format, name)
-            for is_id in refinder:
+            refinder = IS_ID_format.match(name)
+            if refinder:
+                is_id = refinder.group()
                 is_id = is_id.replace(" ", "")
                 is_id_list.append(is_id)
 
+
         id_map.append([genesys_id])
         if len(pi_id_list):
             id_map.append(pi_id_list)
         if len(is_id_list):
             id_map.append(is_id_list)
 
         for i in pi_id_list:
```

### Comparing `biogeoloc-0.0.1/biogeoloc.egg-info/PKG-INFO` & `biogeoloc-0.0.2/biogeoloc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: biogeoloc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for plotting correlations between variants and environmental factors.
 Home-page: https://github.com/SouthernCD/GeoGenoPlot
 Author: Yuxing Xu
 Author-email: xuyuxing@mail.kib.ac.cn
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: toolbiox>=0.0.46
+Requires-Dist: plotbiox>=0.0.2
+Requires-Dist: cyvcf2>=0.30.28
 
 # biogeoloc
 A python object package for storing and managing geographic information about biological samples
 
 ## Installation
 ```
 pip install biogeoloc
@@ -80,9 +81,7 @@
 
 q_id = 'PI207841'
 u_id = sorghumGS.search(q_id)
 acc = sorghumGS.get(u_id)
 ```
 
 
-
-
```

### Comparing `biogeoloc-0.0.1/setup.py` & `biogeoloc-0.0.2/setup.py`

 * *Files identical despite different names*

