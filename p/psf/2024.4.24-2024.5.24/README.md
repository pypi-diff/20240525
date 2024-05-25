# Comparing `tmp/psf-2024.4.24.tar.gz` & `tmp/psf-2024.5.24-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psf-2024.4.24.tar", last modified: Fri Apr 26 23:38:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

