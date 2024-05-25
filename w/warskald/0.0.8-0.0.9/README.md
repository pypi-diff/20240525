# Comparing `tmp/warskald-0.0.8-py3-none-any.whl.zip` & `tmp/warskald-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 34998 bytes, number of entries: 17
+Zip file size: 35261 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      140 b- defN 24-May-15 08:41 warskald/__init__.py
 -rw-rw-r--  2.0 unx      302 b- defN 24-May-15 08:41 warskald/_globals.py
 -rw-rw-r--  2.0 unx     1215 b- defN 24-May-15 08:41 warskald/attr_dict.py
 -rw-rw-r--  2.0 unx     1770 b- defN 24-May-15 08:41 warskald/git_util.py
 -rw-rw-r--  2.0 unx    12921 b- defN 24-May-15 08:41 warskald/ng_scaffold.py
 -rw-rw-r--  2.0 unx      890 b- defN 24-May-15 08:41 warskald/ng_serve.py
--rw-rw-r--  2.0 unx    26797 b- defN 24-May-15 08:41 warskald/ngwidget.py
+-rw-rw-r--  2.0 unx    26820 b- defN 24-May-15 09:42 warskald/ngwidget.py
 -rw-rw-r--  2.0 unx     1731 b- defN 24-May-15 08:41 warskald/req_utils.py
 -rw-rw-r--  2.0 unx     8646 b- defN 24-May-15 08:41 warskald/reqs_gen.py
 -rw-rw-r--  2.0 unx      471 b- defN 24-May-15 08:41 warskald/run_ngwidget.py
 -rw-rw-r--  2.0 unx    14748 b- defN 24-May-15 08:41 warskald/utils.py
 -rw-rw-r--  2.0 unx     3440 b- defN 24-May-15 08:41 warskald/wspub.py
--rw-rw-r--  2.0 unx    35149 b- defN 24-May-15 08:46 warskald-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx      195 b- defN 24-May-15 08:46 warskald-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-15 08:46 warskald-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-May-15 08:46 warskald-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1316 b- defN 24-May-15 08:46 warskald-0.0.8.dist-info/RECORD
-17 files, 109832 bytes uncompressed, 32870 bytes compressed:  70.1%
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-15 09:43 warskald-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      195 b- defN 24-May-15 09:43 warskald-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-15 09:43 warskald-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       52 b- defN 24-May-15 09:43 warskald-0.0.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 24-May-15 09:43 warskald-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1412 b- defN 24-May-15 09:43 warskald-0.0.9.dist-info/RECORD
+18 files, 110003 bytes uncompressed, 32975 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -30,23 +30,26 @@
 
 Filename: warskald/utils.py
 Comment: 
 
 Filename: warskald/wspub.py
 Comment: 
 
-Filename: warskald-0.0.8.dist-info/LICENSE
+Filename: warskald-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: warskald-0.0.8.dist-info/METADATA
+Filename: warskald-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: warskald-0.0.8.dist-info/WHEEL
+Filename: warskald-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: warskald-0.0.8.dist-info/top_level.txt
+Filename: warskald-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: warskald-0.0.8.dist-info/RECORD
+Filename: warskald-0.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: warskald-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## warskald/ngwidget.py

```diff
@@ -767,11 +767,13 @@
     write_prime_templates()
         
     build_widget_config()
     
     update_index_file(GLOBALS.COMPS_INDEX)
 
 # endregion Widget Functions
+def main():
+    get_template_vals()
+    create_widget()
     
 if(__name__ == '__main__'):
-    get_template_vals()
-    create_widget()
+    main()
```

## Comparing `warskald-0.0.8.dist-info/LICENSE` & `warskald-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `warskald-0.0.8.dist-info/RECORD` & `warskald-0.0.9.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 warskald/__init__.py,sha256=-lgRr_CfGAlpaleJQmRQdo6EO0_vapqnLtCMQArSRPM,140
 warskald/_globals.py,sha256=sFNxZZk0KXjQJ49XGAPJoxMvcV_76XXkcNOIQb1clXU,302
 warskald/attr_dict.py,sha256=fOHqjHLaStNL5FhQgadHPaG25IL73c8G8tnWPlO0gas,1215
 warskald/git_util.py,sha256=mLjH2A3MmAEtQun9fet5KPDYvUeYvv1dYeRS5uIYQLw,1770
 warskald/ng_scaffold.py,sha256=cbUGyUbnGRKrCsOYzKEwhQwTcvqLB8X7aHxAt6lQBU8,12921
 warskald/ng_serve.py,sha256=K1OdjHcVdbPSOdOOt2X0355ti3u0dpGBRP-OyuHWguo,890
-warskald/ngwidget.py,sha256=vqqi3QeSQo9YGVEkAR-GWl2FGeX0gM4HJDoY5_LfAyk,26797
+warskald/ngwidget.py,sha256=-9OHLNduEpa2ufPSRgAXToCM-3hxfwbmycKS1XxKMls,26820
 warskald/req_utils.py,sha256=SKohGiIjinYZM8jGmefZF5wSUlI7LKZ8vGHFyA-TuJk,1731
 warskald/reqs_gen.py,sha256=o6ugtpfmD7FwpbFRA73p_X1eOSHK60-nsEXMwMUHE_g,8646
 warskald/run_ngwidget.py,sha256=PQ3E2UlemCMp4xUq9s7TV8LjkzcpcjrE_u0BD23lkHY,471
 warskald/utils.py,sha256=Yur5bGm4PaFikG-U1XeSUpUNuOecE1g2ySCQn2RJOm8,14748
 warskald/wspub.py,sha256=kG0Y1vv6vJPi-Jl0KajFSf1q6pCQ9dA_YukLsyELpOY,3440
-warskald-0.0.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-warskald-0.0.8.dist-info/METADATA,sha256=0K79nqbpTLD_AUHwB_XG5T7XR_GnGJvAY-mRFqyRm9s,195
-warskald-0.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-warskald-0.0.8.dist-info/top_level.txt,sha256=I_fvpkATuaXWoWzGmKopVBYWQOyePiuU0TmizAHIgB4,9
-warskald-0.0.8.dist-info/RECORD,,
+warskald-0.0.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+warskald-0.0.9.dist-info/METADATA,sha256=lsgH27Oj8sleyU2F28o1xDM676q-fWNZJhn_ErFqY0Q,195
+warskald-0.0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+warskald-0.0.9.dist-info/entry_points.txt,sha256=df_QxWYb5u37FWmolm8_RgVqrcUZpVWmJzd0wqafePk,52
+warskald-0.0.9.dist-info/top_level.txt,sha256=I_fvpkATuaXWoWzGmKopVBYWQOyePiuU0TmizAHIgB4,9
+warskald-0.0.9.dist-info/RECORD,,
```

