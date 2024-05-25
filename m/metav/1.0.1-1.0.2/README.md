# Comparing `tmp/metav-1.0.1.tar.gz` & `tmp/metav-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\metav-1.0.1.tar", last modified: Thu May 16 11:13:41 2024, max compression
+gzip compressed data, was "dist\metav-1.0.2.tar", last modified: Fri May 24 13:39:14 2024, max compression
```

## Comparing `metav-1.0.1.tar` & `metav-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:13:41.000000 metav-1.0.1/
--rw-rw-rw-   0        0        0    26526 2023-03-06 15:44:50.000000 metav-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    11107 2024-05-16 11:13:41.000000 metav-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9851 2024-05-16 11:05:18.000000 metav-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:13:41.000000 metav-1.0.1/metav/
--rw-rw-rw-   0        0        0      177 2023-12-20 05:11:07.000000 metav-1.0.1/metav/__init__.py
--rw-rw-rw-   0        0        0     7201 2024-05-16 11:13:19.000000 metav-1.0.1/metav/main.py
--rw-rw-rw-   0        0        0    22961 2023-12-28 07:57:01.000000 metav-1.0.1/metav/my_func.py
--rw-rw-rw-   0        0        0    20669 2024-01-23 05:45:37.000000 metav-1.0.1/metav/pecorec.py
--rw-rw-rw-   0        0        0    17660 2024-01-23 05:45:37.000000 metav-1.0.1/metav/secorec.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:13:41.000000 metav-1.0.1/metav.egg-info/
--rw-rw-rw-   0        0        0    11107 2024-05-16 11:13:41.000000 metav-1.0.1/metav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-16 11:13:41.000000 metav-1.0.1/metav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:13:41.000000 metav-1.0.1/metav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-05-16 11:13:41.000000 metav-1.0.1/metav.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 11:13:41.000000 metav-1.0.1/metav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:13:41.000000 metav-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1433 2024-05-16 11:13:00.000000 metav-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:39:14.000000 metav-1.0.2/
+-rw-rw-rw-   0        0        0    26526 2023-03-06 15:44:50.000000 metav-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    11585 2024-05-24 13:39:14.000000 metav-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10324 2024-05-24 13:36:51.000000 metav-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 13:39:14.000000 metav-1.0.2/metav/
+-rw-rw-rw-   0        0        0      177 2023-12-20 05:11:07.000000 metav-1.0.2/metav/__init__.py
+-rw-rw-rw-   0        0        0     7199 2024-05-24 13:16:38.000000 metav-1.0.2/metav/main.py
+-rw-rw-rw-   0        0        0    22839 2024-05-24 12:53:52.000000 metav-1.0.2/metav/my_func.py
+-rw-rw-rw-   0        0        0    20681 2024-05-24 12:58:57.000000 metav-1.0.2/metav/pecorec.py
+-rw-rw-rw-   0        0        0    17672 2024-05-24 12:58:57.000000 metav-1.0.2/metav/secorec.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:39:14.000000 metav-1.0.2/metav.egg-info/
+-rw-rw-rw-   0        0        0    11585 2024-05-24 13:39:14.000000 metav-1.0.2/metav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-24 13:39:14.000000 metav-1.0.2/metav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:39:14.000000 metav-1.0.2/metav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-05-24 13:39:14.000000 metav-1.0.2/metav.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 13:39:14.000000 metav-1.0.2/metav.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:39:14.000000 metav-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2024-05-24 13:37:24.000000 metav-1.0.2/setup.py
```

### Comparing `metav-1.0.1/LICENSE` & `metav-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metav-1.0.1/PKG-INFO` & `metav-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metav
-Version: 1.0.1
+Version: 1.0.2
 Summary: rapid detection and classification of viruses in metagenomics sequencing.
 Home-page: https://github.com/ZhijianZhou01/nextvirus
 Author: Zhi-Jian Zhou
 Author-email: zjzhou@hnu.edu.cn
 Keywords: virus detection,sequencing,metagenomics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -113,17 +113,17 @@
 |-i1 FORWARD | forward reads (*.fq) using paired-end sequencing.|
 |-i2 REVERSE | reverse reads (*.fq) using paired-end sequencing.|
 |-u UNPAIRED | reads file using single-end sequencing (unpaired reads).|
 |-q QUALITIES | the qualities (phred33 or phred64) of sequenced reads, default: phred33.|
 |-xml PROFILES | the *.xml file with parameters of dependent software and databases.|
 |-len LENGTH | threshold of length of aa alignment in diamond, default: 10.|
 |-s IDENTITY | threshold of identity(%) of alignment aa in diamond, default: 20.|
