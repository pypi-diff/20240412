# Comparing `tmp/geventhttpclient-2.1.1.tar.gz` & `tmp/geventhttpclient-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventhttpclient-2.1.1.tar", last modified: Thu Apr 11 06:49:11 2024, max compression
+gzip compressed data, was "geventhttpclient-2.2.0.tar", last modified: Fri Apr 12 15:24:34 2024, max compression
```

## Comparing `geventhttpclient-2.1.1.tar` & `geventhttpclient-2.2.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/ext/Python_compat.h
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/ext/_parser.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/llhttp/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/LICENSE-MIT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/llhttp/include/
--rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/include/llhttp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/llhttp/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/src/api.c
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/src/http.c
--rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-11 06:49:05.000000 geventhttpclient-2.1.1/llhttp/src/llhttp.c
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.817892 geventhttpclient-2.1.1/src/geventhttpclient/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/connectionpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/src/geventhttpclient/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/oncert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/server.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/server.key
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_http_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_httplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_network_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_no_module_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/tests/test_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/url.py
--rw-r--r--   0 runner    (1001) docker     (127)    20094 2024-04-11 06:49:04.000000 geventhttpclient-2.1.1/src/geventhttpclient/useragent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:49:11.821892 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 06:49:11.000000 geventhttpclient-2.1.1/src/geventhttpclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/ext/Python_compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/ext/_parser.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/llhttp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/LICENSE-MIT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/llhttp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    16417 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/include/llhttp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/llhttp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/src/http.c
+-rw-r--r--   0 runner    (1001) docker     (127)   470541 2024-04-12 15:24:27.000000 geventhttpclient-2.2.0/llhttp/src/llhttp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.086324 geventhttpclient-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.090324 geventhttpclient-2.2.0/src/geventhttpclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/connectionpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/src/geventhttpclient/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/oncert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/server.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/server.key
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8650 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_http_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_httplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_httplib2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_network_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_no_module_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20093 2024-04-12 15:24:26.000000 geventhttpclient-2.2.0/src/geventhttpclient/useragent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:24:34.094324 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 15:24:34.000000 geventhttpclient-2.2.0/src/geventhttpclient.egg-info/top_level.txt
```

### Comparing `geventhttpclient-2.1.1/LICENSE.txt` & `geventhttpclient-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/PKG-INFO` & `geventhttpclient-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.1.1
+Version: 2.2.0
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
 License: Based on llhttp, copyright Fedor Indutny, 2018.
         
         Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
         licensed under the same terms.
         
@@ -58,14 +58,16 @@
 Requires-Dist: dpkt; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Provides-Extra: benchmarks
 Requires-Dist: requests; extra == "benchmarks"
 Requires-Dist: httpx; extra == "benchmarks"
 Requires-Dist: urllib3; extra == "benchmarks"
 Requires-Dist: httplib2; extra == "benchmarks"
