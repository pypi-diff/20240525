# Comparing `tmp/fastqwiper-2024.1.86-py3-none-any.whl.zip` & `tmp/fastqwiper-2024.1.90-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 15025 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1898 b- defN 24-May-18 19:23 fastq_wiper/__init__.py
--rw-r--r--  2.0 unx     2078 b- defN 24-May-18 19:23 fastq_wiper/color_log_formatter.py
--rw-r--r--  2.0 unx    12820 b- defN 24-May-18 19:23 fastq_wiper/wiper.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-18 19:23 tests/__init__.py
--rw-r--r--  2.0 unx      816 b- defN 24-May-18 19:23 tests/test_wiper.py
--rw-r--r--  2.0 unx     7601 b- defN 24-May-18 19:23 fastqwiper-2024.1.86.dist-info/LICENSE
--rw-r--r--  2.0 unx    13353 b- defN 24-May-18 19:23 fastqwiper-2024.1.86.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 19:23 fastqwiper-2024.1.86.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 24-May-18 19:23 fastqwiper-2024.1.86.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 24-May-18 19:23 fastqwiper-2024.1.86.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 24-May-18 19:23 fastqwiper-2024.1.86.dist-info/RECORD
-11 files, 39655 bytes uncompressed, 13459 bytes compressed:  66.1%
+Zip file size: 12875 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 24-May-25 07:35 fastq_wiper/__init__.py
+-rw-r--r--  2.0 unx     9984 b- defN 24-May-25 07:35 fastq_wiper/wiper.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-25 07:35 tests/__init__.py
+-rw-r--r--  2.0 unx      816 b- defN 24-May-25 07:35 tests/test_wiper.py
+-rw-r--r--  2.0 unx     7601 b- defN 24-May-25 07:36 fastqwiper-2024.1.90.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14374 b- defN 24-May-25 07:36 fastqwiper-2024.1.90.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-25 07:36 fastqwiper-2024.1.90.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 24-May-25 07:36 fastqwiper-2024.1.90.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-May-25 07:36 fastqwiper-2024.1.90.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      824 b- defN 24-May-25 07:36 fastqwiper-2024.1.90.dist-info/RECORD
+10 files, 33769 bytes uncompressed, 11453 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,34 +1,31 @@
 Filename: fastq_wiper/__init__.py
 Comment: 
 
-Filename: fastq_wiper/color_log_formatter.py
-Comment: 
-
 Filename: fastq_wiper/wiper.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_wiper.py
 Comment: 
 
-Filename: fastqwiper-2024.1.86.dist-info/LICENSE
+Filename: fastqwiper-2024.1.90.dist-info/LICENSE
 Comment: 
 
-Filename: fastqwiper-2024.1.86.dist-info/METADATA
+Filename: fastqwiper-2024.1.90.dist-info/METADATA
 Comment: 
 
-Filename: fastqwiper-2024.1.86.dist-info/WHEEL
+Filename: fastqwiper-2024.1.90.dist-info/WHEEL
 Comment: 
 
-Filename: fastqwiper-2024.1.86.dist-info/entry_points.txt
+Filename: fastqwiper-2024.1.90.dist-info/entry_points.txt
 Comment: 
 
-Filename: fastqwiper-2024.1.86.dist-info/top_level.txt
+Filename: fastqwiper-2024.1.90.dist-info/top_level.txt
 Comment: 
 
-Filename: fastqwiper-2024.1.86.dist-info/RECORD
+Filename: fastqwiper-2024.1.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastq_wiper/__init__.py