-|-e E_VALUE | specify three e-values threshold used to filter the reads (or contigs) hit viral nr database, default: 1e-6,1e-3,1e-1.|
-|-r1 | run the sub-pipeline 1 (reads → viral nr).|
-|-r2 | run the sub-pipeline 2 (reads → contigs → viral nr).|
+|-e E_VALUE | specify three e-values threshold used to filter the reads (or contigs) hit nr database, default: 1e-6,1e-3,1e-1.|
+|-r1 | run the sub-pipeline 1 (reads → nr database).|
+|-r2 | run the sub-pipeline 2 (reads → contigs → nr database).|
 |-t THREAD | number of used threads, default: 1.|
 |-o OUTDIR | output directory to store all results.|
 
 
 ## 7. Example of usage
 
 + <b>if reads are from paired-end sequencing:</b>
@@ -168,15 +168,15 @@
 identity_threshold:	20.0
 e-value:	['1e-6', '1e-3', '1e-1']
 thread:	8
 outdir:	/home/zzj/datas/test/out6
 ```
 
 ### 8.2. directory pipeline1
-the directory `pipeline1` contains intermediate results and `finally_result` from `sub-pipeline 1` (reads → viral nr). 
+the directory `pipeline1` contains intermediate results and `finally_result` from `sub-pipeline 1` (reads → nr database). 
 
 In the example, three thresholds (`1e-6`, `1e-3` and `1e-1`) of e-value are used to filter the output diamond program. Thus, three corresponding sub-directories is created and used to store results. 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/e-value.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/e-value.png)
 
 The meanings of directory name with e-value in `pipeline1` are as follows,
 
 | sub-directories | description |
@@ -191,15 +191,15 @@
 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/reads_summary.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/reads_summary.png)
 
 <b>In particular, metav extract all hit reads sequences (*fasta format) according to the hierarchical relationship of `order`, `family` and `strain`(organism)</b>. These hit reads sequences are stored in directory `hit_reads_seq`.
 
 
 ### 8.3. directory pipeline2
-the directory `pipeline2` contains intermediate results and `finally_result` from `sub-pipeline 2` (reads → contigs → viral nr). The hierarchy of the directory of output results is the same as directory `pipeline1`.
+the directory `pipeline2` contains intermediate results and `finally_result` from `sub-pipeline 2` (reads → contigs → nr database). The hierarchy of the directory of output results is the same as directory `pipeline1`.
 
 However, the output in directory `finally_result` of the directory `pipeline2` are hit contigs, not reads.
 
 The meanings of directory name with e-value in `pipeline2` are as follows,
 
 | sub-directories | description |
 | --- | --- |
@@ -208,12 +208,17 @@
 |lower_0.1 | `1e-3` < e-value of hit contigs < `1e-1` |
 
 In the directory `hit_summary` of each sub-directory with e-value, the sequences and summary information of hit contigs are provided, and these hit contigs sequences are stored in directory `hit_contigs_seq`.
 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/contigs_symmary.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/contigs_symmary.png)
 
 
+## 9. Functional expansion
+metav was originally designed to detect and count the viral composition of metagenomics-sequencing-data, but it's flexible and not limited to viruses.
 
-## 9. Bug report
+In fact, the viral nr database can be replaced by protein databases of other pathogenic, for example, bacteria, pathogenic fungi. In a word, metav can detect and count other pathogens of metagenomics-sequencing-data by using the corresponding nr database and taxonomy information file.
+
+
+## 10. Bug report
 metav was test on Ubuntu 16.04 and Ubuntu 20.02, which can work well. If you run into a problem or find a bug, please contact us.
 
 [Github issues](https://github.com/ZhijianZhou01/BioAider/issues) or send email to zjzhou@hnu.edu.cn.
```

### Comparing `metav-1.0.1/README.md` & `metav-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -89,17 +89,17 @@
 |-i1 FORWARD | forward reads (*.fq) using paired-end sequencing.|
 |-i2 REVERSE | reverse reads (*.fq) using paired-end sequencing.|
 |-u UNPAIRED | reads file using single-end sequencing (unpaired reads).|
 |-q QUALITIES | the qualities (phred33 or phred64) of sequenced reads, default: phred33.|
 |-xml PROFILES | the *.xml file with parameters of dependent software and databases.|
 |-len LENGTH | threshold of length of aa alignment in diamond, default: 10.|
 |-s IDENTITY | threshold of identity(%) of alignment aa in diamond, default: 20.|
