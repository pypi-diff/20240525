# Comparing `tmp/pkscreener-0.45.20240523.401.tar.gz` & `tmp/pkscreener-0.45.20240525.406-cp311-cp311-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240523.401.tar", last modified: Thu May 23 19:46:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

