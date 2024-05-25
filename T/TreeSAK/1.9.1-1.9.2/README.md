# Comparing `tmp/TreeSAK-1.9.1.tar.gz` & `tmp/TreeSAK-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TreeSAK-1.9.1.tar", last modified: Mon Mar 27 02:58:43 2023, max compression
+gzip compressed data, was "TreeSAK-1.9.2.tar", last modified: Wed Mar 29 05:38:01 2023, max compression
```

## Comparing `TreeSAK-1.9.1.tar` & `TreeSAK-1.9.2.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-27 02:58:43.941041 TreeSAK-1.9.1/
--rw-r--r--   0 songweizhi   (501) staff       (20)        6 2023-02-19 01:40:40.000000 TreeSAK-1.9.1/.gitignore
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      268 2023-03-27 02:58:43.940929 TreeSAK-1.9.1/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1499 2023-03-27 02:56:09.000000 TreeSAK-1.9.1/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-27 02:58:43.939605 TreeSAK-1.9.1/TreeSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     4893 2023-03-01 00:39:36.000000 TreeSAK-1.9.1/TreeSAK/AssessCVG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    15774 2023-03-14 07:40:48.000000 TreeSAK-1.9.1/TreeSAK/AssessMarker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12463 2023-03-27 01:36:17.000000 TreeSAK-1.9.1/TreeSAK/AssessMarkerDeltaLL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    15180 2023-03-25 09:26:04.000000 TreeSAK-1.9.1/TreeSAK/AssessMarkerPA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5871 2023-03-25 09:26:04.000000 TreeSAK-1.9.1/TreeSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7651 2023-03-27 02:58:35.000000 TreeSAK-1.9.1/TreeSAK/Dating.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    44627 2023-03-18 06:04:26.000000 TreeSAK-1.9.1/TreeSAK/KEGG_Luo17.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    40310 2023-03-25 09:26:04.000000 TreeSAK-1.9.1/TreeSAK/Marker2Tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1679 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/TreeSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3200 2023-03-11 08:00:26.000000 TreeSAK-1.9.1/TreeSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1933 2022-07-25 06:25:36.000000 TreeSAK-1.9.1/TreeSAK/TreeSAK_config copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1933 2022-07-25 06:25:36.000000 TreeSAK-1.9.1/TreeSAK/TreeSAK_config.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      361 2023-03-27 02:58:35.000000 TreeSAK-1.9.1/TreeSAK/VERSION
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/TreeSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2022-07-25 06:24:01.000000 TreeSAK-1.9.1/TreeSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9851 2022-07-26 01:13:26.000000 TreeSAK-1.9.1/TreeSAK/compare_trees.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2022-09-05 00:11:52.000000 TreeSAK-1.9.1/TreeSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3542 2023-03-09 07:26:29.000000 TreeSAK-1.9.1/TreeSAK/get_arCOG_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7245 2023-03-25 09:26:04.000000 TreeSAK-1.9.1/TreeSAK/global_functions.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    21221 2022-08-12 11:54:42.000000 TreeSAK-1.9.1/TreeSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3348 2023-03-07 06:10:56.000000 TreeSAK-1.9.1/TreeSAK/parse_deltall_stdout.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2022-08-20 23:38:06.000000 TreeSAK-1.9.1/TreeSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7303 2022-07-25 09:20:23.000000 TreeSAK-1.9.1/TreeSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3108 2023-03-25 09:07:52.000000 TreeSAK-1.9.1/TreeSAK/test_1.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-27 02:58:43.940072 TreeSAK-1.9.1/TreeSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      268 2023-03-27 02:58:43.000000 TreeSAK-1.9.1/TreeSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)      872 2023-03-27 02:58:43.000000 TreeSAK-1.9.1/TreeSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2023-03-27 02:58:43.000000 TreeSAK-1.9.1/TreeSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       96 2023-03-27 02:58:43.000000 TreeSAK-1.9.1/TreeSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        8 2023-03-27 02:58:43.000000 TreeSAK-1.9.1/TreeSAK.egg-info/top_level.txt
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-27 02:58:43.940301 TreeSAK-1.9.1/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    18428 2023-03-27 02:58:35.000000 TreeSAK-1.9.1/bin/TreeSAK
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/bin/__init__.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-27 02:58:43.940760 TreeSAK-1.9.1/images/
--rw-r--r--   0 songweizhi   (501) staff       (20)   395761 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/images/Bioinformatics.jpg
--rw-r--r--   0 songweizhi   (501) staff       (20)    14849 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/images/windows_cmds.docx
--rw-r--r--   0 songweizhi   (501) staff       (20)    33380 2021-11-12 21:13:42.000000 TreeSAK-1.9.1/images/windows_cmds.pdf
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2023-03-27 02:58:43.941077 TreeSAK-1.9.1/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      925 2023-03-01 00:23:48.000000 TreeSAK-1.9.1/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-29 05:38:01.202162 TreeSAK-1.9.2/
+-rw-r--r--   0 songweizhi   (501) staff       (20)        6 2023-02-19 01:40:40.000000 TreeSAK-1.9.2/.gitignore
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      268 2023-03-29 05:38:01.202026 TreeSAK-1.9.2/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1499 2023-03-27 02:56:09.000000 TreeSAK-1.9.2/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-29 05:38:01.199066 TreeSAK-1.9.2/TreeSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4893 2023-03-01 00:39:36.000000 TreeSAK-1.9.2/TreeSAK/AssessCVG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    15774 2023-03-14 07:40:48.000000 TreeSAK-1.9.2/TreeSAK/AssessMarker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12463 2023-03-27 01:36:17.000000 TreeSAK-1.9.2/TreeSAK/AssessMarkerDeltaLL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    15180 2023-03-25 09:26:04.000000 TreeSAK-1.9.2/TreeSAK/AssessMarkerPA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5871 2023-03-25 09:26:04.000000 TreeSAK-1.9.2/TreeSAK/ConvertMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    17984 2023-03-29 01:48:46.000000 TreeSAK-1.9.2/TreeSAK/Dating.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    44627 2023-03-18 06:04:26.000000 TreeSAK-1.9.2/TreeSAK/KEGG_Luo17.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    40191 2023-03-29 01:46:24.000000 TreeSAK-1.9.2/TreeSAK/Marker2Tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1679 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/TreeSAK/OneLineAln.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3200 2023-03-11 08:00:26.000000 TreeSAK-1.9.2/TreeSAK/SliceMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1933 2022-07-25 06:25:36.000000 TreeSAK-1.9.2/TreeSAK/TreeSAK_config copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1933 2022-07-25 06:25:36.000000 TreeSAK-1.9.2/TreeSAK/TreeSAK_config.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      361 2023-03-29 05:37:59.000000 TreeSAK-1.9.2/TreeSAK/VERSION
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/TreeSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2022-07-25 06:24:01.000000 TreeSAK-1.9.2/TreeSAK/compare_trees.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9851 2022-07-26 01:13:26.000000 TreeSAK-1.9.2/TreeSAK/compare_trees.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2022-09-05 00:11:52.000000 TreeSAK-1.9.2/TreeSAK/format_leaf_name.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3542 2023-03-09 07:26:29.000000 TreeSAK-1.9.2/TreeSAK/get_arCOG_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7245 2023-03-25 09:26:04.000000 TreeSAK-1.9.2/TreeSAK/global_functions.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    21221 2022-08-12 11:54:42.000000 TreeSAK-1.9.2/TreeSAK/iTOL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3348 2023-03-07 06:10:56.000000 TreeSAK-1.9.2/TreeSAK/parse_deltall_stdout.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4871 2023-03-28 02:56:45.000000 TreeSAK-1.9.2/TreeSAK/prep_mcmctree_ctl.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2022-08-20 23:38:06.000000 TreeSAK-1.9.2/TreeSAK/rename_leaves.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      692 2023-03-27 08:53:41.000000 TreeSAK-1.9.2/TreeSAK/replace_clades.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2424 2023-03-27 09:09:48.000000 TreeSAK-1.9.2/TreeSAK/root_with_out_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7303 2022-07-25 09:20:23.000000 TreeSAK-1.9.2/TreeSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4840 2023-03-29 03:43:53.000000 TreeSAK-1.9.2/TreeSAK/test_1.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-29 05:38:01.199854 TreeSAK-1.9.2/TreeSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      268 2023-03-29 05:38:00.000000 TreeSAK-1.9.2/TreeSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)      958 2023-03-29 05:38:00.000000 TreeSAK-1.9.2/TreeSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2023-03-29 05:38:00.000000 TreeSAK-1.9.2/TreeSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       96 2023-03-29 05:38:00.000000 TreeSAK-1.9.2/TreeSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        8 2023-03-29 05:38:00.000000 TreeSAK-1.9.2/TreeSAK.egg-info/top_level.txt
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-29 05:38:01.200085 TreeSAK-1.9.2/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    18935 2023-03-29 05:37:59.000000 TreeSAK-1.9.2/bin/TreeSAK
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/bin/__init__.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-03-29 05:38:01.201562 TreeSAK-1.9.2/images/
+-rw-r--r--   0 songweizhi   (501) staff       (20)   395761 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/images/Bioinformatics.jpg
+-rw-r--r--   0 songweizhi   (501) staff       (20)    14849 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/images/windows_cmds.docx
+-rw-r--r--   0 songweizhi   (501) staff       (20)    33380 2021-11-12 21:13:42.000000 TreeSAK-1.9.2/images/windows_cmds.pdf
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2023-03-29 05:38:01.202196 TreeSAK-1.9.2/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      925 2023-03-01 00:23:48.000000 TreeSAK-1.9.2/setup.py
```

### Comparing `TreeSAK-1.9.1/LICENSE` & `TreeSAK-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/README.md` & `TreeSAK-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/AssessCVG.py` & `TreeSAK-1.9.2/TreeSAK/AssessCVG.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/AssessMarker.py` & `TreeSAK-1.9.2/TreeSAK/AssessMarker.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/AssessMarkerDeltaLL.py` & `TreeSAK-1.9.2/TreeSAK/AssessMarkerDeltaLL.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/AssessMarkerPA.py` & `TreeSAK-1.9.2/TreeSAK/AssessMarkerPA.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/ConvertMSA.py` & `TreeSAK-1.9.2/TreeSAK/ConvertMSA.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/KEGG_Luo17.py` & `TreeSAK-1.9.2/TreeSAK/KEGG_Luo17.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/Marker2Tree.py` & `TreeSAK-1.9.2/TreeSAK/Marker2Tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,15 +775,14 @@
     parser.add_argument('-o',               required=True,                          help='output dir')
     parser.add_argument('-e',               required=True,                          help='e-value')
     parser.add_argument('-t',               required=True,  type=int,               help='num of threads')
     parser.add_argument('-skip_align_trim', required=False, action="store_true",    help='skip extracting, aligning and trimming markers')
     parser.add_argument('-mmn',             required=False, default=10, type=int,   help='minimal marker number, default: 10')
     parser.add_argument('-jst',             required=False, default='6',            help='threads to request in job script, for running iqtree')
     parser.add_argument('-qsub',            required=False, action="store_true",    help='submit job scripts')
