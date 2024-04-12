# Comparing `tmp/esrt-1.32.0.tar.gz` & `tmp/esrt-1.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esrt-1.32.0.tar", last modified: Sun Apr  7 18:02:54 2024, max compression
+gzip compressed data, was "esrt-1.33.0.tar", last modified: Fri Apr 12 07:59:44 2024, max compression
```

## Comparing `esrt-1.32.0.tar` & `esrt-1.33.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:02:54.850388 esrt-1.32.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-07 18:02:54.850388 esrt-1.32.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-04-07 18:02:39.000000 esrt-1.32.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-07 18:02:39.000000 esrt-1.32.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:02:54.850388 esrt-1.32.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:02:54.846388 esrt-1.32.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:02:54.846388 esrt-1.32.0/src/esrt/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-07 18:02:39.000000 esrt-1.32.0/src/esrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-04-07 18:02:39.000000 esrt-1.32.0/src/esrt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-07 18:02:39.000000 esrt-1.32.0/src/esrt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 18:02:39.000000 esrt-1.32.0/src/esrt/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-07 18:02:39.000000 esrt-1.32.0/src/esrt/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-07 18:02:39.000000 esrt-1.32.0/src/esrt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:02:54.850388 esrt-1.32.0/src/esrt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-07 18:02:54.000000 esrt-1.32.0/src/esrt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 18:02:54.000000 esrt-1.32.0/src/esrt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:02:54.000000 esrt-1.32.0/src/esrt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 18:02:54.000000 esrt-1.32.0/src/esrt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 18:02:54.000000 esrt-1.32.0/src/esrt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 18:02:54.000000 esrt-1.32.0/src/esrt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:59:44.031142 esrt-1.33.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-12 07:59:44.031142 esrt-1.33.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10548 2024-04-12 07:59:28.000000 esrt-1.33.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-12 07:59:28.000000 esrt-1.33.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:59:44.031142 esrt-1.33.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:59:44.023142 esrt-1.33.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:59:44.027142 esrt-1.33.0/src/esrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 07:59:28.000000 esrt-1.33.0/src/esrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-12 07:59:28.000000 esrt-1.33.0/src/esrt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 07:59:28.000000 esrt-1.33.0/src/esrt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 07:59:28.000000 esrt-1.33.0/src/esrt/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-12 07:59:28.000000 esrt-1.33.0/src/esrt/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 07:59:28.000000 esrt-1.33.0/src/esrt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:59:44.027142 esrt-1.33.0/src/esrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-04-12 07:59:44.000000 esrt-1.33.0/src/esrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 07:59:44.000000 esrt-1.33.0/src/esrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:59:44.000000 esrt-1.33.0/src/esrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 07:59:44.000000 esrt-1.33.0/src/esrt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 07:59:44.000000 esrt-1.33.0/src/esrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 07:59:44.000000 esrt-1.33.0/src/esrt.egg-info/top_level.txt
```

### Comparing `esrt-1.32.0/PKG-INFO` & `esrt-1.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.32.0
+Version: 1.33.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
```

### Comparing `esrt-1.32.0/README.md` & `esrt-1.33.0/README.md`

 * *Files identical despite different names*

### Comparing `esrt-1.32.0/pyproject.toml` & `esrt-1.33.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "esrt"
-version = "1.32.0"
+version = "1.33.0"
 requires-python = ">=3.9"
 readme = "README.md"
 dependencies = [
     "elasticsearch==6.8.2",
     "typer-slim[standard]>=0.12.0",
     # uvicorn.importer.import_from_string
     "uvicorn>=0.2.14",
```

### Comparing `esrt-1.32.0/src/esrt/__main__.py` & `esrt-1.33.0/src/esrt/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,17 @@
     t.Optional[list[dict]],
     typer.Option('-p', '--params', metavar='QUERY_PARAM', parser=parse_params, help='HTTP params'),
 ]
 _headers_annotated = t.Annotated[
     t.Optional[list[dict]],
     typer.Option('-H', '--header', metavar='HTTP_HEADER', parser=parse_header, help='HTTP headers'),
 ]
