# Comparing `tmp/mypy-boto3-cloudformation-1.34.77.tar.gz` & `tmp/mypy_boto3_cloudformation-1.34.84-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.34.77.tar", last modified: Wed Apr  3 19:32:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

