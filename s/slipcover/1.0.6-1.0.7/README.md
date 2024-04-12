# Comparing `tmp/slipcover-1.0.6.tar.gz` & `tmp/slipcover-1.0.7-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slipcover-1.0.6.tar", last modified: Tue Apr  9 23:43:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