+_kwargs_annotated = t.Annotated[
+    t.Optional[list[dict]], typer.Option('-k', '--kwargs', parser=parse_params)
+]
 #
 _finput_annotation = typer.Option('-d', '--data', metavar='FILE', help='Input file')
 _foutput_annotated = t.Annotated[
     typer.FileTextWrite, typer.Option('-o', '--output', metavar='FILE', help='Output file')
 ]
 #
 _doc_type_annotated = t.Annotated[
@@ -136,14 +139,15 @@
     ] = '5m',
     raise_on_error: t.Annotated[bool, typer.Option(' /--no-raise-on-error')] = True,
     preserve_order: t.Annotated[bool, typer.Option('--preserve-order')] = False,
     size: t.Annotated[int, typer.Option('--size')] = 1000,
     request_timeout: t.Annotated[t.Optional[int], typer.Option('--request-timeout')] = None,
     clear_scroll: t.Annotated[bool, typer.Option(' /--keep-scroll')] = True,
     # scroll_kwargs
+    kwargs: _kwargs_annotated = None,
 ):
     client = es.Client(host=host)
     body = finput_body and finput_body.read().strip() or '{}'
     _once_params = merge_dicts(params)
     _once_params['size'] = '1'
     _once = client.search(
         index=index,
@@ -164,14 +168,15 @@
         scroll=scroll,
         raise_on_error=raise_on_error,
         preserve_order=preserve_order,
         size=size,
         request_timeout=request_timeout,
         clear_scroll=clear_scroll,
         # scroll_kwargs
+        **merge_dicts(kwargs),
     )
     context = nullcontext(_iterable)
     if progress:
         context = typer.progressbar(
             iterable=_iterable, label='scan', show_pos=True, file=sys.stderr
         )
     with context as hits:
@@ -190,15 +195,18 @@
     host: _host_annotated,
     finput_body: t.Annotated[t.Optional[typer.FileText], _finput_annotation] = None,
     foutput: _foutput_annotated = t.cast(typer.FileTextWrite, sys.stdout),
     #
     method: _method_annotated = 'GET',
     url: _path_annotated = '/',
     quote_url: t.Annotated[
-        bool, typer.Option('-Q', '--quote-url', help='Encode path with urllib.parse.quote but keep `,` and `*`')
+        bool,
+        typer.Option(
+            '-Q', '--quote-url', help='Encode path with urllib.parse.quote but keep `,` and `*`'
+        ),
     ] = False,
     params: _params_annotated = None,
     headers: _headers_annotated = None,
     #
 ):
     client = es.Client(host=host)
     if not url.startswith('/'):
@@ -245,14 +253,16 @@
     chunk_size: _chunk_size_annotated = 500,
     max_chunk_bytes: t.Annotated[int, typer.Option('--max-chunk-bytes')] = 100 * 1024 * 1024,
     raise_on_error: t.Annotated[bool, typer.Option(' /--no-raise-on-error')] = True,
     raise_on_exception: t.Annotated[bool, typer.Option(' /--no-raise-on-exception')] = True,
     max_retries: t.Annotated[int, typer.Option('--max-retries')] = 3,
     initial_backoff: t.Annotated[int, typer.Option('--initial-backoff')] = 2,
     max_backoff: t.Annotated[int, typer.Option('--max-backoff')] = 600,
+    #
+    kwargs: _kwargs_annotated = None,
 ):
     client = es.Client(host=host)
     with redirect_stdout(sys.stderr):
         print(client)
         print('waiting for seconds to start', end=' ', flush=True)
         for i in range(5, -1, -1):
             print(i, end=' ', flush=True)
@@ -270,14 +280,16 @@
         initial_backoff=initial_backoff,
         max_backoff=max_backoff,
         yield_ok=True,  # *
         #
         index=index,
         doc_type=doc_type,
         params=merge_dicts(params),
+        #
+        **merge_dicts(kwargs),
     )
     context = nullcontext(_iterable)
     if progress:
         context = typer.progressbar(
             iterable=_iterable, label='streaming_bulk', show_pos=True, file=sys.stderr
         )
     with context as items:
```

### Comparing `esrt-1.32.0/src/esrt/handlers.py` & `esrt-1.33.0/src/esrt/handlers.py`

 * *Files identical despite different names*

### Comparing `esrt-1.32.0/src/esrt/utils.py` & `esrt-1.33.0/src/esrt/utils.py`

 * *Files identical despite different names*

### Comparing `esrt-1.32.0/src/esrt.egg-info/PKG-INFO` & `esrt-1.33.0/src/esrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.32.0
+Version: 1.33.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
```

