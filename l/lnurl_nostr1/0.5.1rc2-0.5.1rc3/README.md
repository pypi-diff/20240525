# Comparing `tmp/lnurl_nostr1-0.5.1rc2.tar.gz` & `tmp/lnurl_nostr1-0.5.1rc3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnurl_nostr1-0.5.1rc2.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