+Provides-Extra: examples
+Requires-Dist: oauth2; extra == "examples"
 
 [![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/geventhttpclient/geventhttpclient/test.yml?branch=master&logo=github&style=flat)](https://github.com/geventhttpclient/geventhttpclient/actions)
 [![PyPI](https://img.shields.io/pypi/v/geventhttpclient.svg?style=flat)](https://pypi.org/project/geventhttpclient/)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fgeventhttpclient%2Fgeventhttpclient%2Fmaster%2Fpyproject.toml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/geventhttpclient)
 
 # geventhttpclient
@@ -222,17 +224,20 @@
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
 The benchmark does 10000 get requests against a local nginx server in the default 
 configuration with a concurrency of 10. See `benchmarks` folder. The requests per
-second for a couple of popular clients is given in the table below.
-
-| HTTP Client          | RPS    |
-|----------------------|--------|
-| GeventHTTPClient     | 7181.2 |
-| Urllib3              | 2847.5 |
-| Httpx                | 1682.9 |
-| Requests             | 1186.4 |
+second for a couple of popular clients is given in the table below. Please read
+[benchmarks/README.md](https://github.com/geventhttpclient/geventhttpclient/blob/master/benchmarks/README.md)
+for mor details. Also note, HTTPX is better be used with asyncio, not gevent.
+
+| HTTP Client        | RPS    |
+|--------------------|--------|
+| GeventHTTPClient   | 7268.9 |
+| Httplib2 (patched) | 2323.9 |
+| Urllib3            | 2242.5 |
+| Requests           | 1046.1 |
+| Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
```

### Comparing `geventhttpclient-2.1.1/README.md` & `geventhttpclient-2.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -157,17 +157,20 @@
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
 The benchmark does 10000 get requests against a local nginx server in the default 
 configuration with a concurrency of 10. See `benchmarks` folder. The requests per
-second for a couple of popular clients is given in the table below.
+second for a couple of popular clients is given in the table below. Please read
+[benchmarks/README.md](https://github.com/geventhttpclient/geventhttpclient/blob/master/benchmarks/README.md)
+for mor details. Also note, HTTPX is better be used with asyncio, not gevent.
 
-| HTTP Client          | RPS    |
-|----------------------|--------|
-| GeventHTTPClient     | 7181.2 |
-| Urllib3              | 2847.5 |
-| Httpx                | 1682.9 |
-| Requests             | 1186.4 |
+| HTTP Client        | RPS    |
+|--------------------|--------|
+| GeventHTTPClient   | 7268.9 |
+| Httplib2 (patched) | 2323.9 |
+| Urllib3            | 2242.5 |
+| Requests           | 1046.1 |
+| Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
```

### Comparing `geventhttpclient-2.1.1/ext/_parser.c` & `geventhttpclient-2.2.0/ext/_parser.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/llhttp/LICENSE-MIT` & `geventhttpclient-2.2.0/llhttp/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/llhttp/include/llhttp.h` & `geventhttpclient-2.2.0/llhttp/include/llhttp.h`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/llhttp/src/api.c` & `geventhttpclient-2.2.0/llhttp/src/api.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/llhttp/src/http.c` & `geventhttpclient-2.2.0/llhttp/src/http.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/llhttp/src/llhttp.c` & `geventhttpclient-2.2.0/llhttp/src/llhttp.c`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/pyproject.toml` & `geventhttpclient-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "geventhttpclient"
-version = "2.1.1" # dont forget to update version __init__.py as well
+version = "2.2.0" # dont forget to update version __init__.py as well
 description = "HTTP client library for gevent"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 keywords = ["http", "gevent", "client"]
 authors = [{name = "Antonin Amand", email = "antonin.amand@gmail.com"}]
 classifiers = [
@@ -36,16 +36,20 @@
     "dpkt",
     "requests",
 ]
 optional-dependencies.benchmarks = [
     "requests",
     "httpx",
     "urllib3",
-    "httplib2"
+    "httplib2",
 ]
+optional-dependencies.examples = [
+    "oauth2",
+]
+
 
 [project.urls]
 homepage = "http://github.com/geventhttpclient/geventhttpclient"
 issues = "http://github.com/geventhttpclient/geventhttpclient/issues"
 download = "https://pypi.org/project/geventhttpclient/#files"
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/client.py` & `geventhttpclient-2.2.0/src/geventhttpclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         insecure=False,
         proxy_host=None,
         proxy_port=None,
         version=HTTP_11,
         headers_type=Headers,
     ):
         if headers is None:
-            headers = {}
+            headers = headers_type()
         self.host = host
         self.port = port
         connection_host = self.host
         connection_port = self.port
         if proxy_host is not None:
             assert proxy_port is not None, "you have to provide proxy_port if you set proxy_host"
             self.use_proxy = True
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/connectionpool.py` & `geventhttpclient-2.2.0/src/geventhttpclient/connectionpool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from contextlib import contextmanager
 
 import gevent.queue
 import gevent.socket
 from gevent import lock
 
 _CA_CERTS = None
 
@@ -180,16 +181,29 @@
             sock.close()
         except:
             pass
         if not self._closed:
             self._semaphore.release()
 
 
+def init_ssl_context(ssl_context_factory, ca_certs, check_hostname=True):
+    try:
+        ssl_context = ssl_context_factory(cafile=ca_certs)
+    except TypeError:
+        ssl_context = ssl_context_factory()
+        ssl_context.load_verify_locations(cafile=ca_certs)
+    ssl_context.check_hostname = check_hostname
+    if check_hostname:
+        ssl_context.verify_mode = gevent.ssl.CERT_REQUIRED
+    return ssl_context
+
+
 try:
     import gevent.ssl
+
     try:
         from gevent.ssl import create_default_context
     except ImportError:
         create_default_context = None
 except ImportError:
     pass
 else:
@@ -224,30 +238,52 @@
             self.insecure = insecure
 
             self.ssl_options = self.default_options.copy()
             self.ssl_options.update(ssl_options or {})
 
             ssl_context_factory = ssl_context_factory or create_default_context
             if ssl_context_factory is not None:
-                self.init_ssl_context(ssl_context_factory)
+                self.ssl_context = init_ssl_context(
+                    ssl_context_factory,
+                    self.ssl_options["ca_certs"],
+                    check_hostname=not self.insecure,
+                )
             else:
                 self.ssl_context = None
 
             super().__init__(connection_host, connection_port, request_host, request_port, **kw)
 
-        def init_ssl_context(self, ssl_context_factory):
-            ca_certs = self.ssl_options["ca_certs"]
-            try:
-                self.ssl_context = ssl_context_factory(cafile=ca_certs)
-            except TypeError:
-                self.ssl_context = ssl_context_factory()
-                self.ssl_context.load_verify_locations(cafile=ca_certs)
-            self.ssl_context.check_hostname = not self.insecure
-
         def _connect_socket(self, sock, address):
             sock = super()._connect_socket(sock, address)
 
             if self.ssl_context is None:
                 return gevent.ssl.wrap_socket(sock, **self.ssl_options)
             else:
                 server_hostname = self.ssl_options.get("server_hostname", self._request_host)
                 return self.ssl_context.wrap_socket(sock, server_hostname=server_hostname)
+
+
+class ClientPool:
+    """
+    Pool implementation for HTTP clients, that weren't designed with concurrency in mind.
+    Usage example:
+
+    pool = ClientPool(MyHttpClient)
+    with pool.get() as client:
+        response = client.request("127.0.0.1")
+    """
+
+    def __init__(self, factory, concurrency=5):
+        self.factory = factory
+        self.queue = gevent.queue.Queue(concurrency)
+        for i in range(concurrency):
+            self.queue.put(factory())
+
+    @contextmanager
+    def get(self):
+        client = self.queue.get()
+        yield client
+        self.queue.put(client)
+
+    def close(self):
+        for client in self.queue:
+            client.close()
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/response.py` & `geventhttpclient-2.2.0/src/geventhttpclient/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,31 +43,30 @@
 
     def get(self, key, default=None):
         return self._headers_index.get(key, default)
 
     def items(self):
         return self._headers_index.items()
 
+    headers = property(items)
+
     def info(self):
-        """Basic cookielib compatibility"""
         return self._headers_index
 
+    def __contains__(self, key):
+        return key in self._headers_index
+
     def should_close(self):
         """return if we should close the connection.
 
         It is not the opposite of should_keep_alive method. It also checks
         that the body as been consumed completely.
         """
         return not self.message_complete or self.parser_failed() or not super().should_keep_alive()
 
-    headers = property(items)
-
-    def __contains__(self, key):
-        return key in self._headers_index
-
     @property
     def status_code(self):
         return self.get_code()
 
     @property
     def content_length(self):
         length = self.get("content-length", None)
@@ -133,16 +132,18 @@
     def __repr__(self):
         return f"<{self.__class__.__name__} status={self.status_code} headers={dict(self.headers)}>"
 
 
 class HTTPSocketResponse(HTTPResponse):
     DEFAULT_BLOCK_SIZE = 1024 * 4  # 4KB
 
-    def __init__(self, sock, block_size=DEFAULT_BLOCK_SIZE, method="GET", **kw):
-        super().__init__(method=method, **kw)
+    def __init__(
+        self, sock, block_size=DEFAULT_BLOCK_SIZE, method="GET", headers_type=Headers, **kw
+    ):
+        super().__init__(method=method, headers_type=headers_type)
         self._sock = sock
         self.block_size = block_size
         self._read_headers()
 
     def release(self):
         try:
             if self._sock is not None and self.should_close():
@@ -221,17 +222,15 @@
 
         if self._sock is None:
             read = copy(self._body_buffer)
             del self._body_buffer[:]
             return read
 
         try:
-            while not (self.message_complete) and (
-                length is None or len(self._body_buffer) < length
-            ):
+            while not self.message_complete and (length is None or len(self._body_buffer) < length):
                 data = self._sock.recv(length or self.block_size)
                 self.feed(data)
         except:
             self.release()
             raise
 
         if length is not None:
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/oncert.pem` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/oncert.pem`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/server.crt` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/server.crt`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/server.key` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/server.key`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_client.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 @pytest.fixture
 def httpbin():
     return httpbin_client()
 
 
 @pytest.mark.parametrize("request_uri", ["/tp/", "tp/", f"http://{HTTPBIN_HOST}/tp/"])
 def test_build_request(httpbin, request_uri):
-    request_ref = f"GET /tp/ HTTP/1.1\r\nuser-agent: python/gevent-http-client-{__version__}\r\nhost: {HTTPBIN_HOST}\r\n\r\n"
+    request_ref = f"GET /tp/ HTTP/1.1\r\nUser-Agent: python/gevent-http-client-{__version__}\r\nHost: {HTTPBIN_HOST}\r\n\r\n"
     assert httpbin._build_request("GET", request_uri) == request_ref
 
 
 def test_build_request_invalid_host(httpbin):
     with pytest.raises(ValueError):
         httpbin._build_request("GET", "http://someunrelatedhost.com/")
 
@@ -293,15 +293,15 @@
     "Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:124.0) Gecko/20100101 Firefox/124.0"
 )
 FIREFOX_HEADERS = {"User-Agent": FIREFOX_USER_AGENT}
 
 
 def check_user_agent_header(ua_header, ua_header_ref):
     """
-    unlike original httpbin, httpbingo.org sends back a list of header
+    Unlike original httpbin, httpbingo.org sends back a list of header
     strings instead of a simple string. So we need to be a bit flexible
     with the answer.
     """
     if isinstance(ua_header, list):
         assert len(ua_header) == 1
         assert ua_header[0] == ua_header_ref
         return
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_headers.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_headers.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,26 +81,51 @@
     assert len(h) == 5
     assert "ab" in h
     assert len(h["cookie"]) == 3
     assert h["cookie"][0] == "C"
     assert h["cookie"][-1] == "E"
 
 
+def test_retrieve():
+    h = Headers([("ab", "A"), ("cd", "B"), ("cookie", "C"), ("cookie", "D"), ("cookie", "E")])
+    for key, ref in {"ab": "A", "cd": "B", "cookie": ["C", "D", "E"]}.items():
+        assert h[key] == ref
+        assert h.get(key) == ref
+        assert h.pop(key) == ref
+        assert key not in h
+
+
 def test_case_insensitivity():
     h = Headers({"Content-Type": "text/plain"})
     h.add("Content-Encoding", "utf8")
     for val in ("content-type", "content-encoding"):
         assert val.upper() in h
         assert val.lower() in h
         assert val.capitalize() in h
         assert h.get(val.lower()) == h.get(val.upper()) == h.get(val.capitalize())
         del h[val.upper()]
         assert val.lower() not in h
 
 
+def test_preserve_case():
+    h = Headers(Cookie="C", COOKIE="D", cookie="E", asdf="E")
+    assert len(h) == 4
+    assert h["cookie"] == ["C", "D", "E"]
+    assert list(h.items()) == [("Cookie", "C"), ("COOKIE", "D"), ("cookie", "E"), ("asdf", "E")]
+
+
+def test_update_preserve_case():
+    h = Headers()
+    h.update(COOKIE="A", Cookie="C")
+    assert list(h.items()) == [("Cookie", "C")]
+    h = Headers()
+    h.update(dict(Cookie="C", COOKIE="D", cookiE="E"))
+    assert list(h.items()) == [("cookiE", "E")]
+
+
 def test_read_multiple_header():
     parser = HTTPResponse()
     parser.feed(MULTI_COOKIE_RESPONSE)
     headers = parser._headers_index
     assert len(headers["set-cookie"]) == MULTI_COOKIE_RESPONSE.count("Set-Cookie")
     assert headers["set-cookie"][0].startswith("bb_lastvisit")
     assert headers["set-cookie"][-1].startswith("bb_fbprofilepicurl")
@@ -177,14 +202,19 @@
 def test_header_replace():
     d = Headers()
     d["Content-Type"] = "text/plain"
     d["content-type"] = "text/html"
     assert d["content-type"] == "text/html"
 
 
+def test_formatting():
+    h = Headers(asdf="ddd", ASDF="fff", AsDf="asdfasdf")
+    assert str(h) == "asdf: ddd\nASDF: fff\nAsDf: asdfasdf"
+
+
 def test_compat_dict():
     h = Headers(D="asdf")
     h.add("E", "d")
     h.add("E", "f")
     h.add("Cookie", "d")
     h.add("Cookie", "e")
     h.add("Cookie", "f")
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_httplib.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_httplib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import urllib.request
 from contextlib import contextmanager
 from http.client import HTTPException
 
 import gevent.server
 import pytest
 
 from geventhttpclient.httplib import HTTPConnection
@@ -60,7 +61,15 @@
     with server(success_response):
         connection = HTTPConnection(*LISTENER)
         connection.request("GET", "/")
         response = connection.getresponse()
 
         assert response.msg["Set-Cookie"] == "foo=bar, baz=bar"
         assert response.msg["Content-Type"] == "text/plain"
+
+
+@pytest.mark.network
+@pytest.mark.parametrize("url", ["http://httpbingo.org", "https://github.com"])
+def test_urllib_request(url):
+    content = urllib.request.urlopen(url).read()
+    assert content
+    assert b"body" in content
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_keep_alive.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_keep_alive.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_network_failures.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_network_failures.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_no_module_ssl.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_no_module_ssl.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_parser.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,22 @@
 
     assert parser.message_begun
     assert parser.headers_complete
     assert parser.message_complete
     assert parser.should_keep_alive()
     assert parser.status_code == 301
     assert sorted(parser.items()) == [
-        ("cache-control", "public, max-age=2592000"),
-        ("content-length", "218"),
-        ("content-type", "text/html; charset=UTF-8"),
-        ("date", "Thu, 13 Oct 2011 15:03:12 GMT"),
-        ("expires", "Sat, 12 Nov 2011 15:03:12 GMT"),
-        ("location", "http://www.google.fr/"),
-        ("server", "gws"),
-        ("x-xss-protection", "1; mode=block"),
+        ("Cache-Control", "public, max-age=2592000"),
+        ("Content-Length", "218"),
+        ("Content-Type", "text/html; charset=UTF-8"),
+        ("Date", "Thu, 13 Oct 2011 15:03:12 GMT"),
+        ("Expires", "Sat, 12 Nov 2011 15:03:12 GMT"),
+        ("Location", "http://www.google.fr/"),
+        ("Server", "gws"),
+        ("X-XSS-Protection", "1; mode=block"),
     ]
 
 
 @wrap_refcount
 def test_parse_error():
     response = HTTPResponse()
     try:
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_ssl.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_url.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/tests/test_useragent.py` & `geventhttpclient-2.2.0/src/geventhttpclient/tests/test_useragent.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,15 @@
         yield
     finally:
         server.stop()
 
 
 def check_upload(body, headers=None):
     def wsgi_handler(env, start_response):
-        if headers:
-            # For Python 2.6 which does not have viewitems
-            assert env.items() >= headers.items()
+        assert env["REQUEST_METHOD"] == "POST"
         assert body == env["wsgi.input"].read()
         start_response("200 OK", [])
         return []
 
     return wsgi_handler
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/url.py` & `geventhttpclient-2.2.0/src/geventhttpclient/url.py`

 * *Files identical despite different names*

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient/useragent.py` & `geventhttpclient-2.2.0/src/geventhttpclient/useragent.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def get_header(self, header_name, default=None):
         return self.headers.get(header_name, default)
 
     def has_header(self, header_name):
         return header_name in self.headers
 
     def header_items(self):
-        return self.headers.items()
+        return list(self.headers.items())
 
     def add_unredirected_header(self, key, val):
         self.headers.add(key, val)
 
     def _drop_payload(self):
         self.method = "GET"
         self.payload = None
@@ -505,15 +505,15 @@
                 e = RetriesExceeded(url, f"Redirection limit reached ({self.max_redirects})")
                 last_error = self._handle_error(e, url=url)
         else:
             return self._handle_retries_exceeded(url, last_error=last_error)
 
     @classmethod
     def _conversation_str(cls, url, resp, payload=None):
-        header_str = "\n".join(f"{key}: {val}" for key, val in resp.headers.iteroriginal())
+        header_str = "\n".join(f"{key}: {val}" for key, val in resp.headers.items())
         ret = "REQUEST: " + url + "\n" + resp._sent_request
         if payload:
             if isinstance(payload, bytes):
                 try:
                     ret += payload.decode("utf-8") + "\n\n"
                 except UnicodeDecodeError:
                     ret += "UnicodeDecodeError" + "\n\n"
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient.egg-info/PKG-INFO` & `geventhttpclient-2.2.0/src/geventhttpclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventhttpclient
-Version: 2.1.1
+Version: 2.2.0
 Summary: HTTP client library for gevent
 Author-email: Antonin Amand <antonin.amand@gmail.com>
 License: Based on llhttp, copyright Fedor Indutny, 2018.
         
         Python extension is copyright Antonin Amand <antonin.amand@gmail.com>,
         licensed under the same terms.
         
@@ -58,14 +58,16 @@
 Requires-Dist: dpkt; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Provides-Extra: benchmarks
 Requires-Dist: requests; extra == "benchmarks"
 Requires-Dist: httpx; extra == "benchmarks"
 Requires-Dist: urllib3; extra == "benchmarks"
 Requires-Dist: httplib2; extra == "benchmarks"
+Provides-Extra: examples
+Requires-Dist: oauth2; extra == "examples"
 
 [![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/geventhttpclient/geventhttpclient/test.yml?branch=master&logo=github&style=flat)](https://github.com/geventhttpclient/geventhttpclient/actions)
 [![PyPI](https://img.shields.io/pypi/v/geventhttpclient.svg?style=flat)](https://pypi.org/project/geventhttpclient/)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Fgeventhttpclient%2Fgeventhttpclient%2Fmaster%2Fpyproject.toml)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/geventhttpclient)
 
 # geventhttpclient
@@ -222,17 +224,20 @@
         data = response.read(CHUNK_SIZE)
 ```
 
 ## Benchmarks
 
 The benchmark does 10000 get requests against a local nginx server in the default 
 configuration with a concurrency of 10. See `benchmarks` folder. The requests per
-second for a couple of popular clients is given in the table below.
-
-| HTTP Client          | RPS    |
-|----------------------|--------|
-| GeventHTTPClient     | 7181.2 |
-| Urllib3              | 2847.5 |
-| Httpx                | 1682.9 |
-| Requests             | 1186.4 |
+second for a couple of popular clients is given in the table below. Please read
+[benchmarks/README.md](https://github.com/geventhttpclient/geventhttpclient/blob/master/benchmarks/README.md)
+for mor details. Also note, HTTPX is better be used with asyncio, not gevent.
+
+| HTTP Client        | RPS    |
+|--------------------|--------|
+| GeventHTTPClient   | 7268.9 |
+| Httplib2 (patched) | 2323.9 |
+| Urllib3            | 2242.5 |
+| Requests           | 1046.1 |
+| Httpx              | 770.3  |
 
 *Linux(x86_64), Python 3.11.6 @ Intel i7-7560U*
```

### Comparing `geventhttpclient-2.1.1/src/geventhttpclient.egg-info/SOURCES.txt` & `geventhttpclient-2.2.0/src/geventhttpclient.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 llhttp/src/http.c
 llhttp/src/llhttp.c
 src/geventhttpclient/__init__.py
 src/geventhttpclient/client.py
 src/geventhttpclient/connectionpool.py
 src/geventhttpclient/header.py
 src/geventhttpclient/httplib.py
+src/geventhttpclient/httplib2.py
 src/geventhttpclient/response.py
 src/geventhttpclient/url.py
 src/geventhttpclient/useragent.py
 src/geventhttpclient.egg-info/PKG-INFO
 src/geventhttpclient.egg-info/SOURCES.txt
 src/geventhttpclient.egg-info/dependency_links.txt
 src/geventhttpclient.egg-info/requires.txt
@@ -27,14 +28,15 @@
 src/geventhttpclient/tests/oncert.pem
 src/geventhttpclient/tests/server.crt
 src/geventhttpclient/tests/server.key
 src/geventhttpclient/tests/test_client.py
 src/geventhttpclient/tests/test_headers.py
 src/geventhttpclient/tests/test_http_host.py
 src/geventhttpclient/tests/test_httplib.py
+src/geventhttpclient/tests/test_httplib2.py
 src/geventhttpclient/tests/test_keep_alive.py
 src/geventhttpclient/tests/test_network_failures.py
 src/geventhttpclient/tests/test_no_module_ssl.py
 src/geventhttpclient/tests/test_parser.py
 src/geventhttpclient/tests/test_ssl.py
 src/geventhttpclient/tests/test_url.py
 src/geventhttpclient/tests/test_useragent.py
```

