# Comparing `tmp/calibrated_explanations-0.3.2.tar.gz` & `tmp/calibrated_explanations-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrated_explanations-0.3.2.tar", last modified: Sun Apr 14 00:06:14 2024, max compression
+gzip compressed data, was "calibrated_explanations-0.3.3.tar", last modified: Sat May 25 14:22:18 2024, max compression
```

## Comparing `calibrated_explanations-0.3.2.tar` & `calibrated_explanations-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.966813 calibrated_explanations-0.3.2/
--rw-rw-rw-   0        0        0     1532 2023-12-07 10:33:41.000000 calibrated_explanations-0.3.2/LICENSE
--rw-rw-rw-   0        0        0    20514 2024-04-14 00:06:14.963811 calibrated_explanations-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    19636 2024-04-14 00:01:31.000000 calibrated_explanations-0.3.2/README.md
--rw-rw-rw-   0        0        0     1023 2024-04-14 00:01:31.000000 calibrated_explanations-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 00:06:14.966813 calibrated_explanations-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      226 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.894489 calibrated_explanations-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.919388 calibrated_explanations-0.3.2/src/calibrated_explanations/
--rw-rw-rw-   0        0        0     6977 2024-04-11 08:56:51.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/VennAbers.py
--rw-rw-rw-   0        0        0      808 2024-01-17 09:22:57.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/__init__.py
--rw-rw-rw-   0        0        0     7827 2024-01-18 08:04:34.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/_discretizers.py
--rw-rw-rw-   0        0        0    93400 2024-04-11 17:11:56.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/_explanations.py
--rw-rw-rw-   0        0        0    10362 2024-02-22 18:45:13.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/_interval_regressor.py
--rw-rw-rw-   0        0        0    57289 2024-04-14 00:01:31.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/core.py
--rw-rw-rw-   0        0        0     8105 2024-02-21 11:41:35.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.961810 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/
--rw-rw-rw-   0        0        0    20514 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.958387 calibrated_explanations-0.3.2/tests/
--rw-rw-rw-   0        0        0     8311 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.2/tests/test_classification.py
--rw-rw-rw-   0        0        0    16212 2024-03-23 16:22:05.000000 calibrated_explanations-0.3.2/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-25 14:22:18.964511 calibrated_explanations-0.3.3/
+-rw-rw-rw-   0        0        0     1532 2023-12-07 10:33:41.000000 calibrated_explanations-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0    21841 2024-05-25 14:22:18.960505 calibrated_explanations-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    20963 2024-05-25 14:14:17.000000 calibrated_explanations-0.3.3/README.md
+-rw-rw-rw-   0        0        0     1023 2024-05-25 14:12:18.000000 calibrated_explanations-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 14:22:18.964511 calibrated_explanations-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      226 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 14:22:18.861574 calibrated_explanations-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 14:22:18.896890 calibrated_explanations-0.3.3/src/calibrated_explanations/
+-rw-rw-rw-   0        0        0     6977 2024-04-11 08:56:51.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/VennAbers.py
+-rw-rw-rw-   0        0        0      808 2024-01-17 09:22:57.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/__init__.py
+-rw-rw-rw-   0        0        0     7827 2024-01-18 08:04:34.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/_discretizers.py
+-rw-rw-rw-   0        0        0    93548 2024-05-20 13:46:00.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/_explanations.py
+-rw-rw-rw-   0        0        0    10368 2024-05-14 15:42:09.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/_interval_regressor.py
+-rw-rw-rw-   0        0        0    57290 2024-05-25 14:12:18.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/core.py
+-rw-rw-rw-   0        0        0     8105 2024-02-21 11:41:35.000000 calibrated_explanations-0.3.3/src/calibrated_explanations/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 14:22:18.958507 calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/
+-rw-rw-rw-   0        0        0    21841 2024-05-25 14:22:18.000000 calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2024-05-25 14:22:18.000000 calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 14:22:18.000000 calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-25 14:22:18.000000 calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-25 14:22:18.000000 calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 14:22:18.953499 calibrated_explanations-0.3.3/tests/
+-rw-rw-rw-   0        0        0     8311 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.3/tests/test_classification.py
+-rw-rw-rw-   0        0        0    16218 2024-05-03 12:28:37.000000 calibrated_explanations-0.3.3/tests/test_regression.py
```

### Comparing `calibrated_explanations-0.3.2/LICENSE` & `calibrated_explanations-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/PKG-INFO` & `calibrated_explanations-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,1283 +1,1311 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2063 616c  : 2.1..Name: cal
-00000020: 6962 7261 7465 645f 6578 706c 616e 6174  ibrated_explanat
-00000030: 696f 6e73 0d0a 5665 7273 696f 6e3a 2030  ions..Version: 0
-00000040: 2e33 2e32 0d0a 5375 6d6d 6172 793a 2045  .3.2..Summary: E
-00000050: 7874 7261 6374 2063 616c 6962 7261 7465  xtract calibrate
-00000060: 6420 6578 706c 616e 6174 696f 6e73 2066  d explanations f
-00000070: 726f 6d20 6d61 6368 696e 6520 6c65 6172  rom machine lear
-00000080: 6e69 6e67 206d 6f64 656c 732e 0d0a 4175  ning models...Au
-00000090: 7468 6f72 2d65 6d61 696c 3a20 4865 6c65  thor-email: Hele
-000000a0: 6e61 204c c3b6 6673 7472 c3b6 6d20 3c68  na L..fstr..m <h
-000000b0: 656c 656e 612e 6c6f 6673 7472 6f6d 406a  elena.lofstrom@j
-000000c0: 752e 7365 3e2c 2054 7577 6520 4cc3 b666  u.se>, Tuwe L..f
-000000d0: 7374 72c3 b66d 203c 7475 7765 2e6c 6f66  str..m <tuwe.lof
-000000e0: 7374 726f 6d40 6a75 2e73 653e 0d0a 5072  strom@ju.se>..Pr
-000000f0: 6f6a 6563 742d 5552 4c3a 2048 6f6d 6570  oject-URL: Homep
-00000100: 6167 652c 2068 7474 7073 3a2f 2f67 6974  age, https://git
-00000110: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
-00000120: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
-00000130: 6e61 7469 6f6e 730d 0a50 726f 6a65 6374  nations..Project
-00000140: 2d55 524c 3a20 4275 6720 5472 6163 6b65  -URL: Bug Tracke
-00000150: 722c 2068 7474 7073 3a2f 2f67 6974 6875  r, https://githu
-00000160: 622e 636f 6d2f 4d6f 6666 7261 6e2f 6361  b.com/Moffran/ca
-00000170: 6c69 6272 6174 6564 5f65 7870 6c61 6e61  librated_explana
-00000180: 7469 6f6e 732f 6973 7375 6573 0d0a 436c  tions/issues..Cl
-00000190: 6173 7369 6669 6572 3a20 4465 7665 6c6f  assifier: Develo
-000001a0: 706d 656e 7420 5374 6174 7573 203a 3a20  pment Status :: 
-000001b0: 3320 2d20 416c 7068 610d 0a43 6c61 7373  3 - Alpha..Class
-000001c0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001e0: 7974 686f 6e20 3a3a 2033 0d0a 436c 6173  ython :: 3..Clas
-000001f0: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00000200: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000210: 3a3a 2042 5344 204c 6963 656e 7365 0d0a  :: BSD License..
-00000220: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
-00000230: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000240: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000250: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
-00000260: 203e 3d33 2e38 0d0a 4465 7363 7269 7074   >=3.8..Descript
-00000270: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000280: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0d  : text/markdown.
-00000290: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-000002a0: 4943 454e 5345 0d0a 5265 7175 6972 6573  ICENSE..Requires
-000002b0: 2d44 6973 743a 2063 7265 7065 730d 0a52  -Dist: crepes..R
-000002c0: 6571 7569 7265 732d 4469 7374 3a20 7665  equires-Dist: ve
-000002d0: 6e6e 2d61 6265 7273 0d0a 5265 7175 6972  nn-abers..Requir
-000002e0: 6573 2d44 6973 743a 2069 7079 7468 6f6e  es-Dist: ipython
-000002f0: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
-00000300: 206c 696d 650d 0a52 6571 7569 7265 732d   lime..Requires-
-00000310: 4469 7374 3a20 6d61 7470 6c6f 746c 6962  Dist: matplotlib
-00000320: 0d0a 5265 7175 6972 6573 2d44 6973 743a  ..Requires-Dist:
-00000330: 206e 756d 7079 0d0a 5265 7175 6972 6573   numpy..Requires
-00000340: 2d44 6973 743a 2070 616e 6461 730d 0a52  -Dist: pandas..R
-00000350: 6571 7569 7265 732d 4469 7374 3a20 7363  equires-Dist: sc
-00000360: 696b 6974 2d6c 6561 726e 0d0a 0d0a 4361  ikit-learn....Ca
-00000370: 6c69 6272 6174 6564 2045 7870 6c61 6e61  librated Explana
-00000380: 7469 6f6e 7320 285b 446f 6375 6d65 6e74  tions ([Document
-00000390: 6174 696f 6e5d 2868 7474 7073 3a2f 2f63  ation](https://c
-000003a0: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
-000003b0: 6174 696f 6e73 2e72 6561 6474 6865 646f  ations.readthedo
-000003c0: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-000003d0: 3f62 6164 6765 3d6c 6174 6573 7429 290d  ?badge=latest)).
-000003e0: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
-000003f0: 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 5b21 5b43  ========....[![C
-00000400: 616c 6962 7261 7465 6420 4578 706c 616e  alibrated Explan
-00000410: 6174 696f 6e73 2050 7950 4920 7665 7273  ations PyPI vers
-00000420: 696f 6e5d 5b70 7970 692d 7665 7273 696f  ion][pypi-versio
-00000430: 6e5d 5d5b 6361 6c69 6272 6174 6564 2d65  n]][calibrated-e
-00000440: 7870 6c61 6e61 7469 6f6e 732d 6f6e 2d70  xplanations-on-p
-00000450: 7970 695d 0d0a 5b21 5b43 6f6e 6461 2056  ypi]..[![Conda V
-00000460: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-00000470: 696d 672e 7368 6965 6c64 732e 696f 2f63  img.shields.io/c
-00000480: 6f6e 6461 2f76 6e2f 636f 6e64 612d 666f  onda/vn/conda-fo
-00000490: 7267 652f 6361 6c69 6272 6174 6564 2d65  rge/calibrated-e
-000004a0: 7870 6c61 6e61 7469 6f6e 732e 7376 6729  xplanations.svg)
-000004b0: 5d28 6874 7470 733a 2f2f 616e 6163 6f6e  ](https://anacon
-000004c0: 6461 2e6f 7267 2f63 6f6e 6461 2d66 6f72  da.org/conda-for
-000004d0: 6765 2f63 616c 6962 7261 7465 642d 6578  ge/calibrated-ex
-000004e0: 706c 616e 6174 696f 6e73 290d 0a5b 215b  planations)..[![
-000004f0: 4769 7448 7562 2028 5072 652d 2952 656c  GitHub (Pre-)Rel
-00000500: 6561 7365 2044 6174 655d 2868 7474 7073  ease Date](https
-00000510: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000520: 6f2f 6769 7468 7562 2f72 656c 6561 7365  o/github/release
-00000530: 2d64 6174 652d 7072 652f 4d6f 6666 7261  -date-pre/Moffra
-00000540: 6e2f 6361 6c69 6272 6174 6564 5f65 7870  n/calibrated_exp
-00000550: 6c61 6e61 7469 6f6e 7329 5d28 6874 7470  lanations)](http
-00000560: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
-00000570: 6f66 6672 616e 2f63 616c 6962 7261 7465  offran/calibrate
-00000580: 645f 6578 706c 616e 6174 696f 6e73 2f62  d_explanations/b
-00000590: 6c6f 622f 6d61 696e 2f43 4841 4e47 454c  lob/main/CHANGEL
-000005a0: 4f47 2e6d 6429 0d0a 5b21 5b44 6f63 756d  OG.md)..[![Docum
-000005b0: 656e 7461 7469 6f6e 2053 7461 7475 735d  entation Status]
-000005c0: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
-000005d0: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
-000005e0: 732f 6361 6c69 6272 6174 6564 2d65 7870  s/calibrated-exp
-000005f0: 6c61 6e61 7469 6f6e 732f 6261 6467 652f  lanations/badge/
-00000600: 3f76 6572 7369 6f6e 3d6c 6174 6573 7429  ?version=latest)
-00000610: 5d28 6874 7470 733a 2f2f 6361 6c69 6272  ](https://calibr
-00000620: 6174 6564 2d65 7870 6c61 6e61 7469 6f6e  ated-explanation
-00000630: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
-00000640: 2f65 6e2f 6c61 7465 7374 2f3f 6261 6467  /en/latest/?badg
-00000650: 653d 6c61 7465 7374 290d 0a5b 215b 4275  e=latest)..[![Bu
-00000660: 696c 6420 5374 6174 7573 2066 6f72 2043  ild Status for C
-00000670: 616c 6962 7261 7465 6420 4578 706c 616e  alibrated Explan
-00000680: 6174 696f 6e73 5d5b 6275 696c 642d 7374  ations][build-st
-00000690: 6174 7573 5d5d 5b62 7569 6c64 2d6c 6f67  atus]][build-log
-000006a0: 5d0d 0a5b 215b 4c69 6e74 2053 7461 7475  ]..[![Lint Statu
-000006b0: 7320 666f 7220 4361 6c69 6272 6174 6564  s for Calibrated
-000006c0: 2045 7870 6c61 6e61 7469 6f6e 735d 5b6c   Explanations][l
-000006d0: 696e 742d 7374 6174 7573 5d5d 5b6c 696e  int-status]][lin
-000006e0: 742d 6c6f 675d 0d0a 5b21 5b4c 6963 656e  t-log]..[![Licen
-000006f0: 7365 5d28 6874 7470 733a 2f2f 6261 6467  se](https://badg
-00000700: 656e 2e6e 6574 2f67 6974 6875 622f 6c69  en.net/github/li
-00000710: 6365 6e73 652f 6d6f 6666 7261 6e2f 6361  cense/moffran/ca
-00000720: 6c69 6272 6174 6564 5f65 7870 6c61 6e61  librated_explana
-00000730: 7469 6f6e 7329 5d28 6874 7470 733a 2f2f  tions)](https://
-00000740: 6769 7468 7562 2e63 6f6d 2f6d 6f66 6672  github.com/moffr
-00000750: 616e 2f63 616c 6962 7261 7465 645f 6578  an/calibrated_ex
-00000760: 706c 616e 6174 696f 6e73 2f62 6c6f 622f  planations/blob/
-00000770: 6d61 696e 2f4c 4943 454e 5345 290d 0a5b  main/LICENSE)..[
-00000780: 215b 446f 776e 6c6f 6164 735d 2868 7474  ![Downloads](htt
-00000790: 7073 3a2f 2f73 7461 7469 632e 7065 7079  ps://static.pepy
-000007a0: 2e74 6563 682f 6261 6467 652f 6361 6c69  .tech/badge/cali
-000007b0: 6272 6174 6564 2d65 7870 6c61 6e61 7469  brated-explanati
-000007c0: 6f6e 7329 5d28 6874 7470 733a 2f2f 7065  ons)](https://pe
-000007d0: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-000007e0: 6361 6c69 6272 6174 6564 2d65 7870 6c61  calibrated-expla
-000007f0: 6e61 7469 6f6e 7329 0d0a 5b21 5b42 696e  nations)..[![Bin
-00000800: 6465 725d 2868 7474 7073 3a2f 2f6d 7962  der](https://myb
-00000810: 696e 6465 722e 6f72 672f 6261 6467 655f  inder.org/badge_
-00000820: 6c6f 676f 2e73 7667 295d 2868 7474 7073  logo.svg)](https
-00000830: 3a2f 2f6d 7962 696e 6465 722e 6f72 672f  ://mybinder.org/
-00000840: 7632 2f67 682f 4d6f 6666 7261 6e2f 6361  v2/gh/Moffran/ca
-00000850: 6c69 6272 6174 6564 5f65 7870 6c61 6e61  librated_explana
-00000860: 7469 6f6e 732f 7630 2e33 2e32 290d 0a0d  tions/v0.3.2)...
-00000870: 0a60 6361 6c69 6272 6174 6564 2d65 7870  .`calibrated-exp
-00000880: 6c61 6e61 7469 6f6e 7360 2069 7320 6120  lanations` is a 
-00000890: 5079 7468 6f6e 2070 6163 6b61 6765 2066  Python package f
-000008a0: 6f72 2074 6865 206c 6f63 616c 2066 6561  or the local fea
-000008b0: 7475 7265 2069 6d70 6f72 7461 6e63 6520  ture importance 
-000008c0: 6578 706c 616e 6174 696f 6e20 6d65 7468  explanation meth
-000008d0: 6f64 2063 616c 6c65 6420 4361 6c69 6272  od called Calibr
-000008e0: 6174 6564 2045 7870 6c61 6e61 7469 6f6e  ated Explanation
-000008f0: 732c 2073 7570 706f 7274 696e 6720 626f  s, supporting bo
-00000900: 7468 2063 6c61 7373 6966 6963 6174 696f  th classificatio
-00000910: 6e20 616e 6420 7265 6772 6573 7369 6f6e  n and regression
-00000920: 2e0d 0a54 6865 2070 726f 706f 7365 6420  ...The proposed 
-00000930: 6d65 7468 6f64 2069 7320 6261 7365 6420  method is based 
-00000940: 6f6e 2056 656e 6e2d 4162 6572 7320 2863  on Venn-Abers (c
-00000950: 6c61 7373 6966 6963 6174 696f 6e20 2620  lassification & 
-00000960: 7265 6772 6573 7369 6f6e 2920 616e 6420  regression) and 
-00000970: 436f 6e66 6f72 6d61 6c20 5072 6564 6963  Conformal Predic
-00000980: 7469 7665 2053 7973 7465 6d73 2028 7265  tive Systems (re
-00000990: 6772 6573 7369 6f6e 2920 616e 6420 6861  gression) and ha
-000009a0: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
-000009b0: 6368 6172 6163 7465 7269 7374 6963 733a  characteristics:
-000009c0: 0d0a 2a20 4661 7374 2c20 7265 6c69 6162  ..* Fast, reliab
-000009d0: 6c65 2c20 7374 6162 6c65 2061 6e64 2072  le, stable and r
-000009e0: 6f62 7573 7420 6665 6174 7572 6520 696d  obust feature im
-000009f0: 706f 7274 616e 6365 2065 7870 6c61 6e61  portance explana
-00000a00: 7469 6f6e 732e 0d0a 2a20 4361 6c69 6272  tions...* Calibr
-00000a10: 6174 696f 6e20 6f66 2074 6865 2075 6e64  ation of the und
-00000a20: 6572 6c79 696e 6720 6d6f 6465 6c20 746f  erlying model to
-00000a30: 2065 6e73 7572 6520 7468 6174 2070 7265   ensure that pre
-00000a40: 6469 6374 696f 6e73 2072 6566 6c65 6374  dictions reflect
-00000a50: 2072 6561 6c69 7479 2e0d 0a2a 2055 6e63   reality...* Unc
-00000a60: 6572 7461 696e 7479 2071 7561 6e74 6966  ertainty quantif
-00000a70: 6963 6174 696f 6e20 6f66 2074 6865 2070  ication of the p
-00000a80: 7265 6469 6374 696f 6e20 6672 6f6d 2074  rediction from t
-00000a90: 6865 2075 6e64 6572 6c79 696e 6720 6d6f  he underlying mo
-00000aa0: 6465 6c20 616e 6420 7468 6520 6665 6174  del and the feat
-00000ab0: 7572 6520 696d 706f 7274 616e 6365 2077  ure importance w
-00000ac0: 6569 6768 7473 2e20 0d0a 2a20 5275 6c65  eights. ..* Rule
-00000ad0: 7320 7769 7468 2073 7472 6169 6768 7466  s with straightf
-00000ae0: 6f72 7761 7264 2069 6e74 6572 7072 6574  orward interpret
-00000af0: 6174 696f 6e20 696e 2072 656c 6174 696f  ation in relatio
-00000b00: 6e20 746f 2074 6865 2066 6561 7475 7265  n to the feature
-00000b10: 2077 6569 6768 7473 2e0d 0a2a 2050 6f73   weights...* Pos
-00000b20: 7369 6269 6c69 7479 2074 6f20 6765 6e65  sibility to gene
-00000b30: 7261 7465 2063 6f75 6e74 6572 6661 6374  rate counterfact
-00000b40: 7561 6c20 7275 6c65 7320 7769 7468 2075  ual rules with u
-00000b50: 6e63 6572 7461 696e 7479 2071 7561 6e74  ncertainty quant
-00000b60: 6966 6963 6174 696f 6e20 6f66 2074 6865  ification of the
-00000b70: 2065 7870 6563 7465 6420 7072 6564 6963   expected predic
-00000b80: 7469 6f6e 732e 0d0a 2a20 436f 6e6a 756e  tions...* Conjun
-00000b90: 6374 696f 6e61 6c20 7275 6c65 7320 636f  ctional rules co
-00000ba0: 6e76 6579 696e 6720 6a6f 696e 7420 636f  nveying joint co
-00000bb0: 6e74 7269 6275 7469 6f6e 2062 6574 7765  ntribution betwe
-00000bc0: 656e 2066 6561 7475 7265 732e 0d0a 0d0a  en features.....
-00000bd0: 4265 6c6f 7720 6973 2061 6e20 6578 616d  Below is an exam
-00000be0: 706c 6520 6f66 2061 2070 726f 6261 6269  ple of a probabi
-00000bf0: 6c69 7374 6963 2063 6f75 6e74 6572 6661  listic counterfa
-00000c00: 6374 7561 6c20 6578 706c 616e 6174 696f  ctual explanatio
-00000c10: 6e20 666f 7220 616e 2069 6e73 7461 6e63  n for an instanc
-00000c20: 6520 6f66 2074 6865 2043 616c 6966 6f72  e of the Califor
-00000c30: 6e69 6120 486f 7573 696e 6720 6461 7461  nia Housing data
-00000c40: 7365 7420 2877 6974 6820 7468 6520 7468  set (with the th
-00000c50: 7265 7368 6f6c 6420 3138 3020 3030 3029  reshold 180 000)
-00000c60: 2e20 5468 6520 6c69 6768 7420 7265 6420  . The light red 
-00000c70: 6172 6561 2069 6e20 7468 6520 6261 636b  area in the back
-00000c80: 6772 6f75 6e64 2069 7320 7265 7072 6573  ground is repres
-00000c90: 656e 7469 6e67 2074 6865 2063 616c 6962  enting the calib
-00000ca0: 7261 7465 6420 7072 6f62 6162 696c 6974  rated probabilit
-00000cb0: 7920 696e 7465 7276 616c 2028 666f 7220  y interval (for 
-00000cc0: 7468 6520 7072 6564 6963 7469 6f6e 2062  the prediction b
-00000cd0: 6569 6e67 2062 656c 6f77 2074 6865 2074  eing below the t
-00000ce0: 6872 6573 686f 6c64 2920 6f66 2074 6865  hreshold) of the
-00000cf0: 2075 6e64 6572 6c79 696e 6720 6d6f 6465   underlying mode
-00000d00: 6c2c 2061 7320 696e 6469 6361 7465 6420  l, as indicated 
-00000d10: 6279 2061 2043 6f6e 666f 726d 616c 2050  by a Conformal P
-00000d20: 7265 6469 6374 6976 6520 5379 7374 656d  redictive System
-00000d30: 2061 6e64 2063 616c 6962 7261 7465 6420   and calibrated 
-00000d40: 7468 726f 7567 6820 5665 6e6e 2d41 6265  through Venn-Abe
-00000d50: 7273 2e20 5468 6520 6461 726b 6572 2072  rs. The darker r
-00000d60: 6564 2062 6172 7320 666f 7220 6561 6368  ed bars for each
-00000d70: 2072 756c 6520 7368 6f77 2074 6865 2070   rule show the p
-00000d80: 726f 6261 6269 6c69 7479 2069 6e74 6572  robability inter
-00000d90: 7661 6c73 2074 6861 7420 5665 6e6e 2d41  vals that Venn-A
-00000da0: 6265 7273 2069 6e64 6963 6174 6520 666f  bers indicate fo
-00000db0: 7220 616e 2069 6e73 7461 6e63 6520 6368  r an instance ch
-00000dc0: 616e 6769 6e67 2061 2066 6561 7475 7265  anging a feature
-00000dd0: 2076 616c 7565 2069 6e20 6163 636f 7264   value in accord
-00000de0: 616e 6365 2077 6974 6820 7468 6520 7275  ance with the ru
-00000df0: 6c65 2063 6f6e 6469 7469 6f6e 2e0d 0a0d  le condition....
-00000e00: 0a5b 215b 5072 6f62 6162 696c 6973 7469  .[![Probabilisti
-00000e10: 6320 636f 756e 7465 7266 6163 7475 616c  c counterfactual
-00000e20: 2065 7870 6c61 6e61 7469 6f6e 2066 6f72   explanation for
-00000e30: 2043 616c 6966 6f72 6e69 6120 486f 7573   California Hous
-00000e40: 696e 675d 2868 7474 7073 3a2f 2f67 6974  ing](https://git
-00000e50: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
-00000e60: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
-00000e70: 6e61 7469 6f6e 732f 626c 6f62 2f6d 6169  nations/blob/mai
-00000e80: 6e2f 646f 6373 2f69 6d61 6765 732f 636f  n/docs/images/co
-00000e90: 756e 7465 7266 6163 7475 616c 5f70 726f  unterfactual_pro
-00000ea0: 6261 6269 6c69 7374 6963 5f68 6f75 7365  babilistic_house
-00000eb0: 5f72 6567 7265 7373 696f 6e2e 6a70 6720  _regression.jpg 
-00000ec0: 2250 726f 6261 6269 6c69 7374 6963 2063  "Probabilistic c
-00000ed0: 6f75 6e74 6572 6661 6374 7561 6c20 6578  ounterfactual ex
-00000ee0: 706c 616e 6174 696f 6e20 666f 7220 4361  planation for Ca
-00000ef0: 6c69 666f 726e 6961 2048 6f75 7369 6e67  lifornia Housing
-00000f00: 2229 5d28 6874 7470 733a 2f2f 6361 6c69  ")](https://cali
-00000f10: 6272 6174 6564 2d65 7870 6c61 6e61 7469  brated-explanati
-00000f20: 6f6e 732e 7265 6164 7468 6564 6f63 732e  ons.readthedocs.
-00000f30: 696f 2f65 6e2f 6c61 7465 7374 2f3f 6261  io/en/latest/?ba
-00000f40: 6467 653d 6c61 7465 7374 290d 0a20 0d0a  dge=latest).. ..
-00000f50: 4765 7474 696e 6720 7374 6172 7465 640d  Getting started.
-00000f60: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00000f70: 0d0a 5468 6520 5b6e 6f74 6562 6f6f 6b73  ..The [notebooks
-00000f80: 2066 6f6c 6465 725d 2868 7474 7073 3a2f   folder](https:/
-00000f90: 2f67 6974 6875 622e 636f 6d2f 4d6f 6666  /github.com/Moff
-00000fa0: 7261 6e2f 6361 6c69 6272 6174 6564 5f65  ran/calibrated_e
-00000fb0: 7870 6c61 6e61 7469 6f6e 732f 7472 6565  xplanations/tree
-00000fc0: 2f6d 6169 6e2f 6e6f 7465 626f 6f6b 7329  /main/notebooks)
-00000fd0: 2063 6f6e 7461 696e 7320 6120 6e75 6d62   contains a numb
-00000fe0: 6572 206f 6620 6e6f 7465 626f 6f6b 7320  er of notebooks 
-00000ff0: 696c 6c75 7374 7261 7469 6e67 2064 6966  illustrating dif
-00001000: 6665 7265 6e74 2075 7365 2063 6173 6573  ferent use cases
-00001010: 2066 6f72 2060 6361 6c69 6272 6174 6564   for `calibrated
-00001020: 2d65 7870 6c61 6e61 7469 6f6e 7360 2e20  -explanations`. 
-00001030: 5468 6520 666f 6c6c 6f77 696e 6720 6172  The following ar
-00001040: 6520 636f 6d6d 656e 7465 6420 616e 6420  e commented and 
-00001050: 7368 6f75 6c64 2062 6520 6120 676f 6f64  should be a good
-00001060: 2073 7461 7274 3a0d 0a2a 205b 7175 6963   start:..* [quic
-00001070: 6b73 7461 7274 5d28 6874 7470 733a 2f2f  kstart](https://
-00001080: 6769 7468 7562 2e63 6f6d 2f4d 6f66 6672  github.com/Moffr
-00001090: 616e 2f63 616c 6962 7261 7465 645f 6578  an/calibrated_ex
-000010a0: 706c 616e 6174 696f 6e73 2f62 6c6f 622f  planations/blob/
-000010b0: 6d61 696e 2f6e 6f74 6562 6f6f 6b73 2f71  main/notebooks/q
-000010c0: 7569 636b 7374 6172 742e 6970 796e 6229  uickstart.ipynb)
-000010d0: 2020 2d20 7369 6d69 6c61 7220 746f 2074    - similar to t
-000010e0: 6869 7320 4765 7474 696e 6720 5374 6172  his Getting Star
-000010f0: 7465 642c 2069 6e63 6c75 6469 6e67 2070  ted, including p
-00001100: 6c6f 7473 2e0d 0a2a 205b 7175 6963 6b73  lots...* [quicks
-00001110: 7461 7274 5f77 7261 705d 2868 7474 7073  tart_wrap](https
-00001120: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
-00001130: 6666 7261 6e2f 6361 6c69 6272 6174 6564  ffran/calibrated
-00001140: 5f65 7870 6c61 6e61 7469 6f6e 732f 626c  _explanations/bl
-00001150: 6f62 2f6d 6169 6e2f 6e6f 7465 626f 6f6b  ob/main/notebook
-00001160: 732f 7175 6963 6b73 7461 7274 5f77 7261  s/quickstart_wra
-00001170: 702e 6970 796e 6229 202d 2073 696d 696c  p.ipynb) - simil
-00001180: 6172 2074 6f20 7468 6973 2047 6574 7469  ar to this Getti
-00001190: 6e67 2053 7461 7274 6564 2c20 6275 7420  ng Started, but 
-000011a0: 7769 7468 2061 2077 7261 7070 6572 2063  with a wrapper c
-000011b0: 6c61 7373 2066 6f72 2065 6173 6965 7220  lass for easier 
-000011c0: 7573 652e 0d0a 2a20 5b64 656d 6f5f 6269  use...* [demo_bi
-000011d0: 6e61 7279 5f63 6c61 7373 6966 6963 6174  nary_classificat
-000011e0: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
-000011f0: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
-00001200: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
-00001210: 6e61 7469 6f6e 732f 626c 6f62 2f6d 6169  nations/blob/mai
-00001220: 6e2f 6e6f 7465 626f 6f6b 732f 6465 6d6f  n/notebooks/demo
-00001230: 5f62 696e 6172 795f 636c 6173 7369 6669  _binary_classifi
-00001240: 6361 7469 6f6e 2e69 7079 6e62 2920 0d0a  cation.ipynb) ..
-00001250: 2a20 5b64 656d 6f5f 7265 6772 6573 7369  * [demo_regressi
-00001260: 6f6e 5d28 6874 7470 733a 2f2f 6769 7468  on](https://gith
-00001270: 7562 2e63 6f6d 2f4d 6f66 6672 616e 2f63  ub.com/Moffran/c
-00001280: 616c 6962 7261 7465 645f 6578 706c 616e  alibrated_explan
-00001290: 6174 696f 6e73 2f62 6c6f 622f 6d61 696e  ations/blob/main
-000012a0: 2f6e 6f74 6562 6f6f 6b73 2f64 656d 6f5f  /notebooks/demo_
-000012b0: 7265 6772 6573 7369 6f6e 2e69 7079 6e62  regression.ipynb
-000012c0: 290d 0a2a 205b 6465 6d6f 5f70 726f 6261  )..* [demo_proba
-000012d0: 6269 6c69 7374 6963 5f72 6567 7265 7373  bilistic_regress
-000012e0: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
-000012f0: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
-00001300: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
-00001310: 6e61 7469 6f6e 732f 626c 6f62 2f6d 6169  nations/blob/mai
-00001320: 6e2f 6e6f 7465 626f 6f6b 732f 6465 6d6f  n/notebooks/demo
-00001330: 5f70 726f 6261 6269 6c69 7374 6963 5f72  _probabilistic_r
-00001340: 6567 7265 7373 696f 6e2e 6970 796e 6229  egression.ipynb)
-00001350: 0d0a 0d0a 2323 2320 436c 6173 7369 6669  ....### Classifi
-00001360: 6361 7469 6f6e 0d0a 4c65 7420 7573 2069  cation..Let us i
-00001370: 6c6c 7573 7472 6174 6520 686f 7720 7765  llustrate how we
-00001380: 206d 6179 2075 7365 2060 6361 6c69 6272   may use `calibr
-00001390: 6174 6564 2d65 7870 6c61 6e61 7469 6f6e  ated-explanation
-000013a0: 7360 2074 6f20 6765 6e65 7261 7465 2065  s` to generate e
-000013b0: 7870 6c61 6e61 7469 6f6e 7320 6672 6f6d  xplanations from
-000013c0: 2061 2063 6c61 7373 6966 6965 7220 7472   a classifier tr
-000013d0: 6169 6e65 6420 6f6e 2061 2064 6174 6173  ained on a datas
-000013e0: 6574 2066 726f 6d0d 0a5b 7777 772e 6f70  et from..[www.op
-000013f0: 656e 6d6c 2e6f 7267 5d28 6874 7470 733a  enml.org](https:
-00001400: 2f2f 7777 772e 6f70 656e 6d6c 2e6f 7267  //www.openml.org
-00001410: 292c 2077 6869 6368 2077 6520 6669 7273  ), which we firs
-00001420: 7420 7370 6c69 7420 696e 746f 2061 0d0a  t split into a..
-00001430: 7472 6169 6e69 6e67 2061 6e64 2061 2074  training and a t
-00001440: 6573 7420 7365 7420 7573 696e 6720 6074  est set using `t
-00001450: 7261 696e 5f74 6573 745f 7370 6c69 7460  rain_test_split`
-00001460: 2066 726f 6d0d 0a5b 736b 6c65 6172 6e5d   from..[sklearn]
-00001470: 2868 7474 7073 3a2f 2f73 6369 6b69 742d  (https://scikit-
-00001480: 6c65 6172 6e2e 6f72 6729 2c20 616e 6420  learn.org), and 
-00001490: 7468 656e 2066 7572 7468 6572 2073 706c  then further spl
-000014a0: 6974 2074 6865 0d0a 7472 6169 6e69 6e67  it the..training
-000014b0: 2073 6574 2069 6e74 6f20 6120 7072 6f70   set into a prop
-000014c0: 6572 2074 7261 696e 696e 6720 7365 7420  er training set 
-000014d0: 616e 6420 6120 6361 6c69 6272 6174 696f  and a calibratio
-000014e0: 6e20 7365 743a 0d0a 0d0a 6060 6070 7974  n set:....```pyt
-000014f0: 686f 6e0d 0a66 726f 6d20 736b 6c65 6172  hon..from sklear
-00001500: 6e2e 6461 7461 7365 7473 2069 6d70 6f72  n.datasets impor
-00001510: 7420 6665 7463 685f 6f70 656e 6d6c 0d0a  t fetch_openml..
-00001520: 6672 6f6d 2073 6b6c 6561 726e 2e6d 6f64  from sklearn.mod
-00001530: 656c 5f73 656c 6563 7469 6f6e 2069 6d70  el_selection imp
-00001540: 6f72 7420 7472 6169 6e5f 7465 7374 5f73  ort train_test_s
-00001550: 706c 6974 0d0a 0d0a 6461 7461 7365 7420  plit....dataset 
-00001560: 3d20 6665 7463 685f 6f70 656e 6d6c 286e  = fetch_openml(n
-00001570: 616d 653d 2277 696e 6522 2c20 7665 7273  ame="wine", vers
-00001580: 696f 6e3d 372c 2061 735f 6672 616d 653d  ion=7, as_frame=
-00001590: 5472 7565 290d 0a0d 0a58 203d 2064 6174  True)....X = dat
-000015a0: 6173 6574 2e64 6174 612e 7661 6c75 6573  aset.data.values
-000015b0: 2e61 7374 7970 6528 666c 6f61 7429 0d0a  .astype(float)..
-000015c0: 7920 3d20 2864 6174 6173 6574 2e74 6172  y = (dataset.tar
-000015d0: 6765 742e 7661 6c75 6573 203d 3d20 2754  get.values == 'T
-000015e0: 7275 6527 292e 6173 7479 7065 2869 6e74  rue').astype(int
-000015f0: 290d 0a0d 0a66 6561 7475 7265 5f6e 616d  )....feature_nam
-00001600: 6573 203d 2064 6174 6173 6574 2e66 6561  es = dataset.fea
-00001610: 7475 7265 5f6e 616d 6573 0d0a 0d0a 585f  ture_names....X_
-00001620: 7472 6169 6e2c 2058 5f74 6573 742c 2079  train, X_test, y
-00001630: 5f74 7261 696e 2c20 795f 7465 7374 203d  _train, y_test =
-00001640: 2074 7261 696e 5f74 6573 745f 7370 6c69   train_test_spli
-00001650: 7428 582c 2079 2c20 7465 7374 5f73 697a  t(X, y, test_siz
-00001660: 653d 322c 2073 7472 6174 6966 793d 7929  e=2, stratify=y)
-00001670: 0d0a 0d0a 585f 7072 6f70 5f74 7261 696e  ....X_prop_train
-00001680: 2c20 585f 6361 6c2c 2079 5f70 726f 705f  , X_cal, y_prop_
-00001690: 7472 6169 6e2c 2079 5f63 616c 203d 2074  train, y_cal = t
-000016a0: 7261 696e 5f74 6573 745f 7370 6c69 7428  rain_test_split(
-000016b0: 585f 7472 6169 6e2c 2079 5f74 7261 696e  X_train, y_train
-000016c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001700: 6573 745f 7369 7a65 3d30 2e32 3529 0d0a  est_size=0.25)..
-00001710: 0d0a 6060 600d 0a0d 0a57 6520 6e6f 7720  ..```....We now 
-00001720: 6669 7420 6120 6d6f 6465 6c20 6f6e 206f  fit a model on o
-00001730: 7572 2064 6174 612e 200d 0a0d 0a60 6060  ur data. ....```
-00001740: 7079 7468 6f6e 0d0a 6672 6f6d 2073 6b6c  python..from skl
-00001750: 6561 726e 2e65 6e73 656d 626c 6520 696d  earn.ensemble im
-00001760: 706f 7274 2052 616e 646f 6d46 6f72 6573  port RandomFores
-00001770: 7443 6c61 7373 6966 6965 720d 0a0d 0a72  tClassifier....r
-00001780: 6620 3d20 5261 6e64 6f6d 466f 7265 7374  f = RandomForest
-00001790: 436c 6173 7369 6669 6572 286e 5f6a 6f62  Classifier(n_job
-000017a0: 733d 2d31 290d 0a0d 0a72 662e 6669 7428  s=-1)....rf.fit(
-000017b0: 585f 7072 6f70 5f74 7261 696e 2c20 795f  X_prop_train, y_
-000017c0: 7072 6f70 5f74 7261 696e 290d 0a60 6060  prop_train)..```
-000017d0: 0d0a 0d0a 2323 2323 2046 6163 7475 616c  ....#### Factual
-000017e0: 2045 7870 6c61 6e61 7469 6f6e 730d 0a4c   Explanations..L
-000017f0: 6574 7320 6578 7472 6163 7420 6578 706c  ets extract expl
-00001800: 616e 6174 696f 6e73 2066 6f72 206f 7572  anations for our
-00001810: 2074 6573 7420 7365 7420 7573 696e 6720   test set using 
-00001820: 7468 6520 6063 616c 6962 7261 7465 642d  the `calibrated-
-00001830: 6578 706c 616e 6174 696f 6e73 6020 7061  explanations` pa
-00001840: 636b 6167 6520 6279 2069 6d70 6f72 7469  ckage by importi
-00001850: 6e67 2060 4361 6c69 6272 6174 6564 4578  ng `CalibratedEx
-00001860: 706c 6169 6e65 7260 2066 726f 6d20 6063  plainer` from `c
-00001870: 616c 6962 7261 7465 645f 6578 706c 616e  alibrated_explan
-00001880: 6174 696f 6e73 602e 0d0a 0d0a 6060 6070  ations`.....```p
-00001890: 7974 686f 6e0d 0a66 726f 6d20 6361 6c69  ython..from cali
-000018a0: 6272 6174 6564 5f65 7870 6c61 6e61 7469  brated_explanati
-000018b0: 6f6e 7320 696d 706f 7274 2043 616c 6962  ons import Calib
-000018c0: 7261 7465 6445 7870 6c61 696e 6572 2c20  ratedExplainer, 
-000018d0: 5f5f 7665 7273 696f 6e5f 5f0d 0a70 7269  __version__..pri
-000018e0: 6e74 285f 5f76 6572 7369 6f6e 5f5f 290d  nt(__version__).
-000018f0: 0a0d 0a65 7870 6c61 696e 6572 203d 2043  ...explainer = C
-00001900: 616c 6962 7261 7465 6445 7870 6c61 696e  alibratedExplain
-00001910: 6572 2872 662c 2058 5f63 616c 2c20 795f  er(rf, X_cal, y_
-00001920: 6361 6c2c 2066 6561 7475 7265 5f6e 616d  cal, feature_nam
-00001930: 6573 3d66 6561 7475 7265 5f6e 616d 6573  es=feature_names
-00001940: 290d 0a0d 0a66 6163 7475 616c 5f65 7870  )....factual_exp
-00001950: 6c61 6e61 7469 6f6e 7320 3d20 6578 706c  lanations = expl
-00001960: 6169 6e65 722e 6578 706c 6169 6e5f 6661  ainer.explain_fa
-00001970: 6374 7561 6c28 585f 7465 7374 290d 0a60  ctual(X_test)..`
-00001980: 6060 0d0a 0d0a 4f6e 6365 2077 6520 6861  ``....Once we ha
-00001990: 7665 2074 6865 2065 7870 6c61 6e61 7469  ve the explanati
-000019a0: 6f6e 732c 2077 6520 6361 6e20 706c 6f74  ons, we can plot
-000019b0: 2061 6c6c 206f 6620 7468 656d 2075 7369   all of them usi
-000019c0: 6e67 2060 706c 6f74 5f61 6c6c 602e 2044  ng `plot_all`. D
-000019d0: 6566 6175 6c74 2c20 6120 7265 6775 6c61  efault, a regula
-000019e0: 7220 706c 6f74 2c20 7769 7468 6f75 7420  r plot, without 
-000019f0: 756e 6365 7274 6169 6e74 7920 696e 7465  uncertainty inte
-00001a00: 7276 616c 7320 696e 636c 7564 6564 2c20  rvals included, 
-00001a10: 6973 2063 7265 6174 6564 2e20 546f 2069  is created. To i
-00001a20: 6e63 6c75 6465 2075 6e63 6572 7461 696e  nclude uncertain
-00001a30: 7479 2069 6e74 6572 7661 6c73 2c20 6368  ty intervals, ch
-00001a40: 616e 6765 2074 6865 2070 6172 616d 6574  ange the paramet
-00001a50: 6572 2060 756e 6365 7274 6169 6e74 793d  er `uncertainty=
-00001a60: 5472 7565 602e 2054 6f20 706c 6f74 206f  True`. To plot o
-00001a70: 6e6c 7920 6120 7369 6e67 6c65 2069 6e73  nly a single ins
-00001a80: 7461 6e63 652c 2074 6865 2060 706c 6f74  tance, the `plot
-00001a90: 5f65 7870 6c61 6e61 7469 6f6e 6020 6675  _explanation` fu
-00001aa0: 6e63 7469 6f6e 2063 616e 2062 6520 6361  nction can be ca
-00001ab0: 6c6c 6564 2c20 7375 626d 6974 7469 6e67  lled, submitting
-00001ac0: 2074 6865 2069 6e64 6578 206f 6620 7468   the index of th
-00001ad0: 6520 7465 7374 2069 6e73 7461 6e63 6520  e test instance 
-00001ae0: 746f 2070 6c6f 742e 2059 6f75 2063 616e  to plot. You can
-00001af0: 2061 6c73 6f20 6164 6420 616e 6420 7265   also add and re
-00001b00: 6d6f 7665 2063 6f6e 6a75 6e63 7469 7665  move conjunctive
-00001b10: 2072 756c 6573 2e0d 0a0d 0a60 6060 7079   rules.....```py
-00001b20: 7468 6f6e 0d0a 6661 6374 7561 6c5f 6578  thon..factual_ex
-00001b30: 706c 616e 6174 696f 6e73 2e70 6c6f 745f  planations.plot_
-00001b40: 616c 6c28 290d 0a66 6163 7475 616c 5f65  all()..factual_e
-00001b50: 7870 6c61 6e61 7469 6f6e 732e 706c 6f74  xplanations.plot
-00001b60: 5f61 6c6c 2875 6e63 6572 7461 696e 7479  _all(uncertainty
-00001b70: 3d54 7275 6529 0d0a 0d0a 6661 6374 7561  =True)....factua
-00001b80: 6c5f 6578 706c 616e 6174 696f 6e73 2e70  l_explanations.p
-00001b90: 6c6f 745f 6578 706c 616e 6174 696f 6e28  lot_explanation(
-00001ba0: 302c 2075 6e63 6572 7461 696e 7479 3d54  0, uncertainty=T
-00001bb0: 7275 6529 0d0a 0d0a 6661 6374 7561 6c5f  rue)....factual_
-00001bc0: 6578 706c 616e 6174 696f 6e73 2e61 6464  explanations.add
-00001bd0: 5f63 6f6e 6a75 6e63 7469 6f6e 7328 292e  _conjunctions().
-00001be0: 706c 6f74 5f61 6c6c 2829 0d0a 6661 6374  plot_all()..fact
-00001bf0: 7561 6c5f 6578 706c 616e 6174 696f 6e73  ual_explanations
-00001c00: 2e72 656d 6f76 655f 636f 6e6a 756e 6374  .remove_conjunct
-00001c10: 696f 6e73 2829 2e70 6c6f 745f 616c 6c28  ions().plot_all(
-00001c20: 290d 0a60 6060 0d0a 0d0a 2323 2323 2043  )..```....#### C
-00001c30: 6f75 6e74 6572 6661 6374 7561 6c20 4578  ounterfactual Ex
-00001c40: 706c 616e 6174 696f 6e73 0d0a 416e 2061  planations..An a
-00001c50: 6c74 6572 6e61 7469 7665 2074 6f20 6661  lternative to fa
-00001c60: 6374 7561 6c20 7275 6c65 7320 6973 2074  ctual rules is t
-00001c70: 6f20 6578 7472 6163 7420 636f 756e 7465  o extract counte
-00001c80: 7266 6163 7475 616c 2072 756c 6573 2e20  rfactual rules. 
-00001c90: 0d0a 6065 7870 6c61 696e 5f63 6f75 6e74  ..`explain_count
-00001ca0: 6572 6661 6374 7561 6c60 2063 616e 2062  erfactual` can b
-00001cb0: 6520 6361 6c6c 6564 2074 6f20 6765 7420  e called to get 
-00001cc0: 636f 756e 7465 7266 6163 7475 616c 2072  counterfactual r
-00001cd0: 756c 6573 2077 6974 6820 616e 2061 7070  ules with an app
-00001ce0: 726f 7072 6961 7465 2064 6973 6372 6574  ropriate discret
-00001cf0: 697a 6572 2061 7574 6f6d 6174 6963 616c  izer automatical
-00001d00: 6c79 2061 7373 6967 6e65 642e 2020 0d0a  ly assigned.  ..
-00001d10: 0d0a 6060 6070 7974 686f 6e0d 0a63 6f75  ..```python..cou
-00001d20: 6e74 6572 6661 6374 7561 6c5f 6578 706c  nterfactual_expl
-00001d30: 616e 6174 696f 6e73 203d 2065 7870 6c61  anations = expla
-00001d40: 696e 6572 2e65 7870 6c61 696e 5f63 6f75  iner.explain_cou
-00001d50: 6e74 6572 6661 6374 7561 6c28 585f 7465  nterfactual(X_te
-00001d60: 7374 290d 0a60 6060 0d0a 0d0a 436f 756e  st)..```....Coun
-00001d70: 7465 7266 6163 7475 616c 7320 6172 6520  terfactuals are 
-00001d80: 616c 736f 2076 6973 7561 6c69 7a65 6420  also visualized 
-00001d90: 7573 696e 6720 7468 6520 6070 6c6f 745f  using the `plot_
-00001da0: 616c 6c60 2e20 506c 6f74 7469 6e67 2061  all`. Plotting a
-00001db0: 6e20 696e 6469 7669 6475 616c 2063 6f75  n individual cou
-00001dc0: 6e74 6572 6661 6374 7561 6c20 6578 706c  nterfactual expl
-00001dd0: 616e 6174 696f 6e20 6973 2064 6f6e 6520  anation is done 
-00001de0: 7573 696e 6720 6070 6c6f 745f 6578 706c  using `plot_expl
-00001df0: 616e 6174 696f 6e60 2c20 7375 626d 6974  anation`, submit
-00001e00: 7469 6e67 2074 6865 2069 6e64 6578 206f  ting the index o
-00001e10: 6620 7468 6520 7465 7374 2069 6e73 7461  f the test insta
-00001e20: 6e63 6520 746f 2070 6c6f 742e 2041 6464  nce to plot. Add
-00001e30: 696e 6720 6f72 2072 656d 6f76 696e 6720  ing or removing 
-00001e40: 636f 6e6a 756e 6374 696f 6e73 2069 7320  conjunctions is 
-00001e50: 646f 6e65 2061 7320 6265 666f 7265 2e20  done as before. 
-00001e60: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a63  ....```python..c
-00001e70: 6f75 6e74 6572 6661 6374 7561 6c5f 6578  ounterfactual_ex
-00001e80: 706c 616e 6174 696f 6e73 2e70 6c6f 745f  planations.plot_
-00001e90: 616c 6c28 290d 0a63 6f75 6e74 6572 6661  all()..counterfa
-00001ea0: 6374 7561 6c5f 6578 706c 616e 6174 696f  ctual_explanatio
-00001eb0: 6e73 2e70 6c6f 745f 6578 706c 616e 6174  ns.plot_explanat
-00001ec0: 696f 6e28 3029 0d0a 636f 756e 7465 7266  ion(0)..counterf
-00001ed0: 6163 7475 616c 5f65 7870 6c61 6e61 7469  actual_explanati
-00001ee0: 6f6e 732e 6164 645f 636f 6e6a 756e 6374  ons.add_conjunct
-00001ef0: 696f 6e73 2829 2e70 6c6f 745f 616c 6c28  ions().plot_all(
-00001f00: 290d 0a60 6060 0d0a 0d0a 496e 6469 7669  )..```....Indivi
-00001f10: 6475 616c 2065 7870 6c61 6e61 7469 6f6e  dual explanation
-00001f20: 7320 6361 6e20 616c 736f 2062 6520 706c  s can also be pl
-00001f30: 6f74 7465 6420 7573 696e 6720 6070 6c6f  otted using `plo
-00001f40: 745f 6578 706c 616e 6174 696f 6e60 2e0d  t_explanation`..
-00001f50: 0a20 2020 2020 200d 0a60 6060 7079 7468  .      ..```pyth
-00001f60: 6f6e 0d0a 6661 6374 7561 6c5f 6578 706c  on..factual_expl
-00001f70: 616e 6174 696f 6e73 2e67 6574 5f65 7870  anations.get_exp
-00001f80: 6c61 6e61 7469 6f6e 2830 292e 706c 6f74  lanation(0).plot
-00001f90: 5f65 7870 6c61 6e61 7469 6f6e 2829 0d0a  _explanation()..
-00001fa0: 636f 756e 7465 7266 6163 7475 616c 5f65  counterfactual_e
-00001fb0: 7870 6c61 6e61 7469 6f6e 732e 6765 745f  xplanations.get_
-00001fc0: 6578 706c 616e 6174 696f 6e28 3029 2e70  explanation(0).p
-00001fd0: 6c6f 745f 6578 706c 616e 6174 696f 6e28  lot_explanation(
-00001fe0: 290d 0a60 6060 0d0a 2323 2323 2053 7570  )..```..#### Sup
-00001ff0: 706f 7274 2066 6f72 206d 756c 7469 636c  port for multicl
-00002000: 6173 730d 0a60 6361 6c69 6272 6174 6564  ass..`calibrated
-00002010: 2d65 7870 6c61 6e61 7469 6f6e 7360 2073  -explanations` s
-00002020: 7570 706f 7274 7320 6d75 6c74 6963 6c61  upports multicla
-00002030: 7373 2077 6869 6368 2069 7320 6465 6d6f  ss which is demo
-00002040: 6e73 7472 6174 6564 2069 6e20 5b64 656d  nstrated in [dem
-00002050: 6f5f 6d75 6c74 6963 6c61 7373 5d28 6874  o_multiclass](ht
-00002060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002070: 2f4d 6f66 6672 616e 2f63 616c 6962 7261  /Moffran/calibra
-00002080: 7465 645f 6578 706c 616e 6174 696f 6e73  ted_explanations
-00002090: 2f62 6c6f 622f 6d61 696e 2f6e 6f74 6562  /blob/main/noteb
-000020a0: 6f6f 6b73 2f64 656d 6f5f 6d75 6c74 6963  ooks/demo_multic
-000020b0: 6c61 7373 2e69 7079 6e62 292e 2054 6861  lass.ipynb). Tha
-000020c0: 7420 6e6f 7465 626f 6f6b 2061 6c73 6f20  t notebook also 
-000020d0: 6465 6d6f 6e73 7472 6174 6573 2068 6f77  demonstrates how
-000020e0: 2062 6f74 6820 6665 6174 7572 6520 6e61   both feature na
-000020f0: 6d65 7320 616e 6420 7461 7267 6574 2061  mes and target a
-00002100: 6e64 2063 6174 6567 6f72 6963 616c 206c  nd categorical l
-00002110: 6162 656c 7320 6361 6e20 6265 2061 6464  abels can be add
-00002120: 6564 2074 6f20 696d 7072 6f76 6520 7468  ed to improve th
-00002130: 6520 696e 7465 7270 7265 7461 6269 6c69  e interpretabili
-00002140: 7479 2e20 0d0a 0d0a 2323 2320 5265 6772  ty. ....### Regr
-00002150: 6573 7369 6f6e 0d0a 4578 7472 6163 7469  ession..Extracti
-00002160: 6e67 2065 7870 6c61 6e61 7469 6f6e 7320  ng explanations 
-00002170: 666f 7220 7265 6772 6573 7369 6f6e 2069  for regression i
-00002180: 7320 7665 7279 2073 696d 696c 6172 2074  s very similar t
-00002190: 6f20 686f 7720 6974 2069 7320 646f 6e65  o how it is done
-000021a0: 2066 6f72 2063 6c61 7373 6966 6963 6174   for classificat
-000021b0: 696f 6e2e 200d 0a0d 0a60 6060 7079 7468  ion. ....```pyth
-000021c0: 6f6e 0d0a 6461 7461 7365 7420 3d20 6665  on..dataset = fe
-000021d0: 7463 685f 6f70 656e 6d6c 286e 616d 653d  tch_openml(name=
-000021e0: 2268 6f75 7365 5f73 616c 6573 222c 2076  "house_sales", v
-000021f0: 6572 7369 6f6e 3d33 290d 0a0d 0a58 203d  ersion=3)....X =
-00002200: 2064 6174 6173 6574 2e64 6174 612e 7661   dataset.data.va
-00002210: 6c75 6573 2e61 7374 7970 6528 666c 6f61  lues.astype(floa
-00002220: 7429 0d0a 7920 3d20 6461 7461 7365 742e  t)..y = dataset.
-00002230: 7461 7267 6574 2e76 616c 7565 730d 0a0d  target.values...
-00002240: 0a58 5f74 7261 696e 2c20 585f 7465 7374  .X_train, X_test
-00002250: 2c20 795f 7472 6169 6e2c 2079 5f74 6573  , y_train, y_tes
-00002260: 7420 3d20 7472 6169 6e5f 7465 7374 5f73  t = train_test_s
-00002270: 706c 6974 2858 2c20 792c 2074 6573 745f  plit(X, y, test_
-00002280: 7369 7a65 3d31 290d 0a0d 0a58 5f70 726f  size=1)....X_pro
-00002290: 705f 7472 6169 6e2c 2058 5f63 616c 2c20  p_train, X_cal, 
-000022a0: 795f 7072 6f70 5f74 7261 696e 2c20 795f  y_prop_train, y_
-000022b0: 6361 6c20 3d20 7472 6169 6e5f 7465 7374  cal = train_test
-000022c0: 5f73 706c 6974 2858 5f74 7261 696e 2c20  _split(X_train, 
-000022d0: 795f 7472 6169 6e2c 0d0a 2020 2020 2020  y_train,..      
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002310: 2020 2020 2020 7465 7374 5f73 697a 653d        test_size=
-00002320: 302e 3235 290d 0a60 6060 0d0a 0d0a 4c65  0.25)..```....Le
-00002330: 7420 7573 206e 6f77 2066 6974 2061 2060  t us now fit a `
-00002340: 5261 6e64 6f6d 466f 7265 7374 5265 6772  RandomForestRegr
-00002350: 6573 736f 7260 2066 726f 6d0d 0a5b 736b  essor` from..[sk
-00002360: 6c65 6172 6e5d 2868 7474 7073 3a2f 2f73  learn](https://s
-00002370: 6369 6b69 742d 6c65 6172 6e2e 6f72 6729  cikit-learn.org)
-00002380: 2074 6f20 7468 6520 7072 6f70 6572 2074   to the proper t
-00002390: 7261 696e 696e 670d 0a73 6574 3a0d 0a0d  raining..set:...
-000023a0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-000023b0: 2073 6b6c 6561 726e 2e65 6e73 656d 626c   sklearn.ensembl
-000023c0: 6520 696d 706f 7274 2052 616e 646f 6d46  e import RandomF
-000023d0: 6f72 6573 7452 6567 7265 7373 6f72 0d0a  orestRegressor..
-000023e0: 0d0a 7266 203d 2052 616e 646f 6d46 6f72  ..rf = RandomFor
-000023f0: 6573 7452 6567 7265 7373 6f72 2829 0d0a  estRegressor()..
-00002400: 7266 2e66 6974 2858 5f70 726f 705f 7472  rf.fit(X_prop_tr
-00002410: 6169 6e2c 2079 5f70 726f 705f 7472 6169  ain, y_prop_trai
-00002420: 6e29 0d0a 6060 600d 0a0d 0a23 2323 2320  n)..```....#### 
-00002430: 4661 6374 7561 6c20 4578 706c 616e 6174  Factual Explanat
-00002440: 696f 6e73 0d0a 4465 6669 6e65 2061 2060  ions..Define a `
-00002450: 4361 6c69 6272 6174 6564 4578 706c 6169  CalibratedExplai
-00002460: 6e65 7260 206f 626a 6563 7420 7573 696e  ner` object usin
-00002470: 6720 7468 6520 6e65 7720 6d6f 6465 6c20  g the new model 
-00002480: 616e 6420 6461 7461 2e20 5468 6520 606d  and data. The `m
-00002490: 6f64 6560 2070 6172 616d 6574 6572 206d  ode` parameter m
-000024a0: 7573 7420 6265 2065 7870 6c69 6369 746c  ust be explicitl
-000024b0: 7920 7365 7420 746f 2072 6567 7265 7373  y set to regress
-000024c0: 696f 6e2e 2052 6567 756c 6172 2061 6e64  ion. Regular and
-000024d0: 2075 6e63 6572 7461 696e 7479 2070 6c6f   uncertainty plo
-000024e0: 7473 2077 6f72 6b20 696e 2074 6865 2073  ts work in the s
-000024f0: 616d 6520 7761 7920 6173 2066 6f72 2063  ame way as for c
-00002500: 6c61 7373 6966 6963 6174 696f 6e2e 0d0a  lassification...
-00002510: 0d0a 6060 6070 7974 686f 6e0d 0a65 7870  ..```python..exp
-00002520: 6c61 696e 6572 203d 2043 616c 6962 7261  lainer = Calibra
-00002530: 7465 6445 7870 6c61 696e 6572 2872 662c  tedExplainer(rf,
-00002540: 2058 5f63 616c 2c20 795f 6361 6c2c 206d   X_cal, y_cal, m
-00002550: 6f64 653d 2772 6567 7265 7373 696f 6e27  ode='regression'
-00002560: 290d 0a0d 0a66 6163 7475 616c 5f65 7870  )....factual_exp
-00002570: 6c61 6e61 7469 6f6e 7320 3d20 6578 706c  lanations = expl
-00002580: 6169 6e65 722e 6578 706c 6169 6e5f 6661  ainer.explain_fa
-00002590: 6374 7561 6c28 585f 7465 7374 290d 0a0d  ctual(X_test)...
-000025a0: 0a66 6163 7475 616c 5f65 7870 6c61 6e61  .factual_explana
-000025b0: 7469 6f6e 732e 706c 6f74 5f61 6c6c 2829  tions.plot_all()
-000025c0: 0d0a 6661 6374 7561 6c5f 6578 706c 616e  ..factual_explan
-000025d0: 6174 696f 6e73 2e70 6c6f 745f 616c 6c28  ations.plot_all(
-000025e0: 756e 6365 7274 6169 6e74 793d 5472 7565  uncertainty=True
-000025f0: 290d 0a0d 0a66 6163 7475 616c 5f65 7870  )....factual_exp
-00002600: 6c61 6e61 7469 6f6e 732e 6164 645f 636f  lanations.add_co
-00002610: 6e6a 756e 6374 696f 6e73 2829 2e70 6c6f  njunctions().plo
-00002620: 745f 616c 6c28 290d 0a60 6060 0d0a 4465  t_all()..```..De
-00002630: 6661 756c 742c 2074 6865 2063 6f6e 6669  fault, the confi
-00002640: 6465 6e63 6520 696e 7465 7276 616c 2069  dence interval i
-00002650: 7320 7365 7420 746f 2061 2073 796d 6d65  s set to a symme
-00002660: 7472 6963 2069 6e74 6572 7661 6c20 6f66  tric interval of
-00002670: 2039 3025 2028 6465 6669 6e65 6420 6173   90% (defined as
-00002680: 2060 6c6f 775f 6869 6768 5f70 6572 6365   `low_high_perce
-00002690: 6e74 696c 6573 3d28 352c 3935 2960 292e  ntiles=(5,95)`).
-000026a0: 2054 6865 2069 6e74 6572 7661 6c73 2063   The intervals c
-000026b0: 616e 2063 6f76 6572 2061 6e79 2075 7365  an cover any use
-000026c0: 7220 7370 6563 6966 6965 6420 696e 7465  r specified inte
-000026d0: 7276 616c 2c20 696e 636c 7564 696e 6720  rval, including 
-000026e0: 6f6e 652d 7369 6465 6420 696e 7465 7276  one-sided interv
-000026f0: 616c 732e 2054 6f20 6465 6669 6e65 2061  als. To define a
-00002700: 206f 6e65 2d73 6964 6564 2075 7070 6572   one-sided upper
-00002710: 2d62 6f75 6e64 6564 2039 3025 2069 6e74  -bounded 90% int
-00002720: 6572 7661 6c2c 2073 6574 2060 6c6f 775f  erval, set `low_
-00002730: 6869 6768 5f70 6572 6365 6e74 696c 6573  high_percentiles
-00002740: 3d28 2d6e 702e 696e 662c 3930 2960 2c20  =(-np.inf,90)`, 
-00002750: 616e 6420 746f 2064 6566 696e 6520 6120  and to define a 
-00002760: 6f6e 652d 7369 6465 6420 6c6f 7765 722d  one-sided lower-
-00002770: 626f 756e 6465 6420 3935 2520 696e 7465  bounded 95% inte
-00002780: 7276 616c 2c20 7365 7420 606c 6f77 5f68  rval, set `low_h
-00002790: 6967 685f 7065 7263 656e 7469 6c65 733d  igh_percentiles=
-000027a0: 2835 2c6e 702e 696e 6629 602e 2050 6572  (5,np.inf)`. Per
-000027b0: 6365 6e74 696c 6573 2063 616e 2061 6c73  centiles can als
-000027c0: 6f20 6265 2073 6574 2074 6f20 616e 7920  o be set to any 
-000027d0: 6f74 6865 7220 7661 6c75 6573 2069 6e20  other values in 
-000027e0: 7468 6520 7261 6e67 6520 2830 2c31 3030  the range (0,100
-000027f0: 2920 2865 7863 6c75 7369 7665 292c 2061  ) (exclusive), a
-00002800: 6e64 2069 6e74 6572 7661 6c73 2064 6f20  nd intervals do 
-00002810: 6e6f 7420 6861 7665 2074 6f20 6265 2073  not have to be s
-00002820: 796d 6d65 7472 6963 2e20 0d0a 0d0a 6060  ymmetric. ....``
-00002830: 6070 7974 686f 6e0d 0a6c 6f77 6572 5f62  `python..lower_b
-00002840: 6f75 6e64 6564 5f65 7870 6c61 6e61 7469  ounded_explanati
-00002850: 6f6e 7320 3d20 6578 706c 6169 6e65 722e  ons = explainer.
-00002860: 6578 706c 6169 6e5f 6661 6374 7561 6c28  explain_factual(
-00002870: 585f 7465 7374 2c20 6c6f 775f 6869 6768  X_test, low_high
-00002880: 5f70 6572 6365 6e74 696c 6573 3d28 352c  _percentiles=(5,
-00002890: 6e70 2e69 6e66 2929 0d0a 6173 796d 6d65  np.inf))..asymme
-000028a0: 7472 6963 5f65 7870 6c61 6e61 7469 6f6e  tric_explanation
-000028b0: 7320 3d20 6578 706c 6169 6e65 722e 6578  s = explainer.ex
-000028c0: 706c 6169 6e5f 6661 6374 7561 6c28 585f  plain_factual(X_
-000028d0: 7465 7374 2c20 6c6f 775f 6869 6768 5f70  test, low_high_p
-000028e0: 6572 6365 6e74 696c 6573 3d28 352c 3735  ercentiles=(5,75
-000028f0: 2929 0d0a 6060 600d 0a0d 0a23 2323 2320  ))..```....#### 
-00002900: 436f 756e 7465 7266 6163 7475 616c 2045  Counterfactual E
-00002910: 7870 6c61 6e61 7469 6f6e 730d 0a54 6865  xplanations..The
-00002920: 2060 6578 706c 6169 6e5f 636f 756e 7465   `explain_counte
-00002930: 7266 6163 7475 616c 6020 7769 6c6c 2077  rfactual` will w
-00002940: 6f72 6b20 6578 6163 746c 7920 7468 6520  ork exactly the 
-00002950: 7361 6d65 2061 7320 666f 7220 636c 6173  same as for clas
-00002960: 7369 6669 6361 7469 6f6e 2e20 436f 756e  sification. Coun
-00002970: 7465 7266 6163 7475 616c 2070 6c6f 7473  terfactual plots
-00002980: 2077 6f72 6b20 696e 2074 6865 2073 616d   work in the sam
-00002990: 6520 7761 7920 6173 2066 6f72 2063 6c61  e way as for cla
-000029a0: 7373 6966 6963 6174 696f 6e2e 0d0a 0d0a  ssification.....
-000029b0: 6060 6070 7974 686f 6e0d 0a63 6f75 6e74  ```python..count
-000029c0: 6572 6661 6374 7561 6c5f 6578 706c 616e  erfactual_explan
-000029d0: 6174 696f 6e73 203d 2065 7870 6c61 696e  ations = explain
-000029e0: 6572 2e65 7870 6c61 696e 5f63 6f75 6e74  er.explain_count
-000029f0: 6572 6661 6374 7561 6c28 585f 7465 7374  erfactual(X_test
-00002a00: 290d 0a0d 0a63 6f75 6e74 6572 6661 6374  )....counterfact
-00002a10: 7561 6c5f 6578 706c 616e 6174 696f 6e73  ual_explanations
-00002a20: 2e70 6c6f 745f 616c 6c28 290d 0a63 6f75  .plot_all()..cou
-00002a30: 6e74 6572 6661 6374 7561 6c5f 6578 706c  nterfactual_expl
-00002a40: 616e 6174 696f 6e73 2e61 6464 5f63 6f6e  anations.add_con
-00002a50: 6a75 6e63 7469 6f6e 7328 292e 706c 6f74  junctions().plot
-00002a60: 5f61 6c6c 2829 0d0a 0d0a 636f 756e 7465  _all()....counte
-00002a70: 7266 6163 7475 616c 5f65 7870 6c61 6e61  rfactual_explana
-00002a80: 7469 6f6e 732e 706c 6f74 5f65 7870 6c61  tions.plot_expla
-00002a90: 6e61 7469 6f6e 2830 290d 0a60 6060 0d0a  nation(0)..```..
-00002aa0: 5468 6520 7061 7261 6d65 7465 7220 606c  The parameter `l
-00002ab0: 6f77 5f68 6967 685f 7065 7263 656e 7469  ow_high_percenti
-00002ac0: 6c65 7360 2077 6f72 6b73 2069 6e20 7468  les` works in th
-00002ad0: 6520 7361 6d65 2077 6179 2061 7320 666f  e same way as fo
-00002ae0: 7220 6661 6374 7561 6c20 6578 706c 616e  r factual explan
-00002af0: 6174 696f 6e73 2e20 0d0a 0d0a 2323 2323  ations. ....####
-00002b00: 2050 726f 6261 6269 6c69 7374 6963 2052   Probabilistic R
-00002b10: 6567 7265 7373 696f 6e20 4578 706c 616e  egression Explan
-00002b20: 6174 696f 6e73 0d0a 4974 2069 7320 706f  ations..It is po
-00002b30: 7373 6962 6c65 2074 6f20 6372 6561 7465  ssible to create
-00002b40: 2070 726f 6261 6269 6c69 7374 6963 2065   probabilistic e
-00002b50: 7870 6c61 6e61 7469 6f6e 7320 666f 7220  xplanations for 
-00002b60: 7265 6772 6573 7369 6f6e 2c20 7072 6f76  regression, prov
-00002b70: 6964 696e 6720 7468 6520 7072 6f62 6162  iding the probab
-00002b80: 696c 6974 7920 7468 6174 2074 6865 2074  ility that the t
-00002b90: 6172 6765 7420 7661 6c75 6520 6973 2062  arget value is b
-00002ba0: 656c 6f77 2074 6865 2070 726f 7669 6465  elow the provide
-00002bb0: 6420 7468 7265 7368 6f6c 6420 2877 6869  d threshold (whi
-00002bc0: 6368 2069 7320 3138 3020 3030 3020 696e  ch is 180 000 in
-00002bd0: 2074 6865 2065 7861 6d70 6c65 7320 6265   the examples be
-00002be0: 6c6f 7729 2e20 416c 6c20 6d65 7468 6f64  low). All method
-00002bf0: 7320 6172 6520 7468 6520 7361 6d65 2061  s are the same a
-00002c00: 7320 666f 7220 6e6f 726d 616c 2072 6567  s for normal reg
-00002c10: 7265 7373 696f 6e20 616e 6420 636c 6173  ression and clas
-00002c20: 7369 6669 6361 7469 6f6e 2c20 6578 6365  sification, exce
-00002c30: 7074 2074 6861 7420 7468 6520 6065 7870  pt that the `exp
-00002c40: 6c61 696e 5f66 6163 7475 616c 6020 616e  lain_factual` an
-00002c50: 6420 6065 7870 6c61 696e 5f63 6f75 6e74  d `explain_count
-00002c60: 6572 6661 6374 7561 6c60 206d 6574 686f  erfactual` metho
-00002c70: 6473 206e 6565 6420 7468 6520 6164 6469  ds need the addi
-00002c80: 7469 6f6e 616c 2074 6872 6573 686f 6c64  tional threshold
-00002c90: 2076 616c 7565 2028 6865 7265 2031 3830   value (here 180
-00002ca0: 2030 3030 292e 0d0a 0d0a 6060 6070 7974   000).....```pyt
-00002cb0: 686f 6e0d 0a66 6163 7475 616c 5f65 7870  hon..factual_exp
-00002cc0: 6c61 6e61 7469 6f6e 7320 3d20 6578 706c  lanations = expl
-00002cd0: 6169 6e65 722e 6578 706c 6169 6e5f 6661  ainer.explain_fa
-00002ce0: 6374 7561 6c28 585f 7465 7374 2c20 3138  ctual(X_test, 18
-00002cf0: 3030 3030 290d 0a0d 0a66 6163 7475 616c  0000)....factual
-00002d00: 5f65 7870 6c61 6e61 7469 6f6e 732e 706c  _explanations.pl
-00002d10: 6f74 5f61 6c6c 2829 0d0a 6661 6374 7561  ot_all()..factua
-00002d20: 6c5f 6578 706c 616e 6174 696f 6e73 2e70  l_explanations.p
-00002d30: 6c6f 745f 616c 6c28 756e 6365 7274 6169  lot_all(uncertai
-00002d40: 6e74 793d 5472 7565 290d 0a0d 0a66 6163  nty=True)....fac
-00002d50: 7475 616c 5f65 7870 6c61 6e61 7469 6f6e  tual_explanation
-00002d60: 732e 6164 645f 636f 6e6a 756e 6374 696f  s.add_conjunctio
-00002d70: 6e73 2829 2e70 6c6f 745f 616c 6c28 290d  ns().plot_all().
-00002d80: 0a0d 0a63 6f75 6e74 6572 6661 6374 7561  ...counterfactua
-00002d90: 6c5f 6578 706c 616e 6174 696f 6e73 203d  l_explanations =
-00002da0: 2065 7870 6c61 696e 6572 2e65 7870 6c61   explainer.expla
-00002db0: 696e 5f63 6f75 6e74 6572 6661 6374 7561  in_counterfactua
-00002dc0: 6c28 585f 7465 7374 2c20 3138 3030 3030  l(X_test, 180000
-00002dd0: 290d 0a0d 0a63 6f75 6e74 6572 6661 6374  )....counterfact
-00002de0: 7561 6c5f 6578 706c 616e 6174 696f 6e73  ual_explanations
-00002df0: 2e70 6c6f 745f 616c 6c28 290d 0a63 6f75  .plot_all()..cou
-00002e00: 6e74 6572 6661 6374 7561 6c5f 6578 706c  nterfactual_expl
-00002e10: 616e 6174 696f 6e73 2e61 6464 5f63 6f6e  anations.add_con
-00002e20: 6a75 6e63 7469 6f6e 7328 292e 706c 6f74  junctions().plot
-00002e30: 5f61 6c6c 2829 0d0a 6060 600d 0a0d 0a23  _all()..```....#
-00002e40: 2323 2320 4164 6469 7469 6f6e 616c 2052  ### Additional R
-00002e50: 6567 7265 7373 696f 6e20 5573 6520 4361  egression Use Ca
-00002e60: 7365 730d 0a52 6567 7265 7373 696f 6e20  ses..Regression 
-00002e70: 6f66 6665 7273 206d 616e 7920 6d6f 7265  offers many more
-00002e80: 206f 7074 696f 6e73 2061 6e64 2074 6f20   options and to 
-00002e90: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
-00002ea0: 2074 6865 6d2c 2073 6565 2074 6865 205b   them, see the [
-00002eb0: 6465 6d6f 5f72 6567 7265 7373 696f 6e5d  demo_regression]
-00002ec0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002ed0: 636f 6d2f 4d6f 6666 7261 6e2f 6361 6c69  com/Moffran/cali
-00002ee0: 6272 6174 6564 5f65 7870 6c61 6e61 7469  brated_explanati
-00002ef0: 6f6e 732f 626c 6f62 2f6d 6169 6e2f 6e6f  ons/blob/main/no
-00002f00: 7465 626f 6f6b 732f 6465 6d6f 5f72 6567  tebooks/demo_reg
-00002f10: 7265 7373 696f 6e2e 6970 796e 6229 206f  ression.ipynb) o
-00002f20: 7220 7468 6520 5b64 656d 6f5f 7072 6f62  r the [demo_prob
-00002f30: 6162 696c 6973 7469 635f 7265 6772 6573  abilistic_regres
-00002f40: 7369 6f6e 5d28 6874 7470 733a 2f2f 6769  sion](https://gi
-00002f50: 7468 7562 2e63 6f6d 2f4d 6f66 6672 616e  thub.com/Moffran
-00002f60: 2f63 616c 6962 7261 7465 645f 6578 706c  /calibrated_expl
-00002f70: 616e 6174 696f 6e73 2f62 6c6f 622f 6d61  anations/blob/ma
-00002f80: 696e 2f6e 6f74 6562 6f6f 6b73 2f64 656d  in/notebooks/dem
-00002f90: 6f5f 7072 6f62 6162 696c 6973 7469 635f  o_probabilistic_
-00002fa0: 7265 6772 6573 7369 6f6e 2e69 7079 6e62  regression.ipynb
-00002fb0: 2920 6e6f 7465 626f 6f6b 732e 0d0a 0d0a  ) notebooks.....
-00002fc0: 5b54 6f70 5d28 2363 616c 6962 7261 7465  [Top](#calibrate
-00002fd0: 642d 6578 706c 616e 6174 696f 6e73 2d64  d-explanations-d
-00002fe0: 6f63 756d 656e 7461 7469 6f6e 290d 0a0d  ocumentation)...
-00002ff0: 0a4b 6e6f 776e 204c 696d 6974 6174 696f  .Known Limitatio
-00003000: 6e73 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ns..------------
-00003010: 2d2d 2d2d 2d0d 0a54 6865 2069 6d70 6c65  -----..The imple
-00003020: 6d65 6e74 6174 696f 6e20 6375 7272 656e  mentation curren
-00003030: 746c 7920 6f6e 6c79 2073 7570 706f 7274  tly only support
-00003040: 206e 756d 6572 6963 616c 2069 6e70 7574   numerical input
-00003050: 2e20 5573 6520 7468 6520 6075 7469 6c73  . Use the `utils
-00003060: 2e74 7261 6e73 666f 726d 5f74 6f5f 6e75  .transform_to_nu
-00003070: 6d65 7269 6360 2028 7265 6c65 6173 6564  meric` (released
-00003080: 2069 6e20 7665 7273 696f 6e20 7630 2e33   in version v0.3
-00003090: 2e32 2920 746f 2074 7261 6e73 666f 726d  .2) to transform
-000030a0: 2061 2060 4461 7461 4672 616d 6560 2077   a `DataFrame` w
-000030b0: 6974 6820 7465 7874 2064 6174 6120 696e  ith text data in
-000030c0: 746f 206e 756d 6572 6963 616c 2066 6f72  to numerical for
-000030d0: 6d20 616e 6420 6174 2074 6865 2073 616d  m and at the sam
-000030e0: 6520 7469 6d65 2065 7874 7261 6374 696e  e time extractin
-000030f0: 6720 6063 6174 6567 6f72 6963 616c 5f66  g `categorical_f
-00003100: 6561 7475 7265 7360 2c20 6063 6174 6567  eatures`, `categ
-00003110: 6f72 6963 616c 5f6c 6162 656c 7360 2c20  orical_labels`, 
-00003120: 6074 6172 6765 745f 6c61 6265 6c73 6020  `target_labels` 
-00003130: 2869 6620 7465 7874 206c 6162 656c 7329  (if text labels)
-00003140: 2061 6e64 2060 6d61 7070 696e 6773 6020   and `mappings` 
-00003150: 2875 7365 6420 746f 2061 7070 6c79 2074  (used to apply t
-00003160: 6865 2073 616d 6520 6d61 7070 696e 6773  he same mappings
-00003170: 2074 6f20 6e65 7720 6461 7461 2920 746f   to new data) to
-00003180: 2062 6520 7573 6564 2061 7320 696e 7075   be used as inpu
-00003190: 7420 746f 2074 6865 2060 4361 6c69 6272  t to the `Calibr
-000031a0: 6174 6564 4578 706c 6169 6e65 7260 2e20  atedExplainer`. 
-000031b0: 5468 6520 616c 676f 7269 7468 6d20 646f  The algorithm do
-000031c0: 6573 206e 6f74 2063 7572 7265 6e74 6c79  es not currently
-000031d0: 2073 7570 706f 7274 2069 6d61 6765 2064   support image d
-000031e0: 6174 612e 0d0a 0d0a 5b54 6f70 5d28 2363  ata.....[Top](#c
-000031f0: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
-00003200: 6174 696f 6e73 2d64 6f63 756d 656e 7461  ations-documenta
-00003210: 7469 6f6e 290d 0a0d 0a49 6e73 7461 6c6c  tion)....Install
-00003220: 0d0a 2d2d 2d2d 2d2d 2d0d 0a0d 0a60 6361  ..-------....`ca
-00003230: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
-00003240: 7469 6f6e 7360 2069 7320 696d 706c 656d  tions` is implem
-00003250: 656e 7465 6420 696e 2050 7974 686f 6e2c  ented in Python,
-00003260: 2073 6f20 796f 7520 6e65 6564 2061 2050   so you need a P
-00003270: 7974 686f 6e20 656e 7669 726f 6e6d 656e  ython environmen
-00003280: 742e 0d0a 0d0a 496e 7374 616c 6c20 6063  t.....Install `c
-00003290: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
-000032a0: 6174 696f 6e73 6020 6672 6f6d 2050 7950  ations` from PyP
-000032b0: 493a 0d0a 0d0a 0970 6970 2069 6e73 7461  I:.....pip insta
-000032c0: 6c6c 2063 616c 6962 7261 7465 642d 6578  ll calibrated-ex
-000032d0: 706c 616e 6174 696f 6e73 0d0a 0d0a 6f72  planations....or
-000032e0: 2066 726f 6d20 636f 6e64 612d 666f 7267   from conda-forg
-000032f0: 653a 0d0a 090d 0a20 0963 6f6e 6461 2069  e:..... .conda i
-00003300: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
-00003310: 666f 7267 6520 6361 6c69 6272 6174 6564  forge calibrated
-00003320: 2d65 7870 6c61 6e61 7469 6f6e 730d 0a0d  -explanations...
-00003330: 0a6f 7220 6279 2066 6f6c 6c6f 7769 6e67  .or by following
-00003340: 2066 7572 7468 6572 2069 6e73 7472 7563   further instruc
-00003350: 7469 6f6e 7320 6174 205b 636f 6e64 612d  tions at [conda-
-00003360: 666f 7267 655d 2868 7474 7073 3a2f 2f67  forge](https://g
-00003370: 6974 6875 622e 636f 6d2f 636f 6e64 612d  ithub.com/conda-
-00003380: 666f 7267 652f 6361 6c69 6272 6174 6564  forge/calibrated
-00003390: 2d65 7870 6c61 6e61 7469 6f6e 732d 6665  -explanations-fe
-000033a0: 6564 7374 6f63 6b23 696e 7374 616c 6c69  edstock#installi
-000033b0: 6e67 2d63 616c 6962 7261 7465 642d 6578  ng-calibrated-ex
-000033c0: 706c 616e 6174 696f 6e73 292e 0d0a 0d0a  planations).....
-000033d0: 5468 6520 6465 7065 6e64 656e 6369 6573  The dependencies
-000033e0: 2061 7265 3a0d 0a0d 0a2a 205b 6372 6570   are:....* [crep
-000033f0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00003400: 7562 2e63 6f6d 2f68 656e 7269 6b62 6f73  ub.com/henrikbos
-00003410: 7472 6f6d 2f63 7265 7065 7329 0d0a 2a20  trom/crepes)..* 
-00003420: 5b76 656e 6e2d 6162 6572 735d 2868 7474  [venn-abers](htt
-00003430: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003440: 6970 3230 302f 7665 6e6e 2d61 6265 7273  ip200/venn-abers
-00003450: 290d 0a2a 205b 6c69 6d65 5d28 6874 7470  )..* [lime](http
-00003460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00003470: 6172 636f 7463 722f 6c69 6d65 290d 0a2a  arcotcr/lime)..*
-00003480: 205b 6d61 7470 6c6f 746c 6962 5d28 6874   [matplotlib](ht
-00003490: 7470 733a 2f2f 6d61 7470 6c6f 746c 6962  tps://matplotlib
-000034a0: 2e6f 7267 2f29 0d0a 2a20 5b4e 756d 5079  .org/)..* [NumPy
-000034b0: 5d28 6874 7470 733a 2f2f 6e75 6d70 792e  ](https://numpy.
-000034c0: 6f72 672f 290d 0a20 200d 0a5b 546f 705d  org/)..  ..[Top]
-000034d0: 2823 6361 6c69 6272 6174 6564 2d65 7870  (#calibrated-exp
-000034e0: 6c61 6e61 7469 6f6e 732d 646f 6375 6d65  lanations-docume
-000034f0: 6e74 6174 696f 6e29 0d0a 0d0a 0d0a 436f  ntation)......Co
-00003500: 6e74 7269 6275 7469 6e67 0d0a 2d2d 2d2d  ntributing..----
-00003510: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 436f 6e74  --------....Cont
-00003520: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
-00003530: 6c63 6f6d 652e 0d0a 506c 6561 7365 2073  lcome...Please s
-00003540: 656e 6420 6275 6720 7265 706f 7274 732c  end bug reports,
-00003550: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
-00003560: 7320 6f72 2070 756c 6c20 7265 7175 6573  s or pull reques
-00003570: 7473 2074 6872 6f75 6768 0d0a 7468 6520  ts through..the 
-00003580: 7072 6f6a 6563 7420 7061 6765 206f 6e20  project page on 
-00003590: 5b47 6974 4875 625d 2868 7474 7073 3a2f  [GitHub](https:/
-000035a0: 2f67 6974 6875 622e 636f 6d2f 4d6f 6666  /github.com/Moff
-000035b0: 7261 6e2f 6361 6c69 6272 6174 6564 5f65  ran/calibrated_e
-000035c0: 7870 6c61 6e61 7469 6f6e 7329 2e0d 0a59  xplanations)...Y
-000035d0: 6f75 2063 616e 2066 696e 6420 6120 6465  ou can find a de
-000035e0: 7461 696c 6564 2067 7569 6465 2066 6f72  tailed guide for
-000035f0: 2063 6f6e 7472 6962 7574 696f 6e73 2069   contributions i
-00003600: 6e0d 0a5b 434f 4e54 5249 4255 5449 4e47  n..[CONTRIBUTING
-00003610: 2e6d 645d 2868 7474 7073 3a2f 2f67 6974  .md](https://git
-00003620: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
-00003630: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
-00003640: 6e61 7469 6f6e 732f 626c 6f62 2f6d 6169  nations/blob/mai
-00003650: 6e2f 434f 4e54 5249 4255 5449 4e47 2e6d  n/CONTRIBUTING.m
-00003660: 6429 2e0d 0a0d 0a5b 546f 705d 2823 6361  d).....[Top](#ca
-00003670: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
-00003680: 7469 6f6e 732d 646f 6375 6d65 6e74 6174  tions-documentat
-00003690: 696f 6e29 0d0a 0d0a 0d0a 446f 6375 6d65  ion)......Docume
-000036a0: 6e74 6174 696f 6e0d 0a2d 2d2d 2d2d 2d2d  ntation..-------
-000036b0: 2d2d 2d2d 2d2d 0d0a 466f 7220 646f 6375  ------..For docu
-000036c0: 6d65 6e74 6174 696f 6e2c 2073 6565 205b  mentation, see [
-000036d0: 6361 6c69 6272 6174 6564 2d65 7870 6c61  calibrated-expla
-000036e0: 6e61 7469 6f6e 732e 7265 6164 7468 6564  nations.readthed
-000036f0: 6f63 732e 696f 5d28 6874 7470 733a 2f2f  ocs.io](https://
-00003700: 6361 6c69 6272 6174 6564 2d65 7870 6c61  calibrated-expla
-00003710: 6e61 7469 6f6e 732e 7265 6164 7468 6564  nations.readthed
-00003720: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00003730: 2f3f 6261 6467 653d 6c61 7465 7374 292e  /?badge=latest).
-00003740: 0d0a 2020 0d0a 5b54 6f70 5d28 2363 616c  ..  ..[Top](#cal
-00003750: 6962 7261 7465 642d 6578 706c 616e 6174  ibrated-explanat
-00003760: 696f 6e73 2d64 6f63 756d 656e 7461 7469  ions-documentati
-00003770: 6f6e 290d 0a0d 0a46 7572 7468 6572 2072  on)....Further r
-00003780: 6561 6469 6e67 2061 6e64 2063 6974 696e  eading and citin
-00003790: 670d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  g..-------------
-000037a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a54  -------------..T
-000037b0: 6865 2060 6361 6c69 6272 6174 6564 2d65  he `calibrated-e
-000037c0: 7870 6c61 6e61 7469 6f6e 7360 206d 6574  xplanations` met
-000037d0: 686f 6420 666f 7220 636c 6173 7369 6669  hod for classifi
-000037e0: 6361 7469 6f6e 2069 7320 696e 7472 6f64  cation is introd
-000037f0: 7563 6564 2069 6e20 7468 6520 7061 7065  uced in the pape
-00003800: 723a 0d0a 0d0a 2d20 5b4c c3b6 6673 7472  r:....- [L..fstr
-00003810: c3b6 6d2c 2048 5d28 6874 7470 733a 2f2f  ..m, H](https://
-00003820: 6769 7468 7562 2e63 6f6d 2f4d 6f66 6672  github.com/Moffr
-00003830: 616e 292e 2c20 5b4c c3b6 6673 7472 c3b6  an)., [L..fstr..
-00003840: 6d2c 2054 5d28 6874 7470 733a 2f2f 6769  m, T](https://gi
-00003850: 7468 7562 2e63 6f6d 2f74 7576 656c 6f66  thub.com/tuvelof
-00003860: 7374 726f 6d29 2e2c 204a 6f68 616e 7373  strom)., Johanss
-00003870: 6f6e 2c20 552e 2c20 616e 6420 53c3 b66e  on, U., and S..n
-00003880: 7374 72c3 b664 2c20 432e 2028 3230 3234  str..d, C. (2024
-00003890: 292e 205b 4361 6c69 6272 6174 6564 2045  ). [Calibrated E
-000038a0: 7870 6c61 6e61 7469 6f6e 733a 2077 6974  xplanations: wit
-000038b0: 6820 556e 6365 7274 6169 6e74 7920 496e  h Uncertainty In
-000038c0: 666f 726d 6174 696f 6e20 616e 6420 436f  formation and Co
-000038d0: 756e 7465 7266 6163 7475 616c 735d 2868  unterfactuals](h
-000038e0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-000038f0: 302e 3130 3136 2f6a 2e65 7377 612e 3230  0.1016/j.eswa.20
-00003900: 3234 2e31 3233 3135 3429 2e20 4578 7065  24.123154). Expe
-00003910: 7274 2053 7973 7465 6d73 2077 6974 6820  rt Systems with 
-00003920: 4170 706c 6963 6174 696f 6e73 2c20 312d  Applications, 1-
-00003930: 3237 2e0d 0a0d 0a54 6865 2065 7874 656e  27.....The exten
-00003940: 7369 6f6e 7320 666f 7220 7265 6772 6573  sions for regres
-00003950: 7369 6f6e 2061 7265 2069 6e74 726f 6475  sion are introdu
-00003960: 6365 6420 696e 2074 6865 2070 6170 6572  ced in the paper
-00003970: 3a0d 0a0d 0a2d 205b 4cc3 b666 7374 72c3  :....- [L..fstr.
-00003980: b66d 2c20 545d 2868 7474 7073 3a2f 2f67  .m, T](https://g
-00003990: 6974 6875 622e 636f 6d2f 7475 7665 6c6f  ithub.com/tuvelo
-000039a0: 6673 7472 6f6d 292e 2c20 5b4c c3b6 6673  fstrom)., [L..fs
-000039b0: 7472 c3b6 6d2c 2048 5d28 6874 7470 733a  tr..m, H](https:
-000039c0: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 6f66  //github.com/Mof
-000039d0: 6672 616e 292e 2c20 4a6f 6861 6e73 736f  fran)., Johansso
-000039e0: 6e2c 2055 2e2c 2053 c3b6 6e73 7472 c3b6  n, U., S..nstr..
-000039f0: 642c 2043 2e2c 2061 6e64 205b 4d61 7465  d, C., and [Mate
-00003a00: 6c61 2c20 525d 2868 7474 7073 3a2f 2f67  la, R](https://g
-00003a10: 6974 6875 622e 636f 6d2f 7275 6479 6d61  ithub.com/rudyma
-00003a20: 7465 6c61 292e 205b 4361 6c69 6272 6174  tela). [Calibrat
-00003a30: 6564 2045 7870 6c61 6e61 7469 6f6e 7320  ed Explanations 
-00003a40: 666f 7220 5265 6772 6573 7369 6f6e 5d28  for Regression](
-00003a50: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00003a60: 672f 6162 732f 3233 3038 2e31 3632 3435  g/abs/2308.16245
-00003a70: 292e 2061 7258 6976 2070 7265 7072 696e  ). arXiv preprin
-00003a80: 7420 6172 5869 763a 3233 3038 2e31 3632  t arXiv:2308.162
-00003a90: 3435 2e0d 0a0d 0a54 6865 2070 6170 6572  45.....The paper
-00003aa0: 2074 6861 7420 6f72 6967 696e 6174 6564   that originated
-00003ab0: 2074 6865 2069 6465 6120 6f66 2060 6361   the idea of `ca
-00003ac0: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
-00003ad0: 7469 6f6e 7360 2069 733a 0d0a 0d0a 2d20  tions` is:....- 
-00003ae0: 5b4c c3b6 6673 7472 c3b6 6d2c 2048 2e5d  [L..fstr..m, H.]
-00003af0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00003b00: 636f 6d2f 4d6f 6666 7261 6e29 2c20 5b4c  com/Moffran), [L
-00003b10: c3b6 6673 7472 c3b6 6d2c 2054 2e5d 2868  ..fstr..m, T.](h
-00003b20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003b30: 6d2f 7475 7665 6c6f 6673 7472 6f6d 292c  m/tuvelofstrom),
-00003b40: 204a 6f68 616e 7373 6f6e 2c20 552e 2c20   Johansson, U., 
-00003b50: 2620 53c3 b66e 7374 72c3 b664 2c20 432e  & S..nstr..d, C.
-00003b60: 2028 3230 3233 292e 205b 496e 7665 7374   (2023). [Invest
-00003b70: 6967 6174 696e 6720 7468 6520 696d 7061  igating the impa
-00003b80: 6374 206f 6620 6361 6c69 6272 6174 696f  ct of calibratio
-00003b90: 6e20 6f6e 2074 6865 2071 7561 6c69 7479  n on the quality
-00003ba0: 206f 6620 6578 706c 616e 6174 696f 6e73   of explanations
-00003bb0: 5d28 6874 7470 733a 2f2f 6c69 6e6b 2e73  ](https://link.s
-00003bc0: 7072 696e 6765 722e 636f 6d2f 6172 7469  pringer.com/arti
-00003bd0: 636c 652f 3130 2e31 3030 372f 7331 3034  cle/10.1007/s104
-00003be0: 3732 2d30 3233 2d30 3938 3337 2d32 292e  72-023-09837-2).
-00003bf0: 2041 6e6e 616c 7320 6f66 204d 6174 6865   Annals of Mathe
-00003c00: 6d61 7469 6373 2061 6e64 2041 7274 6966  matics and Artif
-00003c10: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
-00003c20: 6365 2c20 312d 3138 2e20 5b43 6f64 6520  ce, 1-18. [Code 
-00003c30: 616e 6420 7265 7375 6c74 735d 2868 7474  and results](htt
-00003c40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00003c50: 7475 7665 6c6f 6673 7472 6f6d 2f63 616c  tuvelofstrom/cal
-00003c60: 6962 7261 7469 6e67 2d65 7870 6c61 6e61  ibrating-explana
-00003c70: 7469 6f6e 7329 2e0d 0a0d 0a49 6620 796f  tions).....If yo
-00003c80: 7520 7573 6520 6063 616c 6962 7261 7465  u use `calibrate
-00003c90: 642d 6578 706c 616e 6174 696f 6e73 6020  d-explanations` 
-00003ca0: 666f 7220 6120 7363 6965 6e74 6966 6963  for a scientific
-00003cb0: 2070 7562 6c69 6361 7469 6f6e 2c20 796f   publication, yo
-00003cc0: 7520 6172 6520 6b69 6e64 6c79 2072 6571  u are kindly req
-00003cd0: 7565 7374 6564 2074 6f20 6369 7465 206f  uested to cite o
-00003ce0: 6e65 206f 6620 7468 6520 7061 7065 7273  ne of the papers
-00003cf0: 2061 626f 7665 2e0d 0a0d 0a42 6962 7465   above.....Bibte
-00003d00: 7820 656e 7472 7920 666f 7220 7468 6520  x entry for the 
-00003d10: 6f72 6967 696e 616c 2070 6170 6572 3a0d  original paper:.
-00003d20: 0a0d 0a60 6060 6269 6274 6578 0d0a 4061  ...```bibtex..@a
-00003d30: 7274 6963 6c65 7b6c 6f66 7374 726f 6d32  rticle{lofstrom2
-00003d40: 3032 3463 616c 6962 7261 7465 642c 0d0a  024calibrated,..
-00003d50: 0974 6974 6c65 203d 2009 7b43 616c 6962  .title = .{Calib
-00003d60: 7261 7465 6420 6578 706c 616e 6174 696f  rated explanatio
-00003d70: 6e73 3a20 5769 7468 2075 6e63 6572 7461  ns: With uncerta
-00003d80: 696e 7479 2069 6e66 6f72 6d61 7469 6f6e  inty information
-00003d90: 2061 6e64 2063 6f75 6e74 6572 6661 6374   and counterfact
-00003da0: 7561 6c73 7d2c 0d0a 096a 6f75 726e 616c  uals},...journal
-00003db0: 203d 2009 7b45 7870 6572 7420 5379 7374   = .{Expert Syst
-00003dc0: 656d 7320 7769 7468 2041 7070 6c69 6361  ems with Applica
-00003dd0: 7469 6f6e 737d 2c0d 0a09 7061 6765 7320  tions},...pages 
-00003de0: 3d20 097b 3132 3331 3534 7d2c 0d0a 0979  = .{123154},...y
-00003df0: 6561 7220 3d20 0909 7b32 3032 347d 2c0d  ear = ..{2024},.
-00003e00: 0a09 6973 736e 203d 2009 097b 3039 3537  ..issn = ..{0957
-00003e10: 2d34 3137 347d 2c0d 0a09 646f 6920 3d20  -4174},...doi = 
-00003e20: 0909 7b68 7474 7073 3a2f 2f64 6f69 2e6f  ..{https://doi.o
-00003e30: 7267 2f31 302e 3130 3136 2f6a 2e65 7377  rg/10.1016/j.esw
-00003e40: 612e 3230 3234 2e31 3233 3135 347d 2c0d  a.2024.123154},.
-00003e50: 0a09 7572 6c20 3d20 0909 7b68 7474 7073  ..url = ..{https
-00003e60: 3a2f 2f77 7777 2e73 6369 656e 6365 6469  ://www.sciencedi
-00003e70: 7265 6374 2e63 6f6d 2f73 6369 656e 6365  rect.com/science
-00003e80: 2f61 7274 6963 6c65 2f70 6969 2f53 3039  /article/pii/S09
-00003e90: 3537 3431 3734 3234 3030 3031 3938 7d2c  57417424000198},
-00003ea0: 0d0a 0961 7574 686f 7220 3d20 097b 4865  ...author = .{He
-00003eb0: 6c65 6e61 204c c3b6 6673 7472 c3b6 6d20  lena L..fstr..m 
-00003ec0: 616e 6420 5475 7765 204c c3b6 6673 7472  and Tuwe L..fstr
-00003ed0: c3b6 6d20 616e 6420 556c 6620 4a6f 6861  ..m and Ulf Joha
-00003ee0: 6e73 736f 6e20 616e 6420 4365 6369 6c69  nsson and Cecili
-00003ef0: 6120 53c3 b66e 7374 72c3 b664 7d2c 0d0a  a S..nstr..d},..
-00003f00: 096b 6579 776f 7264 7320 3d20 097b 4578  .keywords = .{Ex
-00003f10: 706c 6169 6e61 626c 6520 4149 2c20 4665  plainable AI, Fe
-00003f20: 6174 7572 6520 696d 706f 7274 616e 6365  ature importance
-00003f30: 2c20 4361 6c69 6272 6174 6564 2065 7870  , Calibrated exp
-00003f40: 6c61 6e61 7469 6f6e 732c 2056 656e 6e2d  lanations, Venn-
-00003f50: 4162 6572 732c 2055 6e63 6572 7461 696e  Abers, Uncertain
-00003f60: 7479 2071 7561 6e74 6966 6963 6174 696f  ty quantificatio
-00003f70: 6e2c 2043 6f75 6e74 6572 6661 6374 7561  n, Counterfactua
-00003f80: 6c20 6578 706c 616e 6174 696f 6e73 7d2c  l explanations},
-00003f90: 0d0a 0961 6273 7472 6163 7420 3d20 097b  ...abstract = .{
-00003fa0: 5768 696c 6520 6c6f 6361 6c20 6578 706c  While local expl
-00003fb0: 616e 6174 696f 6e73 2066 6f72 2041 4920  anations for AI 
-00003fc0: 6d6f 6465 6c73 2063 616e 206f 6666 6572  models can offer
-00003fd0: 2069 6e73 6967 6874 7320 696e 746f 2069   insights into i
-00003fe0: 6e64 6976 6964 7561 6c20 7072 6564 6963  ndividual predic
-00003ff0: 7469 6f6e 732c 2073 7563 6820 6173 2066  tions, such as f
-00004000: 6561 7475 7265 2069 6d70 6f72 7461 6e63  eature importanc
-00004010: 652c 2074 6865 7920 6172 6520 706c 6167  e, they are plag
-00004020: 7565 6420 6279 2069 7373 7565 7320 6c69  ued by issues li
-00004030: 6b65 2069 6e73 7461 6269 6c69 7479 2e20  ke instability. 
-00004040: 5468 6520 756e 7265 6c69 6162 696c 6974  The unreliabilit
-00004050: 7920 6f66 2066 6561 7475 7265 2077 6569  y of feature wei
-00004060: 6768 7473 2c20 6f66 7465 6e20 736b 6577  ghts, often skew
-00004070: 6564 2064 7565 2074 6f20 706f 6f72 6c79  ed due to poorly
-00004080: 2063 616c 6962 7261 7465 6420 4d4c 206d   calibrated ML m
-00004090: 6f64 656c 732c 2064 6565 7065 6e73 2074  odels, deepens t
-000040a0: 6865 7365 2063 6861 6c6c 656e 6765 732e  hese challenges.
-000040b0: 204d 6f72 656f 7665 722c 2074 6865 2063   Moreover, the c
-000040c0: 7269 7469 6361 6c20 6173 7065 6374 206f  ritical aspect o
-000040d0: 6620 6665 6174 7572 6520 696d 706f 7274  f feature import
-000040e0: 616e 6365 2075 6e63 6572 7461 696e 7479  ance uncertainty
-000040f0: 2072 656d 6169 6e73 206d 6f73 746c 7920   remains mostly 
-00004100: 756e 6164 6472 6573 7365 6420 696e 2045  unaddressed in E
-00004110: 7870 6c61 696e 6162 6c65 2041 4920 2858  xplainable AI (X
-00004120: 4149 292e 2054 6865 206e 6f76 656c 2066  AI). The novel f
-00004130: 6561 7475 7265 2069 6d70 6f72 7461 6e63  eature importanc
-00004140: 6520 6578 706c 616e 6174 696f 6e20 6d65  e explanation me
-00004150: 7468 6f64 2070 7265 7365 6e74 6564 2069  thod presented i
-00004160: 6e20 7468 6973 2070 6170 6572 2c20 6361  n this paper, ca
-00004170: 6c6c 6564 2043 616c 6962 7261 7465 6420  lled Calibrated 
-00004180: 4578 706c 616e 6174 696f 6e73 2028 4345  Explanations (CE
-00004190: 292c 2069 7320 6465 7369 676e 6564 2074  ), is designed t
-000041a0: 6f20 7461 636b 6c65 2074 6865 7365 2069  o tackle these i
-000041b0: 7373 7565 7320 6865 6164 2d6f 6e2e 2042  ssues head-on. B
-000041c0: 7569 6c74 206f 6e20 7468 6520 666f 756e  uilt on the foun
-000041d0: 6461 7469 6f6e 206f 6620 5665 6e6e 2d41  dation of Venn-A
-000041e0: 6265 7273 2c20 4345 206e 6f74 206f 6e6c  bers, CE not onl
-000041f0: 7920 6361 6c69 6272 6174 6573 2074 6865  y calibrates the
-00004200: 2075 6e64 6572 6c79 696e 6720 6d6f 6465   underlying mode
-00004210: 6c20 6275 7420 616c 736f 2064 656c 6976  l but also deliv
-00004220: 6572 7320 7265 6c69 6162 6c65 2066 6561  ers reliable fea
-00004230: 7475 7265 2069 6d70 6f72 7461 6e63 6520  ture importance 
-00004240: 6578 706c 616e 6174 696f 6e73 2077 6974  explanations wit
-00004250: 6820 616e 2065 7861 6374 2064 6566 696e  h an exact defin
-00004260: 6974 696f 6e20 6f66 2074 6865 2066 6561  ition of the fea
-00004270: 7475 7265 2077 6569 6768 7473 2e20 4345  ture weights. CE
-00004280: 2067 6f65 7320 6265 796f 6e64 2063 6f6e   goes beyond con
-00004290: 7665 6e74 696f 6e61 6c20 736f 6c75 7469  ventional soluti
-000042a0: 6f6e 7320 6279 2061 6464 7265 7373 696e  ons by addressin
-000042b0: 6720 6f75 7470 7574 2075 6e63 6572 7461  g output uncerta
-000042c0: 696e 7479 2e20 4974 2061 6363 6f6d 706c  inty. It accompl
-000042d0: 6973 6865 7320 7468 6973 2062 7920 7072  ishes this by pr
-000042e0: 6f76 6964 696e 6720 756e 6365 7274 6169  oviding uncertai
-000042f0: 6e74 7920 7175 616e 7469 6669 6361 7469  nty quantificati
-00004300: 6f6e 2066 6f72 2062 6f74 6820 6665 6174  on for both feat
-00004310: 7572 6520 7765 6967 6874 7320 616e 6420  ure weights and 
-00004320: 7468 6520 6d6f 6465 6ce2 8099 7320 7072  the model...s pr
-00004330: 6f62 6162 696c 6974 7920 6573 7469 6d61  obability estima
-00004340: 7465 732e 2041 6464 6974 696f 6e61 6c6c  tes. Additionall
-00004350: 792c 2043 4520 6973 206d 6f64 656c 2d61  y, CE is model-a
-00004360: 676e 6f73 7469 632c 2066 6561 7475 7269  gnostic, featuri
-00004370: 6e67 2065 6173 696c 7920 636f 6d70 7265  ng easily compre
-00004380: 6865 6e73 6962 6c65 2063 6f6e 6469 7469  hensible conditi
-00004390: 6f6e 616c 2072 756c 6573 2061 6e64 2074  onal rules and t
-000043a0: 6865 2061 6269 6c69 7479 2074 6f20 6765  he ability to ge
-000043b0: 6e65 7261 7465 2063 6f75 6e74 6572 6661  nerate counterfa
-000043c0: 6374 7561 6c20 6578 706c 616e 6174 696f  ctual explanatio
-000043d0: 6e73 2077 6974 6820 656d 6265 6464 6564  ns with embedded
-000043e0: 2075 6e63 6572 7461 696e 7479 2071 7561   uncertainty qua
-000043f0: 6e74 6966 6963 6174 696f 6e2e 2052 6573  ntification. Res
-00004400: 756c 7473 2066 726f 6d20 616e 2065 7661  ults from an eva
-00004410: 6c75 6174 696f 6e20 7769 7468 2032 3520  luation with 25 
-00004420: 6265 6e63 686d 6172 6b20 6461 7461 7365  benchmark datase
-00004430: 7473 2075 6e64 6572 7363 6f72 6520 7468  ts underscore th
-00004440: 6520 6566 6669 6361 6379 206f 6620 4345  e efficacy of CE
-00004450: 2c20 6d61 6b69 6e67 2069 7420 7374 616e  , making it stan
-00004460: 6420 6173 2061 2066 6173 742c 2072 656c  d as a fast, rel
-00004470: 6961 626c 652c 2073 7461 626c 652c 2061  iable, stable, a
-00004480: 6e64 2072 6f62 7573 7420 736f 6c75 7469  nd robust soluti
-00004490: 6f6e 2e7d 0d0a 7d0d 0a60 6060 0d0a 4269  on.}..}..```..Bi
-000044a0: 6274 6578 2065 6e74 7279 2066 6f72 2074  btex entry for t
-000044b0: 6865 2072 6567 7265 7373 696f 6e20 7061  he regression pa
-000044c0: 7065 723a 0d0a 0d0a 6060 6062 6962 7465  per:....```bibte
-000044d0: 780d 0a40 6d69 7363 7b63 616c 2d65 7870  x..@misc{cal-exp
-000044e0: 6c2d 7265 6772 6573 7369 6f6e 2c0d 0a20  l-regression,.. 
-000044f0: 2020 2020 2074 6974 6c65 203d 2009 2020       title = .  
-00004500: 2020 2020 097b 4361 6c69 6272 6174 6564      .{Calibrated
-00004510: 2045 7870 6c61 6e61 7469 6f6e 7320 666f   Explanations fo
-00004520: 7220 5265 6772 6573 7369 6f6e 7d2c 0d0a  r Regression},..
-00004530: 2020 2020 2020 6175 7468 6f72 203d 2020        author =  
-00004540: 2020 2020 2020 2020 7b4c 5c22 6f66 7374          {L\"ofst
-00004550: 725c 226f 6d2c 2054 7577 6520 616e 6420  r\"om, Tuwe and 
-00004560: 4c5c 226f 6673 7472 5c22 6f6d 2c20 4865  L\"ofstr\"om, He
-00004570: 6c65 6e61 2061 6e64 204a 6f68 616e 7373  lena and Johanss
-00004580: 6f6e 2c20 556c 6620 616e 6420 535c 226f  on, Ulf and S\"o
-00004590: 6e73 7472 5c22 6f64 2c20 4365 6369 6c69  nstr\"od, Cecili
-000045a0: 6120 616e 6420 4d61 7465 6c61 2c20 5275  a and Matela, Ru
-000045b0: 6479 7d2c 0d0a 2020 2020 2020 7965 6172  dy},..      year
-000045c0: 203d 2020 2020 2020 2020 2020 2020 7b32   =            {2
-000045d0: 3032 337d 2c0d 0a20 2020 2020 2065 7072  023},..      epr
-000045e0: 696e 7420 3d20 2020 2020 2020 2020 207b  int =          {
-000045f0: 3233 3038 2e31 3632 3435 7d2c 0d0a 2020  2308.16245},..  
-00004600: 2020 2020 6172 6368 6976 6550 7265 6669      archivePrefi
-00004610: 7820 3d20 2020 7b61 7258 6976 7d2c 0d0a  x =   {arXiv},..
-00004620: 2020 2020 2020 7072 696d 6172 7943 6c61        primaryCla
-00004630: 7373 203d 2020 2020 7b63 732e 4c47 7d0d  ss =    {cs.LG}.
-00004640: 0a7d 0d0a 6060 600d 0a0d 0a54 6f20 6369  .}..```....To ci
-00004650: 7465 2074 6869 7320 736f 6674 7761 7265  te this software
-00004660: 2c20 7573 6520 7468 6520 666f 6c6c 6f77  , use the follow
-00004670: 696e 6720 6269 6274 6578 2065 6e74 7279  ing bibtex entry
-00004680: 3a0d 0a0d 0a60 6060 6269 6274 6578 0d0a  :....```bibtex..
-00004690: 4073 6f66 7477 6172 657b 4c6f 6673 7472  @software{Lofstr
-000046a0: 6f6d 5f43 616c 6962 7261 7465 645f 4578  om_Calibrated_Ex
-000046b0: 706c 616e 6174 696f 6e73 5f32 3032 342c  planations_2024,
-000046c0: 0d0a 0961 7574 686f 7220 3d20 097b 4cc3  ...author = .{L.
-000046d0: b666 7374 72c3 b66d 2c20 4865 6c65 6e61  .fstr..m, Helena
-000046e0: 2061 6e64 204c c3b6 6673 7472 c3b6 6d2c   and L..fstr..m,
-000046f0: 2054 7577 6520 616e 6420 4a6f 6861 6e73   Tuwe and Johans
-00004700: 736f 6e2c 2055 6c66 2061 6e64 2053 c3b6  son, Ulf and S..
-00004710: 6e73 7472 c3b6 642c 2043 6563 696c 6961  nstr..d, Cecilia
-00004720: 2061 6e64 204d 6174 656c 612c 2052 7564   and Matela, Rud
-00004730: 797d 2c0d 0a09 6c69 6365 6e73 6520 3d20  y},...license = 
-00004740: 097b 4253 442d 332d 436c 6175 7365 7d2c  .{BSD-3-Clause},
-00004750: 0d0a 0974 6974 6c65 203d 2009 7b43 616c  ...title = .{Cal
-00004760: 6962 7261 7465 6420 4578 706c 616e 6174  ibrated Explanat
-00004770: 696f 6e73 7d2c 0d0a 0975 726c 203d 2009  ions},...url = .
-00004780: 097b 6874 7470 733a 2f2f 6769 7468 7562  .{https://github
-00004790: 2e63 6f6d 2f4d 6f66 6672 616e 2f63 616c  .com/Moffran/cal
-000047a0: 6962 7261 7465 645f 6578 706c 616e 6174  ibrated_explanat
-000047b0: 696f 6e73 7d2c 0d0a 0976 6572 7369 6f6e  ions},...version
-000047c0: 203d 2009 7b76 302e 332e 327d 2c0d 0a09   = .{v0.3.2},...
-000047d0: 6d6f 6e74 6820 3d20 0946 6562 2c0d 0a09  month = .Feb,...
-000047e0: 7965 6172 203d 2009 097b 3230 3234 7d0d  year = ..{2024}.
-000047f0: 0a7d 0d0a 6060 600d 0a20 200d 0a5b 546f  .}..```..  ..[To
-00004800: 705d 2823 6361 6c69 6272 6174 6564 2d65  p](#calibrated-e
-00004810: 7870 6c61 6e61 7469 6f6e 732d 646f 6375  xplanations-docu
-00004820: 6d65 6e74 6174 696f 6e29 0d0a 0d0a 4163  mentation)....Ac
-00004830: 6b6e 6f77 6c65 6467 656d 656e 7473 0d0a  knowledgements..
-00004840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004850: 0d0a 5468 6973 2072 6573 6561 7263 6820  ..This research 
-00004860: 6973 2066 756e 6465 6420 6279 2074 6865  is funded by the
-00004870: 2053 7765 6469 7368 204b 6e6f 776c 6564   Swedish Knowled
-00004880: 6765 2046 6f75 6e64 6174 696f 6e20 746f  ge Foundation to
-00004890: 6765 7468 6572 2077 6974 6820 696e 6475  gether with indu
-000048a0: 7374 7269 616c 2070 6172 746e 6572 7320  strial partners 
-000048b0: 7375 7070 6f72 7469 6e67 2074 6865 2072  supporting the r
-000048c0: 6573 6561 7263 6820 616e 6420 6564 7563  esearch and educ
-000048d0: 6174 696f 6e20 656e 7669 726f 6e6d 656e  ation environmen
-000048e0: 7420 6f6e 204b 6e6f 776c 6564 6765 2049  t on Knowledge I
-000048f0: 6e74 656e 7369 7665 2050 726f 6475 6374  ntensive Product
-00004900: 2052 6561 6c69 7a61 7469 6f6e 2053 5041   Realization SPA
-00004910: 524b 2061 7420 4ac3 b66e 6bc3 b670 696e  RK at J..nk..pin
-00004920: 6720 556e 6976 6572 7369 7479 2c20 5377  g University, Sw
-00004930: 6564 656e 2c20 7468 726f 7567 6820 7072  eden, through pr
-00004940: 6f6a 6563 7473 3a20 4146 4149 5220 6772  ojects: AFAIR gr
-00004950: 616e 7420 6e6f 2e20 3230 3230 3032 3233  ant no. 20200223
-00004960: 2061 6e64 2050 5245 4d41 434f 5020 6772   and PREMACOP gr
-00004970: 616e 7420 6e6f 2e20 3230 3232 3031 3837  ant no. 20220187
-00004980: 2e20 4865 6c65 6e61 204c c3b6 6673 7472  . Helena L..fstr
-00004990: c3b6 6d20 7761 7320 6120 5068 4420 7374  ..m was a PhD st
-000049a0: 7564 656e 7420 696e 2074 6865 2049 6e64  udent in the Ind
-000049b0: 7573 7472 6961 6c20 4772 6164 7561 7465  ustrial Graduate
-000049c0: 2053 6368 6f6f 6c20 696e 2044 6967 6974   School in Digit
-000049d0: 616c 2052 6574 6169 6c69 6e67 2028 494e  al Retailing (IN
-000049e0: 5369 4452 2920 6174 2074 6865 2055 6e69  SiDR) at the Uni
-000049f0: 7665 7273 6974 7920 6f66 2042 6f72 c3a5  versity of Bor..
-00004a00: 732c 2066 756e 6465 6420 6279 2074 6865  s, funded by the
-00004a10: 2053 7765 6469 7368 204b 6e6f 776c 6564   Swedish Knowled
-00004a20: 6765 2046 6f75 6e64 6174 696f 6e2c 2067  ge Foundation, g
-00004a30: 7261 6e74 206e 6f2e 2032 3031 3630 3033  rant no. 2016003
-00004a40: 352e 200d 0a0d 0a5b 5275 6479 204d 6174  5. ....[Rudy Mat
-00004a50: 656c 615d 2868 7474 7073 3a2f 2f67 6974  ela](https://git
-00004a60: 6875 622e 636f 6d2f 7275 6479 6d61 7465  hub.com/rudymate
-00004a70: 6c61 2920 6861 7320 6265 656e 206f 7572  la) has been our
-00004a80: 2067 6974 2067 7572 7520 616e 6420 6861   git guru and ha
-00004a90: 7320 6865 6c70 6564 2075 7320 7769 7468  s helped us with
-00004aa0: 2074 6865 2072 656c 6561 7365 2070 726f   the release pro
-00004ab0: 6365 7373 2e0d 0a0d 0a57 6520 6861 7665  cess.....We have
-00004ac0: 2075 7365 6420 626f 7468 2074 6865 2060   used both the `
-00004ad0: 436f 6e66 6f72 6d61 6c50 7265 6469 6374  ConformalPredict
-00004ae0: 6976 6553 7973 7465 6d60 2061 6e64 2060  iveSystem` and `
-00004af0: 4469 6666 6963 756c 7479 4573 7469 6d61  DifficultyEstima
-00004b00: 746f 7260 2063 6c61 7373 6573 2066 726f  tor` classes fro
-00004b10: 6d20 5b48 656e 7269 6b20 426f 7374 72c3  m [Henrik Bostr.
-00004b20: b66d 5d28 6874 7470 733a 2f2f 6769 7468  .m](https://gith
-00004b30: 7562 2e63 6f6d 2f68 656e 7269 6b62 6f73  ub.com/henrikbos
-00004b40: 7472 6f6d 2973 205b 6372 6570 6573 5d28  trom)s [crepes](
-00004b50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004b60: 6f6d 2f68 656e 7269 6b62 6f73 7472 6f6d  om/henrikbostrom
-00004b70: 2f63 7265 7065 7329 2070 6163 6b61 6765  /crepes) package
-00004b80: 2074 6f20 7072 6f76 6964 6520 7375 7070   to provide supp
-00004b90: 6f72 7420 666f 7220 7265 6772 6573 7369  ort for regressi
-00004ba0: 6f6e 2e0d 0a0d 0a57 6520 6861 7665 2075  on.....We have u
-00004bb0: 7365 6420 7468 6520 6056 656e 6e41 6265  sed the `VennAbe
-00004bc0: 7273 6020 636c 6173 7320 6672 6f6d 205b  rs` class from [
-00004bd0: 4976 616e 2050 6574 656a 5d28 6874 7470  Ivan Petej](http
-00004be0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00004bf0: 7032 3030 2973 205b 7665 6e6e 2d61 6265  p200)s [venn-abe
-00004c00: 7273 5d28 6874 7470 733a 2f2f 6769 7468  rs](https://gith
-00004c10: 7562 2e63 6f6d 2f69 7032 3030 2f76 656e  ub.com/ip200/ven
-00004c20: 6e2d 6162 6572 7329 2070 6163 6b61 6765  n-abers) package
-00004c30: 2074 6f20 7072 6f76 6964 6520 7375 7070   to provide supp
-00004c40: 6f72 7420 666f 7220 7072 6f62 6162 696c  ort for probabil
-00004c50: 6973 7469 6320 6578 706c 616e 6174 696f  istic explanatio
-00004c60: 6e73 2028 626f 7468 2063 6c61 7373 6966  ns (both classif
-00004c70: 6963 6174 696f 6e20 616e 6420 7072 6f62  ication and prob
-00004c80: 6162 696c 6973 7469 6320 7265 6772 6573  abilistic regres
-00004c90: 7369 6f6e 292e 200d 0a0d 0a57 6520 6861  sion). ....We ha
-00004ca0: 7665 2075 7365 6420 636f 6465 2066 726f  ve used code fro
-00004cb0: 6d20 5b4d 6172 636f 2054 756c 696f 2043  m [Marco Tulio C
-00004cc0: 6f72 7265 6961 2052 6962 6569 726f 5d28  orreia Ribeiro](
-00004cd0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00004ce0: 6f6d 2f6d 6172 636f 7463 7229 7320 5b6c  om/marcotcr)s [l
-00004cf0: 696d 655d 2868 7474 7073 3a2f 2f67 6974  ime](https://git
-00004d00: 6875 622e 636f 6d2f 6d61 7263 6f74 6372  hub.com/marcotcr
-00004d10: 2f6c 696d 6529 2070 6163 6b61 6765 2066  /lime) package f
-00004d20: 6f72 2074 6865 2060 4469 7363 7265 7469  or the `Discreti
-00004d30: 7a65 7260 2063 6c61 7373 2e0d 0a0d 0a54  zer` class.....T
-00004d40: 6865 2060 6368 6563 6b5f 6973 5f66 6974  he `check_is_fit
-00004d50: 7465 6460 2061 6e64 2060 7361 6665 5f69  ted` and `safe_i
-00004d60: 6e73 7461 6e63 6560 2066 756e 6374 696f  nstance` functio
-00004d70: 6e73 2069 6e20 6063 616c 6962 7261 7465  ns in `calibrate
-00004d80: 645f 6578 706c 616e 6174 696f 6e73 2e75  d_explanations.u
-00004d90: 7469 6c73 6020 6172 6520 636f 7069 6564  tils` are copied
-00004da0: 2066 726f 6d20 6073 6b6c 6561 726e 6020   from `sklearn` 
-00004db0: 616e 6420 6073 6861 7060 2e20 200d 0a20  and `shap`.  .. 
-00004dc0: 200d 0a5b 546f 705d 2823 6361 6c69 6272   ..[Top](#calibr
-00004dd0: 6174 6564 2d65 7870 6c61 6e61 7469 6f6e  ated-explanation
-00004de0: 732d 646f 6375 6d65 6e74 6174 696f 6e29  s-documentation)
-00004df0: 0d0a 0d0a 5b62 7569 6c64 2d6c 6f67 5d3a  ....[build-log]:
-00004e00: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
-00004e10: 7562 2e63 6f6d 2f4d 6f66 6672 616e 2f63  ub.com/Moffran/c
-00004e20: 616c 6962 7261 7465 645f 6578 706c 616e  alibrated_explan
-00004e30: 6174 696f 6e73 2f61 6374 696f 6e73 2f77  ations/actions/w
-00004e40: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
-00004e50: 6c0d 0a5b 6275 696c 642d 7374 6174 7573  l..[build-status
-00004e60: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-00004e70: 622e 636f 6d2f 4d6f 6666 7261 6e2f 6361  b.com/Moffran/ca
-00004e80: 6c69 6272 6174 6564 5f65 7870 6c61 6e61  librated_explana
-00004e90: 7469 6f6e 732f 6163 7469 6f6e 732f 776f  tions/actions/wo
-00004ea0: 726b 666c 6f77 732f 7465 7374 2e79 6d6c  rkflows/test.yml
-00004eb0: 2f62 6164 6765 2e73 7667 0d0a 5b6c 696e  /badge.svg..[lin
-00004ec0: 742d 6c6f 675d 3a20 2020 2068 7474 7073  t-log]:    https
-00004ed0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
-00004ee0: 6666 7261 6e2f 6361 6c69 6272 6174 6564  ffran/calibrated
-00004ef0: 5f65 7870 6c61 6e61 7469 6f6e 732f 6163  _explanations/ac
-00004f00: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00004f10: 7079 6c69 6e74 2e79 6d6c 0d0a 5b6c 696e  pylint.yml..[lin
-00004f20: 742d 7374 6174 7573 5d3a 2068 7474 7073  t-status]: https
-00004f30: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
-00004f40: 6666 7261 6e2f 6361 6c69 6272 6174 6564  ffran/calibrated
-00004f50: 5f65 7870 6c61 6e61 7469 6f6e 732f 6163  _explanations/ac
-00004f60: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00004f70: 7079 6c69 6e74 2e79 6d6c 2f62 6164 6765  pylint.yml/badge
-00004f80: 2e73 7667 0d0a 5b70 7970 692d 7665 7273  .svg..[pypi-vers
-00004f90: 696f 6e5d 3a20 6874 7470 733a 2f2f 696d  ion]: https://im
-00004fa0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00004fb0: 692f 762f 6361 6c69 6272 6174 6564 2d65  i/v/calibrated-e
-00004fc0: 7870 6c61 6e61 7469 6f6e 730d 0a5b 6361  xplanations..[ca
-00004fd0: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
-00004fe0: 7469 6f6e 732d 6f6e 2d70 7970 695d 3a20  tions-on-pypi]: 
-00004ff0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00005000: 2f70 726f 6a65 6374 2f63 616c 6962 7261  /project/calibra
-00005010: 7465 642d 6578 706c 616e 6174 696f 6e73  ted-explanations
-00005020: 0d0a                                     ..
+00000000: 4361 6c69 6272 6174 6564 2045 7870 6c61  Calibrated Expla
+00000010: 6e61 7469 6f6e 7320 285b 446f 6375 6d65  nations ([Docume
+00000020: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00000030: 2f63 616c 6962 7261 7465 642d 6578 706c  /calibrated-expl
+00000040: 616e 6174 696f 6e73 2e72 6561 6474 6865  anations.readthe
+00000050: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000060: 742f 3f62 6164 6765 3d6c 6174 6573 7429  t/?badge=latest)
+00000070: 290d 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  )..=============
+00000080: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 5b21  ==========....[!
+00000090: 5b43 616c 6962 7261 7465 6420 4578 706c  [Calibrated Expl
+000000a0: 616e 6174 696f 6e73 2050 7950 4920 7665  anations PyPI ve
+000000b0: 7273 696f 6e5d 5b70 7970 692d 7665 7273  rsion][pypi-vers
+000000c0: 696f 6e5d 5d5b 6361 6c69 6272 6174 6564  ion]][calibrated
+000000d0: 2d65 7870 6c61 6e61 7469 6f6e 732d 6f6e  -explanations-on
+000000e0: 2d70 7970 695d 0d0a 5b21 5b43 6f6e 6461  -pypi]..[![Conda
+000000f0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000100: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000110: 2f63 6f6e 6461 2f76 6e2f 636f 6e64 612d  /conda/vn/conda-
+00000120: 666f 7267 652f 6361 6c69 6272 6174 6564  forge/calibrated
+00000130: 2d65 7870 6c61 6e61 7469 6f6e 732e 7376  -explanations.sv
+00000140: 6729 5d28 6874 7470 733a 2f2f 616e 6163  g)](https://anac
+00000150: 6f6e 6461 2e6f 7267 2f63 6f6e 6461 2d66  onda.org/conda-f
+00000160: 6f72 6765 2f63 616c 6962 7261 7465 642d  orge/calibrated-
+00000170: 6578 706c 616e 6174 696f 6e73 290d 0a5b  explanations)..[
+00000180: 215b 4769 7448 7562 2028 5072 652d 2952  ![GitHub (Pre-)R
+00000190: 656c 6561 7365 2044 6174 655d 2868 7474  elease Date](htt
+000001a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000001b0: 2e69 6f2f 6769 7468 7562 2f72 656c 6561  .io/github/relea
+000001c0: 7365 2d64 6174 652d 7072 652f 4d6f 6666  se-date-pre/Moff
+000001d0: 7261 6e2f 6361 6c69 6272 6174 6564 5f65  ran/calibrated_e
+000001e0: 7870 6c61 6e61 7469 6f6e 7329 5d28 6874  xplanations)](ht
+000001f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000200: 2f4d 6f66 6672 616e 2f63 616c 6962 7261  /Moffran/calibra
+00000210: 7465 645f 6578 706c 616e 6174 696f 6e73  ted_explanations
+00000220: 2f62 6c6f 622f 6d61 696e 2f43 4841 4e47  /blob/main/CHANG
+00000230: 454c 4f47 2e6d 6429 0d0a 5b21 5b44 6f63  ELOG.md)..[![Doc
+00000240: 756d 656e 7461 7469 6f6e 2053 7461 7475  umentation Statu
+00000250: 735d 2868 7474 7073 3a2f 2f72 6561 6474  s](https://readt
+00000260: 6865 646f 6373 2e6f 7267 2f70 726f 6a65  hedocs.org/proje
+00000270: 6374 732f 6361 6c69 6272 6174 6564 2d65  cts/calibrated-e
+00000280: 7870 6c61 6e61 7469 6f6e 732f 6261 6467  xplanations/badg
+00000290: 652f 3f76 6572 7369 6f6e 3d6c 6174 6573  e/?version=lates
+000002a0: 7429 5d28 6874 7470 733a 2f2f 6361 6c69  t)](https://cali
+000002b0: 6272 6174 6564 2d65 7870 6c61 6e61 7469  brated-explanati
+000002c0: 6f6e 732e 7265 6164 7468 6564 6f63 732e  ons.readthedocs.
+000002d0: 696f 2f65 6e2f 6c61 7465 7374 2f3f 6261  io/en/latest/?ba
+000002e0: 6467 653d 6c61 7465 7374 290d 0a5b 215b  dge=latest)..[![
+000002f0: 4275 696c 6420 5374 6174 7573 2066 6f72  Build Status for
+00000300: 2043 616c 6962 7261 7465 6420 4578 706c   Calibrated Expl
+00000310: 616e 6174 696f 6e73 5d5b 6275 696c 642d  anations][build-
+00000320: 7374 6174 7573 5d5d 5b62 7569 6c64 2d6c  status]][build-l
+00000330: 6f67 5d0d 0a5b 215b 4c69 6e74 2053 7461  og]..[![Lint Sta
+00000340: 7475 7320 666f 7220 4361 6c69 6272 6174  tus for Calibrat
+00000350: 6564 2045 7870 6c61 6e61 7469 6f6e 735d  ed Explanations]
+00000360: 5b6c 696e 742d 7374 6174 7573 5d5d 5b6c  [lint-status]][l
+00000370: 696e 742d 6c6f 675d 0d0a 5b21 5b4c 6963  int-log]..[![Lic
+00000380: 656e 7365 5d28 6874 7470 733a 2f2f 6261  ense](https://ba
+00000390: 6467 656e 2e6e 6574 2f67 6974 6875 622f  dgen.net/github/
+000003a0: 6c69 6365 6e73 652f 6d6f 6666 7261 6e2f  license/moffran/
+000003b0: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
+000003c0: 6e61 7469 6f6e 7329 5d28 6874 7470 733a  nations)](https:
+000003d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6f66  //github.com/mof
+000003e0: 6672 616e 2f63 616c 6962 7261 7465 645f  fran/calibrated_
+000003f0: 6578 706c 616e 6174 696f 6e73 2f62 6c6f  explanations/blo
+00000400: 622f 6d61 696e 2f4c 4943 454e 5345 290d  b/main/LICENSE).
+00000410: 0a5b 215b 446f 776e 6c6f 6164 735d 2868  .[![Downloads](h
+00000420: 7474 7073 3a2f 2f73 7461 7469 632e 7065  ttps://static.pe
+00000430: 7079 2e74 6563 682f 6261 6467 652f 6361  py.tech/badge/ca
+00000440: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
+00000450: 7469 6f6e 7329 5d28 6874 7470 733a 2f2f  tions)](https://
+00000460: 7065 7079 2e74 6563 682f 7072 6f6a 6563  pepy.tech/projec
+00000470: 742f 6361 6c69 6272 6174 6564 2d65 7870  t/calibrated-exp
+00000480: 6c61 6e61 7469 6f6e 7329 0d0a 5b21 5b42  lanations)..[![B
+00000490: 696e 6465 725d 2868 7474 7073 3a2f 2f6d  inder](https://m
+000004a0: 7962 696e 6465 722e 6f72 672f 6261 6467  ybinder.org/badg
+000004b0: 655f 6c6f 676f 2e73 7667 295d 2868 7474  e_logo.svg)](htt
+000004c0: 7073 3a2f 2f6d 7962 696e 6465 722e 6f72  ps://mybinder.or
+000004d0: 672f 7632 2f67 682f 4d6f 6666 7261 6e2f  g/v2/gh/Moffran/
+000004e0: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
+000004f0: 6e61 7469 6f6e 732f 7630 2e33 2e33 290d  nations/v0.3.3).
+00000500: 0a0d 0a60 6361 6c69 6272 6174 6564 2d65  ...`calibrated-e
+00000510: 7870 6c61 6e61 7469 6f6e 7360 2069 7320  xplanations` is 
+00000520: 6120 5079 7468 6f6e 2070 6163 6b61 6765  a Python package
+00000530: 2066 6f72 2074 6865 206c 6f63 616c 2066   for the local f
+00000540: 6561 7475 7265 2069 6d70 6f72 7461 6e63  eature importanc
+00000550: 6520 6578 706c 616e 6174 696f 6e20 6d65  e explanation me
+00000560: 7468 6f64 2063 616c 6c65 6420 4361 6c69  thod called Cali
+00000570: 6272 6174 6564 2045 7870 6c61 6e61 7469  brated Explanati
+00000580: 6f6e 732c 2073 7570 706f 7274 696e 6720  ons, supporting 
+00000590: 626f 7468 205b 636c 6173 7369 6669 6361  both [classifica
+000005a0: 7469 6f6e 5d28 6874 7470 733a 2f2f 646f  tion](https://do
+000005b0: 692e 6f72 672f 3130 2e31 3031 362f 6a2e  i.org/10.1016/j.
+000005c0: 6573 7761 2e32 3032 342e 3132 3331 3534  eswa.2024.123154
+000005d0: 2920 616e 6420 5b72 6567 7265 7373 696f  ) and [regressio
+000005e0: 6e5d 2868 7474 7073 3a2f 2f61 7278 6976  n](https://arxiv
+000005f0: 2e6f 7267 2f61 6273 2f32 3330 382e 3136  .org/abs/2308.16
+00000600: 3234 3529 2e0d 0a54 6865 2070 726f 706f  245)...The propo
+00000610: 7365 6420 6d65 7468 6f64 2069 7320 6261  sed method is ba
+00000620: 7365 6420 6f6e 2056 656e 6e2d 4162 6572  sed on Venn-Aber
+00000630: 7320 2863 6c61 7373 6966 6963 6174 696f  s (classificatio
+00000640: 6e20 2620 7265 6772 6573 7369 6f6e 2920  n & regression) 
+00000650: 616e 6420 436f 6e66 6f72 6d61 6c20 5072  and Conformal Pr
+00000660: 6564 6963 7469 7665 2053 7973 7465 6d73  edictive Systems
+00000670: 2028 7265 6772 6573 7369 6f6e 2920 616e   (regression) an
+00000680: 6420 6861 7320 7468 6520 666f 6c6c 6f77  d has the follow
+00000690: 696e 6720 6368 6172 6163 7465 7269 7374  ing characterist
+000006a0: 6963 733a 0d0a 2a20 4661 7374 2c20 7265  ics:..* Fast, re
+000006b0: 6c69 6162 6c65 2c20 7374 6162 6c65 2061  liable, stable a
+000006c0: 6e64 2072 6f62 7573 7420 6665 6174 7572  nd robust featur
+000006d0: 6520 696d 706f 7274 616e 6365 2065 7870  e importance exp
+000006e0: 6c61 6e61 7469 6f6e 7320 666f 723a 0d0a  lanations for:..
+000006f0: 092d 2042 696e 6172 7920 636c 6173 7369  .- Binary classi
+00000700: 6669 6361 7469 6f6e 206d 6f64 656c 730d  fication models.
+00000710: 0a09 2d20 4d75 6c74 692d 636c 6173 7320  ..- Multi-class 
+00000720: 636c 6173 7369 6669 6361 7469 6f6e 206d  classification m
+00000730: 6f64 656c 730d 0a09 2d20 5265 6772 6573  odels...- Regres
+00000740: 7369 6f6e 206d 6f64 656c 730d 0a09 092a  sion models....*
+00000750: 2049 6e63 6c75 6469 6e67 2070 726f 6261   Including proba
+00000760: 6269 6c69 7374 6963 2065 7870 6c61 6e61  bilistic explana
+00000770: 7469 6f6e 7320 6f66 2074 6865 2070 726f  tions of the pro
+00000780: 6261 6269 6c69 7479 2074 6861 7420 7468  bability that th
+00000790: 6520 7461 7267 6574 2065 7863 6565 6473  e target exceeds
+000007a0: 2061 2075 7365 722d 6465 6669 6e65 6420   a user-defined 
+000007b0: 7468 7265 7368 6f6c 6420 0d0a 0909 2a20  threshold ....* 
+000007c0: 5769 7468 2064 6966 6669 6375 6c74 7920  With difficulty 
+000007d0: 6164 6170 7461 626c 6520 6578 706c 616e  adaptable explan
+000007e0: 6174 696f 6e73 2028 636f 6e66 6f72 6d61  ations (conforma
+000007f0: 6c20 6e6f 726d 616c 697a 6174 696f 6e29  l normalization)
+00000800: 200d 0a2a 2043 616c 6962 7261 7469 6f6e   ..* Calibration
+00000810: 206f 6620 7468 6520 756e 6465 726c 7969   of the underlyi
+00000820: 6e67 206d 6f64 656c 2074 6f20 656e 7375  ng model to ensu
+00000830: 7265 2074 6861 7420 7072 6564 6963 7469  re that predicti
+00000840: 6f6e 7320 7265 666c 6563 7420 7265 616c  ons reflect real
+00000850: 6974 792e 0d0a 2a20 556e 6365 7274 6169  ity...* Uncertai
+00000860: 6e74 7920 7175 616e 7469 6669 6361 7469  nty quantificati
+00000870: 6f6e 206f 6620 7468 6520 7072 6564 6963  on of the predic
+00000880: 7469 6f6e 2066 726f 6d20 7468 6520 756e  tion from the un
+00000890: 6465 726c 7969 6e67 206d 6f64 656c 2061  derlying model a
+000008a0: 6e64 2074 6865 2066 6561 7475 7265 2069  nd the feature i
+000008b0: 6d70 6f72 7461 6e63 6520 7765 6967 6874  mportance weight
+000008c0: 732e 200d 0a2a 2052 756c 6573 2077 6974  s. ..* Rules wit
+000008d0: 6820 7374 7261 6967 6874 666f 7277 6172  h straightforwar
+000008e0: 6420 696e 7465 7270 7265 7461 7469 6f6e  d interpretation
+000008f0: 2069 6e20 7265 6c61 7469 6f6e 2074 6f20   in relation to 
+00000900: 696e 7374 616e 6365 2076 616c 7565 7320  instance values 
+00000910: 616e 6420 6665 6174 7572 6520 7765 6967  and feature weig
+00000920: 6874 732e 0d0a 2a20 506f 7373 6962 696c  hts...* Possibil
+00000930: 6974 7920 746f 2067 656e 6572 6174 6520  ity to generate 
+00000940: 636f 756e 7465 7266 6163 7475 616c 2072  counterfactual r
+00000950: 756c 6573 2077 6974 6820 756e 6365 7274  ules with uncert
+00000960: 6169 6e74 7920 7175 616e 7469 6669 6361  ainty quantifica
+00000970: 7469 6f6e 206f 6620 7468 6520 6578 7065  tion of the expe
+00000980: 6374 6564 2070 7265 6469 6374 696f 6e73  cted predictions
+00000990: 2e0d 0a2a 2043 6f6e 6a75 6e63 7469 6f6e  ...* Conjunction
+000009a0: 616c 2072 756c 6573 2063 6f6e 7665 7969  al rules conveyi
+000009b0: 6e67 2066 6561 7475 7265 2069 6d70 6f72  ng feature impor
+000009c0: 7461 6e63 6520 666f 7220 7468 6520 696e  tance for the in
+000009d0: 7465 7261 6374 696f 6e20 6f66 2069 6e63  teraction of inc
+000009e0: 6c75 6465 6420 6665 6174 7572 6573 2e0d  luded features..
+000009f0: 0a2a 2043 6f6e 6469 7469 6f6e 616c 2072  .* Conditional r
+00000a00: 756c 6573 2c20 616c 6c6f 7769 6e67 2075  ules, allowing u
+00000a10: 7365 7273 2074 6865 2061 6269 6c69 7479  sers the ability
+00000a20: 2074 6f20 6372 6561 7465 2063 6f6e 7465   to create conte
+00000a30: 7874 7561 6c20 6578 706c 616e 6174 696f  xtual explanatio
+00000a40: 6e73 2074 6f20 6861 6e64 6c65 2065 2e67  ns to handle e.g
+00000a50: 2e20 6269 6173 2061 6e64 2066 6169 726e  . bias and fairn
+00000a60: 6573 7320 636f 6e73 7472 6169 6e74 732e  ess constraints.
+00000a70: 200d 0a0d 0a42 656c 6f77 2069 7320 616e   ....Below is an
+00000a80: 2065 7861 6d70 6c65 206f 6620 6120 7072   example of a pr
+00000a90: 6f62 6162 696c 6973 7469 6320 636f 756e  obabilistic coun
+00000aa0: 7465 7266 6163 7475 616c 2065 7870 6c61  terfactual expla
+00000ab0: 6e61 7469 6f6e 2066 6f72 2061 6e20 696e  nation for an in
+00000ac0: 7374 616e 6365 206f 6620 7468 6520 7265  stance of the re
+00000ad0: 6772 6573 7369 6f6e 2064 6174 6173 6574  gression dataset
+00000ae0: 2043 616c 6966 6f72 6e69 6120 486f 7573   California Hous
+00000af0: 696e 6720 2877 6974 6820 7468 6520 7468  ing (with the th
+00000b00: 7265 7368 6f6c 6420 3138 3020 3030 3029  reshold 180 000)
+00000b10: 2e20 5468 6520 6c69 6768 7420 7265 6420  . The light red 
+00000b20: 6172 6561 2069 6e20 7468 6520 6261 636b  area in the back
+00000b30: 6772 6f75 6e64 2069 7320 7265 7072 6573  ground is repres
+00000b40: 656e 7469 6e67 2074 6865 2063 616c 6962  enting the calib
+00000b50: 7261 7465 6420 7072 6f62 6162 696c 6974  rated probabilit
+00000b60: 7920 696e 7465 7276 616c 2028 666f 7220  y interval (for 
+00000b70: 7468 6520 7072 6564 6963 7469 6f6e 2062  the prediction b
+00000b80: 6569 6e67 2062 656c 6f77 2074 6865 2074  eing below the t
+00000b90: 6872 6573 686f 6c64 2920 6f66 2074 6865  hreshold) of the
+00000ba0: 2075 6e64 6572 6c79 696e 6720 6d6f 6465   underlying mode
+00000bb0: 6c2c 2061 7320 696e 6469 6361 7465 6420  l, as indicated 
+00000bc0: 6279 2061 2043 6f6e 666f 726d 616c 2050  by a Conformal P
+00000bd0: 7265 6469 6374 6976 6520 5379 7374 656d  redictive System
+00000be0: 2061 6e64 2063 616c 6962 7261 7465 6420   and calibrated 
+00000bf0: 7468 726f 7567 6820 5665 6e6e 2d41 6265  through Venn-Abe
+00000c00: 7273 2e20 5468 6520 6461 726b 6572 2072  rs. The darker r
+00000c10: 6564 2062 6172 7320 666f 7220 6561 6368  ed bars for each
+00000c20: 2072 756c 6520 7368 6f77 2074 6865 2070   rule show the p
+00000c30: 726f 6261 6269 6c69 7479 2069 6e74 6572  robability inter
+00000c40: 7661 6c73 2074 6861 7420 5665 6e6e 2d41  vals that Venn-A
+00000c50: 6265 7273 2069 6e64 6963 6174 6520 666f  bers indicate fo
+00000c60: 7220 616e 2069 6e73 7461 6e63 6520 6368  r an instance ch
+00000c70: 616e 6769 6e67 2061 2066 6561 7475 7265  anging a feature
+00000c80: 2076 616c 7565 2069 6e20 6163 636f 7264   value in accord
+00000c90: 616e 6365 2077 6974 6820 7468 6520 7275  ance with the ru
+00000ca0: 6c65 2063 6f6e 6469 7469 6f6e 2e0d 0a3c  le condition...<
+00000cb0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000cc0: 3e0d 0a20 203c 6120 6872 6566 3d22 6874  >..  <a href="ht
+00000cd0: 7470 733a 2f2f 6361 6c69 6272 6174 6564  tps://calibrated
+00000ce0: 2d65 7870 6c61 6e61 7469 6f6e 732e 7265  -explanations.re
+00000cf0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000d00: 6c61 7465 7374 2f3f 6261 6467 653d 6c61  latest/?badge=la
+00000d10: 7465 7374 223e 0d0a 2020 2020 3c69 6d67  test">..    <img
+00000d20: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000d30: 7468 7562 2e63 6f6d 2f4d 6f66 6672 616e  thub.com/Moffran
+00000d40: 2f63 616c 6962 7261 7465 645f 6578 706c  /calibrated_expl
+00000d50: 616e 6174 696f 6e73 2f62 6c6f 622f 6d61  anations/blob/ma
+00000d60: 696e 2f64 6f63 732f 696d 6167 6573 2f63  in/docs/images/c
+00000d70: 6f75 6e74 6572 6661 6374 7561 6c5f 7072  ounterfactual_pr
+00000d80: 6f62 6162 696c 6973 7469 635f 686f 7573  obabilistic_hous
+00000d90: 655f 7265 6772 6573 7369 6f6e 2e6a 7067  e_regression.jpg
+00000da0: 2220 616c 743d 2250 726f 6261 6269 6c69  " alt="Probabili
+00000db0: 7374 6963 2063 6f75 6e74 6572 6661 6374  stic counterfact
+00000dc0: 7561 6c20 6578 706c 616e 6174 696f 6e20  ual explanation 
+00000dd0: 666f 7220 4361 6c69 666f 726e 6961 2048  for California H
+00000de0: 6f75 7369 6e67 223e 0d0a 2020 3c2f 613e  ousing">..  </a>
+00000df0: 0d0a 3c2f 703e 0d0a 0d0a 5461 626c 6520  ..</p>....Table 
+00000e00: 3120 7375 6d6d 6172 697a 6573 2074 6865  1 summarizes the
+00000e10: 2063 6861 7261 6374 6572 6973 7469 6373   characteristics
+00000e20: 206f 6620 4361 6c69 6272 6174 6564 2045   of Calibrated E
+00000e30: 7870 6c61 6e61 7469 6f6e 732e 0d0a 3c70  xplanations...<p
+00000e40: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+00000e50: 0d0a 2020 3c61 2068 7265 663d 2268 7474  ..  <a href="htt
+00000e60: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000e70: 6273 2f32 3330 382e 3136 3234 3522 3e0d  bs/2308.16245">.
+00000e80: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00000e90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ea0: 6d2f 4d6f 6666 7261 6e2f 6361 6c69 6272  m/Moffran/calibr
+00000eb0: 6174 6564 5f65 7870 6c61 6e61 7469 6f6e  ated_explanation
+00000ec0: 732f 626c 6f62 2f6d 6169 6e2f 646f 6373  s/blob/main/docs
+00000ed0: 2f69 6d61 6765 732f 5461 626c 6531 2e70  /images/Table1.p
+00000ee0: 6e67 2220 616c 743d 2243 6861 7261 6374  ng" alt="Charact
+00000ef0: 6572 6973 7469 6373 206f 6620 4361 6c69  eristics of Cali
+00000f00: 6272 6174 6564 2045 7870 6c61 6e61 6e74  brated Explanant
+00000f10: 696f 6e73 223e 0d0a 2020 3c2f 613e 0d0a  ions">..  </a>..
+00000f20: 3c2f 703e 0d0a 0d0a 4765 7474 696e 6720  </p>....Getting 
+00000f30: 7374 6172 7465 640d 0a2d 2d2d 2d2d 2d2d  started..-------
+00000f40: 2d2d 2d2d 2d2d 2d2d 0d0a 5468 6520 5b6e  --------..The [n
+00000f50: 6f74 6562 6f6f 6b73 2066 6f6c 6465 725d  otebooks folder]
+00000f60: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000f70: 636f 6d2f 4d6f 6666 7261 6e2f 6361 6c69  com/Moffran/cali
+00000f80: 6272 6174 6564 5f65 7870 6c61 6e61 7469  brated_explanati
+00000f90: 6f6e 732f 7472 6565 2f6d 6169 6e2f 6e6f  ons/tree/main/no
+00000fa0: 7465 626f 6f6b 7329 2063 6f6e 7461 696e  tebooks) contain
+00000fb0: 7320 6120 6e75 6d62 6572 206f 6620 6e6f  s a number of no
+00000fc0: 7465 626f 6f6b 7320 696c 6c75 7374 7261  tebooks illustra
+00000fd0: 7469 6e67 2064 6966 6665 7265 6e74 2075  ting different u
+00000fe0: 7365 2063 6173 6573 2066 6f72 2060 6361  se cases for `ca
+00000ff0: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
+00001000: 7469 6f6e 7360 2e20 5468 6520 666f 6c6c  tions`. The foll
+00001010: 6f77 696e 6720 6172 6520 636f 6d6d 656e  owing are commen
+00001020: 7465 6420 616e 6420 7368 6f75 6c64 2062  ted and should b
+00001030: 6520 6120 676f 6f64 2073 7461 7274 3a0d  e a good start:.
+00001040: 0a2a 205b 7175 6963 6b73 7461 7274 5d28  .* [quickstart](
+00001050: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001060: 6f6d 2f4d 6f66 6672 616e 2f63 616c 6962  om/Moffran/calib
+00001070: 7261 7465 645f 6578 706c 616e 6174 696f  rated_explanatio
+00001080: 6e73 2f62 6c6f 622f 6d61 696e 2f6e 6f74  ns/blob/main/not
+00001090: 6562 6f6f 6b73 2f71 7569 636b 7374 6172  ebooks/quickstar
+000010a0: 742e 6970 796e 6229 202d 2073 696d 696c  t.ipynb) - simil
+000010b0: 6172 2074 6f20 7468 6973 2047 6574 7469  ar to this Getti
+000010c0: 6e67 2053 7461 7274 6564 2c20 696e 636c  ng Started, incl
+000010d0: 7564 696e 6720 706c 6f74 732e 0d0a 2a20  uding plots...* 
+000010e0: 5b71 7569 636b 7374 6172 745f 7772 6170  [quickstart_wrap
+000010f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001100: 2e63 6f6d 2f4d 6f66 6672 616e 2f63 616c  .com/Moffran/cal
+00001110: 6962 7261 7465 645f 6578 706c 616e 6174  ibrated_explanat
+00001120: 696f 6e73 2f62 6c6f 622f 6d61 696e 2f6e  ions/blob/main/n
+00001130: 6f74 6562 6f6f 6b73 2f71 7569 636b 7374  otebooks/quickst
+00001140: 6172 745f 7772 6170 2e69 7079 6e62 2920  art_wrap.ipynb) 
+00001150: 2d20 7369 6d69 6c61 7220 746f 2074 6869  - similar to thi
+00001160: 7320 4765 7474 696e 6720 5374 6172 7465  s Getting Starte
+00001170: 642c 2062 7574 2077 6974 6820 6120 7772  d, but with a wr
+00001180: 6170 7065 7220 636c 6173 7320 666f 7220  apper class for 
+00001190: 6561 7369 6572 2075 7365 2e0d 0a2a 205b  easier use...* [
+000011a0: 6465 6d6f 5f62 696e 6172 795f 636c 6173  demo_binary_clas
+000011b0: 7369 6669 6361 7469 6f6e 5d28 6874 7470  sification](http
+000011c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
+000011d0: 6f66 6672 616e 2f63 616c 6962 7261 7465  offran/calibrate
+000011e0: 645f 6578 706c 616e 6174 696f 6e73 2f62  d_explanations/b
+000011f0: 6c6f 622f 6d61 696e 2f6e 6f74 6562 6f6f  lob/main/noteboo
+00001200: 6b73 2f64 656d 6f5f 6269 6e61 7279 5f63  ks/demo_binary_c
+00001210: 6c61 7373 6966 6963 6174 696f 6e2e 6970  lassification.ip
+00001220: 796e 6229 202d 2077 6974 6820 6578 616d  ynb) - with exam
+00001230: 706c 6573 2066 6f72 2062 696e 6172 7920  ples for binary 
+00001240: 636c 6173 7369 6669 6361 7469 6f6e 200d  classification .
+00001250: 0a2a 205b 6465 6d6f 5f6d 756c 7469 636c  .* [demo_multicl
+00001260: 6173 735d 2868 7474 7073 3a2f 2f67 6974  ass](https://git
+00001270: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
+00001280: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
+00001290: 6e61 7469 6f6e 732f 626c 6f62 2f6d 6169  nations/blob/mai
+000012a0: 6e2f 6e6f 7465 626f 6f6b 732f 6465 6d6f  n/notebooks/demo
+000012b0: 5f6d 756c 7469 636c 6173 735f 676c 6173  _multiclass_glas
+000012c0: 732e 6970 796e 6229 202d 2077 6974 6820  s.ipynb) - with 
+000012d0: 6578 616d 706c 6573 2066 6f72 206d 756c  examples for mul
+000012e0: 7469 2d63 6c61 7373 2063 6c61 7373 6966  ti-class classif
+000012f0: 6963 6174 696f 6e0d 0a2a 205b 6465 6d6f  ication..* [demo
+00001300: 5f72 6567 7265 7373 696f 6e5d 2868 7474  _regression](htt
+00001310: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001320: 4d6f 6666 7261 6e2f 6361 6c69 6272 6174  Moffran/calibrat
+00001330: 6564 5f65 7870 6c61 6e61 7469 6f6e 732f  ed_explanations/
+00001340: 626c 6f62 2f6d 6169 6e2f 6e6f 7465 626f  blob/main/notebo
+00001350: 6f6b 732f 6465 6d6f 5f72 6567 7265 7373  oks/demo_regress
+00001360: 696f 6e2e 6970 796e 6229 202d 2077 6974  ion.ipynb) - wit
+00001370: 6820 6578 616d 706c 6573 2066 6f72 2072  h examples for r
+00001380: 6567 7265 7373 696f 6e0d 0a2a 205b 6465  egression..* [de
+00001390: 6d6f 5f70 726f 6261 6269 6c69 7374 6963  mo_probabilistic
+000013a0: 5f72 6567 7265 7373 696f 6e5d 2868 7474  _regression](htt
+000013b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000013c0: 4d6f 6666 7261 6e2f 6361 6c69 6272 6174  Moffran/calibrat
+000013d0: 6564 5f65 7870 6c61 6e61 7469 6f6e 732f  ed_explanations/
+000013e0: 626c 6f62 2f6d 6169 6e2f 6e6f 7465 626f  blob/main/notebo
+000013f0: 6f6b 732f 6465 6d6f 5f70 726f 6261 6269  oks/demo_probabi
+00001400: 6c69 7374 6963 5f72 6567 7265 7373 696f  listic_regressio
+00001410: 6e2e 6970 796e 6229 202d 2077 6974 6820  n.ipynb) - with 
+00001420: 6578 616d 706c 6573 2066 6f72 2072 6567  examples for reg
+00001430: 7265 7373 696f 6e20 7769 7468 2074 6872  ression with thr
+00001440: 6573 686f 6c64 730d 0a2a 205b 6465 6d6f  esholds..* [demo
+00001450: 5f75 6e64 6572 5f74 6865 5f68 6f6f 645d  _under_the_hood]
+00001460: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001470: 636f 6d2f 4d6f 6666 7261 6e2f 6361 6c69  com/Moffran/cali
+00001480: 6272 6174 6564 5f65 7870 6c61 6e61 7469  brated_explanati
+00001490: 6f6e 732f 626c 6f62 2f6d 6169 6e2f 6e6f  ons/blob/main/no
+000014a0: 7465 626f 6f6b 732f 6465 6d6f 5f75 6e64  tebooks/demo_und
+000014b0: 6572 5f74 6865 5f68 6f6f 642e 6970 796e  er_the_hood.ipyn
+000014c0: 6229 202d 2069 6c6c 7573 7472 6174 696e  b) - illustratin
+000014d0: 6720 686f 7720 746f 2061 6363 6573 7320  g how to access 
+000014e0: 7468 6520 696e 666f 726d 6174 696f 6e20  the information 
+000014f0: 636f 6d70 6f73 696e 6720 7468 6520 6578  composing the ex
+00001500: 706c 616e 6174 696f 6e73 0d0a 0d0a 2323  planations....##
+00001510: 2320 436c 6173 7369 6669 6361 7469 6f6e  # Classification
+00001520: 0d0a 4c65 7420 7573 2069 6c6c 7573 7472  ..Let us illustr
+00001530: 6174 6520 686f 7720 7765 206d 6179 2075  ate how we may u
+00001540: 7365 2060 6361 6c69 6272 6174 6564 2d65  se `calibrated-e
+00001550: 7870 6c61 6e61 7469 6f6e 7360 2074 6f20  xplanations` to 
+00001560: 6765 6e65 7261 7465 2065 7870 6c61 6e61  generate explana
+00001570: 7469 6f6e 7320 6672 6f6d 2061 2063 6c61  tions from a cla
+00001580: 7373 6966 6965 7220 7472 6169 6e65 6420  ssifier trained 
+00001590: 6f6e 2061 2064 6174 6173 6574 2066 726f  on a dataset fro
+000015a0: 6d0d 0a5b 7777 772e 6f70 656e 6d6c 2e6f  m..[www.openml.o
+000015b0: 7267 5d28 6874 7470 733a 2f2f 7777 772e  rg](https://www.
+000015c0: 6f70 656e 6d6c 2e6f 7267 292c 2077 6869  openml.org), whi
+000015d0: 6368 2077 6520 6669 7273 7420 7370 6c69  ch we first spli
+000015e0: 7420 696e 746f 2061 0d0a 7472 6169 6e69  t into a..traini
+000015f0: 6e67 2061 6e64 2061 2074 6573 7420 7365  ng and a test se
+00001600: 7420 7573 696e 6720 6074 7261 696e 5f74  t using `train_t
+00001610: 6573 745f 7370 6c69 7460 2066 726f 6d0d  est_split` from.
+00001620: 0a5b 736b 6c65 6172 6e5d 2868 7474 7073  .[sklearn](https
+00001630: 3a2f 2f73 6369 6b69 742d 6c65 6172 6e2e  ://scikit-learn.
+00001640: 6f72 6729 2c20 616e 6420 7468 656e 2066  org), and then f
+00001650: 7572 7468 6572 2073 706c 6974 2074 6865  urther split the
+00001660: 0d0a 7472 6169 6e69 6e67 2073 6574 2069  ..training set i
+00001670: 6e74 6f20 6120 7072 6f70 6572 2074 7261  nto a proper tra
+00001680: 696e 696e 6720 7365 7420 616e 6420 6120  ining set and a 
+00001690: 6361 6c69 6272 6174 696f 6e20 7365 743a  calibration set:
+000016a0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+000016b0: 726f 6d20 736b 6c65 6172 6e2e 6461 7461  rom sklearn.data
+000016c0: 7365 7473 2069 6d70 6f72 7420 6665 7463  sets import fetc
+000016d0: 685f 6f70 656e 6d6c 0d0a 6672 6f6d 2073  h_openml..from s
+000016e0: 6b6c 6561 726e 2e6d 6f64 656c 5f73 656c  klearn.model_sel
+000016f0: 6563 7469 6f6e 2069 6d70 6f72 7420 7472  ection import tr
+00001700: 6169 6e5f 7465 7374 5f73 706c 6974 0d0a  ain_test_split..
+00001710: 0d0a 6461 7461 7365 7420 3d20 6665 7463  ..dataset = fetc
+00001720: 685f 6f70 656e 6d6c 286e 616d 653d 2277  h_openml(name="w
+00001730: 696e 6522 2c20 7665 7273 696f 6e3d 372c  ine", version=7,
+00001740: 2061 735f 6672 616d 653d 5472 7565 290d   as_frame=True).
+00001750: 0a0d 0a58 203d 2064 6174 6173 6574 2e64  ...X = dataset.d
+00001760: 6174 612e 7661 6c75 6573 2e61 7374 7970  ata.values.astyp
+00001770: 6528 666c 6f61 7429 0d0a 7920 3d20 2864  e(float)..y = (d
+00001780: 6174 6173 6574 2e74 6172 6765 742e 7661  ataset.target.va
+00001790: 6c75 6573 203d 3d20 2754 7275 6527 292e  lues == 'True').
+000017a0: 6173 7479 7065 2869 6e74 290d 0a0d 0a66  astype(int)....f
+000017b0: 6561 7475 7265 5f6e 616d 6573 203d 2064  eature_names = d
+000017c0: 6174 6173 6574 2e66 6561 7475 7265 5f6e  ataset.feature_n
+000017d0: 616d 6573 0d0a 0d0a 585f 7472 6169 6e2c  ames....X_train,
+000017e0: 2058 5f74 6573 742c 2079 5f74 7261 696e   X_test, y_train
+000017f0: 2c20 795f 7465 7374 203d 2074 7261 696e  , y_test = train
+00001800: 5f74 6573 745f 7370 6c69 7428 582c 2079  _test_split(X, y
+00001810: 2c20 7465 7374 5f73 697a 653d 322c 2073  , test_size=2, s
+00001820: 7472 6174 6966 793d 7929 0d0a 0d0a 585f  tratify=y)....X_
+00001830: 7072 6f70 5f74 7261 696e 2c20 585f 6361  prop_train, X_ca
+00001840: 6c2c 2079 5f70 726f 705f 7472 6169 6e2c  l, y_prop_train,
+00001850: 2079 5f63 616c 203d 2074 7261 696e 5f74   y_cal = train_t
+00001860: 6573 745f 7370 6c69 7428 585f 7472 6169  est_split(X_trai
+00001870: 6e2c 2079 5f74 7261 696e 2c0d 0a20 2020  n, y_train,..   
+00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 2020 2020 2020 2020 2074 6573 745f 7369           test_si
+000018c0: 7a65 3d30 2e32 3529 0d0a 0d0a 6060 600d  ze=0.25)....```.
+000018d0: 0a0d 0a57 6520 6e6f 7720 6669 7420 6120  ...We now fit a 
+000018e0: 6d6f 6465 6c20 6f6e 206f 7572 2064 6174  model on our dat
+000018f0: 612e 200d 0a0d 0a60 6060 7079 7468 6f6e  a. ....```python
+00001900: 0d0a 6672 6f6d 2073 6b6c 6561 726e 2e65  ..from sklearn.e
+00001910: 6e73 656d 626c 6520 696d 706f 7274 2052  nsemble import R
+00001920: 616e 646f 6d46 6f72 6573 7443 6c61 7373  andomForestClass
+00001930: 6966 6965 720d 0a0d 0a72 6620 3d20 5261  ifier....rf = Ra
+00001940: 6e64 6f6d 466f 7265 7374 436c 6173 7369  ndomForestClassi
+00001950: 6669 6572 286e 5f6a 6f62 733d 2d31 290d  fier(n_jobs=-1).
+00001960: 0a0d 0a72 662e 6669 7428 585f 7072 6f70  ...rf.fit(X_prop
+00001970: 5f74 7261 696e 2c20 795f 7072 6f70 5f74  _train, y_prop_t
+00001980: 7261 696e 290d 0a60 6060 0d0a 0d0a 2323  rain)..```....##
+00001990: 2323 2046 6163 7475 616c 2045 7870 6c61  ## Factual Expla
+000019a0: 6e61 7469 6f6e 730d 0a4c 6574 7320 6578  nations..Lets ex
+000019b0: 7472 6163 7420 6578 706c 616e 6174 696f  tract explanatio
+000019c0: 6e73 2066 6f72 206f 7572 2074 6573 7420  ns for our test 
+000019d0: 7365 7420 7573 696e 6720 7468 6520 6063  set using the `c
+000019e0: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
+000019f0: 6174 696f 6e73 6020 7061 636b 6167 6520  ations` package 
+00001a00: 6279 2069 6d70 6f72 7469 6e67 2060 4361  by importing `Ca
+00001a10: 6c69 6272 6174 6564 4578 706c 6169 6e65  libratedExplaine
+00001a20: 7260 2066 726f 6d20 6063 616c 6962 7261  r` from `calibra
+00001a30: 7465 645f 6578 706c 616e 6174 696f 6e73  ted_explanations
+00001a40: 602e 0d0a 0d0a 6060 6070 7974 686f 6e0d  `.....```python.
+00001a50: 0a66 726f 6d20 6361 6c69 6272 6174 6564  .from calibrated
+00001a60: 5f65 7870 6c61 6e61 7469 6f6e 7320 696d  _explanations im
+00001a70: 706f 7274 2043 616c 6962 7261 7465 6445  port CalibratedE
+00001a80: 7870 6c61 696e 6572 2c20 5f5f 7665 7273  xplainer, __vers
+00001a90: 696f 6e5f 5f0d 0a70 7269 6e74 285f 5f76  ion__..print(__v
+00001aa0: 6572 7369 6f6e 5f5f 290d 0a0d 0a65 7870  ersion__)....exp
+00001ab0: 6c61 696e 6572 203d 2043 616c 6962 7261  lainer = Calibra
+00001ac0: 7465 6445 7870 6c61 696e 6572 2872 662c  tedExplainer(rf,
+00001ad0: 2058 5f63 616c 2c20 795f 6361 6c2c 2066   X_cal, y_cal, f
+00001ae0: 6561 7475 7265 5f6e 616d 6573 3d66 6561  eature_names=fea
+00001af0: 7475 7265 5f6e 616d 6573 290d 0a0d 0a66  ture_names)....f
+00001b00: 6163 7475 616c 5f65 7870 6c61 6e61 7469  actual_explanati
+00001b10: 6f6e 7320 3d20 6578 706c 6169 6e65 722e  ons = explainer.
+00001b20: 6578 706c 6169 6e5f 6661 6374 7561 6c28  explain_factual(
+00001b30: 585f 7465 7374 290d 0a60 6060 0d0a 0d0a  X_test)..```....
+00001b40: 4f6e 6365 2077 6520 6861 7665 2074 6865  Once we have the
+00001b50: 2065 7870 6c61 6e61 7469 6f6e 732c 2077   explanations, w
+00001b60: 6520 6361 6e20 706c 6f74 2061 6c6c 206f  e can plot all o
+00001b70: 6620 7468 656d 2075 7369 6e67 2060 706c  f them using `pl
+00001b80: 6f74 5f61 6c6c 602e 2044 6566 6175 6c74  ot_all`. Default
+00001b90: 2c20 6120 7265 6775 6c61 7220 706c 6f74  , a regular plot
+00001ba0: 2c20 7769 7468 6f75 7420 756e 6365 7274  , without uncert
+00001bb0: 6169 6e74 7920 696e 7465 7276 616c 7320  ainty intervals 
+00001bc0: 696e 636c 7564 6564 2c20 6973 2063 7265  included, is cre
+00001bd0: 6174 6564 2e20 546f 2069 6e63 6c75 6465  ated. To include
+00001be0: 2075 6e63 6572 7461 696e 7479 2069 6e74   uncertainty int
+00001bf0: 6572 7661 6c73 2c20 6368 616e 6765 2074  ervals, change t
+00001c00: 6865 2070 6172 616d 6574 6572 2060 756e  he parameter `un
+00001c10: 6365 7274 6169 6e74 793d 5472 7565 602e  certainty=True`.
+00001c20: 2054 6f20 706c 6f74 206f 6e6c 7920 6120   To plot only a 
+00001c30: 7369 6e67 6c65 2069 6e73 7461 6e63 652c  single instance,
+00001c40: 2074 6865 2060 706c 6f74 5f65 7870 6c61   the `plot_expla
+00001c50: 6e61 7469 6f6e 6020 6675 6e63 7469 6f6e  nation` function
+00001c60: 2063 616e 2062 6520 6361 6c6c 6564 2c20   can be called, 
+00001c70: 7375 626d 6974 7469 6e67 2074 6865 2069  submitting the i
+00001c80: 6e64 6578 206f 6620 7468 6520 7465 7374  ndex of the test
+00001c90: 2069 6e73 7461 6e63 6520 746f 2070 6c6f   instance to plo
+00001ca0: 742e 2059 6f75 2063 616e 2061 6c73 6f20  t. You can also 
+00001cb0: 6164 6420 616e 6420 7265 6d6f 7665 2063  add and remove c
+00001cc0: 6f6e 6a75 6e63 7469 7665 2072 756c 6573  onjunctive rules
+00001cd0: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
+00001ce0: 6661 6374 7561 6c5f 6578 706c 616e 6174  factual_explanat
+00001cf0: 696f 6e73 2e70 6c6f 745f 616c 6c28 290d  ions.plot_all().
+00001d00: 0a66 6163 7475 616c 5f65 7870 6c61 6e61  .factual_explana
+00001d10: 7469 6f6e 732e 706c 6f74 5f61 6c6c 2875  tions.plot_all(u
+00001d20: 6e63 6572 7461 696e 7479 3d54 7275 6529  ncertainty=True)
+00001d30: 0d0a 0d0a 6661 6374 7561 6c5f 6578 706c  ....factual_expl
+00001d40: 616e 6174 696f 6e73 2e70 6c6f 745f 6578  anations.plot_ex
+00001d50: 706c 616e 6174 696f 6e28 302c 2075 6e63  planation(0, unc
+00001d60: 6572 7461 696e 7479 3d54 7275 6529 0d0a  ertainty=True)..
+00001d70: 0d0a 6661 6374 7561 6c5f 6578 706c 616e  ..factual_explan
+00001d80: 6174 696f 6e73 2e61 6464 5f63 6f6e 6a75  ations.add_conju
+00001d90: 6e63 7469 6f6e 7328 292e 706c 6f74 5f61  nctions().plot_a
+00001da0: 6c6c 2829 0d0a 6661 6374 7561 6c5f 6578  ll()..factual_ex
+00001db0: 706c 616e 6174 696f 6e73 2e72 656d 6f76  planations.remov
+00001dc0: 655f 636f 6e6a 756e 6374 696f 6e73 2829  e_conjunctions()
+00001dd0: 2e70 6c6f 745f 616c 6c28 290d 0a60 6060  .plot_all()..```
+00001de0: 0d0a 0d0a 2323 2323 2043 6f75 6e74 6572  ....#### Counter
+00001df0: 6661 6374 7561 6c20 4578 706c 616e 6174  factual Explanat
+00001e00: 696f 6e73 0d0a 416e 2061 6c74 6572 6e61  ions..An alterna
+00001e10: 7469 7665 2074 6f20 6661 6374 7561 6c20  tive to factual 
+00001e20: 7275 6c65 7320 6973 2074 6f20 6578 7472  rules is to extr
+00001e30: 6163 7420 636f 756e 7465 7266 6163 7475  act counterfactu
+00001e40: 616c 2072 756c 6573 2e20 0d0a 6065 7870  al rules. ..`exp
+00001e50: 6c61 696e 5f63 6f75 6e74 6572 6661 6374  lain_counterfact
+00001e60: 7561 6c60 2063 616e 2062 6520 6361 6c6c  ual` can be call
+00001e70: 6564 2074 6f20 6765 7420 636f 756e 7465  ed to get counte
+00001e80: 7266 6163 7475 616c 2072 756c 6573 2077  rfactual rules w
+00001e90: 6974 6820 616e 2061 7070 726f 7072 6961  ith an appropria
+00001ea0: 7465 2064 6973 6372 6574 697a 6572 2061  te discretizer a
+00001eb0: 7574 6f6d 6174 6963 616c 6c79 2061 7373  utomatically ass
+00001ec0: 6967 6e65 642e 2020 0d0a 0d0a 6060 6070  igned.  ....```p
+00001ed0: 7974 686f 6e0d 0a63 6f75 6e74 6572 6661  ython..counterfa
+00001ee0: 6374 7561 6c5f 6578 706c 616e 6174 696f  ctual_explanatio
+00001ef0: 6e73 203d 2065 7870 6c61 696e 6572 2e65  ns = explainer.e
+00001f00: 7870 6c61 696e 5f63 6f75 6e74 6572 6661  xplain_counterfa
+00001f10: 6374 7561 6c28 585f 7465 7374 290d 0a60  ctual(X_test)..`
+00001f20: 6060 0d0a 0d0a 436f 756e 7465 7266 6163  ``....Counterfac
+00001f30: 7475 616c 7320 6172 6520 616c 736f 2076  tuals are also v
+00001f40: 6973 7561 6c69 7a65 6420 7573 696e 6720  isualized using 
+00001f50: 7468 6520 6070 6c6f 745f 616c 6c60 2e20  the `plot_all`. 
+00001f60: 506c 6f74 7469 6e67 2061 6e20 696e 6469  Plotting an indi
+00001f70: 7669 6475 616c 2063 6f75 6e74 6572 6661  vidual counterfa
+00001f80: 6374 7561 6c20 6578 706c 616e 6174 696f  ctual explanatio
+00001f90: 6e20 6973 2064 6f6e 6520 7573 696e 6720  n is done using 
+00001fa0: 6070 6c6f 745f 6578 706c 616e 6174 696f  `plot_explanatio
+00001fb0: 6e60 2c20 7375 626d 6974 7469 6e67 2074  n`, submitting t
+00001fc0: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+00001fd0: 7465 7374 2069 6e73 7461 6e63 6520 746f  test instance to
+00001fe0: 2070 6c6f 742e 2041 6464 696e 6720 6f72   plot. Adding or
+00001ff0: 2072 656d 6f76 696e 6720 636f 6e6a 756e   removing conjun
+00002000: 6374 696f 6e73 2069 7320 646f 6e65 2061  ctions is done a
+00002010: 7320 6265 666f 7265 2e20 0d0a 0d0a 6060  s before. ....``
+00002020: 6070 7974 686f 6e0d 0a63 6f75 6e74 6572  `python..counter
+00002030: 6661 6374 7561 6c5f 6578 706c 616e 6174  factual_explanat
+00002040: 696f 6e73 2e70 6c6f 745f 616c 6c28 290d  ions.plot_all().
+00002050: 0a63 6f75 6e74 6572 6661 6374 7561 6c5f  .counterfactual_
+00002060: 6578 706c 616e 6174 696f 6e73 2e70 6c6f  explanations.plo
+00002070: 745f 6578 706c 616e 6174 696f 6e28 3029  t_explanation(0)
+00002080: 0d0a 636f 756e 7465 7266 6163 7475 616c  ..counterfactual
+00002090: 5f65 7870 6c61 6e61 7469 6f6e 732e 6164  _explanations.ad
+000020a0: 645f 636f 6e6a 756e 6374 696f 6e73 2829  d_conjunctions()
+000020b0: 2e70 6c6f 745f 616c 6c28 290d 0a60 6060  .plot_all()..```
+000020c0: 0d0a 0d0a 496e 6469 7669 6475 616c 2065  ....Individual e
+000020d0: 7870 6c61 6e61 7469 6f6e 7320 6361 6e20  xplanations can 
+000020e0: 616c 736f 2062 6520 706c 6f74 7465 6420  also be plotted 
+000020f0: 7573 696e 6720 6070 6c6f 745f 6578 706c  using `plot_expl
+00002100: 616e 6174 696f 6e60 2e0d 0a20 2020 2020  anation`...     
+00002110: 200d 0a60 6060 7079 7468 6f6e 0d0a 6661   ..```python..fa
+00002120: 6374 7561 6c5f 6578 706c 616e 6174 696f  ctual_explanatio
+00002130: 6e73 2e67 6574 5f65 7870 6c61 6e61 7469  ns.get_explanati
+00002140: 6f6e 2830 292e 706c 6f74 5f65 7870 6c61  on(0).plot_expla
+00002150: 6e61 7469 6f6e 2829 0d0a 636f 756e 7465  nation()..counte
+00002160: 7266 6163 7475 616c 5f65 7870 6c61 6e61  rfactual_explana
+00002170: 7469 6f6e 732e 6765 745f 6578 706c 616e  tions.get_explan
+00002180: 6174 696f 6e28 3029 2e70 6c6f 745f 6578  ation(0).plot_ex
+00002190: 706c 616e 6174 696f 6e28 290d 0a60 6060  planation()..```
+000021a0: 0d0a 2323 2323 2053 7570 706f 7274 2066  ..#### Support f
+000021b0: 6f72 206d 756c 7469 636c 6173 730d 0a60  or multiclass..`
+000021c0: 6361 6c69 6272 6174 6564 2d65 7870 6c61  calibrated-expla
+000021d0: 6e61 7469 6f6e 7360 2073 7570 706f 7274  nations` support
+000021e0: 7320 6d75 6c74 6963 6c61 7373 2077 6869  s multiclass whi
+000021f0: 6368 2069 7320 6465 6d6f 6e73 7472 6174  ch is demonstrat
+00002200: 6564 2069 6e20 5b64 656d 6f5f 6d75 6c74  ed in [demo_mult
+00002210: 6963 6c61 7373 5d28 6874 7470 733a 2f2f  iclass](https://
+00002220: 6769 7468 7562 2e63 6f6d 2f4d 6f66 6672  github.com/Moffr
+00002230: 616e 2f63 616c 6962 7261 7465 645f 6578  an/calibrated_ex
+00002240: 706c 616e 6174 696f 6e73 2f62 6c6f 622f  planations/blob/
+00002250: 6d61 696e 2f6e 6f74 6562 6f6f 6b73 2f64  main/notebooks/d
+00002260: 656d 6f5f 6d75 6c74 6963 6c61 7373 5f67  emo_multiclass_g
+00002270: 6c61 7373 2e69 7079 6e62 292e 2054 6861  lass.ipynb). Tha
+00002280: 7420 6e6f 7465 626f 6f6b 2061 6c73 6f20  t notebook also 
+00002290: 6465 6d6f 6e73 7472 6174 6573 2068 6f77  demonstrates how
+000022a0: 2062 6f74 6820 6665 6174 7572 6520 6e61   both feature na
+000022b0: 6d65 7320 616e 6420 7461 7267 6574 2061  mes and target a
+000022c0: 6e64 2063 6174 6567 6f72 6963 616c 206c  nd categorical l
+000022d0: 6162 656c 7320 6361 6e20 6265 2061 6464  abels can be add
+000022e0: 6564 2074 6f20 696d 7072 6f76 6520 7468  ed to improve th
+000022f0: 6520 696e 7465 7270 7265 7461 6269 6c69  e interpretabili
+00002300: 7479 2e20 0d0a 0d0a 2323 2320 5265 6772  ty. ....### Regr
+00002310: 6573 7369 6f6e 0d0a 4578 7472 6163 7469  ession..Extracti
+00002320: 6e67 2065 7870 6c61 6e61 7469 6f6e 7320  ng explanations 
+00002330: 666f 7220 7265 6772 6573 7369 6f6e 2069  for regression i
+00002340: 7320 7665 7279 2073 696d 696c 6172 2074  s very similar t
+00002350: 6f20 686f 7720 6974 2069 7320 646f 6e65  o how it is done
+00002360: 2066 6f72 2063 6c61 7373 6966 6963 6174   for classificat
+00002370: 696f 6e2e 200d 0a0d 0a60 6060 7079 7468  ion. ....```pyth
+00002380: 6f6e 0d0a 6461 7461 7365 7420 3d20 6665  on..dataset = fe
+00002390: 7463 685f 6f70 656e 6d6c 286e 616d 653d  tch_openml(name=
+000023a0: 2268 6f75 7365 5f73 616c 6573 222c 2076  "house_sales", v
+000023b0: 6572 7369 6f6e 3d33 290d 0a0d 0a58 203d  ersion=3)....X =
+000023c0: 2064 6174 6173 6574 2e64 6174 612e 7661   dataset.data.va
+000023d0: 6c75 6573 2e61 7374 7970 6528 666c 6f61  lues.astype(floa
+000023e0: 7429 0d0a 7920 3d20 6461 7461 7365 742e  t)..y = dataset.
+000023f0: 7461 7267 6574 2e76 616c 7565 730d 0a0d  target.values...
+00002400: 0a58 5f74 7261 696e 2c20 585f 7465 7374  .X_train, X_test
+00002410: 2c20 795f 7472 6169 6e2c 2079 5f74 6573  , y_train, y_tes
+00002420: 7420 3d20 7472 6169 6e5f 7465 7374 5f73  t = train_test_s
+00002430: 706c 6974 2858 2c20 792c 2074 6573 745f  plit(X, y, test_
+00002440: 7369 7a65 3d31 290d 0a0d 0a58 5f70 726f  size=1)....X_pro
+00002450: 705f 7472 6169 6e2c 2058 5f63 616c 2c20  p_train, X_cal, 
+00002460: 795f 7072 6f70 5f74 7261 696e 2c20 795f  y_prop_train, y_
+00002470: 6361 6c20 3d20 7472 6169 6e5f 7465 7374  cal = train_test
+00002480: 5f73 706c 6974 2858 5f74 7261 696e 2c20  _split(X_train, 
+00002490: 795f 7472 6169 6e2c 0d0a 2020 2020 2020  y_train,..      
+000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2020 2020 7465 7374 5f73 697a 653d        test_size=
+000024e0: 302e 3235 290d 0a60 6060 0d0a 0d0a 4c65  0.25)..```....Le
+000024f0: 7420 7573 206e 6f77 2066 6974 2061 2060  t us now fit a `
+00002500: 5261 6e64 6f6d 466f 7265 7374 5265 6772  RandomForestRegr
+00002510: 6573 736f 7260 2066 726f 6d0d 0a5b 736b  essor` from..[sk
+00002520: 6c65 6172 6e5d 2868 7474 7073 3a2f 2f73  learn](https://s
+00002530: 6369 6b69 742d 6c65 6172 6e2e 6f72 6729  cikit-learn.org)
+00002540: 2074 6f20 7468 6520 7072 6f70 6572 2074   to the proper t
+00002550: 7261 696e 696e 670d 0a73 6574 3a0d 0a0d  raining..set:...
+00002560: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00002570: 2073 6b6c 6561 726e 2e65 6e73 656d 626c   sklearn.ensembl
+00002580: 6520 696d 706f 7274 2052 616e 646f 6d46  e import RandomF
+00002590: 6f72 6573 7452 6567 7265 7373 6f72 0d0a  orestRegressor..
+000025a0: 0d0a 7266 203d 2052 616e 646f 6d46 6f72  ..rf = RandomFor
+000025b0: 6573 7452 6567 7265 7373 6f72 2829 0d0a  estRegressor()..
+000025c0: 7266 2e66 6974 2858 5f70 726f 705f 7472  rf.fit(X_prop_tr
+000025d0: 6169 6e2c 2079 5f70 726f 705f 7472 6169  ain, y_prop_trai
+000025e0: 6e29 0d0a 6060 600d 0a0d 0a23 2323 2320  n)..```....#### 
+000025f0: 4661 6374 7561 6c20 4578 706c 616e 6174  Factual Explanat
+00002600: 696f 6e73 0d0a 4465 6669 6e65 2061 2060  ions..Define a `
+00002610: 4361 6c69 6272 6174 6564 4578 706c 6169  CalibratedExplai
+00002620: 6e65 7260 206f 626a 6563 7420 7573 696e  ner` object usin
+00002630: 6720 7468 6520 6e65 7720 6d6f 6465 6c20  g the new model 
+00002640: 616e 6420 6461 7461 2e20 5468 6520 606d  and data. The `m
+00002650: 6f64 6560 2070 6172 616d 6574 6572 206d  ode` parameter m
+00002660: 7573 7420 6265 2065 7870 6c69 6369 746c  ust be explicitl
+00002670: 7920 7365 7420 746f 2072 6567 7265 7373  y set to regress
+00002680: 696f 6e2e 2052 6567 756c 6172 2061 6e64  ion. Regular and
+00002690: 2075 6e63 6572 7461 696e 7479 2070 6c6f   uncertainty plo
+000026a0: 7473 2077 6f72 6b20 696e 2074 6865 2073  ts work in the s
+000026b0: 616d 6520 7761 7920 6173 2066 6f72 2063  ame way as for c
+000026c0: 6c61 7373 6966 6963 6174 696f 6e2e 0d0a  lassification...
+000026d0: 0d0a 6060 6070 7974 686f 6e0d 0a65 7870  ..```python..exp
+000026e0: 6c61 696e 6572 203d 2043 616c 6962 7261  lainer = Calibra
+000026f0: 7465 6445 7870 6c61 696e 6572 2872 662c  tedExplainer(rf,
+00002700: 2058 5f63 616c 2c20 795f 6361 6c2c 206d   X_cal, y_cal, m
+00002710: 6f64 653d 2772 6567 7265 7373 696f 6e27  ode='regression'
+00002720: 290d 0a0d 0a66 6163 7475 616c 5f65 7870  )....factual_exp
+00002730: 6c61 6e61 7469 6f6e 7320 3d20 6578 706c  lanations = expl
+00002740: 6169 6e65 722e 6578 706c 6169 6e5f 6661  ainer.explain_fa
+00002750: 6374 7561 6c28 585f 7465 7374 290d 0a0d  ctual(X_test)...
+00002760: 0a66 6163 7475 616c 5f65 7870 6c61 6e61  .factual_explana
+00002770: 7469 6f6e 732e 706c 6f74 5f61 6c6c 2829  tions.plot_all()
+00002780: 0d0a 6661 6374 7561 6c5f 6578 706c 616e  ..factual_explan
+00002790: 6174 696f 6e73 2e70 6c6f 745f 616c 6c28  ations.plot_all(
+000027a0: 756e 6365 7274 6169 6e74 793d 5472 7565  uncertainty=True
+000027b0: 290d 0a0d 0a66 6163 7475 616c 5f65 7870  )....factual_exp
+000027c0: 6c61 6e61 7469 6f6e 732e 6164 645f 636f  lanations.add_co
+000027d0: 6e6a 756e 6374 696f 6e73 2829 2e70 6c6f  njunctions().plo
+000027e0: 745f 616c 6c28 290d 0a60 6060 0d0a 4465  t_all()..```..De
+000027f0: 6661 756c 742c 2074 6865 2063 6f6e 6669  fault, the confi
+00002800: 6465 6e63 6520 696e 7465 7276 616c 2069  dence interval i
+00002810: 7320 7365 7420 746f 2061 2073 796d 6d65  s set to a symme
+00002820: 7472 6963 2069 6e74 6572 7661 6c20 6f66  tric interval of
+00002830: 2039 3025 2028 6465 6669 6e65 6420 6173   90% (defined as
+00002840: 2060 6c6f 775f 6869 6768 5f70 6572 6365   `low_high_perce
+00002850: 6e74 696c 6573 3d28 352c 3935 2960 292e  ntiles=(5,95)`).
+00002860: 2054 6865 2069 6e74 6572 7661 6c73 2063   The intervals c
+00002870: 616e 2063 6f76 6572 2061 6e79 2075 7365  an cover any use
+00002880: 7220 7370 6563 6966 6965 6420 696e 7465  r specified inte
+00002890: 7276 616c 2c20 696e 636c 7564 696e 6720  rval, including 
+000028a0: 6f6e 652d 7369 6465 6420 696e 7465 7276  one-sided interv
+000028b0: 616c 732e 2054 6f20 6465 6669 6e65 2061  als. To define a
+000028c0: 206f 6e65 2d73 6964 6564 2075 7070 6572   one-sided upper
+000028d0: 2d62 6f75 6e64 6564 2039 3025 2069 6e74  -bounded 90% int
+000028e0: 6572 7661 6c2c 2073 6574 2060 6c6f 775f  erval, set `low_
+000028f0: 6869 6768 5f70 6572 6365 6e74 696c 6573  high_percentiles
+00002900: 3d28 2d6e 702e 696e 662c 3930 2960 2c20  =(-np.inf,90)`, 
+00002910: 616e 6420 746f 2064 6566 696e 6520 6120  and to define a 
+00002920: 6f6e 652d 7369 6465 6420 6c6f 7765 722d  one-sided lower-
+00002930: 626f 756e 6465 6420 3935 2520 696e 7465  bounded 95% inte
+00002940: 7276 616c 2c20 7365 7420 606c 6f77 5f68  rval, set `low_h
+00002950: 6967 685f 7065 7263 656e 7469 6c65 733d  igh_percentiles=
+00002960: 2835 2c6e 702e 696e 6629 602e 2050 6572  (5,np.inf)`. Per
+00002970: 6365 6e74 696c 6573 2063 616e 2061 6c73  centiles can als
+00002980: 6f20 6265 2073 6574 2074 6f20 616e 7920  o be set to any 
+00002990: 6f74 6865 7220 7661 6c75 6573 2069 6e20  other values in 
+000029a0: 7468 6520 7261 6e67 6520 2830 2c31 3030  the range (0,100
+000029b0: 2920 2865 7863 6c75 7369 7665 292c 2061  ) (exclusive), a
+000029c0: 6e64 2069 6e74 6572 7661 6c73 2064 6f20  nd intervals do 
+000029d0: 6e6f 7420 6861 7665 2074 6f20 6265 2073  not have to be s
+000029e0: 796d 6d65 7472 6963 2e20 0d0a 0d0a 6060  ymmetric. ....``
+000029f0: 6070 7974 686f 6e0d 0a6c 6f77 6572 5f62  `python..lower_b
+00002a00: 6f75 6e64 6564 5f65 7870 6c61 6e61 7469  ounded_explanati
+00002a10: 6f6e 7320 3d20 6578 706c 6169 6e65 722e  ons = explainer.
+00002a20: 6578 706c 6169 6e5f 6661 6374 7561 6c28  explain_factual(
+00002a30: 585f 7465 7374 2c20 6c6f 775f 6869 6768  X_test, low_high
+00002a40: 5f70 6572 6365 6e74 696c 6573 3d28 352c  _percentiles=(5,
+00002a50: 6e70 2e69 6e66 2929 0d0a 6173 796d 6d65  np.inf))..asymme
+00002a60: 7472 6963 5f65 7870 6c61 6e61 7469 6f6e  tric_explanation
+00002a70: 7320 3d20 6578 706c 6169 6e65 722e 6578  s = explainer.ex
+00002a80: 706c 6169 6e5f 6661 6374 7561 6c28 585f  plain_factual(X_
+00002a90: 7465 7374 2c20 6c6f 775f 6869 6768 5f70  test, low_high_p
+00002aa0: 6572 6365 6e74 696c 6573 3d28 352c 3735  ercentiles=(5,75
+00002ab0: 2929 0d0a 6060 600d 0a0d 0a23 2323 2320  ))..```....#### 
+00002ac0: 436f 756e 7465 7266 6163 7475 616c 2045  Counterfactual E
+00002ad0: 7870 6c61 6e61 7469 6f6e 730d 0a54 6865  xplanations..The
+00002ae0: 2060 6578 706c 6169 6e5f 636f 756e 7465   `explain_counte
+00002af0: 7266 6163 7475 616c 6020 7769 6c6c 2077  rfactual` will w
+00002b00: 6f72 6b20 6578 6163 746c 7920 7468 6520  ork exactly the 
+00002b10: 7361 6d65 2061 7320 666f 7220 636c 6173  same as for clas
+00002b20: 7369 6669 6361 7469 6f6e 2e20 436f 756e  sification. Coun
+00002b30: 7465 7266 6163 7475 616c 2070 6c6f 7473  terfactual plots
+00002b40: 2077 6f72 6b20 696e 2074 6865 2073 616d   work in the sam
+00002b50: 6520 7761 7920 6173 2066 6f72 2063 6c61  e way as for cla
+00002b60: 7373 6966 6963 6174 696f 6e2e 0d0a 0d0a  ssification.....
+00002b70: 6060 6070 7974 686f 6e0d 0a63 6f75 6e74  ```python..count
+00002b80: 6572 6661 6374 7561 6c5f 6578 706c 616e  erfactual_explan
+00002b90: 6174 696f 6e73 203d 2065 7870 6c61 696e  ations = explain
+00002ba0: 6572 2e65 7870 6c61 696e 5f63 6f75 6e74  er.explain_count
+00002bb0: 6572 6661 6374 7561 6c28 585f 7465 7374  erfactual(X_test
+00002bc0: 290d 0a0d 0a63 6f75 6e74 6572 6661 6374  )....counterfact
+00002bd0: 7561 6c5f 6578 706c 616e 6174 696f 6e73  ual_explanations
+00002be0: 2e70 6c6f 745f 616c 6c28 290d 0a63 6f75  .plot_all()..cou
+00002bf0: 6e74 6572 6661 6374 7561 6c5f 6578 706c  nterfactual_expl
+00002c00: 616e 6174 696f 6e73 2e61 6464 5f63 6f6e  anations.add_con
+00002c10: 6a75 6e63 7469 6f6e 7328 292e 706c 6f74  junctions().plot
+00002c20: 5f61 6c6c 2829 0d0a 0d0a 636f 756e 7465  _all()....counte
+00002c30: 7266 6163 7475 616c 5f65 7870 6c61 6e61  rfactual_explana
+00002c40: 7469 6f6e 732e 706c 6f74 5f65 7870 6c61  tions.plot_expla
+00002c50: 6e61 7469 6f6e 2830 290d 0a60 6060 0d0a  nation(0)..```..
+00002c60: 5468 6520 7061 7261 6d65 7465 7220 606c  The parameter `l
+00002c70: 6f77 5f68 6967 685f 7065 7263 656e 7469  ow_high_percenti
+00002c80: 6c65 7360 2077 6f72 6b73 2069 6e20 7468  les` works in th
+00002c90: 6520 7361 6d65 2077 6179 2061 7320 666f  e same way as fo
+00002ca0: 7220 6661 6374 7561 6c20 6578 706c 616e  r factual explan
+00002cb0: 6174 696f 6e73 2e20 0d0a 0d0a 2323 2323  ations. ....####
+00002cc0: 2050 726f 6261 6269 6c69 7374 6963 2052   Probabilistic R
+00002cd0: 6567 7265 7373 696f 6e20 4578 706c 616e  egression Explan
+00002ce0: 6174 696f 6e73 0d0a 4974 2069 7320 706f  ations..It is po
+00002cf0: 7373 6962 6c65 2074 6f20 6372 6561 7465  ssible to create
+00002d00: 2070 726f 6261 6269 6c69 7374 6963 2065   probabilistic e
+00002d10: 7870 6c61 6e61 7469 6f6e 7320 666f 7220  xplanations for 
+00002d20: 7265 6772 6573 7369 6f6e 2c20 7072 6f76  regression, prov
+00002d30: 6964 696e 6720 7468 6520 7072 6f62 6162  iding the probab
+00002d40: 696c 6974 7920 7468 6174 2074 6865 2074  ility that the t
+00002d50: 6172 6765 7420 7661 6c75 6520 6973 2062  arget value is b
+00002d60: 656c 6f77 2074 6865 2070 726f 7669 6465  elow the provide
+00002d70: 6420 7468 7265 7368 6f6c 6420 2877 6869  d threshold (whi
+00002d80: 6368 2069 7320 3138 3020 3030 3020 696e  ch is 180 000 in
+00002d90: 2074 6865 2065 7861 6d70 6c65 7320 6265   the examples be
+00002da0: 6c6f 7729 2e20 416c 6c20 6d65 7468 6f64  low). All method
+00002db0: 7320 6172 6520 7468 6520 7361 6d65 2061  s are the same a
+00002dc0: 7320 666f 7220 6e6f 726d 616c 2072 6567  s for normal reg
+00002dd0: 7265 7373 696f 6e20 616e 6420 636c 6173  ression and clas
+00002de0: 7369 6669 6361 7469 6f6e 2c20 6578 6365  sification, exce
+00002df0: 7074 2074 6861 7420 7468 6520 6065 7870  pt that the `exp
+00002e00: 6c61 696e 5f66 6163 7475 616c 6020 616e  lain_factual` an
+00002e10: 6420 6065 7870 6c61 696e 5f63 6f75 6e74  d `explain_count
+00002e20: 6572 6661 6374 7561 6c60 206d 6574 686f  erfactual` metho
+00002e30: 6473 206e 6565 6420 7468 6520 6164 6469  ds need the addi
+00002e40: 7469 6f6e 616c 2074 6872 6573 686f 6c64  tional threshold
+00002e50: 2076 616c 7565 2028 6865 7265 2031 3830   value (here 180
+00002e60: 2030 3030 292e 0d0a 0d0a 6060 6070 7974   000).....```pyt
+00002e70: 686f 6e0d 0a66 6163 7475 616c 5f65 7870  hon..factual_exp
+00002e80: 6c61 6e61 7469 6f6e 7320 3d20 6578 706c  lanations = expl
+00002e90: 6169 6e65 722e 6578 706c 6169 6e5f 6661  ainer.explain_fa
+00002ea0: 6374 7561 6c28 585f 7465 7374 2c20 3138  ctual(X_test, 18
+00002eb0: 3030 3030 290d 0a0d 0a66 6163 7475 616c  0000)....factual
+00002ec0: 5f65 7870 6c61 6e61 7469 6f6e 732e 706c  _explanations.pl
+00002ed0: 6f74 5f61 6c6c 2829 0d0a 6661 6374 7561  ot_all()..factua
+00002ee0: 6c5f 6578 706c 616e 6174 696f 6e73 2e70  l_explanations.p
+00002ef0: 6c6f 745f 616c 6c28 756e 6365 7274 6169  lot_all(uncertai
+00002f00: 6e74 793d 5472 7565 290d 0a0d 0a66 6163  nty=True)....fac
+00002f10: 7475 616c 5f65 7870 6c61 6e61 7469 6f6e  tual_explanation
+00002f20: 732e 6164 645f 636f 6e6a 756e 6374 696f  s.add_conjunctio
+00002f30: 6e73 2829 2e70 6c6f 745f 616c 6c28 290d  ns().plot_all().
+00002f40: 0a0d 0a63 6f75 6e74 6572 6661 6374 7561  ...counterfactua
+00002f50: 6c5f 6578 706c 616e 6174 696f 6e73 203d  l_explanations =
+00002f60: 2065 7870 6c61 696e 6572 2e65 7870 6c61   explainer.expla
+00002f70: 696e 5f63 6f75 6e74 6572 6661 6374 7561  in_counterfactua
+00002f80: 6c28 585f 7465 7374 2c20 3138 3030 3030  l(X_test, 180000
+00002f90: 290d 0a0d 0a63 6f75 6e74 6572 6661 6374  )....counterfact
+00002fa0: 7561 6c5f 6578 706c 616e 6174 696f 6e73  ual_explanations
+00002fb0: 2e70 6c6f 745f 616c 6c28 290d 0a63 6f75  .plot_all()..cou
+00002fc0: 6e74 6572 6661 6374 7561 6c5f 6578 706c  nterfactual_expl
+00002fd0: 616e 6174 696f 6e73 2e61 6464 5f63 6f6e  anations.add_con
+00002fe0: 6a75 6e63 7469 6f6e 7328 292e 706c 6f74  junctions().plot
+00002ff0: 5f61 6c6c 2829 0d0a 6060 600d 0a0d 0a23  _all()..```....#
+00003000: 2323 2320 4164 6469 7469 6f6e 616c 2052  ### Additional R
+00003010: 6567 7265 7373 696f 6e20 5573 6520 4361  egression Use Ca
+00003020: 7365 730d 0a52 6567 7265 7373 696f 6e20  ses..Regression 
+00003030: 6f66 6665 7273 206d 616e 7920 6d6f 7265  offers many more
+00003040: 206f 7074 696f 6e73 2061 6e64 2074 6f20   options and to 
+00003050: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
+00003060: 2074 6865 6d2c 2073 6565 2074 6865 205b   them, see the [
+00003070: 6465 6d6f 5f72 6567 7265 7373 696f 6e5d  demo_regression]
+00003080: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003090: 636f 6d2f 4d6f 6666 7261 6e2f 6361 6c69  com/Moffran/cali
+000030a0: 6272 6174 6564 5f65 7870 6c61 6e61 7469  brated_explanati
+000030b0: 6f6e 732f 626c 6f62 2f6d 6169 6e2f 6e6f  ons/blob/main/no
+000030c0: 7465 626f 6f6b 732f 6465 6d6f 5f72 6567  tebooks/demo_reg
+000030d0: 7265 7373 696f 6e2e 6970 796e 6229 206f  ression.ipynb) o
+000030e0: 7220 7468 6520 5b64 656d 6f5f 7072 6f62  r the [demo_prob
+000030f0: 6162 696c 6973 7469 635f 7265 6772 6573  abilistic_regres
+00003100: 7369 6f6e 5d28 6874 7470 733a 2f2f 6769  sion](https://gi
+00003110: 7468 7562 2e63 6f6d 2f4d 6f66 6672 616e  thub.com/Moffran
+00003120: 2f63 616c 6962 7261 7465 645f 6578 706c  /calibrated_expl
+00003130: 616e 6174 696f 6e73 2f62 6c6f 622f 6d61  anations/blob/ma
+00003140: 696e 2f6e 6f74 6562 6f6f 6b73 2f64 656d  in/notebooks/dem
+00003150: 6f5f 7072 6f62 6162 696c 6973 7469 635f  o_probabilistic_
+00003160: 7265 6772 6573 7369 6f6e 2e69 7079 6e62  regression.ipynb
+00003170: 2920 6e6f 7465 626f 6f6b 732e 0d0a 0d0a  ) notebooks.....
+00003180: 5b54 6f70 5d28 2363 616c 6962 7261 7465  [Top](#calibrate
+00003190: 642d 6578 706c 616e 6174 696f 6e73 2d64  d-explanations-d
+000031a0: 6f63 756d 656e 7461 7469 6f6e 290d 0a0d  ocumentation)...
+000031b0: 0a4b 6e6f 776e 204c 696d 6974 6174 696f  .Known Limitatio
+000031c0: 6e73 0d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ns..------------
+000031d0: 2d2d 2d2d 2d0d 0a54 6865 2069 6d70 6c65  -----..The imple
+000031e0: 6d65 6e74 6174 696f 6e20 6375 7272 656e  mentation curren
+000031f0: 746c 7920 6f6e 6c79 2073 7570 706f 7274  tly only support
+00003200: 206e 756d 6572 6963 616c 2069 6e70 7574   numerical input
+00003210: 2e20 5573 6520 7468 6520 6075 7469 6c73  . Use the `utils
+00003220: 2e74 7261 6e73 666f 726d 5f74 6f5f 6e75  .transform_to_nu
+00003230: 6d65 7269 6360 2028 7265 6c65 6173 6564  meric` (released
+00003240: 2069 6e20 7665 7273 696f 6e20 7630 2e33   in version v0.3
+00003250: 2e31 2920 746f 2074 7261 6e73 666f 726d  .1) to transform
+00003260: 2061 2060 4461 7461 4672 616d 6560 2077   a `DataFrame` w
+00003270: 6974 6820 7465 7874 2064 6174 6120 696e  ith text data in
+00003280: 746f 206e 756d 6572 6963 616c 2066 6f72  to numerical for
+00003290: 6d20 616e 6420 6174 2074 6865 2073 616d  m and at the sam
+000032a0: 6520 7469 6d65 2065 7874 7261 6374 696e  e time extractin
+000032b0: 6720 6063 6174 6567 6f72 6963 616c 5f66  g `categorical_f
+000032c0: 6561 7475 7265 7360 2c20 6063 6174 6567  eatures`, `categ
+000032d0: 6f72 6963 616c 5f6c 6162 656c 7360 2c20  orical_labels`, 
+000032e0: 6074 6172 6765 745f 6c61 6265 6c73 6020  `target_labels` 
+000032f0: 2869 6620 7465 7874 206c 6162 656c 7329  (if text labels)
+00003300: 2061 6e64 2060 6d61 7070 696e 6773 6020   and `mappings` 
+00003310: 2875 7365 6420 746f 2061 7070 6c79 2074  (used to apply t
+00003320: 6865 2073 616d 6520 6d61 7070 696e 6773  he same mappings
+00003330: 2074 6f20 6e65 7720 6461 7461 2920 746f   to new data) to
+00003340: 2062 6520 7573 6564 2061 7320 696e 7075   be used as inpu
+00003350: 7420 746f 2074 6865 2060 4361 6c69 6272  t to the `Calibr
+00003360: 6174 6564 4578 706c 6169 6e65 7260 2e20  atedExplainer`. 
+00003370: 5468 6520 616c 676f 7269 7468 6d20 646f  The algorithm do
+00003380: 6573 206e 6f74 2063 7572 7265 6e74 6c79  es not currently
+00003390: 2073 7570 706f 7274 2069 6d61 6765 2064   support image d
+000033a0: 6174 612e 0d0a 0d0a 5b54 6f70 5d28 2363  ata.....[Top](#c
+000033b0: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
+000033c0: 6174 696f 6e73 2d64 6f63 756d 656e 7461  ations-documenta
+000033d0: 7469 6f6e 290d 0a0d 0a49 6e73 7461 6c6c  tion)....Install
+000033e0: 0d0a 2d2d 2d2d 2d2d 2d0d 0a0d 0a60 6361  ..-------....`ca
+000033f0: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
+00003400: 7469 6f6e 7360 2069 7320 696d 706c 656d  tions` is implem
+00003410: 656e 7465 6420 696e 2050 7974 686f 6e2c  ented in Python,
+00003420: 2073 6f20 796f 7520 6e65 6564 2061 2050   so you need a P
+00003430: 7974 686f 6e20 656e 7669 726f 6e6d 656e  ython environmen
+00003440: 742e 0d0a 0d0a 496e 7374 616c 6c20 6063  t.....Install `c
+00003450: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
+00003460: 6174 696f 6e73 6020 6672 6f6d 2050 7950  ations` from PyP
+00003470: 493a 0d0a 0d0a 0970 6970 2069 6e73 7461  I:.....pip insta
+00003480: 6c6c 2063 616c 6962 7261 7465 642d 6578  ll calibrated-ex
+00003490: 706c 616e 6174 696f 6e73 0d0a 0d0a 6f72  planations....or
+000034a0: 2066 726f 6d20 636f 6e64 612d 666f 7267   from conda-forg
+000034b0: 653a 0d0a 090d 0a20 0963 6f6e 6461 2069  e:..... .conda i
+000034c0: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
+000034d0: 666f 7267 6520 6361 6c69 6272 6174 6564  forge calibrated
+000034e0: 2d65 7870 6c61 6e61 7469 6f6e 730d 0a0d  -explanations...
+000034f0: 0a6f 7220 6279 2066 6f6c 6c6f 7769 6e67  .or by following
+00003500: 2066 7572 7468 6572 2069 6e73 7472 7563   further instruc
+00003510: 7469 6f6e 7320 6174 205b 636f 6e64 612d  tions at [conda-
+00003520: 666f 7267 655d 2868 7474 7073 3a2f 2f67  forge](https://g
+00003530: 6974 6875 622e 636f 6d2f 636f 6e64 612d  ithub.com/conda-
+00003540: 666f 7267 652f 6361 6c69 6272 6174 6564  forge/calibrated
+00003550: 2d65 7870 6c61 6e61 7469 6f6e 732d 6665  -explanations-fe
+00003560: 6564 7374 6f63 6b23 696e 7374 616c 6c69  edstock#installi
+00003570: 6e67 2d63 616c 6962 7261 7465 642d 6578  ng-calibrated-ex
+00003580: 706c 616e 6174 696f 6e73 292e 0d0a 0d0a  planations).....
+00003590: 5468 6520 6465 7065 6e64 656e 6369 6573  The dependencies
+000035a0: 2061 7265 3a0d 0a0d 0a2a 205b 6372 6570   are:....* [crep
+000035b0: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+000035c0: 7562 2e63 6f6d 2f68 656e 7269 6b62 6f73  ub.com/henrikbos
+000035d0: 7472 6f6d 2f63 7265 7065 7329 0d0a 2a20  trom/crepes)..* 
+000035e0: 5b76 656e 6e2d 6162 6572 735d 2868 7474  [venn-abers](htt
+000035f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003600: 6970 3230 302f 7665 6e6e 2d61 6265 7273  ip200/venn-abers
+00003610: 290d 0a2a 205b 6c69 6d65 5d28 6874 7470  )..* [lime](http
+00003620: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00003630: 6172 636f 7463 722f 6c69 6d65 290d 0a2a  arcotcr/lime)..*
+00003640: 205b 6d61 7470 6c6f 746c 6962 5d28 6874   [matplotlib](ht
+00003650: 7470 733a 2f2f 6d61 7470 6c6f 746c 6962  tps://matplotlib
+00003660: 2e6f 7267 2f29 0d0a 2a20 5b4e 756d 5079  .org/)..* [NumPy
+00003670: 5d28 6874 7470 733a 2f2f 6e75 6d70 792e  ](https://numpy.
+00003680: 6f72 672f 290d 0a20 200d 0a5b 546f 705d  org/)..  ..[Top]
+00003690: 2823 6361 6c69 6272 6174 6564 2d65 7870  (#calibrated-exp
+000036a0: 6c61 6e61 7469 6f6e 732d 646f 6375 6d65  lanations-docume
+000036b0: 6e74 6174 696f 6e29 0d0a 0d0a 0d0a 436f  ntation)......Co
+000036c0: 6e74 7269 6275 7469 6e67 0d0a 2d2d 2d2d  ntributing..----
+000036d0: 2d2d 2d2d 2d2d 2d2d 0d0a 0d0a 436f 6e74  --------....Cont
+000036e0: 7269 6275 7469 6f6e 7320 6172 6520 7765  ributions are we
+000036f0: 6c63 6f6d 652e 0d0a 506c 6561 7365 2073  lcome...Please s
+00003700: 656e 6420 6275 6720 7265 706f 7274 732c  end bug reports,
+00003710: 2066 6561 7475 7265 2072 6571 7565 7374   feature request
+00003720: 7320 6f72 2070 756c 6c20 7265 7175 6573  s or pull reques
+00003730: 7473 2074 6872 6f75 6768 0d0a 7468 6520  ts through..the 
+00003740: 7072 6f6a 6563 7420 7061 6765 206f 6e20  project page on 
+00003750: 5b47 6974 4875 625d 2868 7474 7073 3a2f  [GitHub](https:/
+00003760: 2f67 6974 6875 622e 636f 6d2f 4d6f 6666  /github.com/Moff
+00003770: 7261 6e2f 6361 6c69 6272 6174 6564 5f65  ran/calibrated_e
+00003780: 7870 6c61 6e61 7469 6f6e 7329 2e0d 0a59  xplanations)...Y
+00003790: 6f75 2063 616e 2066 696e 6420 6120 6465  ou can find a de
+000037a0: 7461 696c 6564 2067 7569 6465 2066 6f72  tailed guide for
+000037b0: 2063 6f6e 7472 6962 7574 696f 6e73 2069   contributions i
+000037c0: 6e0d 0a5b 434f 4e54 5249 4255 5449 4e47  n..[CONTRIBUTING
+000037d0: 2e6d 645d 2868 7474 7073 3a2f 2f67 6974  .md](https://git
+000037e0: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
+000037f0: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
+00003800: 6e61 7469 6f6e 732f 626c 6f62 2f6d 6169  nations/blob/mai
+00003810: 6e2f 434f 4e54 5249 4255 5449 4e47 2e6d  n/CONTRIBUTING.m
+00003820: 6429 2e0d 0a0d 0a5b 546f 705d 2823 6361  d).....[Top](#ca
+00003830: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
+00003840: 7469 6f6e 732d 646f 6375 6d65 6e74 6174  tions-documentat
+00003850: 696f 6e29 0d0a 0d0a 0d0a 446f 6375 6d65  ion)......Docume
+00003860: 6e74 6174 696f 6e0d 0a2d 2d2d 2d2d 2d2d  ntation..-------
+00003870: 2d2d 2d2d 2d2d 0d0a 466f 7220 646f 6375  ------..For docu
+00003880: 6d65 6e74 6174 696f 6e2c 2073 6565 205b  mentation, see [
+00003890: 6361 6c69 6272 6174 6564 2d65 7870 6c61  calibrated-expla
+000038a0: 6e61 7469 6f6e 732e 7265 6164 7468 6564  nations.readthed
+000038b0: 6f63 732e 696f 5d28 6874 7470 733a 2f2f  ocs.io](https://
+000038c0: 6361 6c69 6272 6174 6564 2d65 7870 6c61  calibrated-expla
+000038d0: 6e61 7469 6f6e 732e 7265 6164 7468 6564  nations.readthed
+000038e0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000038f0: 2f3f 6261 6467 653d 6c61 7465 7374 292e  /?badge=latest).
+00003900: 0d0a 2020 0d0a 5b54 6f70 5d28 2363 616c  ..  ..[Top](#cal
+00003910: 6962 7261 7465 642d 6578 706c 616e 6174  ibrated-explanat
+00003920: 696f 6e73 2d64 6f63 756d 656e 7461 7469  ions-documentati
+00003930: 6f6e 290d 0a0d 0a46 7572 7468 6572 2072  on)....Further r
+00003940: 6561 6469 6e67 2061 6e64 2063 6974 696e  eading and citin
+00003950: 670d 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  g..-------------
+00003960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a54  -------------..T
+00003970: 6865 2060 6361 6c69 6272 6174 6564 2d65  he `calibrated-e
+00003980: 7870 6c61 6e61 7469 6f6e 7360 206d 6574  xplanations` met
+00003990: 686f 6420 666f 7220 636c 6173 7369 6669  hod for classifi
+000039a0: 6361 7469 6f6e 2069 7320 696e 7472 6f64  cation is introd
+000039b0: 7563 6564 2069 6e20 7468 6520 7061 7065  uced in the pape
+000039c0: 723a 0d0a 0d0a 2d20 5b4c c3b6 6673 7472  r:....- [L..fstr
+000039d0: c3b6 6d2c 2048 5d28 6874 7470 733a 2f2f  ..m, H](https://
+000039e0: 6769 7468 7562 2e63 6f6d 2f4d 6f66 6672  github.com/Moffr
+000039f0: 616e 292e 2c20 5b4c c3b6 6673 7472 c3b6  an)., [L..fstr..
+00003a00: 6d2c 2054 5d28 6874 7470 733a 2f2f 6769  m, T](https://gi
+00003a10: 7468 7562 2e63 6f6d 2f74 7576 656c 6f66  thub.com/tuvelof
+00003a20: 7374 726f 6d29 2e2c 204a 6f68 616e 7373  strom)., Johanss
+00003a30: 6f6e 2c20 552e 2c20 616e 6420 53c3 b66e  on, U., and S..n
+00003a40: 7374 72c3 b664 2c20 432e 2028 3230 3234  str..d, C. (2024
+00003a50: 292e 205b 4361 6c69 6272 6174 6564 2045  ). [Calibrated E
+00003a60: 7870 6c61 6e61 7469 6f6e 733a 2077 6974  xplanations: wit
+00003a70: 6820 556e 6365 7274 6169 6e74 7920 496e  h Uncertainty In
+00003a80: 666f 726d 6174 696f 6e20 616e 6420 436f  formation and Co
+00003a90: 756e 7465 7266 6163 7475 616c 735d 2868  unterfactuals](h
+00003aa0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
+00003ab0: 302e 3130 3136 2f6a 2e65 7377 612e 3230  0.1016/j.eswa.20
+00003ac0: 3234 2e31 3233 3135 3429 2e20 4578 7065  24.123154). Expe
+00003ad0: 7274 2053 7973 7465 6d73 2077 6974 6820  rt Systems with 
+00003ae0: 4170 706c 6963 6174 696f 6e73 2c20 312d  Applications, 1-
+00003af0: 3237 2e0d 0a0d 0a54 6865 2065 7874 656e  27.....The exten
+00003b00: 7369 6f6e 7320 666f 7220 7265 6772 6573  sions for regres
+00003b10: 7369 6f6e 2061 7265 2069 6e74 726f 6475  sion are introdu
+00003b20: 6365 6420 696e 2074 6865 2070 6170 6572  ced in the paper
+00003b30: 3a0d 0a0d 0a2d 205b 4cc3 b666 7374 72c3  :....- [L..fstr.
+00003b40: b66d 2c20 545d 2868 7474 7073 3a2f 2f67  .m, T](https://g
+00003b50: 6974 6875 622e 636f 6d2f 7475 7665 6c6f  ithub.com/tuvelo
+00003b60: 6673 7472 6f6d 292e 2c20 5b4c c3b6 6673  fstrom)., [L..fs
+00003b70: 7472 c3b6 6d2c 2048 5d28 6874 7470 733a  tr..m, H](https:
+00003b80: 2f2f 6769 7468 7562 2e63 6f6d 2f4d 6f66  //github.com/Mof
+00003b90: 6672 616e 292e 2c20 4a6f 6861 6e73 736f  fran)., Johansso
+00003ba0: 6e2c 2055 2e2c 2053 c3b6 6e73 7472 c3b6  n, U., S..nstr..
+00003bb0: 642c 2043 2e2c 2061 6e64 205b 4d61 7465  d, C., and [Mate
+00003bc0: 6c61 2c20 525d 2868 7474 7073 3a2f 2f67  la, R](https://g
+00003bd0: 6974 6875 622e 636f 6d2f 7275 6479 6d61  ithub.com/rudyma
+00003be0: 7465 6c61 292e 205b 4361 6c69 6272 6174  tela). [Calibrat
+00003bf0: 6564 2045 7870 6c61 6e61 7469 6f6e 7320  ed Explanations 
+00003c00: 666f 7220 5265 6772 6573 7369 6f6e 5d28  for Regression](
+00003c10: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00003c20: 672f 6162 732f 3233 3038 2e31 3632 3435  g/abs/2308.16245
+00003c30: 292e 2061 7258 6976 2070 7265 7072 696e  ). arXiv preprin
+00003c40: 7420 6172 5869 763a 3233 3038 2e31 3632  t arXiv:2308.162
+00003c50: 3435 2e0d 0a0d 0a54 6865 2070 6170 6572  45.....The paper
+00003c60: 2074 6861 7420 6f72 6967 696e 6174 6564   that originated
+00003c70: 2074 6865 2069 6465 6120 6f66 2060 6361   the idea of `ca
+00003c80: 6c69 6272 6174 6564 2d65 7870 6c61 6e61  librated-explana
+00003c90: 7469 6f6e 7360 2069 733a 0d0a 0d0a 2d20  tions` is:....- 
+00003ca0: 5b4c c3b6 6673 7472 c3b6 6d2c 2048 2e5d  [L..fstr..m, H.]
+00003cb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00003cc0: 636f 6d2f 4d6f 6666 7261 6e29 2c20 5b4c  com/Moffran), [L
+00003cd0: c3b6 6673 7472 c3b6 6d2c 2054 2e5d 2868  ..fstr..m, T.](h
+00003ce0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003cf0: 6d2f 7475 7665 6c6f 6673 7472 6f6d 292c  m/tuvelofstrom),
+00003d00: 204a 6f68 616e 7373 6f6e 2c20 552e 2c20   Johansson, U., 
+00003d10: 2620 53c3 b66e 7374 72c3 b664 2c20 432e  & S..nstr..d, C.
+00003d20: 2028 3230 3233 292e 205b 496e 7665 7374   (2023). [Invest
+00003d30: 6967 6174 696e 6720 7468 6520 696d 7061  igating the impa
+00003d40: 6374 206f 6620 6361 6c69 6272 6174 696f  ct of calibratio
+00003d50: 6e20 6f6e 2074 6865 2071 7561 6c69 7479  n on the quality
+00003d60: 206f 6620 6578 706c 616e 6174 696f 6e73   of explanations
+00003d70: 5d28 6874 7470 733a 2f2f 6c69 6e6b 2e73  ](https://link.s
+00003d80: 7072 696e 6765 722e 636f 6d2f 6172 7469  pringer.com/arti
+00003d90: 636c 652f 3130 2e31 3030 372f 7331 3034  cle/10.1007/s104
+00003da0: 3732 2d30 3233 2d30 3938 3337 2d32 292e  72-023-09837-2).
+00003db0: 2041 6e6e 616c 7320 6f66 204d 6174 6865   Annals of Mathe
+00003dc0: 6d61 7469 6373 2061 6e64 2041 7274 6966  matics and Artif
+00003dd0: 6963 6961 6c20 496e 7465 6c6c 6967 656e  icial Intelligen
+00003de0: 6365 2c20 312d 3138 2e20 5b43 6f64 6520  ce, 1-18. [Code 
+00003df0: 616e 6420 7265 7375 6c74 735d 2868 7474  and results](htt
+00003e00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00003e10: 7475 7665 6c6f 6673 7472 6f6d 2f63 616c  tuvelofstrom/cal
+00003e20: 6962 7261 7469 6e67 2d65 7870 6c61 6e61  ibrating-explana
+00003e30: 7469 6f6e 7329 2e0d 0a0d 0a49 6620 796f  tions).....If yo
+00003e40: 7520 7573 6520 6063 616c 6962 7261 7465  u use `calibrate
+00003e50: 642d 6578 706c 616e 6174 696f 6e73 6020  d-explanations` 
+00003e60: 666f 7220 6120 7363 6965 6e74 6966 6963  for a scientific
+00003e70: 2070 7562 6c69 6361 7469 6f6e 2c20 796f   publication, yo
+00003e80: 7520 6172 6520 6b69 6e64 6c79 2072 6571  u are kindly req
+00003e90: 7565 7374 6564 2074 6f20 6369 7465 206f  uested to cite o
+00003ea0: 6e65 206f 6620 7468 6520 7061 7065 7273  ne of the papers
+00003eb0: 2061 626f 7665 2e0d 0a0d 0a42 6962 7465   above.....Bibte
+00003ec0: 7820 656e 7472 7920 666f 7220 7468 6520  x entry for the 
+00003ed0: 6f72 6967 696e 616c 2070 6170 6572 3a0d  original paper:.
+00003ee0: 0a0d 0a60 6060 6269 6274 6578 0d0a 4061  ...```bibtex..@a
+00003ef0: 7274 6963 6c65 7b6c 6f66 7374 726f 6d32  rticle{lofstrom2
+00003f00: 3032 3463 655f 636c 6173 7369 6669 6361  024ce_classifica
+00003f10: 7469 6f6e 2c0d 0a09 7469 746c 6520 3d20  tion,...title = 
+00003f20: 097b 4361 6c69 6272 6174 6564 2065 7870  .{Calibrated exp
+00003f30: 6c61 6e61 7469 6f6e 733a 2057 6974 6820  lanations: With 
+00003f40: 756e 6365 7274 6169 6e74 7920 696e 666f  uncertainty info
+00003f50: 726d 6174 696f 6e20 616e 6420 636f 756e  rmation and coun
+00003f60: 7465 7266 6163 7475 616c 737d 2c0d 0a09  terfactuals},...
+00003f70: 6a6f 7572 6e61 6c20 3d20 097b 4578 7065  journal = .{Expe
+00003f80: 7274 2053 7973 7465 6d73 2077 6974 6820  rt Systems with 
+00003f90: 4170 706c 6963 6174 696f 6e73 7d2c 0d0a  Applications},..
+00003fa0: 0970 6167 6573 203d 2009 7b31 3233 3135  .pages = .{12315
+00003fb0: 347d 2c0d 0a09 7965 6172 203d 2009 097b  4},...year = ..{
+00003fc0: 3230 3234 7d2c 0d0a 0969 7373 6e20 3d20  2024},...issn = 
+00003fd0: 0909 7b30 3935 372d 3431 3734 7d2c 0d0a  ..{0957-4174},..
+00003fe0: 0964 6f69 203d 2009 097b 6874 7470 733a  .doi = ..{https:
+00003ff0: 2f2f 646f 692e 6f72 672f 3130 2e31 3031  //doi.org/10.101
+00004000: 362f 6a2e 6573 7761 2e32 3032 342e 3132  6/j.eswa.2024.12
+00004010: 3331 3534 7d2c 0d0a 0975 726c 203d 2009  3154},...url = .
+00004020: 097b 6874 7470 733a 2f2f 7777 772e 7363  .{https://www.sc
+00004030: 6965 6e63 6564 6972 6563 742e 636f 6d2f  iencedirect.com/
+00004040: 7363 6965 6e63 652f 6172 7469 636c 652f  science/article/
+00004050: 7069 692f 5330 3935 3734 3137 3432 3430  pii/S09574174240
+00004060: 3030 3139 387d 2c0d 0a09 6175 7468 6f72  00198},...author
+00004070: 203d 2009 7b48 656c 656e 6120 4cc3 b666   = .{Helena L..f
+00004080: 7374 72c3 b66d 2061 6e64 2054 7577 6520  str..m and Tuwe 
+00004090: 4cc3 b666 7374 72c3 b66d 2061 6e64 2055  L..fstr..m and U
+000040a0: 6c66 204a 6f68 616e 7373 6f6e 2061 6e64  lf Johansson and
+000040b0: 2043 6563 696c 6961 2053 c3b6 6e73 7472   Cecilia S..nstr
+000040c0: c3b6 647d 2c0d 0a09 6b65 7977 6f72 6473  ..d},...keywords
+000040d0: 203d 2009 7b45 7870 6c61 696e 6162 6c65   = .{Explainable
+000040e0: 2041 492c 2046 6561 7475 7265 2069 6d70   AI, Feature imp
+000040f0: 6f72 7461 6e63 652c 2043 616c 6962 7261  ortance, Calibra
+00004100: 7465 6420 6578 706c 616e 6174 696f 6e73  ted explanations
+00004110: 2c20 5665 6e6e 2d41 6265 7273 2c20 556e  , Venn-Abers, Un
+00004120: 6365 7274 6169 6e74 7920 7175 616e 7469  certainty quanti
+00004130: 6669 6361 7469 6f6e 2c20 436f 756e 7465  fication, Counte
+00004140: 7266 6163 7475 616c 2065 7870 6c61 6e61  rfactual explana
+00004150: 7469 6f6e 737d 2c0d 0a09 6162 7374 7261  tions},...abstra
+00004160: 6374 203d 2009 7b57 6869 6c65 206c 6f63  ct = .{While loc
+00004170: 616c 2065 7870 6c61 6e61 7469 6f6e 7320  al explanations 
+00004180: 666f 7220 4149 206d 6f64 656c 7320 6361  for AI models ca
+00004190: 6e20 6f66 6665 7220 696e 7369 6768 7473  n offer insights
+000041a0: 2069 6e74 6f20 696e 6469 7669 6475 616c   into individual
+000041b0: 2070 7265 6469 6374 696f 6e73 2c20 7375   predictions, su
+000041c0: 6368 2061 7320 6665 6174 7572 6520 696d  ch as feature im
+000041d0: 706f 7274 616e 6365 2c20 7468 6579 2061  portance, they a
+000041e0: 7265 2070 6c61 6775 6564 2062 7920 6973  re plagued by is
+000041f0: 7375 6573 206c 696b 6520 696e 7374 6162  sues like instab
+00004200: 696c 6974 792e 2054 6865 2075 6e72 656c  ility. The unrel
+00004210: 6961 6269 6c69 7479 206f 6620 6665 6174  iability of feat
+00004220: 7572 6520 7765 6967 6874 732c 206f 6674  ure weights, oft
+00004230: 656e 2073 6b65 7765 6420 6475 6520 746f  en skewed due to
+00004240: 2070 6f6f 726c 7920 6361 6c69 6272 6174   poorly calibrat
+00004250: 6564 204d 4c20 6d6f 6465 6c73 2c20 6465  ed ML models, de
+00004260: 6570 656e 7320 7468 6573 6520 6368 616c  epens these chal
+00004270: 6c65 6e67 6573 2e20 4d6f 7265 6f76 6572  lenges. Moreover
+00004280: 2c20 7468 6520 6372 6974 6963 616c 2061  , the critical a
+00004290: 7370 6563 7420 6f66 2066 6561 7475 7265  spect of feature
+000042a0: 2069 6d70 6f72 7461 6e63 6520 756e 6365   importance unce
+000042b0: 7274 6169 6e74 7920 7265 6d61 696e 7320  rtainty remains 
+000042c0: 6d6f 7374 6c79 2075 6e61 6464 7265 7373  mostly unaddress
+000042d0: 6564 2069 6e20 4578 706c 6169 6e61 626c  ed in Explainabl
+000042e0: 6520 4149 2028 5841 4929 2e20 5468 6520  e AI (XAI). The 
+000042f0: 6e6f 7665 6c20 6665 6174 7572 6520 696d  novel feature im
+00004300: 706f 7274 616e 6365 2065 7870 6c61 6e61  portance explana
+00004310: 7469 6f6e 206d 6574 686f 6420 7072 6573  tion method pres
+00004320: 656e 7465 6420 696e 2074 6869 7320 7061  ented in this pa
+00004330: 7065 722c 2063 616c 6c65 6420 4361 6c69  per, called Cali
+00004340: 6272 6174 6564 2045 7870 6c61 6e61 7469  brated Explanati
+00004350: 6f6e 7320 2843 4529 2c20 6973 2064 6573  ons (CE), is des
+00004360: 6967 6e65 6420 746f 2074 6163 6b6c 6520  igned to tackle 
+00004370: 7468 6573 6520 6973 7375 6573 2068 6561  these issues hea
+00004380: 642d 6f6e 2e20 4275 696c 7420 6f6e 2074  d-on. Built on t
+00004390: 6865 2066 6f75 6e64 6174 696f 6e20 6f66  he foundation of
+000043a0: 2056 656e 6e2d 4162 6572 732c 2043 4520   Venn-Abers, CE 
+000043b0: 6e6f 7420 6f6e 6c79 2063 616c 6962 7261  not only calibra
+000043c0: 7465 7320 7468 6520 756e 6465 726c 7969  tes the underlyi
+000043d0: 6e67 206d 6f64 656c 2062 7574 2061 6c73  ng model but als
+000043e0: 6f20 6465 6c69 7665 7273 2072 656c 6961  o delivers relia
+000043f0: 626c 6520 6665 6174 7572 6520 696d 706f  ble feature impo
+00004400: 7274 616e 6365 2065 7870 6c61 6e61 7469  rtance explanati
+00004410: 6f6e 7320 7769 7468 2061 6e20 6578 6163  ons with an exac
+00004420: 7420 6465 6669 6e69 7469 6f6e 206f 6620  t definition of 
+00004430: 7468 6520 6665 6174 7572 6520 7765 6967  the feature weig
+00004440: 6874 732e 2043 4520 676f 6573 2062 6579  hts. CE goes bey
+00004450: 6f6e 6420 636f 6e76 656e 7469 6f6e 616c  ond conventional
+00004460: 2073 6f6c 7574 696f 6e73 2062 7920 6164   solutions by ad
+00004470: 6472 6573 7369 6e67 206f 7574 7075 7420  dressing output 
+00004480: 756e 6365 7274 6169 6e74 792e 2049 7420  uncertainty. It 
+00004490: 6163 636f 6d70 6c69 7368 6573 2074 6869  accomplishes thi
+000044a0: 7320 6279 2070 726f 7669 6469 6e67 2075  s by providing u
+000044b0: 6e63 6572 7461 696e 7479 2071 7561 6e74  ncertainty quant
+000044c0: 6966 6963 6174 696f 6e20 666f 7220 626f  ification for bo
+000044d0: 7468 2066 6561 7475 7265 2077 6569 6768  th feature weigh
+000044e0: 7473 2061 6e64 2074 6865 206d 6f64 656c  ts and the model
+000044f0: e280 9973 2070 726f 6261 6269 6c69 7479  ...s probability
+00004500: 2065 7374 696d 6174 6573 2e20 4164 6469   estimates. Addi
+00004510: 7469 6f6e 616c 6c79 2c20 4345 2069 7320  tionally, CE is 
+00004520: 6d6f 6465 6c2d 6167 6e6f 7374 6963 2c20  model-agnostic, 
+00004530: 6665 6174 7572 696e 6720 6561 7369 6c79  featuring easily
+00004540: 2063 6f6d 7072 6568 656e 7369 626c 6520   comprehensible 
+00004550: 636f 6e64 6974 696f 6e61 6c20 7275 6c65  conditional rule
+00004560: 7320 616e 6420 7468 6520 6162 696c 6974  s and the abilit
+00004570: 7920 746f 2067 656e 6572 6174 6520 636f  y to generate co
+00004580: 756e 7465 7266 6163 7475 616c 2065 7870  unterfactual exp
+00004590: 6c61 6e61 7469 6f6e 7320 7769 7468 2065  lanations with e
+000045a0: 6d62 6564 6465 6420 756e 6365 7274 6169  mbedded uncertai
+000045b0: 6e74 7920 7175 616e 7469 6669 6361 7469  nty quantificati
+000045c0: 6f6e 2e20 5265 7375 6c74 7320 6672 6f6d  on. Results from
+000045d0: 2061 6e20 6576 616c 7561 7469 6f6e 2077   an evaluation w
+000045e0: 6974 6820 3235 2062 656e 6368 6d61 726b  ith 25 benchmark
+000045f0: 2064 6174 6173 6574 7320 756e 6465 7273   datasets unders
+00004600: 636f 7265 2074 6865 2065 6666 6963 6163  core the efficac
+00004610: 7920 6f66 2043 452c 206d 616b 696e 6720  y of CE, making 
+00004620: 6974 2073 7461 6e64 2061 7320 6120 6661  it stand as a fa
+00004630: 7374 2c20 7265 6c69 6162 6c65 2c20 7374  st, reliable, st
+00004640: 6162 6c65 2c20 616e 6420 726f 6275 7374  able, and robust
+00004650: 2073 6f6c 7574 696f 6e2e 7d0d 0a7d 0d0a   solution.}..}..
+00004660: 6060 600d 0a42 6962 7465 7820 656e 7472  ```..Bibtex entr
+00004670: 7920 666f 7220 7468 6520 7265 6772 6573  y for the regres
+00004680: 7369 6f6e 2070 6170 6572 3a0d 0a0d 0a60  sion paper:....`
+00004690: 6060 6269 6274 6578 0d0a 406d 6973 637b  ``bibtex..@misc{
+000046a0: 6c6f 6673 7472 6f6d 3230 3233 6365 5f72  lofstrom2023ce_r
+000046b0: 6567 7265 7373 696f 6e2c 0d0a 2020 2020  egression,..    
+000046c0: 2020 7469 746c 6520 3d20 0920 2020 2020    title = .     
+000046d0: 2009 7b43 616c 6962 7261 7465 6420 4578   .{Calibrated Ex
+000046e0: 706c 616e 6174 696f 6e73 2066 6f72 2052  planations for R
+000046f0: 6567 7265 7373 696f 6e7d 2c0d 0a20 2020  egression},..   
+00004700: 2020 2061 7574 686f 7220 3d20 2020 2020     author =     
+00004710: 2020 2020 207b 4c5c 226f 6673 7472 5c22       {L\"ofstr\"
+00004720: 6f6d 2c20 5475 7765 2061 6e64 204c 5c22  om, Tuwe and L\"
+00004730: 6f66 7374 725c 226f 6d2c 2048 656c 656e  ofstr\"om, Helen
+00004740: 6120 616e 6420 4a6f 6861 6e73 736f 6e2c  a and Johansson,
+00004750: 2055 6c66 2061 6e64 2053 5c22 6f6e 7374   Ulf and S\"onst
+00004760: 725c 226f 642c 2043 6563 696c 6961 2061  r\"od, Cecilia a
+00004770: 6e64 204d 6174 656c 612c 2052 7564 797d  nd Matela, Rudy}
+00004780: 2c0d 0a20 2020 2020 2079 6561 7220 3d20  ,..      year = 
+00004790: 2020 2020 2020 2020 2020 207b 3230 3233             {2023
+000047a0: 7d2c 0d0a 2020 2020 2020 6570 7269 6e74  },..      eprint
+000047b0: 203d 2020 2020 2020 2020 2020 7b32 3330   =          {230
+000047c0: 382e 3136 3234 357d 2c0d 0a20 2020 2020  8.16245},..     
+000047d0: 2061 7263 6869 7665 5072 6566 6978 203d   archivePrefix =
+000047e0: 2020 207b 6172 5869 767d 2c0d 0a20 2020     {arXiv},..   
+000047f0: 2020 2070 7269 6d61 7279 436c 6173 7320     primaryClass 
+00004800: 3d20 2020 207b 6373 2e4c 477d 0d0a 7d0d  =    {cs.LG}..}.
+00004810: 0a60 6060 0d0a 0d0a 546f 2063 6974 6520  .```....To cite 
+00004820: 7468 6973 2073 6f66 7477 6172 652c 2075  this software, u
+00004830: 7365 2074 6865 2066 6f6c 6c6f 7769 6e67  se the following
+00004840: 2062 6962 7465 7820 656e 7472 793a 0d0a   bibtex entry:..
+00004850: 0d0a 6060 6062 6962 7465 780d 0a40 736f  ..```bibtex..@so
+00004860: 6674 7761 7265 7b6c 6f66 7374 726f 6d32  ftware{lofstrom2
+00004870: 3032 3463 655f 7265 706f 7369 746f 7279  024ce_repository
+00004880: 2c0d 0a09 6175 7468 6f72 203d 2009 7b4c  ,...author = .{L
+00004890: c3b6 6673 7472 c3b6 6d2c 2048 656c 656e  ..fstr..m, Helen
+000048a0: 6120 616e 6420 4cc3 b666 7374 72c3 b66d  a and L..fstr..m
+000048b0: 2c20 5475 7765 2061 6e64 204a 6f68 616e  , Tuwe and Johan
+000048c0: 7373 6f6e 2c20 556c 6620 616e 6420 53c3  sson, Ulf and S.
+000048d0: b66e 7374 72c3 b664 2c20 4365 6369 6c69  .nstr..d, Cecili
+000048e0: 6120 616e 6420 4d61 7465 6c61 2c20 5275  a and Matela, Ru
+000048f0: 6479 7d2c 0d0a 096c 6963 656e 7365 203d  dy},...license =
+00004900: 2009 7b42 5344 2d33 2d43 6c61 7573 657d   .{BSD-3-Clause}
+00004910: 2c0d 0a09 7469 746c 6520 3d20 097b 4361  ,...title = .{Ca
+00004920: 6c69 6272 6174 6564 2045 7870 6c61 6e61  librated Explana
+00004930: 7469 6f6e 737d 2c0d 0a09 7572 6c20 3d20  tions},...url = 
+00004940: 0909 7b68 7474 7073 3a2f 2f67 6974 6875  ..{https://githu
+00004950: 622e 636f 6d2f 4d6f 6666 7261 6e2f 6361  b.com/Moffran/ca
+00004960: 6c69 6272 6174 6564 5f65 7870 6c61 6e61  librated_explana
+00004970: 7469 6f6e 737d 2c0d 0a09 7665 7273 696f  tions},...versio
+00004980: 6e20 3d20 097b 7630 2e33 2e33 7d2c 0d0a  n = .{v0.3.3},..
+00004990: 096d 6f6e 7468 203d 2009 4d61 792c 0d0a  .month = .May,..
+000049a0: 0979 6561 7220 3d20 0909 7b32 3032 347d  .year = ..{2024}
+000049b0: 0d0a 7d0d 0a60 6060 0d0a 2020 0d0a 5b54  ..}..```..  ..[T
+000049c0: 6f70 5d28 2363 616c 6962 7261 7465 642d  op](#calibrated-
+000049d0: 6578 706c 616e 6174 696f 6e73 2d64 6f63  explanations-doc
+000049e0: 756d 656e 7461 7469 6f6e 290d 0a0d 0a41  umentation)....A
+000049f0: 636b 6e6f 776c 6564 6765 6d65 6e74 730d  cknowledgements.
+00004a00: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00004a10: 2d0d 0a54 6869 7320 7265 7365 6172 6368  -..This research
+00004a20: 2069 7320 6675 6e64 6564 2062 7920 7468   is funded by th
+00004a30: 6520 5377 6564 6973 6820 4b6e 6f77 6c65  e Swedish Knowle
+00004a40: 6467 6520 466f 756e 6461 7469 6f6e 2074  dge Foundation t
+00004a50: 6f67 6574 6865 7220 7769 7468 2069 6e64  ogether with ind
+00004a60: 7573 7472 6961 6c20 7061 7274 6e65 7273  ustrial partners
+00004a70: 2073 7570 706f 7274 696e 6720 7468 6520   supporting the 
+00004a80: 7265 7365 6172 6368 2061 6e64 2065 6475  research and edu
+00004a90: 6361 7469 6f6e 2065 6e76 6972 6f6e 6d65  cation environme
+00004aa0: 6e74 206f 6e20 4b6e 6f77 6c65 6467 6520  nt on Knowledge 
+00004ab0: 496e 7465 6e73 6976 6520 5072 6f64 7563  Intensive Produc
+00004ac0: 7420 5265 616c 697a 6174 696f 6e20 5350  t Realization SP
+00004ad0: 4152 4b20 6174 204a c3b6 6e6b c3b6 7069  ARK at J..nk..pi
+00004ae0: 6e67 2055 6e69 7665 7273 6974 792c 2053  ng University, S
+00004af0: 7765 6465 6e2c 2074 6872 6f75 6768 2070  weden, through p
+00004b00: 726f 6a65 6374 733a 2041 4641 4952 2067  rojects: AFAIR g
+00004b10: 7261 6e74 206e 6f2e 2032 3032 3030 3232  rant no. 2020022
+00004b20: 3320 616e 6420 5052 454d 4143 4f50 2067  3 and PREMACOP g
+00004b30: 7261 6e74 206e 6f2e 2032 3032 3230 3138  rant no. 2022018
+00004b40: 372e 2048 656c 656e 6120 4cc3 b666 7374  7. Helena L..fst
+00004b50: 72c3 b66d 2077 6173 2061 2050 6844 2073  r..m was a PhD s
+00004b60: 7475 6465 6e74 2069 6e20 7468 6520 496e  tudent in the In
+00004b70: 6475 7374 7269 616c 2047 7261 6475 6174  dustrial Graduat
+00004b80: 6520 5363 686f 6f6c 2069 6e20 4469 6769  e School in Digi
+00004b90: 7461 6c20 5265 7461 696c 696e 6720 2849  tal Retailing (I
+00004ba0: 4e53 6944 5229 2061 7420 7468 6520 556e  NSiDR) at the Un
+00004bb0: 6976 6572 7369 7479 206f 6620 426f 72c3  iversity of Bor.
+00004bc0: a573 2c20 6675 6e64 6564 2062 7920 7468  .s, funded by th
+00004bd0: 6520 5377 6564 6973 6820 4b6e 6f77 6c65  e Swedish Knowle
+00004be0: 6467 6520 466f 756e 6461 7469 6f6e 2c20  dge Foundation, 
+00004bf0: 6772 616e 7420 6e6f 2e20 3230 3136 3030  grant no. 201600
+00004c00: 3335 2e20 0d0a 0d0a 5b52 7564 7920 4d61  35. ....[Rudy Ma
+00004c10: 7465 6c61 5d28 6874 7470 733a 2f2f 6769  tela](https://gi
+00004c20: 7468 7562 2e63 6f6d 2f72 7564 796d 6174  thub.com/rudymat
+00004c30: 656c 6129 2068 6173 2062 6565 6e20 6f75  ela) has been ou
+00004c40: 7220 6769 7420 6775 7275 2061 6e64 2068  r git guru and h
+00004c50: 6173 2068 656c 7065 6420 7573 2077 6974  as helped us wit
+00004c60: 6820 7468 6520 7265 6c65 6173 6520 7072  h the release pr
+00004c70: 6f63 6573 732e 0d0a 0d0a 5765 2068 6176  ocess.....We hav
+00004c80: 6520 7573 6564 2062 6f74 6820 7468 6520  e used both the 
+00004c90: 6043 6f6e 666f 726d 616c 5072 6564 6963  `ConformalPredic
+00004ca0: 7469 7665 5379 7374 656d 6020 616e 6420  tiveSystem` and 
+00004cb0: 6044 6966 6669 6375 6c74 7945 7374 696d  `DifficultyEstim
+00004cc0: 6174 6f72 6020 636c 6173 7365 7320 6672  ator` classes fr
+00004cd0: 6f6d 205b 4865 6e72 696b 2042 6f73 7472  om [Henrik Bostr
+00004ce0: c3b6 6d5d 2868 7474 7073 3a2f 2f67 6974  ..m](https://git
+00004cf0: 6875 622e 636f 6d2f 6865 6e72 696b 626f  hub.com/henrikbo
+00004d00: 7374 726f 6d29 7320 5b63 7265 7065 735d  strom)s [crepes]
+00004d10: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004d20: 636f 6d2f 6865 6e72 696b 626f 7374 726f  com/henrikbostro
+00004d30: 6d2f 6372 6570 6573 2920 7061 636b 6167  m/crepes) packag
+00004d40: 6520 746f 2070 726f 7669 6465 2073 7570  e to provide sup
+00004d50: 706f 7274 2066 6f72 2072 6567 7265 7373  port for regress
+00004d60: 696f 6e2e 0d0a 0d0a 5765 2068 6176 6520  ion.....We have 
+00004d70: 7573 6564 2074 6865 2060 5665 6e6e 4162  used the `VennAb
+00004d80: 6572 7360 2063 6c61 7373 2066 726f 6d20  ers` class from 
+00004d90: 5b49 7661 6e20 5065 7465 6a5d 2868 7474  [Ivan Petej](htt
+00004da0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004db0: 6970 3230 3029 7320 5b76 656e 6e2d 6162  ip200)s [venn-ab
+00004dc0: 6572 735d 2868 7474 7073 3a2f 2f67 6974  ers](https://git
+00004dd0: 6875 622e 636f 6d2f 6970 3230 302f 7665  hub.com/ip200/ve
+00004de0: 6e6e 2d61 6265 7273 2920 7061 636b 6167  nn-abers) packag
+00004df0: 6520 746f 2070 726f 7669 6465 2073 7570  e to provide sup
+00004e00: 706f 7274 2066 6f72 2070 726f 6261 6269  port for probabi
+00004e10: 6c69 7374 6963 2065 7870 6c61 6e61 7469  listic explanati
+00004e20: 6f6e 7320 2862 6f74 6820 636c 6173 7369  ons (both classi
+00004e30: 6669 6361 7469 6f6e 2061 6e64 2070 726f  fication and pro
+00004e40: 6261 6269 6c69 7374 6963 2072 6567 7265  babilistic regre
+00004e50: 7373 696f 6e29 2e20 0d0a 0d0a 5765 2068  ssion). ....We h
+00004e60: 6176 6520 7573 6564 2063 6f64 6520 6672  ave used code fr
+00004e70: 6f6d 205b 4d61 7263 6f20 5475 6c69 6f20  om [Marco Tulio 
+00004e80: 436f 7272 6569 6120 5269 6265 6972 6f5d  Correia Ribeiro]
+00004e90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004ea0: 636f 6d2f 6d61 7263 6f74 6372 2973 205b  com/marcotcr)s [
+00004eb0: 6c69 6d65 5d28 6874 7470 733a 2f2f 6769  lime](https://gi
+00004ec0: 7468 7562 2e63 6f6d 2f6d 6172 636f 7463  thub.com/marcotc
+00004ed0: 722f 6c69 6d65 2920 7061 636b 6167 6520  r/lime) package 
+00004ee0: 666f 7220 7468 6520 6044 6973 6372 6574  for the `Discret
+00004ef0: 697a 6572 6020 636c 6173 732e 0d0a 0d0a  izer` class.....
+00004f00: 5468 6520 6063 6865 636b 5f69 735f 6669  The `check_is_fi
+00004f10: 7474 6564 6020 616e 6420 6073 6166 655f  tted` and `safe_
+00004f20: 696e 7374 616e 6365 6020 6675 6e63 7469  instance` functi
+00004f30: 6f6e 7320 696e 2060 6361 6c69 6272 6174  ons in `calibrat
+00004f40: 6564 5f65 7870 6c61 6e61 7469 6f6e 732e  ed_explanations.
+00004f50: 7574 696c 7360 2061 7265 2063 6f70 6965  utils` are copie
+00004f60: 6420 6672 6f6d 2060 736b 6c65 6172 6e60  d from `sklearn`
+00004f70: 2061 6e64 2060 7368 6170 602e 2020 0d0a   and `shap`.  ..
+00004f80: 2020 0d0a 5b54 6f70 5d28 2363 616c 6962    ..[Top](#calib
+00004f90: 7261 7465 642d 6578 706c 616e 6174 696f  rated-explanatio
+00004fa0: 6e73 2d64 6f63 756d 656e 7461 7469 6f6e  ns-documentation
+00004fb0: 290d 0a0d 0a5b 6275 696c 642d 6c6f 675d  )....[build-log]
+00004fc0: 3a20 2020 2068 7474 7073 3a2f 2f67 6974  :    https://git
+00004fd0: 6875 622e 636f 6d2f 4d6f 6666 7261 6e2f  hub.com/Moffran/
+00004fe0: 6361 6c69 6272 6174 6564 5f65 7870 6c61  calibrated_expla
+00004ff0: 6e61 7469 6f6e 732f 6163 7469 6f6e 732f  nations/actions/
+00005000: 776f 726b 666c 6f77 732f 7465 7374 2e79  workflows/test.y
+00005010: 6d6c 0d0a 5b62 7569 6c64 2d73 7461 7475  ml..[build-statu
+00005020: 735d 3a20 6874 7470 733a 2f2f 6769 7468  s]: https://gith
+00005030: 7562 2e63 6f6d 2f4d 6f66 6672 616e 2f63  ub.com/Moffran/c
+00005040: 616c 6962 7261 7465 645f 6578 706c 616e  alibrated_explan
+00005050: 6174 696f 6e73 2f61 6374 696f 6e73 2f77  ations/actions/w
+00005060: 6f72 6b66 6c6f 7773 2f74 6573 742e 796d  orkflows/test.ym
+00005070: 6c2f 6261 6467 652e 7376 670d 0a5b 6c69  l/badge.svg..[li
+00005080: 6e74 2d6c 6f67 5d3a 2020 2020 6874 7470  nt-log]:    http
+00005090: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
+000050a0: 6f66 6672 616e 2f63 616c 6962 7261 7465  offran/calibrate
+000050b0: 645f 6578 706c 616e 6174 696f 6e73 2f61  d_explanations/a
+000050c0: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+000050d0: 2f70 796c 696e 742e 796d 6c0d 0a5b 6c69  /pylint.yml..[li
+000050e0: 6e74 2d73 7461 7475 735d 3a20 6874 7470  nt-status]: http
+000050f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4d  s://github.com/M
+00005100: 6f66 6672 616e 2f63 616c 6962 7261 7465  offran/calibrate
+00005110: 645f 6578 706c 616e 6174 696f 6e73 2f61  d_explanations/a
+00005120: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00005130: 2f70 796c 696e 742e 796d 6c2f 6261 6467  /pylint.yml/badg
+00005140: 652e 7376 670d 0a5b 7079 7069 2d76 6572  e.svg..[pypi-ver
+00005150: 7369 6f6e 5d3a 2068 7474 7073 3a2f 2f69  sion]: https://i
+00005160: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00005170: 7069 2f76 2f63 616c 6962 7261 7465 642d  pi/v/calibrated-
+00005180: 6578 706c 616e 6174 696f 6e73 0d0a 5b63  explanations..[c
+00005190: 616c 6962 7261 7465 642d 6578 706c 616e  alibrated-explan
+000051a0: 6174 696f 6e73 2d6f 6e2d 7079 7069 5d3a  ations-on-pypi]:
+000051b0: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
+000051c0: 672f 7072 6f6a 6563 742f 6361 6c69 6272  g/project/calibr
+000051d0: 6174 6564 2d65 7870 6c61 6e61 7469 6f6e  ated-explanation
+000051e0: 730d 0a                                  s..
```

### Comparing `calibrated_explanations-0.3.2/README.md` & `calibrated_explanations-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,82 @@
+Metadata-Version: 2.1
+Name: calibrated_explanations
+Version: 0.3.3
+Summary: Extract calibrated explanations from machine learning models.
+Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
+Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
+Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: crepes
+Requires-Dist: venn-abers
+Requires-Dist: ipython
+Requires-Dist: lime
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
+
 Calibrated Explanations ([Documentation](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest))
 =======================
 
 [![Calibrated Explanations PyPI version][pypi-version]][calibrated-explanations-on-pypi]
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/calibrated-explanations.svg)](https://anaconda.org/conda-forge/calibrated-explanations)
 [![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Moffran/calibrated_explanations)](https://github.com/Moffran/calibrated_explanations/blob/main/CHANGELOG.md)
 [![Documentation Status](https://readthedocs.org/projects/calibrated-explanations/badge/?version=latest)](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 [![Lint Status for Calibrated Explanations][lint-status]][lint-log]
 [![License](https://badgen.net/github/license/moffran/calibrated_explanations)](https://github.com/moffran/calibrated_explanations/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/calibrated-explanations)](https://pepy.tech/project/calibrated-explanations)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.2)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.3)
 
-`calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both classification and regression.
+`calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both [classification](https://doi.org/10.1016/j.eswa.2024.123154) and [regression](https://arxiv.org/abs/2308.16245).
 The proposed method is based on Venn-Abers (classification & regression) and Conformal Predictive Systems (regression) and has the following characteristics:
-* Fast, reliable, stable and robust feature importance explanations.
+* Fast, reliable, stable and robust feature importance explanations for:
+	- Binary classification models
+	- Multi-class classification models
+	- Regression models
+		* Including probabilistic explanations of the probability that the target exceeds a user-defined threshold 
+		* With difficulty adaptable explanations (conformal normalization) 
 * Calibration of the underlying model to ensure that predictions reflect reality.
 * Uncertainty quantification of the prediction from the underlying model and the feature importance weights. 
-* Rules with straightforward interpretation in relation to the feature weights.
+* Rules with straightforward interpretation in relation to instance values and feature weights.
 * Possibility to generate counterfactual rules with uncertainty quantification of the expected predictions.
-* Conjunctional rules conveying joint contribution between features.
+* Conjunctional rules conveying feature importance for the interaction of included features.
+* Conditional rules, allowing users the ability to create contextual explanations to handle e.g. bias and fairness constraints. 
 
-Below is an example of a probabilistic counterfactual explanation for an instance of the California Housing dataset (with the threshold 180 000). The light red area in the background is representing the calibrated probability interval (for the prediction being below the threshold) of the underlying model, as indicated by a Conformal Predictive System and calibrated through Venn-Abers. The darker red bars for each rule show the probability intervals that Venn-Abers indicate for an instance changing a feature value in accordance with the rule condition.
+Below is an example of a probabilistic counterfactual explanation for an instance of the regression dataset California Housing (with the threshold 180 000). The light red area in the background is representing the calibrated probability interval (for the prediction being below the threshold) of the underlying model, as indicated by a Conformal Predictive System and calibrated through Venn-Abers. The darker red bars for each rule show the probability intervals that Venn-Abers indicate for an instance changing a feature value in accordance with the rule condition.
+<p align="center">
+  <a href="https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest">
+    <img src="https://github.com/Moffran/calibrated_explanations/blob/main/docs/images/counterfactual_probabilistic_house_regression.jpg" alt="Probabilistic counterfactual explanation for California Housing">
+  </a>
+</p>
+
+Table 1 summarizes the characteristics of Calibrated Explanations.
+<p align="center">
+  <a href="https://arxiv.org/abs/2308.16245">
+    <img src="https://github.com/Moffran/calibrated_explanations/blob/main/docs/images/Table1.png" alt="Characteristics of Calibrated Explanantions">
+  </a>
+</p>
 
-[![Probabilistic counterfactual explanation for California Housing](https://github.com/Moffran/calibrated_explanations/blob/main/docs/images/counterfactual_probabilistic_house_regression.jpg "Probabilistic counterfactual explanation for California Housing")](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
- 
 Getting started
 ---------------
 The [notebooks folder](https://github.com/Moffran/calibrated_explanations/tree/main/notebooks) contains a number of notebooks illustrating different use cases for `calibrated-explanations`. The following are commented and should be a good start:
-* [quickstart](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/quickstart.ipynb)  - similar to this Getting Started, including plots.
+* [quickstart](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/quickstart.ipynb) - similar to this Getting Started, including plots.
 * [quickstart_wrap](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/quickstart_wrap.ipynb) - similar to this Getting Started, but with a wrapper class for easier use.
-* [demo_binary_classification](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_binary_classification.ipynb) 
-* [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb)
-* [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb)
+* [demo_binary_classification](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_binary_classification.ipynb) - with examples for binary classification 
+* [demo_multiclass](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_multiclass_glass.ipynb) - with examples for multi-class classification
+* [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) - with examples for regression
+* [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) - with examples for regression with thresholds
+* [demo_under_the_hood](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_under_the_hood.ipynb) - illustrating how to access the information composing the explanations
 
 ### Classification
 Let us illustrate how we may use `calibrated-explanations` to generate explanations from a classifier trained on a dataset from
 [www.openml.org](https://www.openml.org), which we first split into a
 training and a test set using `train_test_split` from
 [sklearn](https://scikit-learn.org), and then further split the
 training set into a proper training set and a calibration set:
@@ -111,15 +152,15 @@
 Individual explanations can also be plotted using `plot_explanation`.
       
 ```python
 factual_explanations.get_explanation(0).plot_explanation()
 counterfactual_explanations.get_explanation(0).plot_explanation()
 ```
 #### Support for multiclass
-`calibrated-explanations` supports multiclass which is demonstrated in [demo_multiclass](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_multiclass.ipynb). That notebook also demonstrates how both feature names and target and categorical labels can be added to improve the interpretability. 
+`calibrated-explanations` supports multiclass which is demonstrated in [demo_multiclass](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_multiclass_glass.ipynb). That notebook also demonstrates how both feature names and target and categorical labels can be added to improve the interpretability. 
 
 ### Regression
 Extracting explanations for regression is very similar to how it is done for classification. 
 
 ```python
 dataset = fetch_openml(name="house_sales", version=3)
 
@@ -196,15 +237,15 @@
 #### Additional Regression Use Cases
 Regression offers many more options and to learn more about them, see the [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) or the [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) notebooks.
 
 [Top](#calibrated-explanations-documentation)
 
 Known Limitations
 -----------------
-The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.2) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
+The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.1) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
 
 [Top](#calibrated-explanations-documentation)
 
 Install
 -------
 
 `calibrated-explanations` is implemented in Python, so you need a Python environment.
@@ -263,15 +304,15 @@
 - [Löfström, H.](https://github.com/Moffran), [Löfström, T.](https://github.com/tuvelofstrom), Johansson, U., & Sönströd, C. (2023). [Investigating the impact of calibration on the quality of explanations](https://link.springer.com/article/10.1007/s10472-023-09837-2). Annals of Mathematics and Artificial Intelligence, 1-18. [Code and results](https://github.com/tuvelofstrom/calibrating-explanations).
 
 If you use `calibrated-explanations` for a scientific publication, you are kindly requested to cite one of the papers above.
 
 Bibtex entry for the original paper:
 
 ```bibtex
-@article{lofstrom2024calibrated,
+@article{lofstrom2024ce_classification,
 	title = 	{Calibrated explanations: With uncertainty information and counterfactuals},
 	journal = 	{Expert Systems with Applications},
 	pages = 	{123154},
 	year = 		{2024},
 	issn = 		{0957-4174},
 	doi = 		{https://doi.org/10.1016/j.eswa.2024.123154},
 	url = 		{https://www.sciencedirect.com/science/article/pii/S0957417424000198},
@@ -279,34 +320,34 @@
 	keywords = 	{Explainable AI, Feature importance, Calibrated explanations, Venn-Abers, Uncertainty quantification, Counterfactual explanations},
 	abstract = 	{While local explanations for AI models can offer insights into individual predictions, such as feature importance, they are plagued by issues like instability. The unreliability of feature weights, often skewed due to poorly calibrated ML models, deepens these challenges. Moreover, the critical aspect of feature importance uncertainty remains mostly unaddressed in Explainable AI (XAI). The novel feature importance explanation method presented in this paper, called Calibrated Explanations (CE), is designed to tackle these issues head-on. Built on the foundation of Venn-Abers, CE not only calibrates the underlying model but also delivers reliable feature importance explanations with an exact definition of the feature weights. CE goes beyond conventional solutions by addressing output uncertainty. It accomplishes this by providing uncertainty quantification for both feature weights and the model’s probability estimates. Additionally, CE is model-agnostic, featuring easily comprehensible conditional rules and the ability to generate counterfactual explanations with embedded uncertainty quantification. Results from an evaluation with 25 benchmark datasets underscore the efficacy of CE, making it stand as a fast, reliable, stable, and robust solution.}
 }
 ```
 Bibtex entry for the regression paper:
 
 ```bibtex
-@misc{cal-expl-regression,
+@misc{lofstrom2023ce_regression,
       title = 	      	{Calibrated Explanations for Regression},
       author =          {L\"ofstr\"om, Tuwe and L\"ofstr\"om, Helena and Johansson, Ulf and S\"onstr\"od, Cecilia and Matela, Rudy},
       year =            {2023},
       eprint =          {2308.16245},
       archivePrefix =   {arXiv},
       primaryClass =    {cs.LG}
 }
 ```
 
 To cite this software, use the following bibtex entry:
 
 ```bibtex
-@software{Lofstrom_Calibrated_Explanations_2024,
+@software{lofstrom2024ce_repository,
 	author = 	{Löfström, Helena and Löfström, Tuwe and Johansson, Ulf and Sönströd, Cecilia and Matela, Rudy},
 	license = 	{BSD-3-Clause},
 	title = 	{Calibrated Explanations},
 	url = 		{https://github.com/Moffran/calibrated_explanations},
-	version = 	{v0.3.2},
-	month = 	Feb,
+	version = 	{v0.3.3},
+	month = 	May,
 	year = 		{2024}
 }
 ```
   
 [Top](#calibrated-explanations-documentation)
 
 Acknowledgements
```

### Comparing `calibrated_explanations-0.3.2/pyproject.toml` & `calibrated_explanations-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calibrated_explanations"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="Helena Löfström", email="helena.lofstrom@ju.se" },
   { name="Tuwe Löfström", email="tuwe.lofstrom@ju.se" },
 ]
 description = "Extract calibrated explanations from machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/VennAbers.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/VennAbers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/__init__.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/_discretizers.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/_discretizers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/_explanations.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/_explanations.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,19 +486,20 @@
                     rule = f"{self._get_explainer().feature_names[f]} = {x[f]}"
             else:
                 rule = self._get_explainer().discretizer.names[f][int(x[f])]
             self.conditions.append(rule)
         return self.conditions
     
     
-
+    # pylint: disable=possibly-used-before-assignment
     def _predict_conjunctive(self, rule_value_set, original_features, perturbed, threshold, # pylint: disable=invalid-name, too-many-locals, too-many-arguments
                             predicted_class, bins=None):
         # """support function to calculate the prediction for a conjunctive rule
         # """
+        assert len(original_features) >= 2, 'Conjunctive rules require at least two features'
         rule_predict, rule_low, rule_high, rule_count = 0,0,0,0
         if len(original_features) == 2:
             of1, of2 = original_features[0], original_features[1]
             rule_value1, rule_value2 = rule_value_set[0], rule_value_set[1]
         elif len(original_features) >= 3:
             of1, of2, of3 = original_features[0], original_features[1], original_features[2]
             rule_value1, rule_value2, rule_value3 = rule_value_set[0], rule_value_set[1], rule_value_set[2]
```

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/_interval_regressor.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/_interval_regressor.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,27 @@
         values for the instances in the calibration set.
         
         '''
         self.ce = calibrated_explainer
         self.model = self
         self.cal_y_hat = self.ce.model.predict(self.ce.cal_X)  # can be calculated through calibrated_explainer
         self.residual_cal = self.ce.cal_y - self.cal_y_hat  # can be calculated through calibrated_explainer
+        self.sigma_cal = self.ce._get_sigma_test(X=self.ce.cal_X)  # pylint: disable=protected-access
         cps = crepes.ConformalPredictiveSystem()
         if self.ce.difficulty_estimator is not None:
-            sigma_cal = self.ce._get_sigma_test(X=self.ce.cal_X)
-            cps.fit(residuals=self.residual_cal, sigmas=sigma_cal, bins=self.ce.bins)
+            cps.fit(residuals=self.residual_cal, sigmas=self.sigma_cal, bins=self.ce.bins)
         else:
             cps.fit(residuals=self.residual_cal, bins=self.ce.bins)
         self.cps = cps
         self.venn_abers = None
         self.proba_cal = None
         self.y_threshold = None
         self.current_y_threshold = None
+        self.split = {}
+        self.pre_fit_for_probabilistic()
 
     def predict_probability(self, test_X, y_threshold, bins=None):
         '''The `predict_probability` function takes in a test dataset and a threshold value, and returns
         the predicted probabilities for each instance in the dataset being above the threshold(s), along 
         with confidence intervals.
         
         Parameters
@@ -71,23 +73,23 @@
         '''
         self.y_threshold = y_threshold
         if np.isscalar(self.y_threshold):
             self.current_y_threshold = self.y_threshold
             if bins is not None:
                 assert self.ce.bins is not None, 'Calibration bins must be assigned when test bins are submitted.'
             self.compute_proba_cal(self.y_threshold)
-            proba, low, high = self.venn_abers.predict_proba(test_X, output_interval=True, bins=bins)
+            proba, low, high = self.split['va'].predict_proba(test_X, output_interval=True, bins=bins)
             return proba[:, 1], low, high, None
 
         interval = np.zeros((test_X.shape[0],2))
         proba = np.zeros(test_X.shape[0])
         for i, _ in enumerate(proba):
             self.current_y_threshold = self.y_threshold[i]
             self.compute_proba_cal(self.y_threshold[i])
-            p, low, high = self.venn_abers.predict_proba(test_X[i, :].reshape(1, -1), output_interval=True, bins=bins)
+            p, low, high = self.split['va'].predict_proba(test_X[i, :].reshape(1, -1), output_interval=True, bins=bins)
             proba[i] = p[:,1]
             interval[i, :] = np.array([low[0], high[0]])
         return proba, interval[:, 0], interval[:, 1], None
 
     def predict_uncertainty(self, test_X, low_high_percentiles, bins=None):
         '''The function `predict_uncertainty` predicts the uncertainty of a given set of instances using a
         `ConformalPredictiveSystem` and returns the predicted values along with the lower and upper bounds of
@@ -151,46 +153,54 @@
         '''
         test_y_hat = self.ce.model.predict(test_X)
 
         sigma_test = self.ce._get_sigma_test(X=test_X)  # pylint: disable=protected-access
         proba = self.cps.predict(y_hat=test_y_hat, sigmas=sigma_test, y=self.current_y_threshold, bins=bins)
         return np.array([[1-proba[i], proba[i]] for i in range(len(proba))])
 
+    def pre_fit_for_probabilistic(self):
+        '''
+        The `pre_fit_for_probabilistic` function is used to split the calibration set into two parts. 
+        The first part is used to fit the `ConformalPredictiveSystem` and the second part is used to
+        calculate the probability calibration for a given threshold (at prediction time).
+        '''
+        n = len(self.ce.cal_y)
+        cal_parts = np.random.permutation(n).tolist()
+        self.split['parts'] = [cal_parts[:n//2], cal_parts[n//2:]]
+        cal_cps = self.split['parts'][0]
+        self.split['cps'] = crepes.ConformalPredictiveSystem()
+        if self.ce.bins is None:
+            self.split['cps'].fit(residuals=self.residual_cal[cal_cps],
+                            sigmas=self.sigma_cal[cal_cps])
+        else:
+            self.split['cps'].fit(residuals=self.residual_cal[cal_cps],
+                            sigmas=self.sigma_cal[cal_cps],
+                            bins=self.ce.bins[cal_cps])
+
     def compute_proba_cal(self, y_threshold: float):
         '''The `compute_proba_cal` function calculates the probability calibration for a given threshold.
         
         Parameters
         ----------
         y_threshold : float
             The `y_threshold` parameter is a float value that represents the threshold for the probability.
         It is used in the `compute_proba_cal` method to determine the predicted probabilities of the 
         calibration set for a given threshold value.     
         bins 
             array-like of shape (n_samples,), default=None
             Mondrian categories
         
         '''
-        # A less exact but faster solution, suitable when difficulty_estimator is assigned.
-        # Activated temporarily
-        if self.ce.difficulty_estimator is not None:
-            sigmas = self.ce._get_sigma_test(self.ce.cal_X)  # pylint: disable=protected-access
-            proba = self.cps.predict(y_hat=self.cal_y_hat,
-                                                y=y_threshold,
-                                                sigmas=sigmas,
-                                                bins=self.ce.bins)
-            self.proba_cal = np.array([[1-proba[i], proba[i]] for i in range(len(proba))])
+        cal_va = self.split['parts'][1]
+        if self.ce.bins is None:
+            bins = None
         else:
-            cps = crepes.ConformalPredictiveSystem()
-            self.proba_cal = np.zeros((len(self.residual_cal),2))
-            for i, _ in enumerate(self.residual_cal):
-                idx = np.setdiff1d(np.arange(len(self.residual_cal)), i)
-                sigma_cal = self.ce._get_sigma_test(self.ce.cal_X[idx, :])  # pylint: disable=protected-access
-                bin_cal = self.ce.bins[idx] if self.ce.bins is not None else None
-                bin_i = [self.ce.bins[i]] if self.ce.bins is not None else None
-                cps.fit(residuals=self.residual_cal[idx], sigmas=sigma_cal, bins=bin_cal)
-                sigma_i = self.ce._get_sigma_test(self.ce.cal_X[i, :].reshape(1, -1))  # pylint: disable=protected-access
-                self.proba_cal[i, 1] = cps.predict(y_hat=[self.cal_y_hat[i]],
-                                                y=y_threshold,
-                                                sigmas=sigma_i,
-                                                bins=bin_i)
-                self.proba_cal[i, 0] = 1 - self.proba_cal[i, 1]
-        self.venn_abers = VennAbers(self.proba_cal, (self.ce.cal_y <= y_threshold).astype(int), self, bins=self.ce.bins)
+            bins = self.ce.bins[cal_va]
+        proba = self.split['cps'].predict(y_hat=self.cal_y_hat[cal_va],
+                                y=y_threshold,
+                                sigmas=self.sigma_cal[cal_va],
+                                bins=bins)
+        self.split['proba'] = np.array([[1-proba[i], proba[i]] for i in range(len(proba))])
+        self.split['va'] = VennAbers(self.split['proba'],
+                                        (self.ce.cal_y[cal_va] <= y_threshold).astype(int),
+                                        self,
+                                        bins=bins)
```

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/core.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ._discretizers import BinaryDiscretizer, BinaryEntropyDiscretizer, \
                 DecileDiscretizer, QuartileDiscretizer, EntropyDiscretizer, \
                 RegressorDiscretizer, BinaryRegressorDiscretizer
 from .VennAbers import VennAbers
 from ._interval_regressor import IntervalRegressor
 from .utils import safe_isinstance, safe_import, check_is_fitted
 
-__version__ = 'v0.3.2'
+__version__ = 'v0.3.3'
 
 
 
 class CalibratedExplainer:
     """The CalibratedExplainer class is used for explaining machine learning models with calibrated
     predictions.
 
@@ -619,15 +619,15 @@
     def set_random_state(self, random_state: int) -> None:
         """changes the random seed
 
         Args:
             random_state (int): a seed to the random number generator
         """
         self.random_state = random_state
-        np.random.seed(self.random_state)
+        np.random.seed = self.random_state
 
 
 
     def set_difficulty_estimator(self, difficulty_estimator, initialize=True) -> None:
         """assigns a difficulty estimator for regression. For further information, 
         see the documentation for the difficulty estimator or refer to the crepes package 
         for further information.
```

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations/utils.py` & `calibrated_explanations-0.3.3/src/calibrated_explanations/utils.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/PKG-INFO` & `calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrated_explanations
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extract calibrated explanations from machine learning models.
 Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
 Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
 Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -28,37 +28,55 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/calibrated-explanations.svg)](https://anaconda.org/conda-forge/calibrated-explanations)
 [![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Moffran/calibrated_explanations)](https://github.com/Moffran/calibrated_explanations/blob/main/CHANGELOG.md)
 [![Documentation Status](https://readthedocs.org/projects/calibrated-explanations/badge/?version=latest)](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 [![Lint Status for Calibrated Explanations][lint-status]][lint-log]
 [![License](https://badgen.net/github/license/moffran/calibrated_explanations)](https://github.com/moffran/calibrated_explanations/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/calibrated-explanations)](https://pepy.tech/project/calibrated-explanations)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.2)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.3)
 
-`calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both classification and regression.
+`calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both [classification](https://doi.org/10.1016/j.eswa.2024.123154) and [regression](https://arxiv.org/abs/2308.16245).
 The proposed method is based on Venn-Abers (classification & regression) and Conformal Predictive Systems (regression) and has the following characteristics:
-* Fast, reliable, stable and robust feature importance explanations.
+* Fast, reliable, stable and robust feature importance explanations for:
+	- Binary classification models
+	- Multi-class classification models
+	- Regression models
+		* Including probabilistic explanations of the probability that the target exceeds a user-defined threshold 
+		* With difficulty adaptable explanations (conformal normalization) 
 * Calibration of the underlying model to ensure that predictions reflect reality.
 * Uncertainty quantification of the prediction from the underlying model and the feature importance weights. 
-* Rules with straightforward interpretation in relation to the feature weights.
+* Rules with straightforward interpretation in relation to instance values and feature weights.
 * Possibility to generate counterfactual rules with uncertainty quantification of the expected predictions.
-* Conjunctional rules conveying joint contribution between features.
+* Conjunctional rules conveying feature importance for the interaction of included features.
+* Conditional rules, allowing users the ability to create contextual explanations to handle e.g. bias and fairness constraints. 
 
-Below is an example of a probabilistic counterfactual explanation for an instance of the California Housing dataset (with the threshold 180 000). The light red area in the background is representing the calibrated probability interval (for the prediction being below the threshold) of the underlying model, as indicated by a Conformal Predictive System and calibrated through Venn-Abers. The darker red bars for each rule show the probability intervals that Venn-Abers indicate for an instance changing a feature value in accordance with the rule condition.
+Below is an example of a probabilistic counterfactual explanation for an instance of the regression dataset California Housing (with the threshold 180 000). The light red area in the background is representing the calibrated probability interval (for the prediction being below the threshold) of the underlying model, as indicated by a Conformal Predictive System and calibrated through Venn-Abers. The darker red bars for each rule show the probability intervals that Venn-Abers indicate for an instance changing a feature value in accordance with the rule condition.
+<p align="center">
+  <a href="https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest">
+    <img src="https://github.com/Moffran/calibrated_explanations/blob/main/docs/images/counterfactual_probabilistic_house_regression.jpg" alt="Probabilistic counterfactual explanation for California Housing">
+  </a>
+</p>
+
+Table 1 summarizes the characteristics of Calibrated Explanations.
+<p align="center">
+  <a href="https://arxiv.org/abs/2308.16245">
+    <img src="https://github.com/Moffran/calibrated_explanations/blob/main/docs/images/Table1.png" alt="Characteristics of Calibrated Explanantions">
+  </a>
+</p>
 
-[![Probabilistic counterfactual explanation for California Housing](https://github.com/Moffran/calibrated_explanations/blob/main/docs/images/counterfactual_probabilistic_house_regression.jpg "Probabilistic counterfactual explanation for California Housing")](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
- 
 Getting started
 ---------------
 The [notebooks folder](https://github.com/Moffran/calibrated_explanations/tree/main/notebooks) contains a number of notebooks illustrating different use cases for `calibrated-explanations`. The following are commented and should be a good start:
-* [quickstart](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/quickstart.ipynb)  - similar to this Getting Started, including plots.
+* [quickstart](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/quickstart.ipynb) - similar to this Getting Started, including plots.
 * [quickstart_wrap](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/quickstart_wrap.ipynb) - similar to this Getting Started, but with a wrapper class for easier use.
-* [demo_binary_classification](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_binary_classification.ipynb) 
-* [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb)
-* [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb)
+* [demo_binary_classification](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_binary_classification.ipynb) - with examples for binary classification 
+* [demo_multiclass](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_multiclass_glass.ipynb) - with examples for multi-class classification
+* [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) - with examples for regression
+* [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) - with examples for regression with thresholds
+* [demo_under_the_hood](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_under_the_hood.ipynb) - illustrating how to access the information composing the explanations
 
 ### Classification
 Let us illustrate how we may use `calibrated-explanations` to generate explanations from a classifier trained on a dataset from
 [www.openml.org](https://www.openml.org), which we first split into a
 training and a test set using `train_test_split` from
 [sklearn](https://scikit-learn.org), and then further split the
 training set into a proper training set and a calibration set:
@@ -134,15 +152,15 @@
 Individual explanations can also be plotted using `plot_explanation`.
       
 ```python
 factual_explanations.get_explanation(0).plot_explanation()
 counterfactual_explanations.get_explanation(0).plot_explanation()
 ```
 #### Support for multiclass
-`calibrated-explanations` supports multiclass which is demonstrated in [demo_multiclass](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_multiclass.ipynb). That notebook also demonstrates how both feature names and target and categorical labels can be added to improve the interpretability. 
+`calibrated-explanations` supports multiclass which is demonstrated in [demo_multiclass](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_multiclass_glass.ipynb). That notebook also demonstrates how both feature names and target and categorical labels can be added to improve the interpretability. 
 
 ### Regression
 Extracting explanations for regression is very similar to how it is done for classification. 
 
 ```python
 dataset = fetch_openml(name="house_sales", version=3)
 
@@ -219,15 +237,15 @@
 #### Additional Regression Use Cases
 Regression offers many more options and to learn more about them, see the [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) or the [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) notebooks.
 
 [Top](#calibrated-explanations-documentation)
 
 Known Limitations
 -----------------
-The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.2) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
+The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.1) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
 
 [Top](#calibrated-explanations-documentation)
 
 Install
 -------
 
 `calibrated-explanations` is implemented in Python, so you need a Python environment.
@@ -286,15 +304,15 @@
 - [Löfström, H.](https://github.com/Moffran), [Löfström, T.](https://github.com/tuvelofstrom), Johansson, U., & Sönströd, C. (2023). [Investigating the impact of calibration on the quality of explanations](https://link.springer.com/article/10.1007/s10472-023-09837-2). Annals of Mathematics and Artificial Intelligence, 1-18. [Code and results](https://github.com/tuvelofstrom/calibrating-explanations).
 
 If you use `calibrated-explanations` for a scientific publication, you are kindly requested to cite one of the papers above.
 
 Bibtex entry for the original paper:
 
 ```bibtex
-@article{lofstrom2024calibrated,
+@article{lofstrom2024ce_classification,
 	title = 	{Calibrated explanations: With uncertainty information and counterfactuals},
 	journal = 	{Expert Systems with Applications},
 	pages = 	{123154},
 	year = 		{2024},
 	issn = 		{0957-4174},
 	doi = 		{https://doi.org/10.1016/j.eswa.2024.123154},
 	url = 		{https://www.sciencedirect.com/science/article/pii/S0957417424000198},
@@ -302,34 +320,34 @@
 	keywords = 	{Explainable AI, Feature importance, Calibrated explanations, Venn-Abers, Uncertainty quantification, Counterfactual explanations},
 	abstract = 	{While local explanations for AI models can offer insights into individual predictions, such as feature importance, they are plagued by issues like instability. The unreliability of feature weights, often skewed due to poorly calibrated ML models, deepens these challenges. Moreover, the critical aspect of feature importance uncertainty remains mostly unaddressed in Explainable AI (XAI). The novel feature importance explanation method presented in this paper, called Calibrated Explanations (CE), is designed to tackle these issues head-on. Built on the foundation of Venn-Abers, CE not only calibrates the underlying model but also delivers reliable feature importance explanations with an exact definition of the feature weights. CE goes beyond conventional solutions by addressing output uncertainty. It accomplishes this by providing uncertainty quantification for both feature weights and the model’s probability estimates. Additionally, CE is model-agnostic, featuring easily comprehensible conditional rules and the ability to generate counterfactual explanations with embedded uncertainty quantification. Results from an evaluation with 25 benchmark datasets underscore the efficacy of CE, making it stand as a fast, reliable, stable, and robust solution.}
 }
 ```
 Bibtex entry for the regression paper:
 
 ```bibtex
-@misc{cal-expl-regression,
+@misc{lofstrom2023ce_regression,
       title = 	      	{Calibrated Explanations for Regression},
       author =          {L\"ofstr\"om, Tuwe and L\"ofstr\"om, Helena and Johansson, Ulf and S\"onstr\"od, Cecilia and Matela, Rudy},
       year =            {2023},
       eprint =          {2308.16245},
       archivePrefix =   {arXiv},
       primaryClass =    {cs.LG}
 }
 ```
 
 To cite this software, use the following bibtex entry:
 
 ```bibtex
-@software{Lofstrom_Calibrated_Explanations_2024,
+@software{lofstrom2024ce_repository,
 	author = 	{Löfström, Helena and Löfström, Tuwe and Johansson, Ulf and Sönströd, Cecilia and Matela, Rudy},
 	license = 	{BSD-3-Clause},
 	title = 	{Calibrated Explanations},
 	url = 		{https://github.com/Moffran/calibrated_explanations},
-	version = 	{v0.3.2},
-	month = 	Feb,
+	version = 	{v0.3.3},
+	month = 	May,
 	year = 		{2024}
 }
 ```
   
 [Top](#calibrated-explanations-documentation)
 
 Acknowledgements
```

### Comparing `calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/SOURCES.txt` & `calibrated_explanations-0.3.3/src/calibrated_explanations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/tests/test_classification.py` & `calibrated_explanations-0.3.3/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.2/tests/test_regression.py` & `calibrated_explanations-0.3.3/tests/test_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             CalibratedExplainer(RandomForestRegressor(), calX, calY, feature_names=feature_names, categorical_features=categorical_features, categorical_labels=categorical_labels, mode='regression')
         cal_exp = CalibratedExplainer(model, calX, calY, feature_names=feature_names, categorical_features=categorical_features, mode='regression')
         with pytest.raises(NotFittedError):
             cal_exp.set_difficulty_estimator(DifficultyEstimator())
 
 
     # NOTE: this takes takes about 70s to run
-    @unittest.skip('Test fails online but passes locally. Error/warning raised by crepes. Skipping provisionally.')
+    # @unittest.skip('Test fails online but passes locally. Error/warning raised by crepes. Skipping provisionally.')
     def test_regression_ce(self):
         trainX, trainY, calX, calY, testX, _, _, _, categorical_features, categorical_labels, feature_names = load_regression_dataset()
         model, _ = get_regression_model('RF', trainX, trainY) # pylint: disable=redefined-outer-name
         cal_exp = CalibratedExplainer(
             model,
             calX,
             calY,
@@ -138,15 +138,15 @@
         self.assertExplanation(counterfactual_explanation)
 
         counterfactual_explanation = cal_exp.explain_counterfactual(testX, testY[0])
         self.assertIsInstance(counterfactual_explanation.calibrated_explainer.discretizer, RegressorDiscretizer)
         self.assertExplanation(counterfactual_explanation)
 
 
-    @unittest.skip('Test fails online but passes locally. Error/warning raised by crepes. Skipping provisionally.')
+    # @unittest.skip('Test fails online but passes locally. Error/warning raised by crepes. Skipping provisionally.')
     def test_knn_normalized_regression_ce(self):
         trainX, trainY, calX, calY, testX, _, _, _, categorical_features, categorical_labels, feature_names = load_regression_dataset()
         model, _ = get_regression_model('RF', trainX, trainY) # pylint: disable=redefined-outer-name
         cal_exp = CalibratedExplainer(
             model,
             calX,
             calY,
@@ -213,15 +213,15 @@
         self.assertExplanation(counterfactual_explanation)
 
         counterfactual_explanation = cal_exp.explain_counterfactual(testX, testY[0])
         self.assertIsInstance(counterfactual_explanation.calibrated_explainer.discretizer, RegressorDiscretizer)
         self.assertExplanation(counterfactual_explanation)
 
 
-    @unittest.skip('Test fails online but passes locally. Error/warning raised by crepes. Skipping provisionally.')
+    # @unittest.skip('Test fails online but passes locally. Error/warning raised by crepes. Skipping provisionally.')
     def test_var_normalized_regression_ce(self):
         trainX, trainY, calX, calY, testX, _, _, _, categorical_features, categorical_labels, feature_names = load_regression_dataset()
         model, _ = get_regression_model('RF', trainX, trainY) # pylint: disable=redefined-outer-name
         cal_exp = CalibratedExplainer(
             model,
             calX,
             calY,
```

