# Comparing `tmp/runes-client-0.8.3.tar.gz` & `tmp/runes_client-0.8.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-client-0.8.3.tar", last modified: Tue Apr  9 03:35:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
