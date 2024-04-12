# Comparing `tmp/gpt-researcher-0.2.2.tar.gz` & `tmp/gpt_researcher-0.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.2.2.tar", last modified: Fri Apr 12 13:20:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

