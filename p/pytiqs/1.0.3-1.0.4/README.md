# Comparing `tmp/pytiqs-1.0.3.tar.gz` & `tmp/pytiqs-1.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytiqs-1.0.3.tar", last modified: Wed Apr 10 04:20:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

