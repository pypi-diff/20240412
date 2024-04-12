# Comparing `tmp/gloe-0.5.2.tar.gz` & `tmp/gloe-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gloe-0.5.2.tar", last modified: Fri Apr 12 09:56:52 2024, max compression
+gzip compressed data, was "gloe-0.5.3.tar", last modified: Fri Apr 12 10:18:54 2024, max compression
```

## Comparing `gloe-0.5.2.tar` & `gloe-0.5.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.896667 gloe-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 09:56:47.000000 gloe-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 09:56:47.000000 gloe-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 09:56:47.000000 gloe-0.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-12 09:56:52.892667 gloe-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-12 09:56:47.000000 gloe-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.880667 gloe-0.5.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.884667 gloe-0.5.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.884667 gloe-0.5.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.884667 gloe-0.5.2/docs/source/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/_static/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/_static/assets/gloe-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/_static/assets/gloe-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/_static/assets/graph_example.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/_static/theme_customs.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.884667 gloe-0.5.2/docs/source/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/api-reference/gloe.collection.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/api-reference/gloe.experimental.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/api-reference/gloe.utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.888667 gloe-0.5.2/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/async-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/conditional-flows.md
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/ensurers.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/partial-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/getting-started/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/limitations.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.888667 gloe-0.5.2/docs/source/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/pygments/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-12 09:56:47.000000 gloe-0.5.2/docs/source/theory.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.888667 gloe-0.5.2/gloe/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/_composition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.888667 gloe-0.5.2/gloe/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/collection/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/collection/_mapover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/gloe/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/conditional/_conditioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/gloe/ensurer/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/ensurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/ensurer/_transformer_ensurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/gloe/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/gloe/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/experimental/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 09:56:47.000000 gloe-0.5.2/gloe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/gloe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-12 09:56:52.000000 gloe-0.5.2/gloe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-12 09:56:52.000000 gloe-0.5.2/gloe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:56:52.000000 gloe-0.5.2/gloe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 09:56:52.000000 gloe-0.5.2/gloe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 09:56:52.000000 gloe-0.5.2/gloe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 09:56:47.000000 gloe-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:56:52.896667 gloe-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:56:52.892667 gloe-0.5.2/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/lib/conditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/lib/ensurers.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/lib/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_conditioner_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_transformer_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_transformer_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_transformer_ensurer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_transformer_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_transformer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 09:56:47.000000 gloe-0.5.2/tests/test_transformer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 10:18:48.000000 gloe-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 10:18:48.000000 gloe-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 10:18:48.000000 gloe-0.5.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 10:18:54.643336 gloe-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 10:18:48.000000 gloe-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.631336 gloe-0.5.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/gloe-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/gloe-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/graph_example.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/theme_customs.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/gloe.collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/gloe.experimental.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/gloe.utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/async-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/conditional-flows.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/ensurers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/partial-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/limitations.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/pygments/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/theory.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/_composition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/collection/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/collection/_mapover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/conditional/_conditioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/ensurer/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/ensurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/ensurer/_transformer_ensurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/experimental/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/gloe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 10:18:48.000000 gloe-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:18:54.643336 gloe-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/conditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/ensurers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_conditioner_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_ensurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_utils.py
```

### Comparing `gloe-0.5.2/LICENSE` & `gloe-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/Makefile` & `gloe-0.5.3/Makefile`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/PKG-INFO` & `gloe-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.2
+Version: 0.5.3
 Summary: Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 </div>
 
 
 | | |
 | --- |-|
 | Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml)|
 | Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)|
-| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
+| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
 
 
 
 Let Gloe help you
 ===
 
 Gloe (pronounced /ɡloʊ/, like "glow") is a general purpose library made to help developers to create, maintain, document and test operational and data flows. It can be used in data science and machine learning pipelines as well in servers, scripts or wherever else one identifies a lack between the code and the understanding of logical business. Gloe was not thought to be used in the entire application even less replacing any existing library, it was built to be integrated with other tools and to be implemented where the code complexity can be bigger than the desired.
```

### Comparing `gloe-0.5.2/README.md` & `gloe-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 </div>
 
 
 | | |
 | --- |-|
 | Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml)|
 | Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)|
-| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
+| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
 
 
 
 Let Gloe help you
 ===
 
 Gloe (pronounced /ɡloʊ/, like "glow") is a general purpose library made to help developers to create, maintain, document and test operational and data flows. It can be used in data science and machine learning pipelines as well in servers, scripts or wherever else one identifies a lack between the code and the understanding of logical business. Gloe was not thought to be used in the entire application even less replacing any existing library, it was built to be integrated with other tools and to be implemented where the code complexity can be bigger than the desired.
