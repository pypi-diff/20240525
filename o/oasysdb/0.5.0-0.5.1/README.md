# Comparing `tmp/oasysdb-0.5.0.tar.gz` & `tmp/oasysdb-0.5.1-cp310-cp310-macosx_10_12_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

