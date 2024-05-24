# Comparing `tmp/lumipy-1.0.94-py3-none-any.whl.zip` & `tmp/lumipy-1.0.96-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -73,15 +73,15 @@
 -rw-r--r--  2.0 unx      793 b- defN 24-May-23 13:24 lumipy/provider/__init__.py
 -rw-r--r--  2.0 unx     3716 b- defN 24-May-23 13:24 lumipy/provider/api_server.py
 -rw-r--r--  2.0 unx    16297 b- defN 24-May-23 13:24 lumipy/provider/base_provider.py
 -rw-r--r--  2.0 unx     4804 b- defN 24-May-23 13:24 lumipy/provider/common.py
 -rw-r--r--  2.0 unx     5382 b- defN 24-May-23 13:24 lumipy/provider/context.py
 -rw-r--r--  2.0 unx     8754 b- defN 24-May-23 13:24 lumipy/provider/factory.py
 -rw-r--r--  2.0 unx     7061 b- defN 24-May-23 13:24 lumipy/provider/manager.py
--rw-r--r--  2.0 unx       27 b- defN 24-May-23 20:13 lumipy/provider/max_version.py
+-rw-r--r--  2.0 unx       27 b- defN 24-May-24 09:51 lumipy/provider/max_version.py
 -rw-r--r--  2.0 unx     5483 b- defN 24-May-23 13:24 lumipy/provider/metadata.py
 -rw-r--r--  2.0 unx     1262 b- defN 24-May-23 13:24 lumipy/provider/provider_sets.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:24 lumipy/provider/implementation/__init__.py
 -rw-r--r--  2.0 unx     2945 b- defN 24-May-23 13:24 lumipy/provider/implementation/index_builder.py
 -rw-r--r--  2.0 unx     4034 b- defN 24-May-23 13:24 lumipy/provider/implementation/pandas_provider.py
 -rw-r--r--  2.0 unx    10278 b- defN 24-May-23 13:24 lumipy/provider/implementation/test_providers.py
 -rw-r--r--  2.0 unx     5936 b- defN 24-May-23 13:24 lumipy/provider/implementation/world_bank.py
@@ -370,13 +370,13 @@
 -rw-r--r--  2.0 unx        0 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/__init__.py
 -rw-r--r--  2.0 unx    15270 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/test_base_provider.py
 -rw-r--r--  2.0 unx     9063 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/test_context_classes.py
 -rw-r--r--  2.0 unx    23165 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/test_pandas_provider.py
 -rw-r--r--  2.0 unx     2992 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/test_provider_api.py
 -rw-r--r--  2.0 unx     3561 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/test_provider_factory.py
 -rw-r--r--  2.0 unx    13456 b- defN 24-May-23 13:24 lumipy/test/unit/provider_tests/test_provider_manager.py
--rw-r--r--  2.0 unx      691 b- defN 24-May-23 20:13 lumipy-1.0.94.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 20:13 lumipy-1.0.94.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-May-23 20:13 lumipy-1.0.94.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-May-23 20:13 lumipy-1.0.94.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    42170 b- defN 24-May-23 20:13 lumipy-1.0.94.dist-info/RECORD
+-rw-r--r--  2.0 unx      691 b- defN 24-May-24 09:51 lumipy-1.0.96.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 09:51 lumipy-1.0.96.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-May-24 09:51 lumipy-1.0.96.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-May-24 09:51 lumipy-1.0.96.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    42170 b- defN 24-May-24 09:51 lumipy-1.0.96.dist-info/RECORD
 380 files, 5560996 bytes uncompressed, 723306 bytes compressed:  87.0%
```

## zipnote {}

```diff
@@ -1119,23 +1119,23 @@
 
 Filename: lumipy/test/unit/provider_tests/test_provider_factory.py
 Comment: 
 
 Filename: lumipy/test/unit/provider_tests/test_provider_manager.py
 Comment: 
 
-Filename: lumipy-1.0.94.dist-info/METADATA
+Filename: lumipy-1.0.96.dist-info/METADATA
 Comment: 
 
-Filename: lumipy-1.0.94.dist-info/WHEEL
+Filename: lumipy-1.0.96.dist-info/WHEEL
 Comment: 
 
-Filename: lumipy-1.0.94.dist-info/entry_points.txt
+Filename: lumipy-1.0.96.dist-info/entry_points.txt
 Comment: 
 
-Filename: lumipy-1.0.94.dist-info/top_level.txt
+Filename: lumipy-1.0.96.dist-info/top_level.txt
 Comment: 
 
-Filename: lumipy-1.0.94.dist-info/RECORD
+Filename: lumipy-1.0.96.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lumipy-1.0.94.dist-info/METADATA` & `lumipy-1.0.96.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumipy
-Version: 1.0.94
+Version: 1.0.96
 Summary: Python library for Luminesce
 Home-page: UNKNOWN
 Author: FINBOURNE Technology
 Author-email: engineering@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `lumipy-1.0.94.dist-info/RECORD` & `lumipy-1.0.96.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -369,12 +369,12 @@
 lumipy/test/unit/provider_tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lumipy/test/unit/provider_tests/test_base_provider.py,sha256=NkfSAm-Buy7L_pQgRJHcOSOjkuv7_BWHbubYwrpbTiY,15270
 lumipy/test/unit/provider_tests/test_context_classes.py,sha256=TxJ3EFK4bPDp6OgAeT1jx0DCJATAqqclX-cgLSx9If4,9063
 lumipy/test/unit/provider_tests/test_pandas_provider.py,sha256=GVhNPq_-ud-4LSNzvZU6wBbXgdxKq7YPw9lmlcjca2M,23165
 lumipy/test/unit/provider_tests/test_provider_api.py,sha256=ZovhykIlIRzEG5jj7-icLicP9ySW5fRWol02cvJBnGg,2992
 lumipy/test/unit/provider_tests/test_provider_factory.py,sha256=rSQ3SNGqumq-f1w6sCV54DkXcvbWTn3CS4hkFAumAs4,3561
 lumipy/test/unit/provider_tests/test_provider_manager.py,sha256=-TT-3ZGpDsFKMz4efWIy7TGAUVtZ2gTDa67DiorIioc,13456
-lumipy-1.0.94.dist-info/METADATA,sha256=vGmsmmXsKYNlnl94DUnn8L7gwoONBNPTmLmrIh9iIxk,691
-lumipy-1.0.94.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-lumipy-1.0.94.dist-info/entry_points.txt,sha256=WbFEbaJT6BlIlgVgEaxo--H4SjwDX2nEVcCKwih-WG0,47
-lumipy-1.0.94.dist-info/top_level.txt,sha256=DVww8LaQM3Xm0WOgo4JE0epePgCM1xGWWWxh7wuv-CY,7
-lumipy-1.0.94.dist-info/RECORD,,
+lumipy-1.0.96.dist-info/METADATA,sha256=hN5_7k20JzPWLGEd-2D_JT5Jxin0zz5YiZdilY7F1Gg,691
+lumipy-1.0.96.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+lumipy-1.0.96.dist-info/entry_points.txt,sha256=WbFEbaJT6BlIlgVgEaxo--H4SjwDX2nEVcCKwih-WG0,47
+lumipy-1.0.96.dist-info/top_level.txt,sha256=DVww8LaQM3Xm0WOgo4JE0epePgCM1xGWWWxh7wuv-CY,7
+lumipy-1.0.96.dist-info/RECORD,,
```