-|-e E_VALUE | specify three e-values threshold used to filter the reads (or contigs) hit viral nr database, default: 1e-6,1e-3,1e-1.|
-|-r1 | run the sub-pipeline 1 (reads → viral nr).|
-|-r2 | run the sub-pipeline 2 (reads → contigs → viral nr).|
+|-e E_VALUE | specify three e-values threshold used to filter the reads (or contigs) hit nr database, default: 1e-6,1e-3,1e-1.|
+|-r1 | run the sub-pipeline 1 (reads → nr database).|
+|-r2 | run the sub-pipeline 2 (reads → contigs → nr database).|
 |-t THREAD | number of used threads, default: 1.|
 |-o OUTDIR | output directory to store all results.|
 
 
 ## 7. Example of usage
 
 + <b>if reads are from paired-end sequencing:</b>
@@ -144,15 +144,15 @@
 identity_threshold:	20.0
 e-value:	['1e-6', '1e-3', '1e-1']
 thread:	8
 outdir:	/home/zzj/datas/test/out6
 ```
 
 ### 8.2. directory pipeline1
-the directory `pipeline1` contains intermediate results and `finally_result` from `sub-pipeline 1` (reads → viral nr). 
+the directory `pipeline1` contains intermediate results and `finally_result` from `sub-pipeline 1` (reads → nr database). 
 
 In the example, three thresholds (`1e-6`, `1e-3` and `1e-1`) of e-value are used to filter the output diamond program. Thus, three corresponding sub-directories is created and used to store results. 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/e-value.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/e-value.png)
 
 The meanings of directory name with e-value in `pipeline1` are as follows,
 
 | sub-directories | description |
@@ -167,15 +167,15 @@
 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/reads_summary.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/reads_summary.png)
 
 <b>In particular, metav extract all hit reads sequences (*fasta format) according to the hierarchical relationship of `order`, `family` and `strain`(organism)</b>. These hit reads sequences are stored in directory `hit_reads_seq`.
 
 
 ### 8.3. directory pipeline2
-the directory `pipeline2` contains intermediate results and `finally_result` from `sub-pipeline 2` (reads → contigs → viral nr). The hierarchy of the directory of output results is the same as directory `pipeline1`.
+the directory `pipeline2` contains intermediate results and `finally_result` from `sub-pipeline 2` (reads → contigs → nr database). The hierarchy of the directory of output results is the same as directory `pipeline1`.
 
 However, the output in directory `finally_result` of the directory `pipeline2` are hit contigs, not reads.
 
 The meanings of directory name with e-value in `pipeline2` are as follows,
 
 | sub-directories | description |
 | --- | --- |
@@ -184,12 +184,17 @@
 |lower_0.1 | `1e-3` < e-value of hit contigs < `1e-1` |
 
 In the directory `hit_summary` of each sub-directory with e-value, the sequences and summary information of hit contigs are provided, and these hit contigs sequences are stored in directory `hit_contigs_seq`.
 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/contigs_symmary.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/contigs_symmary.png)
 
 
+## 9. Functional expansion
+metav was originally designed to detect and count the viral composition of metagenomics-sequencing-data, but it's flexible and not limited to viruses.
 
-## 9. Bug report
+In fact, the viral nr database can be replaced by protein databases of other pathogenic, for example, bacteria, pathogenic fungi. In a word, metav can detect and count other pathogens of metagenomics-sequencing-data by using the corresponding nr database and taxonomy information file.
+
+
+## 10. Bug report
 metav was test on Ubuntu 16.04 and Ubuntu 20.02, which can work well. If you run into a problem or find a bug, please contact us.
 
 [Github issues](https://github.com/ZhijianZhou01/BioAider/issues) or send email to zjzhou@hnu.edu.cn.
```