```diff
@@ -1,119 +0,0 @@
-00000000: 2222 2222 0a46 696c 6520 6465 7363 7269  """".File descri
-00000010: 7074 696f 6e0a 2222 220a 0a69 6d70 6f72  ption."""..impor
-00000020: 7420 6c6f 6767 696e 670a 6672 6f6d 2066  t logging.from f
-00000030: 6173 7471 5f77 6970 6572 2e63 6f6c 6f72  astq_wiper.color
-00000040: 5f6c 6f67 5f66 6f72 6d61 7474 6572 2069  _log_formatter i
-00000050: 6d70 6f72 7420 436f 6c6f 7246 6f72 6d61  mport ColorForma
-00000060: 7474 6572 0a0a 5f5f 6175 7468 6f72 5f5f  tter..__author__
-00000070: 203d 2022 546f 6d6d 6173 6f20 4d61 7a7a   = "Tommaso Mazz
-00000080: 6122 0a5f 5f63 6f70 7972 6967 6874 5f5f  a".__copyright__
-00000090: 203d 2022 436f 7079 7269 6768 7420 3230   = "Copyright 20
-000000a0: 3230 2c20 5468 6520 4661 7374 7157 6970  20, The FastqWip
-000000b0: 6572 2050 726f 6a65 6374 220a 5f5f 7665  er Project".__ve
-000000c0: 7273 696f 6e5f 5f20 3d20 2230 2e30 2e31  rsion__ = "0.0.1
-000000d0: 220a 5f5f 6d61 696e 7461 696e 6572 5f5f  ".__maintainer__
-000000e0: 203d 2022 546f 6d6d 6173 6f20 4d61 7a7a   = "Tommaso Mazz
-000000f0: 6122 0a5f 5f65 6d61 696c 5f5f 203d 2022  a".__email__ = "
-00000100: 6269 6f69 6e66 6f72 6d61 7469 6373 4063  bioinformatics@c
-00000110: 7373 2d6d 656e 6465 6c2e 6974 220a 5f5f  ss-mendel.it".__
-00000120: 7374 6174 7573 5f5f 203d 2022 4465 7665  status__ = "Deve
-00000130: 6c6f 706d 656e 7422 0a5f 5f64 6174 655f  lopment".__date_
-00000140: 5f20 3d20 2232 382f 3132 2f32 3032 3022  _ = "28/12/2020"
-00000150: 0a5f 5f63 7265 6174 6f72 5f5f 203d 2022  .__creator__ = "
-00000160: 742e 6d61 7a7a 6122 0a5f 5f6c 6963 656e  t.mazza".__licen
-00000170: 7365 5f5f 203d 2075 2222 220a 2020 436f  se__ = u""".  Co
-00000180: 7079 7269 6768 7420 2843 2920 3230 3230  pyright (C) 2020
-00000190: 2054 6f6d 6d61 736f 204d 617a 7a61 203c   Tommaso Mazza <
-000001a0: 742e 6d61 7a7a 6140 6373 732d 6d65 6e64  t.mazza@css-mend
-000001b0: 656c 2e69 743e 0a20 2056 6961 6c65 2052  el.it>.  Viale R
-000001c0: 6567 696e 6120 4d61 7267 6865 7269 7461  egina Margherita
-000001d0: 2032 3631 2c20 3030 3139 3820 526f 6d65   261, 00198 Rome
-000001e0: 2c20 4974 616c 790a 0a20 2054 6869 7320  , Italy..  This 
-000001f0: 7072 6f67 7261 6d20 6973 2066 7265 6520  program is free 
-00000200: 736f 6674 7761 7265 3b20 796f 7520 6361  software; you ca
-00000210: 6e20 7265 6469 7374 7269 6275 7465 2069  n redistribute i
-00000220: 7420 616e 642f 6f72 206d 6f64 6966 790a  t and/or modify.
-00000230: 2020 6974 2075 6e64 6572 2074 6865 2074    it under the t
-00000240: 6572 6d73 206f 6620 7468 6520 474e 5520  erms of the GNU 
-00000250: 4765 6e65 7261 6c20 5075 626c 6963 204c  General Public L
-00000260: 6963 656e 7365 2061 7320 7075 626c 6973  icense as publis
-00000270: 6865 6420 6279 0a20 2074 6865 2046 7265  hed by.  the Fre
-00000280: 6520 536f 6674 7761 7265 2046 6f75 6e64  e Software Found
-00000290: 6174 696f 6e3b 2065 6974 6865 7220 7665  ation; either ve
-000002a0: 7273 696f 6e20 3220 6f66 2074 6865 204c  rsion 2 of the L
-000002b0: 6963 656e 7365 2c20 6f72 0a20 2028 6174  icense, or.  (at
-000002c0: 2079 6f75 7220 6f70 7469 6f6e 2920 616e   your option) an
-000002d0: 7920 6c61 7465 7220 7665 7273 696f 6e2e  y later version.
-000002e0: 0a0a 2020 5468 6973 2070 726f 6772 616d  ..  This program
-000002f0: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
-00000300: 696e 2074 6865 2068 6f70 6520 7468 6174  in the hope that
-00000310: 2069 7420 7769 6c6c 2062 6520 7573 6566   it will be usef
-00000320: 756c 2c0a 2020 6275 7420 5749 5448 4f55  ul,.  but WITHOU
-00000330: 5420 414e 5920 5741 5252 414e 5459 3b20  T ANY WARRANTY; 
-00000340: 7769 7468 6f75 7420 6576 656e 2074 6865  without even the
-00000350: 2069 6d70 6c69 6564 2077 6172 7261 6e74   implied warrant
-00000360: 7920 6f66 0a20 204d 4552 4348 414e 5441  y of.  MERCHANTA
-00000370: 4249 4c49 5459 206f 7220 4649 544e 4553  BILITY or FITNES
-00000380: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
-00000390: 4152 2050 5552 504f 5345 2e20 2053 6565  AR PURPOSE.  See
-000003a0: 2074 6865 0a20 2047 4e55 2047 656e 6572   the.  GNU Gener
-000003b0: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-000003c0: 6520 666f 7220 6d6f 7265 2064 6574 6169  e for more detai
-000003d0: 6c73 2e0a 0a20 2059 6f75 2073 686f 756c  ls...  You shoul
-000003e0: 6420 6861 7665 2072 6563 6569 7665 6420  d have received 
-000003f0: 6120 636f 7079 206f 6620 7468 6520 474e  a copy of the GN
-00000400: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-00000410: 204c 6963 656e 7365 0a20 2061 6c6f 6e67   License.  along
-00000420: 2077 6974 6820 7468 6973 2070 726f 6772   with this progr
-00000430: 616d 3b20 6966 206e 6f74 2c20 7772 6974  am; if not, writ
-00000440: 6520 746f 2074 6865 2046 7265 6520 536f  e to the Free So
-00000450: 6674 7761 7265 0a20 2046 6f75 6e64 6174  ftware.  Foundat
-00000460: 696f 6e2c 2049 6e63 2e2c 2020 3531 2046  ion, Inc.,  51 F
-00000470: 7261 6e6b 6c69 6e20 5374 7265 6574 2c20  ranklin Street, 
-00000480: 4669 6674 6820 466c 6f6f 722c 2042 6f73  Fifth Floor, Bos
-00000490: 746f 6e2c 204d 410a 2020 3032 3131 302d  ton, MA.  02110-
-000004a0: 3133 3031 2055 5341 0a20 2022 2222 0a0a  1301 USA.  """..
-000004b0: 2320 6c6f 6767 696e 672e 6261 7369 6343  # logging.basicC
-000004c0: 6f6e 6669 6728 666f 726d 6174 3d27 2528  onfig(format='%(
-000004d0: 6173 6374 696d 6529 7320 2d20 2528 6d65  asctime)s - %(me
-000004e0: 7373 6167 6529 7327 2c20 6c65 7665 6c3d  ssage)s', level=
-000004f0: 6c6f 6767 696e 672e 494e 464f 290a 2320  logging.INFO).# 
-00000500: 6c6f 6767 696e 672e 6765 744c 6f67 6765  logging.getLogge
-00000510: 7228 5f5f 6e61 6d65 5f5f 292e 6164 6448  r(__name__).addH
-00000520: 616e 646c 6572 286c 6f67 6769 6e67 2e4e  andler(logging.N
-00000530: 756c 6c48 616e 646c 6572 2829 290a 6c6f  ullHandler()).lo
-00000540: 6720 3d20 6c6f 6767 696e 672e 6765 744c  g = logging.getL
-00000550: 6f67 6765 7228 5f5f 6e61 6d65 5f5f 290a  ogger(__name__).
-00000560: 6c6f 672e 7365 744c 6576 656c 286c 6f67  log.setLevel(log
-00000570: 6769 6e67 2e44 4542 5547 290a 0a23 2044  ging.DEBUG)..# D
-00000580: 4542 5547 464f 524d 4154 5445 5220 3d20  EBUGFORMATTER = 
-00000590: 2725 2866 696c 656e 616d 6529 733a 2528  '%(filename)s:%(
-000005a0: 6e61 6d65 2973 3a25 2866 756e 634e 616d  name)s:%(funcNam
-000005b0: 6529 733a 2528 6c69 6e65 6e6f 2964 3a20  e)s:%(lineno)d: 
-000005c0: 2528 6d65 7373 6167 6529 7327 0a44 4542  %(message)s'.DEB
-000005d0: 5547 464f 524d 4154 5445 5220 3d20 2725  UGFORMATTER = '%
-000005e0: 2861 7363 7469 6d65 2973 202d 2025 286e  (asctime)s - %(n
-000005f0: 616d 6529 732f 2528 6669 6c65 6e61 6d65  ame)s/%(filename
-00000600: 2973 2825 2866 756e 634e 616d 6529 7329  )s(%(funcName)s)
-00000610: 202d 2025 286c 6576 656c 6e61 6d65 2973   - %(levelname)s
-00000620: 202d 2025 286d 6573 7361 6765 2973 270a   - %(message)s'.
-00000630: 2222 2244 6562 7567 2066 696c 6520 666f  """Debug file fo
-00000640: 726d 6174 7465 722e 2222 220a 0a23 2064  rmatter."""..# d
-00000650: 6566 696e 6573 2074 6865 2073 7472 6561  efines the strea
-00000660: 6d20 6861 6e64 6c65 720a 6368 203d 206c  m handler.ch = l
-00000670: 6f67 6769 6e67 2e53 7472 6561 6d48 616e  ogging.StreamHan
-00000680: 646c 6572 2829 2020 2320 6372 6561 7465  dler()  # create
-00000690: 7320 7468 6520 6861 6e64 6c65 720a 6368  s the handler.ch
-000006a0: 2e73 6574 4c65 7665 6c28 6c6f 6767 696e  .setLevel(loggin
-000006b0: 672e 494e 464f 2920 2023 2073 6574 7320  g.INFO)  # sets 
-000006c0: 7468 6520 6861 6e64 6c65 7220 696e 666f  the handler info
-000006d0: 0a63 6620 3d20 436f 6c6f 7246 6f72 6d61  .cf = ColorForma
-000006e0: 7474 6572 2844 4542 5547 464f 524d 4154  tter(DEBUGFORMAT
-000006f0: 5445 5229 0a63 682e 7365 7446 6f72 6d61  TER).ch.setForma
-00000700: 7474 6572 2863 6629 2020 2320 7365 7473  tter(cf)  # sets
-00000710: 2074 6865 2068 616e 646c 6572 2066 6f72   the handler for
-00000720: 6d61 7474 696e 670a 0a23 2061 6464 7320  matting..# adds 
-00000730: 7468 6520 6861 6e64 6c65 7220 746f 2074  the handler to t
-00000740: 6865 2067 6c6f 6261 6c20 7661 7269 6162  he global variab
-00000750: 6c65 3a20 6c6f 670a 6c6f 672e 6164 6448  le: log.log.addH
-00000760: 616e 646c 6572 2863 6829                 andler(ch)
```