-    #parser.add_argument('-pl',              required=True,                          help='path to catfasta2phyml.pl')
     parser.add_argument('-f',               required=False, action="store_true",    help='force overwrite')
     args = vars(parser.parse_args())
     Marker2Tree(args)
 
 
 '''
```

### Comparing `TreeSAK-1.9.1/TreeSAK/OneLineAln.py` & `TreeSAK-1.9.2/TreeSAK/OneLineAln.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/SliceMSA.py` & `TreeSAK-1.9.2/TreeSAK/SliceMSA.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/TreeSAK_config copy.py` & `TreeSAK-1.9.2/TreeSAK/TreeSAK_config copy.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/TreeSAK_config.py` & `TreeSAK-1.9.2/TreeSAK/TreeSAK_config.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/compare_trees.R` & `TreeSAK-1.9.2/TreeSAK/compare_trees.R`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/compare_trees.py` & `TreeSAK-1.9.2/TreeSAK/compare_trees.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/format_leaf_name.py` & `TreeSAK-1.9.2/TreeSAK/format_leaf_name.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/get_arCOG_seq.py` & `TreeSAK-1.9.2/TreeSAK/get_arCOG_seq.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/global_functions.py` & `TreeSAK-1.9.2/TreeSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/iTOL.py` & `TreeSAK-1.9.2/TreeSAK/iTOL.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/parse_deltall_stdout.py` & `TreeSAK-1.9.2/TreeSAK/parse_deltall_stdout.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/rename_leaves.py` & `TreeSAK-1.9.2/TreeSAK/rename_leaves.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK/subset_tree.py` & `TreeSAK-1.9.2/TreeSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/TreeSAK.egg-info/SOURCES.txt` & `TreeSAK-1.9.2/TreeSAK.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 TreeSAK/compare_trees.R
 TreeSAK/compare_trees.py
 TreeSAK/format_leaf_name.py
 TreeSAK/get_arCOG_seq.py
 TreeSAK/global_functions.py
 TreeSAK/iTOL.py
 TreeSAK/parse_deltall_stdout.py
+TreeSAK/prep_mcmctree_ctl.py
 TreeSAK/rename_leaves.py
+TreeSAK/replace_clades.py
+TreeSAK/root_with_out_group.py
 TreeSAK/subset_tree.py
 TreeSAK/test_1.py
 TreeSAK.egg-info/PKG-INFO
 TreeSAK.egg-info/SOURCES.txt
 TreeSAK.egg-info/dependency_links.txt
 TreeSAK.egg-info/requires.txt
 TreeSAK.egg-info/top_level.txt
```

### Comparing `TreeSAK-1.9.1/bin/TreeSAK` & `TreeSAK-1.9.2/bin/TreeSAK`

 * *Files 1% similar despite different names*

```diff
@@ -243,18 +243,22 @@
         AssessMarkerDeltaLL.AssessMarkerDeltaLL(args)
 
     elif sys.argv[1] == 'Dating':
         from TreeSAK import Dating
         Dating_parser = subparsers.add_parser('Dating', usage=Dating.Dating_usage)
         Dating_parser.add_argument('-deltall', required=True,                          help='DeltaLL stdout')
         Dating_parser.add_argument('-aod',     required=True,                          help='AssessMarkerDeltaLL output dir')
+        Dating_parser.add_argument('-og',      required=True,                          help='outgroup leaves, one leaf id per line')
+        Dating_parser.add_argument('-eu',      required=True,                          help='EU tree with time constraints')
         Dating_parser.add_argument('-o',       required=True,                          help='dating wd')
         Dating_parser.add_argument('-c',       required=False, default='25-50-75-100', help='cutoffs, default: 25-50-75-100')
         Dating_parser.add_argument('-mmn',     required=False, default=20, type=int,   help='minimal marker number, default: 20')
+        Dating_parser.add_argument('-ra',      required=False, default=45, type=int,   help='root age, default: 45')
         Dating_parser.add_argument('-jst',     required=False, default='6',            help='threads to request in job script, for performing dating')
+        Dating_parser.add_argument('-qsub',    required=False, action="store_true",    help='submit job scripts for getting in.BV')
         Dating_parser.add_argument('-f',       required=False, action="store_true",    help='force overwrite')
         args = vars(parser.parse_args())
         Dating.Dating(args)
 
     else:
         print('Unrecognized command: %s, program exited' % sys.argv[1])
         exit()
```

### Comparing `TreeSAK-1.9.1/images/Bioinformatics.jpg` & `TreeSAK-1.9.2/images/Bioinformatics.jpg`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/images/windows_cmds.docx` & `TreeSAK-1.9.2/images/windows_cmds.docx`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/images/windows_cmds.pdf` & `TreeSAK-1.9.2/images/windows_cmds.pdf`

 * *Files identical despite different names*

### Comparing `TreeSAK-1.9.1/setup.py` & `TreeSAK-1.9.2/setup.py`

 * *Files identical despite different names*

