# Comparing `tmp/quantify-core-0.7.4.tar.gz` & `tmp/quantify_core-0.7.6.dev0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantify-core-0.7.4.tar", last modified: Fri Dec 15 16:23:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

