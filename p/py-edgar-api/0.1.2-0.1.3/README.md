# Comparing `tmp/py_edgar_api-0.1.2.tar.gz` & `tmp/py_edgar_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_edgar_api-0.1.2.tar", max compression
+gzip compressed data, was "py_edgar_api-0.1.3.tar", max compression
```

## Comparing `py_edgar_api-0.1.2.tar` & `py_edgar_api-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       36 2024-04-11 17:47:49.705998 py_edgar_api-0.1.2/README.md
--rw-r--r--   0        0        0       48 2024-04-11 17:44:22.068498 py_edgar_api-0.1.2/py_edgar_api/__init__.py
--rw-r--r--   0        0        0      149 2024-04-11 05:42:08.861786 py_edgar_api-0.1.2/py_edgar_api/client.py
--rw-r--r--   0        0        0      300 2024-04-11 17:47:59.958332 py_edgar_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      406 1970-01-01 00:00:00.000000 py_edgar_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2024-04-11 17:47:49.705998 py_edgar_api-0.1.3/README.md
+-rw-r--r--   0        0        0       88 2024-04-12 03:48:41.010748 py_edgar_api-0.1.3/py_edgar_api/__init__.py
+-rw-r--r--   0        0        0     1279 2024-04-12 04:04:23.132757 py_edgar_api-0.1.3/py_edgar_api/client.py
+-rw-r--r--   0        0        0      190 2024-04-12 04:01:24.187947 py_edgar_api-0.1.3/py_edgar_api/company.py
+-rw-r--r--   0        0        0      321 2024-04-12 03:58:57.992494 py_edgar_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 py_edgar_api-0.1.3/PKG-INFO
```

