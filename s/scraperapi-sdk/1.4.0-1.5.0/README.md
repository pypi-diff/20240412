# Comparing `tmp/scraperapi_sdk-1.4.0.tar.gz` & `tmp/scraperapi_sdk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraperapi_sdk-1.4.0.tar", max compression
+gzip compressed data, was "scraperapi_sdk-1.5.0.tar", max compression
```

## Comparing `scraperapi_sdk-1.4.0.tar` & `scraperapi_sdk-1.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6889 2024-04-09 08:05:37.432469 scraperapi_sdk-1.4.0/README.md
--rw-r--r--   0        0        0      713 2024-04-09 08:06:03.554654 scraperapi_sdk-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      195 2024-04-09 08:05:37.432747 scraperapi_sdk-1.4.0/scraperapi_sdk/__init__.py
--rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.4.0/scraperapi_sdk/__version__.py
--rw-r--r--   0        0        0     7687 2024-04-09 08:05:37.433102 scraperapi_sdk-1.4.0/scraperapi_sdk/_client.py
--rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.4.0/scraperapi_sdk/exceptions.py
--rw-r--r--   0        0        0     7398 1970-01-01 00:00:00.000000 scraperapi_sdk-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    13602 2024-04-12 08:48:46.591955 scraperapi_sdk-1.5.0/README.md
+-rw-r--r--   0        0        0      713 2024-04-12 08:54:02.415986 scraperapi_sdk-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      195 2024-04-09 08:05:37.432747 scraperapi_sdk-1.5.0/scraperapi_sdk/__init__.py
+-rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.5.0/scraperapi_sdk/__version__.py
+-rw-r--r--   0        0        0    22915 2024-04-12 08:18:56.293477 scraperapi_sdk-1.5.0/scraperapi_sdk/_client.py
+-rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.5.0/scraperapi_sdk/exceptions.py
+-rw-r--r--   0        0        0    14111 1970-01-01 00:00:00.000000 scraperapi_sdk-1.5.0/PKG-INFO
```

### Comparing `scraperapi_sdk-1.4.0/pyproject.toml` & `scraperapi_sdk-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scraperapi-sdk"
-version = "1.4.0"
+version = "1.5.0"
 description = "ScraperAPI Python SDK"
 authors = ["ScraperAPI"]
 readme = "README.md"
 
 [project]
 requires-python = ">= 3.8"
```

