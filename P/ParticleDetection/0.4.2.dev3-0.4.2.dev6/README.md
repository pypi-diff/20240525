# Comparing `tmp/particledetection-0.4.2.dev3.tar.gz` & `tmp/particledetection-0.4.2.dev6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "particledetection-0.4.2.dev3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