## fastq_wiper/wiper.py

```diff
@@ -1,40 +1,34 @@
 import os.path
 import sys
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from colorama import init
-
-init(convert=True)
-import click
 import gzip
 import re
 import codecs
-from fastq_wiper import log
+import argparse
+import logging
 
+logging.basicConfig(level=logging.DEBUG)
 
 # region Variables for final report
+blank: int = 0
 tot_lines: int = 0
+bad_seq: int = 0
+fixed_header: int = 0
+bad_header: int = 0
+bad_plus: int = 0
+fixed_plus: int = 0
+bad_qual: int = 0
+qual_out_of_range: int = 0
 clean_reads: int = 0
 seq_len_neq_qual_len: int = 0
-qual_out_range: int = 0
-plus_row: int = 0
-seq_odd_chars: int = 0
-qual_odd_chars: int = 0
-head_print: int = 0
-head_at: int = 0
-blank: int = 0
-head_plus: int = 0
-unexpected_line: int = 0
 # endregion
 
-# Allowed character of the SEQ line
-reg = re.compile("^[ACGTN]+$")
-
 
 def open_fastq_file(file_path: str):
     fastq_file_handler = None
 
     if "/" not in file_path and "\\" not in file_path:
         file_path = os.path.join(os.getcwd(), file_path)
 
@@ -47,14 +41,26 @@
             fastq_file_handler = codecs.open(
                 file_path, encoding="utf-8", errors="ignore"
             )
 
     return fastq_file_handler
 
 
+def read_next_line(fin, log_frequency: int):
+    global tot_lines
+
+    line = fin.readline()
+    if line:
+        # increment the total number of read not-empty lines
+        tot_lines += 1
+        print_log_during_reading(tot_lines, log_frequency)
+
+    return line
+
+
 def write_fastq_file(file_path: str):
     fastq_file_handler = None
 
     if "/" not in file_path or "\\" not in file_path:
         parent_folder = os.getcwd()
     else:
         parent_folder = os.path.abspath(os.path.join(file_path, os.pardir))
@@ -64,372 +70,248 @@
             fastq_file_handler = gzip.open(file_path, "wt", encoding="utf-8")
         elif file_path.endswith(".fastq"):
             fastq_file_handler = open(file_path, "wt", encoding="utf-8")
 
     return fastq_file_handler
 
 
-def fix_header_line(line: str, checkpoint_flags: dict) -> str:
-    header: str = line.rstrip()
+def check_header_line(line: str) -> str:
+    global fixed_header, bad_header
+    header: str = ""
+
+    if line.isprintable() and line.rfind("@") == 0:
+        header = line
+    elif not line.isprintable():
+        # This is a not printable header
+        bad_header += 1
+    elif "@" not in line:
+        # This is an uncompliant header line
+        bad_header += 1
+    else:  # elif header.rfind("@") > 0:
+        header = line
+        header = header[header.rfind("@"):]
+        fixed_header += 1
 
-    # Drop all character preceding the last @ character of the header
-    if header.rfind("@") > 0:
-        header = header[header.rfind("@") :]
-
-    if header == "@":
-        checkpoint_flags["at"] = False
-    else:
-        checkpoint_flags["at"] = True
-        
-        global head_at
-        head_at += 1
-    
     return header
 
 
-def fix_seq_line(line: str, checkpoint_flags: dict) -> str:
+def check_seq_line(line: str) -> str:
+    global bad_seq
     raw_seq: str = ""
 
-    if reg.match(line):
-        checkpoint_flags["seq"] = True
+    if not line.isprintable() or not reg.match(line):
+        bad_seq += 1
+    else:
         raw_seq = line
 
     return raw_seq
 
 
-def fix_plus_line(line: str, checkpoint_flags: dict) -> str:
-    checkpoint_flags["plus"] = True
-
-    if line != "+":
-        # Drop all characters except + of the qual line separator
-        line = "+"
-
-        global head_plus
-        head_plus += 1
+def check_plus_line(line: str) -> str:
+    global bad_plus, fixed_plus
+    plus: str = ""
+
+    if not line.isprintable() or line.find("+") == -1:
+        bad_plus += 1
+    elif line.find("+") > 0:
+        # Drop all characters except '+' character
+        plus = '+'
+        fixed_plus += 1
+    else:
+        plus = line
 
-    return line
+    return plus
 
 
-def fix_qual_line(line: str, checkpoint_flags: dict) -> str:
+def check_qual_line(line: str) -> str:
+    global qual_out_of_range, bad_qual
     qual: str = ""
 
-    if(line):
+    if not line.isprintable():
+        bad_qual += 1
+
+    if line:
         min_ascii = min(ord(c) for c in line)
         max_ascii = max(ord(c) for c in line)
         if min_ascii >= 33 and max_ascii <= 126:
-            checkpoint_flags["qual"] = True
-            qual: str = line
+            qual = line
         else:
-            global qual_out_range
-            qual_out_range += 1
+            qual_out_of_range += 1
 
     return qual
 
 
-def skip_empty_lines(line: str, fin) -> str:
-    while True:
-        if line:
-            line = line.rstrip()
-            break
-        else:
-            global blank
-            blank += 1
-            line = fin.readline()
-            continue
-
-    return line
-
-
 def print_log_during_reading(lines, log_frequency):
     if lines % log_frequency == 0:
-        log.info(f"Cleaned {lines} reads")
+        logging.info(f"Cleaned {lines} reads")
 
 
 def print_to_file(header, raw_seq, head_qual_sep, qual, fout):
     fout.write(header + "\n")
     fout.write(raw_seq + "\n")
     fout.write(head_qual_sep + "\n")
     fout.write(qual + "\n")
 
 
 def print_log_to_file(log_out):
-    global tot_lines, clean_reads, seq_len_neq_qual_len, head_print, seq_odd_chars, plus_row, qual_odd_chars, unexpected_line
+    global tot_lines, clean_reads, seq_len_neq_qual_len, bad_qual, qual_out_of_range, bad_plus, \
+        bad_seq, bad_header, fixed_header, fixed_plus, blank
 
     # Open file out summary log
     flog = open(log_out, "wt", encoding="utf-8")
 
     flog.write("SUMMARY:" + "\n" + "\n")
     flog.write(
         f"Clean lines: {clean_reads*4}/{tot_lines} ({round((clean_reads*4 / tot_lines) * 100, 2)}%)"
         + "\n"
     )
+    flog.write(f"Not printable or uncompliant header lines: {bad_header}/{tot_lines}" + "\n")
+    flog.write(f"Fixed header lines: {fixed_header}/{tot_lines}" + "\n")
+    flog.write(f"BAD SEQ lines: {bad_seq}/{tot_lines}" + "\n")
+    flog.write(f"BAD '+' lines: {bad_plus}/{tot_lines}" + "\n")
+    flog.write(f"Fixed + lines: {fixed_plus}/{tot_lines}" + "\n")
+    flog.write(f"BAD QUAL lines: {bad_qual}/{tot_lines}" + "\n")
+    flog.write(f"QUAL out of range lines: {qual_out_of_range}/{tot_lines}" + "\n")
     flog.write(f"Len(SEQ) neq Len(QUAL): {seq_len_neq_qual_len}/{tot_lines}" + "\n")
-    flog.write(f"BAD QUAL lines: {qual_out_range}/{tot_lines}" + "\n")
-    flog.write(f"BAD '+' lines: {plus_row}/{tot_lines}" + "\n")
-    flog.write(f"BAD SEQ lines: {seq_odd_chars}/{tot_lines}" + "\n")
-    flog.write(
-        f"Not printable or uncompliant header lines: {head_print}/{tot_lines}" + "\n"
-    )
-    flog.write(f"Not printable qual lines: {qual_odd_chars}/{tot_lines}" + "\n")
-    flog.write(f"Fixed header lines: {head_at}/{tot_lines}" + "\n")
-    flog.write(f"Fixed + lines: {head_plus}/{tot_lines}" + "\n")
     flog.write(f"Blank lines: {blank}/{tot_lines}" + "\n")
-    flog.write(f"Missplaced lines: {unexpected_line}/{tot_lines}" + "\n")
 
     flog.close()
 
 
 def print_log_to_screen():
-    global tot_lines, clean_reads, seq_len_neq_qual_len, head_print, seq_odd_chars, plus_row, qual_odd_chars, unexpected_line
+    global tot_lines, clean_reads, seq_len_neq_qual_len, bad_qual, qual_out_of_range, bad_plus, \
+        bad_seq, bad_header, fixed_header, fixed_plus, blank
 
-    click.echo(
-        click.style(
-            f"Clean lines: {clean_reads*4}/{tot_lines} ({round((clean_reads*4 / tot_lines) * 100, 2)}%)",
-            fg="blue" if tot_lines == clean_reads else "yellow",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Len(SEQ) neq Len(QUAL): {seq_len_neq_qual_len}/{tot_lines}",
-            fg="blue" if seq_len_neq_qual_len == 0 else "red",
-        )
-    )
-    click.echo(
-        click.style(
-            f"BAD QUAL lines: {qual_out_range}/{tot_lines}",
-            fg="blue" if qual_out_range == 0 else "red",
-        )
-    )
-    click.echo(
-        click.style(
-            f"BAD '+' lines: {plus_row}/{tot_lines}",
-            fg="blue" if plus_row == 0 else "red",
-        )
-    )
-    click.echo(
-        click.style(
-            f"BAD SEQ lines: {seq_odd_chars}/{tot_lines}",
-            fg="blue" if seq_odd_chars == 0 else "red",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Not printable or uncompliant header lines: {head_print}/{tot_lines}",
-            fg="blue" if head_print == 0 else "red",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Not printable qual lines: {qual_odd_chars}/{tot_lines}",
-            fg="blue" if qual_odd_chars == 0 else "red",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Fixed header lines: {head_at}/{tot_lines}",
-            fg="blue" if head_at == 0 else "yellow",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Fixed + lines: {head_plus}/{tot_lines}",
-            fg="blue" if head_plus == 0 else "yellow",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Blank lines: {blank}/{tot_lines}",
-            fg="blue" if blank == 0 else "yellow",
-        )
-    )
-    click.echo(
-        click.style(
-            f"Missplaced lines: {unexpected_line}/{tot_lines}",
-            fg="blue" if unexpected_line == 0 else "yellow",
-        )
-    )
+    if tot_lines == (clean_reads*4):
+        logging.info(f"Clean lines: {clean_reads * 4}/{tot_lines} ({round((clean_reads * 4 / tot_lines) * 100, 2)}%)")
+    else:
+        logging.warning(
+            f"Clean lines: {clean_reads * 4}/{tot_lines} ({round((clean_reads * 4 / tot_lines) * 100, 2)}%)")
 
+    if bad_header == 0:
+        logging.info(f"Not printable or uncompliant header lines: {bad_header}/{tot_lines}")
+    else:
+        logging.warning(f"Not printable or uncompliant header lines: {bad_header}/{tot_lines}")
 
-def reset_flags(checkpoint_flags: dict):
-    checkpoint_flags["at"] = False
-    checkpoint_flags["seq"] = False
-    checkpoint_flags["plus"] = False
-    checkpoint_flags["qual"] = False
+    if fixed_header == 0:
+        logging.info(f"Fixed header lines: {fixed_header}/{tot_lines}")
+    else:
+        logging.warning(f"Fixed header lines: {fixed_header}/{tot_lines}")
 
+    if bad_seq == 0:
+        logging.info(f"BAD SEQ lines: {bad_seq}/{tot_lines}")
+    else:
+        logging.warning(f"BAD SEQ lines: {bad_seq}/{tot_lines}")
 
-def count_remainder():
-    global tot_lines
-    return tot_lines % 4
+    if bad_plus == 0:
+        logging.info(f"BAD '+' lines: {bad_plus}/{tot_lines}")
+    else:
+        logging.warning(f"BAD '+' lines: {bad_plus}/{tot_lines}")
+
+    if fixed_plus == 0:
+        logging.info(f"Fixed + lines: {fixed_plus}/{tot_lines}")
+    else:
+        logging.warning(f"Fixed + lines: {fixed_plus}/{tot_lines}")
+
+    if bad_qual == 0:
+        logging.info(f"BAD QUAL lines: {qual_out_of_range}/{tot_lines}")
+    else:
+        logging.warning(f"BAD QUAL lines: {qual_out_of_range}/{tot_lines}")
+
+    if qual_out_of_range == 0:
+        logging.info(f"QUAL out of range lines: {qual_out_of_range}/{tot_lines}")
+    else:
+        logging.warning(f"QUAL out of range lines: {qual_out_of_range}/{tot_lines}")
+
+    if seq_len_neq_qual_len == 0:
+        logging.info(f"Len(SEQ) neq Len(QUAL): {seq_len_neq_qual_len}/{tot_lines}")
+    else:
+        logging.warning(f"Len(SEQ) neq Len(QUAL): {seq_len_neq_qual_len}/{tot_lines}")
+
+    if blank == 0:
+        logging.info(f"Blank lines: {blank}/{tot_lines}")
+    else:
+        logging.warning(f"Blank lines: {blank}/{tot_lines}")
 
 
-@click.command()
-@click.option(
-    "--fastq_in", type=click.STRING, required=True, help="The input FASTQ file"
-)
-@click.option(
-    "--fastq_out", type=click.STRING, required=True, help="The wiped FASTQ file"
-)
-@click.option(
-    "--log_out",
-    type=click.STRING,
-    required=False,
-    help="The file name of the final quality report summary",
-)
-@click.option(
-    "--log_frequency",
-    type=click.INT,
-    default=500000,
-    help="The number of reads you want to print a status message",
-)
 def wipe_fastq(fastq_in: str, fastq_out: str, log_out: str, log_frequency: int):
     # MIN_HEADER_LEN = 10
 
     fin = open_fastq_file(fastq_in)
     if not fin:
-        click.echo(
-            click.style(
-                "The input FASTQ file does not exist or bad extension (.gz or .fastq.gz)",
-                fg="red",
-            )
-        )
+        logging.critical("The input FASTQ file does not exist or bad extension (.gz or .fastq.gz)")
     else:
-        click.echo(click.style(f"Start wiping {fastq_in}", fg="blue"))
+        logging.info(f"Start wiping {fastq_in}")
 
         # Open file out stream
         fout = write_fastq_file(fastq_out)
 
-        # change if a lines is parsed succesfully
-        checkpoint_flags = {
-            "at": False,
-            "seq": False,
-            "plus": False,
-            "qual": False,
-        }
-
-        # Cleaned lines to be printed
-        header: str = ""
-        raw_seq: str = ""
-        head_qual_sep: str = ""
-        qual: str = ""
-
         # global variables anchor
-        global tot_lines, clean_reads, seq_len_neq_qual_len, head_print, seq_odd_chars, plus_row, qual_odd_chars, unexpected_line
+        global tot_lines, clean_reads, seq_len_neq_qual_len
 
         # Loop through 4-line reads
         for line in fin:
-            tot_lines += 1  # increment the total number of read lines
+            if not line.strip():
+                # skip empty lines
+                continue
 
+            tot_lines += 1
             print_log_during_reading(tot_lines, log_frequency)
-            line = skip_empty_lines(line, fin)
-
-            # header line
-            if (
-                line.isprintable()
-                and "@" in line
-                and not checkpoint_flags["at"]
-                and not checkpoint_flags["seq"]
-                and not checkpoint_flags["plus"]
-                and not checkpoint_flags["qual"]
-            ):
-                header = fix_header_line(line, checkpoint_flags)
-
-            # seq line
-            elif (
-                line.isprintable()
-                and checkpoint_flags["at"]
-                and not checkpoint_flags["seq"]
-                and not checkpoint_flags["plus"]
-                and not checkpoint_flags["qual"]
-            ):
-                raw_seq = fix_seq_line(line, checkpoint_flags)
-
-            # + line
-            elif (
-                "+" in line
-                and line.isprintable()
-                and checkpoint_flags["at"]
-                and checkpoint_flags["seq"]
-                and not checkpoint_flags["plus"]
-                and not checkpoint_flags["qual"]
-            ):
-                head_qual_sep = fix_plus_line(line, checkpoint_flags)
-
-            # qual line
-            elif (
-                line.isprintable()
-                and checkpoint_flags["at"]
-                and checkpoint_flags["seq"]
-                and checkpoint_flags["plus"]
-                and not checkpoint_flags["qual"]
-            ):
-                qual = fix_qual_line(line, checkpoint_flags)
-
-                # Eventually print to file
-                if len(raw_seq) == len(qual) and len(qual) != 0:
-                    print_to_file(header, raw_seq, head_qual_sep, qual, fout)
-                    clean_reads += 1
-                else:
-                    seq_len_neq_qual_len += 1
 
-                reset_flags(checkpoint_flags)
-
-            # unexpected line
+            # PROCESS THE HEADER LINE
+            header: str = check_header_line(line.rstrip())
+            if not header:
+                continue
+
+            # PROCESS THE SEQ LINE
+            line = read_next_line(fin, log_frequency)
+            raw_seq: str = check_seq_line(line.rstrip())
+            if not raw_seq:
+                continue
+
+            # PROCESS the + line
+            line = read_next_line(fin, log_frequency)
+            plus: str = check_plus_line(line.rstrip())
+            if not plus:
+                continue
+
+            # PROCESS the QUAL line
+            line = read_next_line(fin, log_frequency)
+            qual: str = check_qual_line(line.rstrip())
+            if not qual:
+                continue
+
+            # Eventually print to file
+            if len(raw_seq) == len(qual) and len(qual) != 0:
+                print_to_file(header, raw_seq, plus, qual, fout)
+                clean_reads += 1
             else:
-                if (
-                    "@" in line
-                    and not checkpoint_flags["at"]
-                    and not checkpoint_flags["seq"]
-                    and not checkpoint_flags["plus"]
-                    and not checkpoint_flags["qual"]
-                ):
-                    head_print += 1
-                elif (
-                    "@" not in line
-                    and not checkpoint_flags["at"]
-                    and not checkpoint_flags["seq"]
-                    and not checkpoint_flags["plus"]
-                    and not checkpoint_flags["qual"]
-                ):
-                    unexpected_line += 1
-                elif (
-                    checkpoint_flags["at"]
-                    and not checkpoint_flags["seq"]
-                    and not checkpoint_flags["plus"]
-                    and not checkpoint_flags["qual"]
-                ):
-                    seq_odd_chars += 1
-                elif (
-                    checkpoint_flags["at"]
-                    and checkpoint_flags["seq"]
-                    and not checkpoint_flags["plus"]
-                    and not checkpoint_flags["qual"]
-                ):
-                    plus_row += 1
-                elif (
-                    checkpoint_flags["at"]
-                    and checkpoint_flags["seq"]
-                    and checkpoint_flags["plus"]
-                    and not checkpoint_flags["qual"]
-                ):
-                    qual_odd_chars += 1
-                else:
-                    unexpected_line += 1
-
-                reset_flags(checkpoint_flags)
-
-        # All lines that do not refer to any header at the end of the file are considered "unexpected" (1 to 3 lines max)
-        unexpected_line += count_remainder()
+                seq_len_neq_qual_len += 1
 
         fout.close()
         fin.close()
 
         # Print short report
-        click.echo(click.style("Successfully terminated\n", fg="blue"))
+        logging.info("Successfully terminated\n")
 
         if log_out:
             print_log_to_file(log_out)
         else:
             print_log_to_screen()
 
 
 if __name__ == "__main__":
-    wipe_fastq()
+    parser = argparse.ArgumentParser(description='FastqWiper entrypoint')
+    parser.add_argument("-i", '--fastq_in', help='The corrupted FASTQ file', required=True)
+    parser.add_argument("-o", '--fastq_out', help='The wiped FASTQ file', required=True)
+    parser.add_argument("-l", '--log_out', nargs='?',
+                        help='The file name of the final quality report summary. Print on the screen if not specified')
+    parser.add_argument("-f", '--log_frequency', type=int, nargs='?', default=500000, const=500000,
+                        help='The number of reads you want to print a status message. Default: 500000')
+    parser.add_argument("-a", '--alphabet', type=str, nargs='?', default="ACGTN", const="ACGTN",
+                        help='Allowed character in the SEQ line. Default: ACGTN')
+    args = parser.parse_args()
+
+    # Allowed character of the SEQ line
+    reg = re.compile(f"^[{args.alphabet}]+$")
+
+    wipe_fastq(args.fastq_in, args.fastq_out,args.log_out, args.log_frequency)
```