### Comparing `metav-1.0.1/metav/main.py` & `metav-1.0.2/metav/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,30 +95,30 @@
             "-s", dest="identity",
             help="threshold of identity(%%) of alignment aa in diamond, default: 20.",
             type=float,
             default=20)
 
       parser.add_argument(
             "-e",dest="e_value",
-            help="specify three e-values threshold used to filter the reads (or contigs) hit viral nr database, default: 1e-6,1e-3,1e-1.",
+            help="specify three e-values threshold used to filter the reads (or contigs) hit nr database, default: 1e-6,1e-3,1e-1.",
             type=str,
             default="1e-6,1e-3,1e-1")
 
 
       parser.add_argument(
             "-r1",
             dest="run1",
             action="store_true",
-            help="run the sub-pipeline 1 (reads → viral nr).")
+            help="run the sub-pipeline 1 (reads → nr database).")
 
       parser.add_argument(
             "-r2",
             action="store_true",
             dest="run2",
-            help="run the sub-pipeline 2 (reads → contigs → viral nr).")
+            help="run the sub-pipeline 2 (reads → contigs → nr database).")
 
 
       parser.add_argument(
             "-t", dest="thread",
             help="number of used threads, default: 1.",
             type=int,
             default=1)
@@ -144,15 +144,15 @@
 
       print("  Name: Metagenomics virus detection (MetaV)")
 
 
       print(
             "  Description: rapid detection and classification of viruses in metagenomics sequencing.")
 
-      print("  Version: 1.0.1 (2023-12-20)")
+      print("  Version: 1.02 (2024-5-24)")
 
       print("  Author: Zhi-Jian Zhou")
 
 
       print("-------------------------------------------------" + "\n")
```

### Comparing `metav-1.0.1/metav/my_func.py` & `metav-1.0.2/metav/my_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -249,15 +249,15 @@
 
 def reads_diamond_class(reads_R1_path,
                   reads_R2_path,
                   filter_result_path,
                   refer_spiece_path,
                   out_dir):
     """
-    viral reads classifier
+    hit reads classifier
     :param reads_R1_path: the file-path of the forward sequencing reads
     :param reads_R2_path: the file-path of the reverse sequencing reads
     :param filter_result_path: the path of the filter file of diamond
     :param refer_spiece_path: the file-path of taxonomic information of viruses
     :param out_dir: the output directory
     :return: None
     """
@@ -268,15 +268,15 @@
         filter_result_list = filter_result_file.read().strip().split("\n")
 
     for n in range(1, len(filter_result_list)):
         line = filter_result_list[n]
 
         qseqid = line.split("\t")[0]  # the ID of reads (query sequence)
 
-        sseqid = line.split("\t")[1]  # the subject ID (from viral protein database)
+        sseqid = line.split("\t")[1]  # the subject ID (from protein database)
 
         stitle = line.split("\t")[2].replace(sseqid, "").strip()
 
         qst = (qseqid + "\t" + sseqid + "\t" + stitle)
 
         qst_list.append(qst)
 
@@ -321,19 +321,19 @@
 
 
     # count the number of reads
 
     with open(qst_AlesDae_path, "r",encoding="utf-8") as qst_AlesDae_input:
         qst_AlesDae_list = qst_AlesDae_input.readlines()
 
-    virus_ale_dic = {}  # dictionary that stores viral order
+    virus_ale_dic = {}  # dictionary that stores hit order
 
-    virus_dae_dic = {}  # dictionary that stores viral family
+    virus_dae_dic = {}  # dictionary that stores hit family
 
-    virus_strain_dic = {}  # dictionary that stores viral strain
+    virus_strain_dic = {}  # dictionary that stores hit strain
 
 
     for each_line in qst_AlesDae_list:
 
         each_line = each_line.strip()
 
         each_line_list = each_line.split("\t")
@@ -360,30 +360,30 @@
         if virus_dae_name not in virus_dae_dic:
             virus_dae_dic[virus_dae_name] = 1
         else:
             virus_dae_dic[virus_dae_name] += 1
 
 
     # output
-    # reads count based on viral strain
-    with open(out_dir + r"/viral_strain_count.csv", "w",encoding="utf-8") as virus_strain_out:
-        virus_strain_out.write("hit viral strain" + "," + "reads count" + "\n")
+    # reads count based on hit strain
+    with open(out_dir + r"/hit_strain_count.csv", "w",encoding="utf-8") as virus_strain_out:
+        virus_strain_out.write("hit strain" + "," + "reads count" + "\n")
         for key in list(virus_strain_dic.keys()):
             virus_strain_out.write(key + "," + str(virus_strain_dic[key])
                                    + "\n")
     
