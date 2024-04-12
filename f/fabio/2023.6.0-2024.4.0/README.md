# Comparing `tmp/fabio-2023.6.0.tar.gz` & `tmp/fabio-2024.4.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabio-2023.6.0.tar", last modified: Wed Jun 21 11:33:17 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

