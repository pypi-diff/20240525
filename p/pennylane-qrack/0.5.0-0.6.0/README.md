# Comparing `tmp/pennylane-qrack-0.5.0.tar.gz` & `tmp/pennylane_qrack-0.6.0-cp312-cp312-manylinux_2_39_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-qrack-0.5.0.tar", last modified: Fri Dec  1 20:15:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