-    # reads count based on viral order
-    with open(out_dir + r"/viral_order_count.csv", "w",encoding="utf-8") as virus_ales_out:
-        virus_ales_out.write("hit viral order" + "," + "reads count" + "\n")
+    # reads count based on hit order
+    with open(out_dir + r"/hit_order_count.csv", "w",encoding="utf-8") as virus_ales_out:
+        virus_ales_out.write("hit order" + "," + "reads count" + "\n")
         for key in list(virus_ale_dic.keys()):
             virus_ales_out.write(key + "," + str(virus_ale_dic[key]) + "\n")
 
-    # reads count based on viral family
-    with open(out_dir + r"/viral_family_count.csv", "w",encoding="utf-8") as virus_dae_out:
-        virus_dae_out.write("hit viral family" + "," + "reads count" + "\n")
+    # reads count based on hit family
+    with open(out_dir + r"/hit_family_count.csv", "w",encoding="utf-8") as virus_dae_out:
+        virus_dae_out.write("hit family" + "," + "reads count" + "\n")
         for key in list(virus_dae_dic.keys()):
             virus_dae_out.write(key + "," + str(virus_dae_dic[key]) + "\n")
 
     # get the original sequence
     reads_dic = {}
 
     with open(reads_R1_path, "r",encoding="utf-8") as reads_file:
@@ -433,16 +433,16 @@
 
 
 def contig_diamond_class(contig_path,
                          filter_result_path,
                          refer_spiece_path,
                          out_dir):
     """
-    viral contigs classifier
-    :param contig_path: the path of viral contigs
+    hit contigs classifier
+    :param contig_path: the path of hit contigs
     :param filter_result_path: the path of the filter file of diamond
     :param refer_spiece_path: the file-path of taxonomic information of viruses
     :param out_dir: the output directory
     :return: None
     """
 
     qst_list = []
@@ -531,49 +531,49 @@
         virus_ale_name = each_line_list[-3].strip()
 
         virus_dae_name = each_line_list[-2].strip()
 
         virus_name = each_line_list[-1].strip()
 
 
-        # contig count based on viral strains
+        # contig count based on hit strains
         if virus_name not in virus_strain_dic:
             virus_strain_dic[virus_name] = 1
         else:
             virus_strain_dic[virus_name] += 1
 
-        # contig count based on viral order
+        # contig count based on hit order
         if virus_ale_name not in virus_ale_dic:
             virus_ale_dic[virus_ale_name] = 1
         else:
             virus_ale_dic[virus_ale_name] += 1
 
-        # contig count based on viral family
+        # contig count based on hit family
         if virus_dae_name not in virus_dae_dic:
             virus_dae_dic[virus_dae_name] = 1
         else:
             virus_dae_dic[virus_dae_name] += 1
 
 