## Comparing `fastqwiper-2024.1.86.dist-info/LICENSE` & `fastqwiper-2024.1.90.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastqwiper-2024.1.86.dist-info/METADATA` & `fastqwiper-2024.1.90.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 Metadata-Version: 2.1
 Name: fastqwiper
-Version: 2024.1.86
-Summary: An ensamble method to recover corrupted FASTQ files, drop or fix pesky lines, remove unpaired reads, and fix reads interleaving
+Version: 2024.1.90
+Summary: An ensemble method to recover corrupted FASTQ files, drop or fix pesky lines, remove unpaired reads, and fix reads interleaving
 Home-page: https://github.com/mazzalab/fastqwiper
 Author: Tommaso Mazza
 Author-email: bioinformatics@css-mendel.it
 License: MIT
 Project-URL: Source, https://github.com/mazzalab/fastqwiper
 Project-URL: Tracker, https://github.com/mazzalab/fastqwiper/issues
 Project-URL: Developmental plan, https://github.com/mazzalab/fastqwiper/projects
 Keywords: genomics,ngs,fastq,bioinformatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
-Requires-Dist: colorama
-Requires-Dist: click
 
 # FastqWiper 
 [![Build](https://github.com/mazzalab/fastqwiper/actions/workflows/buildall_and_publish.yml/badge.svg)](https://github.com/mazzalab/fastqwiper/actions/workflows/buildall_and_publish.yml) [![codecov](https://codecov.io/gh/mazzalab/fastqwiper/graph/badge.svg?token=5V4AQTK619)](https://codecov.io/gh/mazzalab/fastqwiper) [![GitHub issues](https://img.shields.io/github/issues-raw/mazzalab/fastqwiper)](https://github.com/mazzalab/fastqwiper/issues) 
 
 [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/version.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/latest_release_date.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/platforms.svg)](https://anaconda.org/bfxcss/fastqwiper) [![Anaconda-Server Badge](https://anaconda.org/bfxcss/fastqwiper/badges/downloads.svg)](https://anaconda.org/bfxcss/fastqwiper)
 
 [![PyPI version](https://badge.fury.io/py/fastqwiper.svg)](https://badge.fury.io/py/fastqwiper) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/fastqwiper.svg)](https://pypi.python.org/pypi/fastqwiper/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/fastqwiper)
 
 [![Docker](https://badgen.net/badge/icon/docker?icon=docker&label)](https://hub.docker.com/r/mazzalab/fastqwiper) ![Docker Pulls](https://img.shields.io/docker/pulls/mazzalab/fastqwiper)
 
-`FastqWiper` is a Snakemake-enabled application that wipes out bad reads from broken FASTQ files. Additionally, the available and pre-designed Snakemake [workflows](https://github.com/mazzalab/fastqwiper/tree/main/pipeline) allows **recovering** corrupted `fastq.gz`, **dropping** or **fixing** pesky lines, **removing** unpaired reads, and **fixing** reads interleaving.
+`FastqWiper` is a Snakemake-enabled application that wipes out bad reads from broken FASTQ files. Additionally, the available and pre-designed Snakemake [workflows](https://github.com/mazzalab/fastqwiper/tree/main/pipeline) allows **recovering** corrupted `fastq.gz`, **dropping** or **fixing** pesky lines, **removing** unpaired reads, and **settling** reads interleaving.
 
-* Compatibility: Python ≥3.7, <3.11
-* OS: Windows, Linux, Mac OS (Snakemake workflows through Docker for Windows)
+* Compatibility: Python ≥3.7, <3.13
+* OS: Windows, Linux, Mac OS (Snakemake workflows only through Docker for Windows)
 * Contributions: [bioinformatics@css-mendel.it](bioinformatics@css-mendel.it)
 * Docker: https://hub.docker.com/r/mazzalab/fastqwiper
 * Singularity: https://cloud.sylabs.io/library/mazzalab/fastqwiper/fastqwiper.sif
 * Bug report: [https://github.com/mazzalab/fastqwiper/issues](https://github.com/mazzalab/fastqwiper/issues)
 
 
 ## USAGE
-- **Case 1**. You have one or a couple (R1&R2) of **computer readable** FASTQ files which contain pesky, unformatted, uncompliant lines: Use *FastWiper* to clean them;
-- **Case 2**. You have one or a couple (R1&R2) of **computer readable** FASTQ files that you want to drop unpaired reads from or fix reads interleaving: Use the FastqWiper's *Snakemake workflows*;
-- **Case 3**. You have one `fastq.gz` file or a couple (R1&R2) of `fastq.gz` files which are corrupted (**unreadable**) and you want to recover healthy reads and reformat them: Use the FastqWiper's *Snakemake workflows*;
+- <code style="color : greenyellow">**Case 1.**</code>You have one or a couple (R1&R2) of **computer readable** (meaning that the .gz files can be successfully decompressed or that the .fa/.fasta files can be viewed from the beginning to the EOF) FASTQ files which contain pesky, unformatted, uncompliant lines: Use *FastWiper* to clean them;
+- <code style="color : darkorange">**Case 2.**</code>You have one or a couple (R1&R2) of **computer readable** FASTQ files that you want to drop unpaired reads from or fix reads interleaving: Use the FastqWiper's *Snakemake workflows*;
+- <code style="color : orangered">**Case 3.**</code>You have one `fastq.gz` file or a couple (R1&R2) of `fastq.gz` files which are corrupted (**unreadable**, meaning that the .gz files cannot be successfully decompressed) and you want to recover healthy reads and reformat them: Use the FastqWiper's *Snakemake workflows*;
 
 
 ## Installation
-### Case 1
-This requires you to install FastqWiper and therefore does not require you to configure *workflows* also. You can do it for all OSs:
+### <code style="color : greenyellow">Case 1</code>
+This requires you to install FastqWiper and therefore <u>not</u> to use *workflows*. You can do it for all OSs:
 
 #### Use Conda
 
 ```
-conda create -n fastqwiper python=3.10
+conda create -n fastqwiper python=3.11
 conda activate fastqwiper
 conda install -c bfxcss -c conda-forge fastqwiper
 
 fastqwiper --help
 ```
 *Hint: for an healthier experience, use* **mamba**
 
@@ -73,143 +73,146 @@
 fastqwiper --help
 ```
 <br/>
 
 `fastqwiper  <options>`
 ```
 options:
-  --fastq_in TEXT          The input FASTQ file to be cleaned  [required]
-  --fastq_out TEXT         The wiped FASTQ file                [required]
-  --log_frequency INTEGER  The number of reads you want to print a status message
-  --log_out TEXT           The file name of the final quality report summary
-  --help                   Show this message and exit.
+  -i, --fastq_in TEXT          The input FASTQ file to be cleaned  [required]
+  -o, --fastq_out TEXT         The wiped FASTQ file                [required]
+  -l, --log_frequency INTEGER  The number of reads you want to print a status message. Default: 500000
+  -f, --log_out TEXT           The file name of the final quality report summary. Print on the screen if not specified
+  -a, --alphabet               Allowed character in the SEQ line. Default: ACGTN
+  -h, --help                   Show this message and exit.
 ```
-It  accepts in input and outputs **readable** `*.fastq` or `*.fastq.gz` files.
+It accepts strictly **readable** `*.fastq` or `*.fastq.gz` files in input.
 
 
-### Cases 2 & 3
+### <code style="color : darkorange">Case 2</code> & <code style="color : orangered">Case 3</code>
 There are <b>QUICK</b> and a <b>SLOW</b> methods to configure `FastqWiper`'s workflows.
 
 
 #### One quick way (Docker)
 1. Pull the Docker image from DockerHub:
 
 `docker pull mazzalab/fastqwiper`
 
 2. Once downloaded the image, type:
 
-CMD: `docker run --rm -ti --name fastqwiper -v "YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data" mazzalab/fastqwiper paired 8 sample 50000000 33`
+CMD: `docker run --rm -ti --name fastqwiper -v "YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data" mazzalab/fastqwiper paired 8 sample 50000000 33 ACGTN`
 
 #### Another quick way (Singularity)
 1. Pull the Singularity image from the Cloud Library:
 
 `singularity pull library://mazzalab/fastqwiper/fastqwiper.sif`
 
-2. Once downloaded the image (e.g., fastqwiper.sif_2023.2.70.sif), type:
+2. Once downloaded the image (e.g., fastqwiper.sif_2024.1.89.sif), type:
 
-CMD `singularity run --bind /scratch/tom/fastqwiper_singularity/data:/fastqwiper/data --writable-tmpfs fastqwiper.sif_2023.2.70.sif paired 8 sample 50000000 33`
+CMD `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER:/fastqwiper/data --writable-tmpfs fastqwiper.sif_2024.1.89.sif paired 8 sample 50000000 33 ACGTN`
 
 If you want to bind the `.singularity` cache folder and the `logs` folder, you can omit `--writable-tmpfs`, create the folders `.singularity` and `logs` (`mkdir .singularity logs`) on the host system, and use this command instead:
 
-CMD: `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER/:/fastqwiper/data --bind YOUR_LOCAL_PATH_TO_.singularity_FOLDER/:/fastqwiper/.snakemake --bind YOUR_LOCAL_PATH_TO_LOGS_FOLDER/:/fastqwiper/logs fastqwiper.sif_2023.2.70.sif paired 8 sample 50000000 33`
+CMD: `singularity run --bind YOUR_LOCAL_PATH_TO_DATA_FOLDER/:/fastqwiper/data --bind YOUR_LOCAL_PATH_TO_.SNAKEMAKE_FOLDER/:/fastqwiper/.snakemake --bind YOUR_LOCAL_PATH_TO_LOGS_FOLDER/:/fastqwiper/logs fastqwiper.sif_2024.1.89.sif paired 8 sample 50000000 33 ACGTN`
 
 For both **Docker** and **Singularity**:
 
 - `YOUR_LOCAL_PATH_TO_DATA_FOLDER` is the path of the folder where the fastq.gz files to be wiped are located;
 - `paired` triggers the cleaning of R1 and R2. Alternatively, `single` will trigger the wipe of individual FASTQ files;
 - `8` is the number of your choice of computing cores to be spawned;
 - `sample` is part of the names of the FASTQ files to be wiped. <b>Be aware</b> that: for <b>paired-end</b> files (e.g., "sample_R1.fastq.gz" and "sample_R2.fastq.gz"), your files must finish with `_R1.fastq.gz` and `_R2.fastq.gz`. Therefore, the argument to pass is everything before these texts: `sample` in this case. For <b>single end</b>/individual files (e.g., "excerpt_R1_001.fastq.gz"), your file must end with the string `.fastq.gz`; the preceding text, i.e., "excerpt_R1_001" in this case, will be the text to be passed to the command as an argument. 
 - `50000000` (optional) is the number of rows-per-chunk (used when cores>1. It must be a number multiple of 4). Increasing this number too much would reduce the parallelism advantage. Decreasing this number too much would increase the number of chunks more than the number of available cpus, making parallelism unefficient. Choose this number wisely depending on the total number of reads in your starting file.
-- `33` (optional) is the ASCII offset (33=Sanger, 64=old Solexa) 
+- `33` (optional) is the ASCII offset (33=Sanger, 64=old Solexa)
+- `ACGTN` (optional) is the allowed alphabet in the SEQ line of the FASTQ file
 
-#### The slow way (Linux & Mac OS)
+### <code style="color : red">The slow way (Linux & Mac OS)</code>
 To enable the use of preconfigured [pipelines](https://github.com/mazzalab/fastqwiper/tree/main/pipeline), you need to install **Snakemake**. The recommended way to install Snakemake is via Conda, because it enables **Snakemake** to [handle software dependencies of your workflow](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html#integrated-package-management).
 However, the default conda solver is slow and often hangs. Therefore, we recommend installing [Mamba](https://github.com/mamba-org/mamba) as a drop-in replacement via
 
 `$ conda install -c conda-forge mamba`
 
 if you have anaconda/miniconda already installed, or directly installing `Mambaforge` as described [here](https://github.com/conda-forge/miniforge#mambaforge).
 
 
 Then, create and activate a clean environment as above:
 
 ```
-mamba create -n fastqwiper python=3.10
+mamba create -n fastqwiper python=3.11
 mamba activate fastqwiper
 ```
-Finally, install a few dependencies:
+Finally, install the Snakemake dependency:
 
 ```
 $ mamba install -c bioconda snakemake
-$ mamba install colorama click
 ```
 
 
 #### Usage
 Clone the FastqWiper repository in a folder of your choice and enter it:
 
 ```
 git clone https://github.com/mazzalab/fastqwiper.git
 cd fastqwiper
 ```
 
 It contains, in particular, a folder `data` containing the fastq files to be processed, a folder `pipeline` containing the released pipelines and a folder `fastq_wiper` with the source files of `FastqWiper`. <br/>
-Input files to be processed should be copied into the **data** folder.
+Input files to be processed must be copied into the **data** folder.
 
 Currently, to run the `FastqWiper` pipelines, the following packages need to be installed manually:
 
 ### required packages:
-[gzrt](https://github.com/arenn/gzrt) (Linux build fron source [instructions](https://github.com/arenn/gzrt/blob/master/README.build), Ubuntu install [instructions](https://howtoinstall.co/en/gzrt), Mac OS install [instructions](https://formulae.brew.sh/formula/gzrt))
+[gzrt](https://github.com/arenn/gzrt) (Linux build from source [instructions](https://github.com/arenn/gzrt/blob/master/README.build), Ubuntu install [instructions](https://howtoinstall.co/en/gzrt), Mac OS install [instructions](https://formulae.brew.sh/formula/gzrt))
 
 [BBTools](https://jgi.doe.gov/data-and-tools/software-tools/bbtools/) (install [instructions](https://jgi.doe.gov/data-and-tools/software-tools/bbtools/bb-tools-user-guide/installation-guide/))
 
 If installed from source, `gzrt` scripts need to be put on PATH. `bbmap` must be installed in the root folder of FastqWiper, as the image below
 
 ![FastqWiper folder yierarchy](assets/hierarchy.png)
 
 ### Commands:
 Copy the fastq files you want to fix in the `data` folder.
-**N.b.**: In all commands above, you will pass to the workflow the name of the sample to be analyzed through the config argument: `sample_name`. Remember that your fastq files' names must finish with `_R1.fastq.gz` and `_R2.fastq.gz`, for paired fastq files, and with `.fastq.gz`, for individual fastq files, and, therefore, the text to be assigned to the variable `sample_name` must be everything before them. E.g., if your files are `my_sample_R1.fastq.gz` and `my_sample_R2.fastq.gz`, then `--config sample_name=my_sample`.
+
+<code style="color : orange">**N.b.**: In all commands above, you will pass the name of the sample to be analyzed to the workflow through the config argument: `sample_name`. Remember that your fastq files' names must finish with `_R1.fastq.gz` and `_R2.fastq.gz`, for paired fastq files, and with `.fastq.gz`, for individual fastq files, and, therefore, the text to be assigned to the variable `sample_name` must be everything before them. E.g., if your files are `my_sample_R1.fastq.gz` and `my_sample_R2.fastq.gz`, then `--config sample_name=my_sample`.</code>
+
 
 #### Paired-end files
 
 - **Get a dry run** of a pipeline (e.g., `fix_wipe_pairs_reads_sequential.smk`):<br />
-`snakemake --config sample_name=my_sample qin=33 -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 4`
+`snakemake --config sample_name=my_sample qin=33 alphabet=ACGTN -s pipeline/fix_wipe_pairs_reads_sequential.smk --use-conda --cores 4`
 
 - **Generate the planned DAG**:<br />
-`snakemake --config sample_name=my_sample qin=33 -s pipeline/fix_wipe_pairs_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /> <br />
+`snakemake --config sample_name=my_sample qin=33 alphabet=ACGTN -s pipeline/fix_wipe_pairs_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /> <br />
 <img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_pairs_reads.png?raw=true" width="400">
 
 - **Run the pipeline** (n.b., during the first execution, Snakemake will download and install some required remote packages and may take longer). The number of computing cores can be tuned accordingly:<br />
-`snakemake --config sample_name=my_sample qin=33 -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
+`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
 
 Fixed files will be copied in the `data` folder and will be suffixed with the string `_fixed_wiped_paired_interleaving`.
 We remind that the `fix_wipe_pairs_reads_sequential.smk` and `fix_wipe_pairs_reads_parallel.smk` pipelines perform the following actions:
 - execute `gzrt` on corrupted fastq.gz files (i.e., that cannot be unzipped because of errors) and recover readable reads;
 - execute `FastqWiper` on recovered reads to make them compliant with the FASTQ format (source: [Wipipedia](https://en.wikipedia.org/wiki/FASTQ_format))
 - execute `Trimmomatic` on wiped reads to remove residual unpaired reads
 - execute `BBmap (repair.sh)` on paired reads to fix the correct interleaving and sort fastq files.  
 
 #### Single-end files
 `fix_wipe_single_reads_parallel.smk` and `fix_wipe_single_reads_sequential.smk` will not execute `trimmomatic` and BBmap's `repair.sh`.
 
 - **Get a dry run** of a pipeline (e.g., `fix_wipe_single_reads_sequential.smk`):<br />
-`snakemake --config sample_name=my_sample -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2 -np`
+`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2 -np`
 
 - **Generate the planned DAG**:<br />
-`snakemake --config sample_name=my_sample -s pipeline/fix_wipe_single_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /><br />
+`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --dag | dot -Tpdf > dag.pdf`<br /><br />
 <img src="https://github.com/mazzalab/fastqwiper/blob/main/pipeline/fix_wipe_single_reads.png?raw=true" width="200">
 
 - **Run the pipeline** (n.b., The number of computing cores can be tuned accordingly):<br />
-`snakemake --config sample_name=my_sample -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
+`snakemake --config sample_name=my_sample alphabet=ACGTN -s pipeline/fix_wipe_single_reads_sequential.smk --use-conda --cores 2`
 
 # Author
 **Tommaso Mazza**  
-[![Tweeting](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/irongraft)
+[![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=X&logoColor=white)](https://twitter.com/irongraft) [![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/tommasomazza/)
 
 Laboratory of Bioinformatics</br>
 Fondazione IRCCS Casa Sollievo della Sofferenza</br>
 Viale Regina Margherita 261 - 00198 Roma IT</br>
 Tel: +39 06 44160526 - Fax: +39 06 44160548</br>
-E-mail: t.mazza@css-mendel.it</br>
+E-mail: t.mazza@operapadrepio.it</br>
 Web page: http://www.css-mendel.it</br>
 Web page: http://bioinformatics.css-mendel.it</br>
```

## Comparing `fastqwiper-2024.1.86.dist-info/RECORD` & `fastqwiper-2024.1.90.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-fastq_wiper/__init__.py,sha256=Vw6SSLfa_80p9bStBwVJyuvMW9H71om0lYFdWiIKrnk,1898
-fastq_wiper/color_log_formatter.py,sha256=mt7wZ2t4urWy6AiGXOZUEYDfDqckF4resxO2NJbKhzY,2078
-fastq_wiper/wiper.py,sha256=s4ZIKFoeAyVl5RXrrrmDAtrKNaJ-GbFp8OS74hV6UTs,12820
+fastq_wiper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fastq_wiper/wiper.py,sha256=VW2w-TjE_EZnxF7djWepATjl6-3ll1Iy2dmZSuJ0QiE,9984
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_wiper.py,sha256=SC8gElm6F6E1SXnPHGSznduT7T03E5u5G82btLjMzMc,816
-fastqwiper-2024.1.86.dist-info/LICENSE,sha256=DWt8ibsIVfsr_QsQ8XUkSM5hf5T0TJRHUc350xWkcdM,7601
-fastqwiper-2024.1.86.dist-info/METADATA,sha256=q8ED3xrImOx1ZegzmBiKe3XwZsbKSdd8elP0pVv8AB8,13353
-fastqwiper-2024.1.86.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-fastqwiper-2024.1.86.dist-info/entry_points.txt,sha256=4tbn0oF9lACKncVCqCsYTIYqyo0TGQuFv0KCzgdJX4A,60
-fastqwiper-2024.1.86.dist-info/top_level.txt,sha256=PoRVateDzVx-xrn4iraE8TOWCGvtsEwbaM97BHkr6bU,18
-fastqwiper-2024.1.86.dist-info/RECORD,,
+fastqwiper-2024.1.90.dist-info/LICENSE,sha256=DWt8ibsIVfsr_QsQ8XUkSM5hf5T0TJRHUc350xWkcdM,7601
+fastqwiper-2024.1.90.dist-info/METADATA,sha256=o_-lPokqK-KW92U3-kPbQzBVFqAGXuSU5r1RDzqyFWU,14374
+fastqwiper-2024.1.90.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+fastqwiper-2024.1.90.dist-info/entry_points.txt,sha256=4tbn0oF9lACKncVCqCsYTIYqyo0TGQuFv0KCzgdJX4A,60
+fastqwiper-2024.1.90.dist-info/top_level.txt,sha256=PoRVateDzVx-xrn4iraE8TOWCGvtsEwbaM97BHkr6bU,18
+fastqwiper-2024.1.90.dist-info/RECORD,,
```