```

### Comparing `gloe-0.5.2/docs/source/_static/assets/favicon.ico` & `gloe-0.5.3/docs/source/_static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/_static/assets/gloe-logo-small.png` & `gloe-0.5.3/docs/source/_static/assets/gloe-logo-small.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/_static/assets/gloe-logo.png` & `gloe-0.5.3/docs/source/_static/assets/gloe-logo.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/_static/assets/graph_example.jpeg` & `gloe-0.5.3/docs/source/_static/assets/graph_example.jpeg`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/api-reference/index.md` & `gloe-0.5.3/docs/source/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/conf.py` & `gloe-0.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/async-transformers.md` & `gloe-0.5.3/docs/source/getting-started/async-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/conditional-flows.md` & `gloe-0.5.3/docs/source/getting-started/conditional-flows.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/ensurers.md` & `gloe-0.5.3/docs/source/getting-started/ensurers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/partial-transformers.md` & `gloe-0.5.3/docs/source/getting-started/partial-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/plotting.md` & `gloe-0.5.3/docs/source/getting-started/plotting.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/transformers.md` & `gloe-0.5.3/docs/source/getting-started/transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/getting-started/utilities.md` & `gloe-0.5.3/docs/source/getting-started/utilities.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/index.md` & `gloe-0.5.3/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/limitations.md` & `gloe-0.5.3/docs/source/limitations.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/pygments/styles.py` & `gloe-0.5.3/docs/source/pygments/styles.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/docs/source/theory.md` & `gloe-0.5.3/docs/source/theory.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/__init__.py` & `gloe-0.5.3/gloe/__init__.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/_composition_utils.py` & `gloe-0.5.3/gloe/_composition_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/_utils.py` & `gloe-0.5.3/gloe/_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/async_transformer.py` & `gloe-0.5.3/gloe/async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/base_transformer.py` & `gloe-0.5.3/gloe/base_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/collection/_map.py` & `gloe-0.5.3/gloe/collection/_map.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/collection/_mapover.py` & `gloe-0.5.3/gloe/collection/_mapover.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/conditional/_conditioner.py` & `gloe-0.5.3/gloe/conditional/_conditioner.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/ensurer/_transformer_ensurer.py` & `gloe-0.5.3/gloe/ensurer/_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/experimental/_bridge.py` & `gloe-0.5.3/gloe/experimental/_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/functional.py` & `gloe-0.5.3/gloe/functional.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/transformers.py` & `gloe-0.5.3/gloe/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe/utils.py` & `gloe-0.5.3/gloe/utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/gloe.egg-info/PKG-INFO` & `gloe-0.5.3/gloe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.2
+Version: 0.5.3
 Summary: Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 </div>
 
 
 | | |
 | --- |-|
 | Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml)|
 | Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)|
-| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
+| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
 
 
 
 Let Gloe help you
 ===
 
 Gloe (pronounced /ɡloʊ/, like "glow") is a general purpose library made to help developers to create, maintain, document and test operational and data flows. It can be used in data science and machine learning pipelines as well in servers, scripts or wherever else one identifies a lack between the code and the understanding of logical business. Gloe was not thought to be used in the entire application even less replacing any existing library, it was built to be integrated with other tools and to be implemented where the code complexity can be bigger than the desired.
```

### Comparing `gloe-0.5.2/gloe.egg-info/SOURCES.txt` & `gloe-0.5.3/gloe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/pyproject.toml` & `gloe-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gloe"
-version = "0.5.2"
+version = "0.5.3"
 authors = [
   { name="Samir Braga", email="samirchavess@gmail.com" },
 ]
 description = "Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gloe-0.5.2/tests/lib/ensurers.py` & `gloe-0.5.3/tests/lib/ensurers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/lib/transformers.py` & `gloe-0.5.3/tests/lib/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_async_transformer.py` & `gloe-0.5.3/tests/test_async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_conditioner_transformer.py` & `gloe-0.5.3/tests/test_conditioner_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_function_transformer.py` & `gloe-0.5.3/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_transformer_bridge.py` & `gloe-0.5.3/tests/test_transformer_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_transformer_collections.py` & `gloe-0.5.3/tests/test_transformer_collections.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_transformer_ensurer.py` & `gloe-0.5.3/tests/test_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_transformer_graph.py` & `gloe-0.5.3/tests/test_transformer_graph.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.2/tests/test_transformer_types.py` & `gloe-0.5.3/tests/test_transformer_types.py`

 * *Files identical despite different names*

