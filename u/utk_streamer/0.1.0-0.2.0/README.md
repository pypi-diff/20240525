# Comparing `tmp/utk_streamer-0.1.0.tar.gz` & `tmp/utk_streamer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_streamer-0.1.0.tar", max compression
+gzip compressed data, was "utk_streamer-0.2.0.tar", max compression
```

## Comparing `utk_streamer-0.1.0.tar` & `utk_streamer-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      541 2024-05-23 18:01:31.547727 utk_streamer-0.1.0/README.md
--rw-r--r--   0        0        0      481 2024-05-23 17:40:10.361499 utk_streamer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-23 17:23:53.157452 utk_streamer-0.1.0/utk_streamer/__init__.py
--rw-r--r--   0        0        0       70 2024-05-23 17:23:53.155525 utk_streamer-0.1.0/utk_streamer/download/__init__.py
--rw-r--r--   0        0        0      258 2024-05-23 17:40:53.088674 utk_streamer-0.1.0/utk_streamer/download/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1691 2024-05-23 17:40:53.090115 utk_streamer-0.1.0/utk_streamer/download/__pycache__/download.cpython-312.pyc
--rw-r--r--   0        0        0      571 2024-05-23 17:23:53.153071 utk_streamer-0.1.0/utk_streamer/download/download.py
--rw-r--r--   0        0        0     1237 2024-05-23 17:58:50.888832 utk_streamer-0.1.0/utk_streamer/streamer.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 utk_streamer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      624 2024-05-25 04:46:34.390014 utk_streamer-0.2.0/README.md
+-rw-r--r--   0        0        0      497 2024-05-25 04:46:50.276792 utk_streamer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-25 04:32:52.425650 utk_streamer-0.2.0/utk_streamer/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-25 04:32:52.421328 utk_streamer-0.2.0/utk_streamer/convert/__init__.py
+-rw-r--r--   0        0        0     1294 2024-05-25 04:30:44.929442 utk_streamer-0.2.0/utk_streamer/convert/convert.py
+-rw-r--r--   0        0        0       70 2024-05-23 17:23:53.155525 utk_streamer-0.2.0/utk_streamer/download/__init__.py
+-rw-r--r--   0        0        0      596 2024-05-24 00:54:47.468555 utk_streamer-0.2.0/utk_streamer/download/download.py
+-rw-r--r--   0        0        0     2209 2024-05-25 04:44:46.682350 utk_streamer-0.2.0/utk_streamer/streamer.py
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 utk_streamer-0.2.0/PKG-INFO
```

### Comparing `utk_streamer-0.1.0/README.md` & `utk_streamer-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,15 @@
 Because multiple files can exist in a row, this doesn't align to rows but the range of files to download.
 
 For instance, to download the first 10 files and your csv is called `example.csv`:
 
 ```shell
 
 streamer download -c example.csv -o output -s 1 -e 10
+```
+
+To convert TTAFS to VTTS, use:
+
+```shell
+
+streamer convert -p /path/to/ttafs 
 ```
```

### Comparing `utk_streamer-0.1.0/utk_streamer/download/download.py` & `utk_streamer-0.2.0/utk_streamer/download/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,10 +12,10 @@
         if not os.path.exists(self.download_path):
             os.makedirs(self.download_path)
         return
 
     def download(self):
         r = requests.get(self.path)
         filename = f"{self.path.split('/')[-2]}_{self.path.split('/')[-1]}"
-        with open(filename, 'wb') as f:
+        with open(f"{self.download_path}/{filename}", 'wb') as f:
             f.write(r.content)
-        return
+        return
```

### Comparing `utk_streamer-0.1.0/utk_streamer/streamer.py` & `utk_streamer-0.2.0/utk_streamer/streamer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import click
 from utk_streamer.download import StreamerDownload
+from utk_streamer.convert import TTAFConverter
 from csv import DictReader
 from tqdm import tqdm
+import os
 
 
 @click.group()
 def cli() -> None:
     pass
 
 @cli.command("download", help="Download multiple files from a Spreadsheet")
@@ -45,8 +47,41 @@
         for row in rows:
             in_row  = row.split(" | ")
             for file in in_row:
                 all_files.append(file)
         print(f"Downloading files {start} to {end} to {output}.")
         for row in tqdm(all_files[int(start):int(end)]):
             StreamerDownload(row, output).download()
-    return
+    return
+
+@cli.command("get_captions", help="Download captions")
+@click.option(
+    "--captions_sheet",
+    "-c",
+    required=True,
+    help="Path to text file with captions",
+)
+def get_captions(
+    captions_sheet: str,
+) -> None:
+    with open(captions_sheet, "r") as file:
+        captions = file.readlines()
+        for caption in tqdm(captions):
+            path = f"http://streamer-migration.lib.utk.edu/files/catstream/{caption.replace('./', '').strip()}"
+            StreamerDownload(path, "captions").download()
+    return
+
+@cli.command("convert", help="Convert TTAF to VTT")
+@click.option(
+    "--path",
+    "-p",
+    required=True,
+    help="Path to TTAFS",
+)
+def convert(
+    path: str
+) -> None:
+    print(f"Converting TTAFS to VTT at {path}")
+    for path_on_disk, directories, files in os.walk(path):
+        for file in tqdm(files):
+            x = TTAFConverter(f"{path}/{file}")
+            x.write_vtt()
```

### Comparing `utk_streamer-0.1.0/PKG-INFO` & `utk_streamer-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: utk_streamer
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple utility to download multiple files from a sheet at once
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: lxml (>=5.2.2,<6.0.0)
 Requires-Dist: requests (>=2.32.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Streamer Download
 
 Tool to easily download multiple files from streamer.
@@ -36,7 +37,14 @@
 
 For instance, to download the first 10 files and your csv is called `example.csv`:
 
 ```shell
 
 streamer download -c example.csv -o output -s 1 -e 10
 ```
+
+To convert TTAFS to VTTS, use:
+
+```shell
+
+streamer convert -p /path/to/ttafs 
+```
```

