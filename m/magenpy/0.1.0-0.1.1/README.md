# Comparing `tmp/magenpy-0.1.0.tar.gz` & `tmp/magenpy-0.1.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magenpy-0.1.0.tar", last modified: Fri Apr  5 00:48:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

