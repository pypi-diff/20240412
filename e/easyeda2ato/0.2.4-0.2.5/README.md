# Comparing `tmp/easyeda2ato-0.2.4.tar.gz` & `tmp/easyeda2ato-0.2.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyeda2ato-0.2.4.tar", last modified: Thu Apr 11 18:25:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

