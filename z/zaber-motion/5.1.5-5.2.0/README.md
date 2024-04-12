# Comparing `tmp/zaber_motion-5.1.5.tar.gz` & `tmp/zaber_motion-5.2.0-py3-none-manylinux_2_27_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-5.1.5.tar", last modified: Wed Mar 13 21:17:59 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

