# Comparing `tmp/absfuyu-3.3.1.tar.gz` & `tmp/absfuyu-3.3.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absfuyu-3.3.1.tar", last modified: Fri Apr  5 15:56:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

