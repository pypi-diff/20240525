# Comparing `tmp/elucidoc-2024.5.17.tar.gz` & `tmp/elucidoc-2024.5.25-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elucidoc-2024.5.17.tar", last modified: Fri May 17 13:07:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

