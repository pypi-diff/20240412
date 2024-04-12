# Comparing `tmp/botocore-a-la-carte-timestream-influxdb-1.34.82.tar.gz` & `tmp/botocore_a_la_carte_timestream_influxdb-1.34.83-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-timestream-influxdb-1.34.82.tar", last modified: Thu Apr 11 01:01:11 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

