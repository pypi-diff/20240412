# Comparing `tmp/denmanlab-0.3.tar.gz` & `tmp/denmanlab-0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmanlab-0.3.tar", last modified: Wed Nov  2 22:25:16 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

