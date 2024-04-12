# Comparing `tmp/b2sim-2.1.2.tar.gz` & `tmp/b2sim-2.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-2.1.2.tar", last modified: Sun Mar 17 04:25:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