-    with open(out_dir + r"/viral_strain_count.csv", "w",
+    with open(out_dir + r"/hit_strain_count.csv", "w",
               encoding="utf-8") as virus_strain_out:
-        virus_strain_out.write("hit viral strain" + "," + "contig count" + "\n")
+        virus_strain_out.write("hit strain" + "," + "contig count" + "\n")
         for key in list(virus_strain_dic.keys()):
             virus_strain_out.write(key + "," + str(virus_strain_dic[key])
                                    + "\n")
 
-    with open(out_dir + r"/viral_order_count.csv", "w",
+    with open(out_dir + r"/hit_order_count.csv", "w",
               encoding="utf-8") as virus_ales_out:
-        virus_ales_out.write("hit viral order" + "," + "contig count" + "\n")
+        virus_ales_out.write("hit order" + "," + "contig count" + "\n")
         for key in list(virus_ale_dic.keys()):
             virus_ales_out.write(key + "," + str(virus_ale_dic[key]) + "\n")
 
-    with open(out_dir + r"/viral_family_count.csv", "w",
+    with open(out_dir + r"/hit_family_count.csv", "w",
               encoding="utf-8") as virus_dae_out:
-        virus_dae_out.write("hit viral family" + "," + "contig count" + "\n")
+        virus_dae_out.write("hit family" + "," + "contig count" + "\n")
         for key in list(virus_dae_dic.keys()):
             virus_dae_out.write(key + "," + str(virus_dae_dic[key]) + "\n")
 
 
     contig_dic = read_fasta_dic(contig_path)
 
 
@@ -604,15 +604,15 @@
 
 
 def reads_diamond_class2(reads_path,
                         filter_result_path,
                         refer_spiece_path,
                         out_dir):
     """
-    viral reads classifier
+    hit reads classifier
     :param reads_path: the file-path of the single-end sequencing reads
     :param filter_result_path: the path of the filter file of diamond
     :param refer_spiece_path: the file-path of taxonomic information of viruses
     :param out_dir: the output directory
     :return: None
     """
 
@@ -623,15 +623,15 @@
 
     for n in range(1, len(filter_result_list)):
         line = filter_result_list[n]
 
         qseqid = line.split("\t")[0]  # the ID of reads (query sequence)
 
         sseqid = line.split("\t")[
-            1]  # the subject ID (from viral protein database)
+            1]  # the subject ID (from protein database)
 
         stitle = line.split("\t")[2].replace(sseqid, "").strip()
 
         qst = (qseqid + "\t" + sseqid + "\t" + stitle)
 
         qst_list.append(qst)
 
@@ -676,19 +676,19 @@
     qst_AlesDae.close()
 
     # count the number of reads
 
     with open(qst_AlesDae_path, "r", encoding="utf-8") as qst_AlesDae_input:
         qst_AlesDae_list = qst_AlesDae_input.readlines()
 
-    virus_ale_dic = {}  # dictionary that stores viral order
+    virus_ale_dic = {}  # dictionary that stores hit order
 
-    virus_dae_dic = {}  # dictionary that stores viral family
+    virus_dae_dic = {}  # dictionary that stores hit family
 
-    virus_strain_dic = {}  # dictionary that stores viral strain
+    virus_strain_dic = {}  # dictionary that stores hit strain
 
     for each_line in qst_AlesDae_list:
 
         each_line = each_line.strip()
 
         each_line_list = each_line.split("\t")
 
@@ -711,33 +711,33 @@
 
         if virus_dae_name not in virus_dae_dic:
             virus_dae_dic[virus_dae_name] = 1
         else:
             virus_dae_dic[virus_dae_name] += 1
 
     # output
-    # reads count based on viral strain
-    with open(out_dir + r"/viral_strain_count.csv", "w",
+    # reads count based on hit strain
+    with open(out_dir + r"/hit_strain_count.csv", "w",
               encoding="utf-8") as virus_strain_out:
-        virus_strain_out.write("hit viral strain" + "," + "reads count" + "\n")
+        virus_strain_out.write("hit strain" + "," + "reads count" + "\n")
         for key in list(virus_strain_dic.keys()):
             virus_strain_out.write(key + "," + str(virus_strain_dic[key])
                                    + "\n")
 
-    # reads count based on viral order
-    with open(out_dir + r"/viral_order_count.csv", "w",
+    # reads count based on hit order
+    with open(out_dir + r"/hit_order_count.csv", "w",
               encoding="utf-8") as virus_ales_out:
-        virus_ales_out.write("hit viral order" + "," + "reads count" + "\n")
+        virus_ales_out.write("hit order" + "," + "reads count" + "\n")
         for key in list(virus_ale_dic.keys()):
             virus_ales_out.write(key + "," + str(virus_ale_dic[key]) + "\n")
 
-    # reads count based on viral family
-    with open(out_dir + r"/viral_family_count.csv", "w",
+    # reads count based on hit family
+    with open(out_dir + r"/hit_family_count.csv", "w",
               encoding="utf-8") as virus_dae_out:
-        virus_dae_out.write("hit viral family" + "," + "reads count" + "\n")
+        virus_dae_out.write("hit family" + "," + "reads count" + "\n")
         for key in list(virus_dae_dic.keys()):
             virus_dae_out.write(key + "," + str(virus_dae_dic[key]) + "\n")
 
     # get the original sequence
     reads_dic = {}
 
     with open(reads_path, "r", encoding="utf-8") as reads_file:
```

### Comparing `metav-1.0.1/metav/pecorec.py` & `metav-1.0.2/metav/pecorec.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     return clean_data1_path,clean_data2_path
 
 
 
 def sub_run1(parameter_dic,xml_dic,clean_data1_path,clean_data2_path):
 
     """
-    the sub-pipeline of nextvirus, reads → viral nr
+    the sub-pipeline of nextvirus, reads → nr database
     :param parameter_dic:
     :param xml_dic:
     :param clean_data1_path: fq format of cleaned forward reads
     :param clean_data2_path: fq format of cleaned reverse reads
     :return:
     """
     out_dir = parameter_dic["outdir"] + "/pipeline1"
@@ -306,15 +306,15 @@
     diamond_commond = diamond_commond1 + ";" + diamond_commond2
 
     print(diamond_commond)
 
     runprocess(diamond_commond)
 
 
-    print(">>> " + "reads map to viral nr: completed!",
+    print(">>> " + "reads map to nr database: completed!",
           time.strftime("%Y.%m.%d %H:%M:%S ", time.localtime(time.time())))
 
     print("\n")
 
 
     # Step 5. filter the results from dimond
 
@@ -431,15 +431,15 @@
     return
 
 
 
 
 def sub_run2(parameter_dic,xml_dic,clean_data1_path,clean_data2_path):
     """
-    the sub-pipeline of nextvirus, reads → contigs → viral nr
+    the sub-pipeline of nextvirus, reads → contigs → nr database
     :param parameter_dic:
     :param xml_dic:
     :param clean_data1_path: fq format of cleaned forward reads
     :param clean_data2_path: fq format of cleaned reverse reads
     :return:
     """
 
@@ -527,15 +527,15 @@
 
     diamond_commond = " ".join(diamond_commond_list)
 
     print(diamond_commond)
     runprocess(diamond_commond)
 
 
-    print(">>> " + "contigs map to viral nr: completed!",
+    print(">>> " + "contigs map to nr database: completed!",
           time.strftime("%Y.%m.%d %H:%M:%S ", time.localtime(time.time())))
 
     print("\n")
 
 
     # Step 6. filter the results from dimond
```

### Comparing `metav-1.0.1/metav/secorec.py` & `metav-1.0.2/metav/secorec.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     return clean_data_fas
 
 
 
 def sub_run1(parameter_dic,xml_dic,clean_data_fas):
 
     """
-    the sub-pipeline of nextvirus, reads → viral nr
+    the sub-pipeline of nextvirus, reads → nr database
     :param parameter_dic:
     :param xml_dic:
     :param clean_data_fas: fasta format of cleaned reads
     :return:
     """
 
 
@@ -266,15 +266,15 @@
 
 
     print(diamond_commond)
 
     runprocess(diamond_commond)
 
 
-    print(">>> " + "reads map to viral nr: completed!",
+    print(">>> " + "reads map to nr database: completed!",
           time.strftime("%Y.%m.%d %H:%M:%S ", time.localtime(time.time())))
 
     print("\n")
 
 
     # Step 5. filter the results from dimond
 
@@ -383,15 +383,15 @@
     return
 
 
 
 
 def sub_run2(parameter_dic,xml_dic,clean_data_fas):
     """
-    the sub-pipeline of nextvirus, reads → contigs → viral nr
+    the sub-pipeline of nextvirus, reads → contigs → nr database
     :param parameter_dic:
     :param xml_dic:
     :param clean_data_fas fasta: format of cleaned reads
     :return:
     """
 
 
@@ -458,15 +458,15 @@
 
     diamond_commond = " ".join(diamond_commond_list)
 
     print(diamond_commond)
     runprocess(diamond_commond)
 
 
-    print(">>> " + "contigs map to viral nr: completed!",
+    print(">>> " + "contigs map to nr database: completed!",
           time.strftime("%Y.%m.%d %H:%M:%S ", time.localtime(time.time())))
 
     print("\n")
 
 
     # Step 6. filter the results from dimond
```

### Comparing `metav-1.0.1/metav.egg-info/PKG-INFO` & `metav-1.0.2/metav.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metav
-Version: 1.0.1
+Version: 1.0.2
 Summary: rapid detection and classification of viruses in metagenomics sequencing.
 Home-page: https://github.com/ZhijianZhou01/nextvirus
 Author: Zhi-Jian Zhou
 Author-email: zjzhou@hnu.edu.cn
 Keywords: virus detection,sequencing,metagenomics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -113,17 +113,17 @@
 |-i1 FORWARD | forward reads (*.fq) using paired-end sequencing.|
 |-i2 REVERSE | reverse reads (*.fq) using paired-end sequencing.|
 |-u UNPAIRED | reads file using single-end sequencing (unpaired reads).|
 |-q QUALITIES | the qualities (phred33 or phred64) of sequenced reads, default: phred33.|
 |-xml PROFILES | the *.xml file with parameters of dependent software and databases.|
 |-len LENGTH | threshold of length of aa alignment in diamond, default: 10.|
 |-s IDENTITY | threshold of identity(%) of alignment aa in diamond, default: 20.|
-|-e E_VALUE | specify three e-values threshold used to filter the reads (or contigs) hit viral nr database, default: 1e-6,1e-3,1e-1.|
-|-r1 | run the sub-pipeline 1 (reads → viral nr).|
-|-r2 | run the sub-pipeline 2 (reads → contigs → viral nr).|
+|-e E_VALUE | specify three e-values threshold used to filter the reads (or contigs) hit nr database, default: 1e-6,1e-3,1e-1.|
+|-r1 | run the sub-pipeline 1 (reads → nr database).|
+|-r2 | run the sub-pipeline 2 (reads → contigs → nr database).|
 |-t THREAD | number of used threads, default: 1.|
 |-o OUTDIR | output directory to store all results.|
 
 
 ## 7. Example of usage
 
 + <b>if reads are from paired-end sequencing:</b>
@@ -168,15 +168,15 @@
 identity_threshold:	20.0
 e-value:	['1e-6', '1e-3', '1e-1']
 thread:	8
 outdir:	/home/zzj/datas/test/out6
 ```
 
 ### 8.2. directory pipeline1
-the directory `pipeline1` contains intermediate results and `finally_result` from `sub-pipeline 1` (reads → viral nr). 
+the directory `pipeline1` contains intermediate results and `finally_result` from `sub-pipeline 1` (reads → nr database). 
 
 In the example, three thresholds (`1e-6`, `1e-3` and `1e-1`) of e-value are used to filter the output diamond program. Thus, three corresponding sub-directories is created and used to store results. 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/e-value.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/e-value.png)
 
 The meanings of directory name with e-value in `pipeline1` are as follows,
 
 | sub-directories | description |
@@ -191,15 +191,15 @@
 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/reads_summary.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/reads_summary.png)
 
 <b>In particular, metav extract all hit reads sequences (*fasta format) according to the hierarchical relationship of `order`, `family` and `strain`(organism)</b>. These hit reads sequences are stored in directory `hit_reads_seq`.
 
 
 ### 8.3. directory pipeline2
-the directory `pipeline2` contains intermediate results and `finally_result` from `sub-pipeline 2` (reads → contigs → viral nr). The hierarchy of the directory of output results is the same as directory `pipeline1`.
+the directory `pipeline2` contains intermediate results and `finally_result` from `sub-pipeline 2` (reads → contigs → nr database). The hierarchy of the directory of output results is the same as directory `pipeline1`.
 
 However, the output in directory `finally_result` of the directory `pipeline2` are hit contigs, not reads.
 
 The meanings of directory name with e-value in `pipeline2` are as follows,
 
 | sub-directories | description |
 | --- | --- |
@@ -208,12 +208,17 @@
 |lower_0.1 | `1e-3` < e-value of hit contigs < `1e-1` |
 
 In the directory `hit_summary` of each sub-directory with e-value, the sequences and summary information of hit contigs are provided, and these hit contigs sequences are stored in directory `hit_contigs_seq`.
 
 ![https://github.com/ZhijianZhou01/metav/blob/main/figure/contigs_symmary.png](https://github.com/ZhijianZhou01/metav/blob/main/figure/contigs_symmary.png)
 
 
+## 9. Functional expansion
+metav was originally designed to detect and count the viral composition of metagenomics-sequencing-data, but it's flexible and not limited to viruses.
 
-## 9. Bug report
+In fact, the viral nr database can be replaced by protein databases of other pathogenic, for example, bacteria, pathogenic fungi. In a word, metav can detect and count other pathogens of metagenomics-sequencing-data by using the corresponding nr database and taxonomy information file.
+
+
+## 10. Bug report
 metav was test on Ubuntu 16.04 and Ubuntu 20.02, which can work well. If you run into a problem or find a bug, please contact us.
 
 [Github issues](https://github.com/ZhijianZhou01/BioAider/issues) or send email to zjzhou@hnu.edu.cn.
```

### Comparing `metav-1.0.1/setup.py` & `metav-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="metav",
-  version="1.0.1",
+  version="1.0.2",
   author="Zhi-Jian Zhou",
   author_email="zjzhou@hnu.edu.cn",
   description="rapid detection and classification of viruses in metagenomics sequencing.",
   keywords="virus detection, sequencing, metagenomics",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ZhijianZhou01/nextvirus",
```

