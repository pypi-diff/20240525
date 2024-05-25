# Comparing `tmp/pproject-0.0.1.tar.gz` & `tmp/pproject-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pproject-0.0.1.tar", last modified: Sat May 25 15:10:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

