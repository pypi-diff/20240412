# Comparing `tmp/chikvdf-1.1.2.tar.gz` & `tmp/chikvdf-1.1.3-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chikvdf-1.1.2.tar", last modified: Mon Feb 26 06:11:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

