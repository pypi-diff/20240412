# Comparing `tmp/sdwi2iextender-0.1.1.tar.gz` & `tmp/sdwi2iextender-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdwi2iextender-0.1.1.tar", last modified: Mon Apr  8 23:15:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

