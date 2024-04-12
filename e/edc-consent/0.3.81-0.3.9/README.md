# Comparing `tmp/edc-consent-0.3.81.tar.gz` & `tmp/edc_consent-0.3.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-consent-0.3.81.tar", last modified: Fri Apr 12 15:28:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

