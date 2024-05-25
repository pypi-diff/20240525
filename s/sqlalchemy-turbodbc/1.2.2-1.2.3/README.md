# Comparing `tmp/sqlalchemy_turbodbc-1.2.2.tar.gz` & `tmp/sqlalchemy_turbodbc-1.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_turbodbc-1.2.2.tar", last modified: Sat Apr 29 15:28:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

