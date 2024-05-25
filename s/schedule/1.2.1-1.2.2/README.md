# Comparing `tmp/schedule-1.2.1.tar.gz` & `tmp/schedule-1.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedule-1.2.1.tar", last modified: Sun Oct  1 13:52:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

