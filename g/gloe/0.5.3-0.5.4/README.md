# Comparing `tmp/gloe-0.5.3.tar.gz` & `tmp/gloe-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gloe-0.5.3.tar", last modified: Fri Apr 12 10:18:54 2024, max compression
+gzip compressed data, was "gloe-0.5.4.tar", last modified: Fri Apr 12 18:07:15 2024, max compression
```

## Comparing `gloe-0.5.3.tar` & `gloe-0.5.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 10:18:48.000000 gloe-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 10:18:48.000000 gloe-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 10:18:48.000000 gloe-0.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 10:18:54.643336 gloe-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 10:18:48.000000 gloe-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.631336 gloe-0.5.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/gloe-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/gloe-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/assets/graph_example.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/_static/theme_customs.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/gloe.collection.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/gloe.experimental.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/gloe.utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/async-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/conditional-flows.md
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/ensurers.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/partial-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/getting-started/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/limitations.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.635336 gloe-0.5.3/docs/source/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/pygments/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-12 10:18:48.000000 gloe-0.5.3/docs/source/theory.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/_composition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/collection/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/collection/_mapover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/conditional/_conditioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/ensurer/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/ensurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/ensurer/_transformer_ensurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.639336 gloe-0.5.3/gloe/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/experimental/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 10:18:48.000000 gloe-0.5.3/gloe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/gloe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 10:18:54.000000 gloe-0.5.3/gloe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 10:18:48.000000 gloe-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:18:54.643336 gloe-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:18:54.643336 gloe-0.5.3/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/conditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/ensurers.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/lib/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_conditioner_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_ensurer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 10:18:48.000000 gloe-0.5.3/tests/test_transformer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 18:07:10.000000 gloe-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 18:07:10.000000 gloe-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 18:07:10.000000 gloe-0.5.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 18:07:15.955186 gloe-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 18:07:10.000000 gloe-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.943186 gloe-0.5.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/gloe-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/gloe-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/graph_example.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/theme_customs.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/gloe.collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/gloe.experimental.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/gloe.utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/async-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/conditional-flows.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/ensurers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/partial-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/limitations.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/docs/source/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/pygments/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/theory.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/_composition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/collection/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/collection/_mapover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/conditional/_conditioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/ensurer/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/ensurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/ensurer/_transformer_ensurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/gloe/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/experimental/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/gloe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 18:07:10.000000 gloe-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:07:15.955186 gloe-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/conditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/ensurers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_conditioner_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_ensurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_utils.py
```

### Comparing `gloe-0.5.3/LICENSE` & `gloe-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/Makefile` & `gloe-0.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/PKG-INFO` & `gloe-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.3
+Version: 0.5.4
 Summary: Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gloe-0.5.3/README.md` & `gloe-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/_static/assets/favicon.ico` & `gloe-0.5.4/docs/source/_static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/_static/assets/gloe-logo-small.png` & `gloe-0.5.4/docs/source/_static/assets/gloe-logo-small.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/_static/assets/gloe-logo.png` & `gloe-0.5.4/docs/source/_static/assets/gloe-logo.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/_static/assets/graph_example.jpeg` & `gloe-0.5.4/docs/source/_static/assets/graph_example.jpeg`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/api-reference/index.md` & `gloe-0.5.4/docs/source/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/conf.py` & `gloe-0.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/async-transformers.md` & `gloe-0.5.4/docs/source/getting-started/async-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/conditional-flows.md` & `gloe-0.5.4/docs/source/getting-started/conditional-flows.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/ensurers.md` & `gloe-0.5.4/docs/source/getting-started/ensurers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/partial-transformers.md` & `gloe-0.5.4/docs/source/getting-started/partial-transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/plotting.md` & `gloe-0.5.4/docs/source/getting-started/plotting.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/transformers.md` & `gloe-0.5.4/docs/source/getting-started/transformers.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/getting-started/utilities.md` & `gloe-0.5.4/docs/source/getting-started/utilities.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/index.md` & `gloe-0.5.4/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/limitations.md` & `gloe-0.5.4/docs/source/limitations.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/pygments/styles.py` & `gloe-0.5.4/docs/source/pygments/styles.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/docs/source/theory.md` & `gloe-0.5.4/docs/source/theory.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/__init__.py` & `gloe-0.5.4/gloe/__init__.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/_composition_utils.py` & `gloe-0.5.4/gloe/_composition_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -196,44 +196,54 @@
             )
             return new_signature
 
         def __len__(self):
             lengths = [len(t) for t in receiving_transformers]
             return sum(lengths) + len(incident_transformer)
 
-    async def split_result(data: _In) -> tuple[Any, ...]:
-        if asyncio.iscoroutinefunction(incident_transformer.__call__):
-            intermediate_result = await incident_transformer(data)
-        else:
+    new_transformer = None
+    if is_transformer(incident_transformer) and is_transformer(receiving_transformers):
+
+        def split_result(data: _In) -> tuple[Any, ...]:
             intermediate_result = incident_transformer(data)
 
-        outputs = []
-        for receiving_transformer in receiving_transformers:
-            if asyncio.iscoroutinefunction(receiving_transformer.__call__):
-                output = await receiving_transformer(intermediate_result)
-            else:
+            outputs = []
+            for receiving_transformer in receiving_transformers:
                 output = receiving_transformer(intermediate_result)
-            outputs.append(output)
+                outputs.append(output)
 
-        return tuple(outputs)
-
-    new_transformer = None
-    if is_transformer(incident_transformer) and is_transformer(receiving_transformers):
+            return tuple(outputs)
 
         class NewTransformer1(BaseNewTransformer, Transformer[_In, tuple[Any, ...]]):
             def transform(self, data: _In) -> tuple[Any, ...]:
-                return asyncio.run(split_result(data))
+                return split_result(data)
 
         new_transformer = NewTransformer1()
 
     else:
 
+        async def split_result_async(data: _In) -> tuple[Any, ...]:
+            if asyncio.iscoroutinefunction(incident_transformer.__call__):
+                intermediate_result = await incident_transformer(data)
+            else:
+                intermediate_result = incident_transformer(data)
+
+            outputs = []
+            for receiving_transformer in receiving_transformers:
+                if asyncio.iscoroutinefunction(receiving_transformer.__call__):
+                    output = await receiving_transformer(intermediate_result)
+                else:
+                    output = receiving_transformer(intermediate_result)
+                outputs.append(output)
+
+            return tuple(outputs)
+
         class NewTransformer2(BaseNewTransformer, AsyncTransformer[_In, tuple[Any, ...]]):
             async def transform_async(self, data: _In) -> tuple[Any, ...]:
-                return await split_result(data)
+                return await split_result_async(data)
 
         new_transformer = NewTransformer2()
 
     new_transformer._previous = cast(Transformer, receiving_transformers)
     new_transformer.__class__.__name__ = "Converge"
     new_transformer._label = ""
     new_transformer._graph_node_props = {
```

### Comparing `gloe-0.5.3/gloe/_utils.py` & `gloe-0.5.4/gloe/_utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/async_transformer.py` & `gloe-0.5.4/gloe/async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/base_transformer.py` & `gloe-0.5.4/gloe/base_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/collection/_map.py` & `gloe-0.5.4/gloe/collection/_map.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/collection/_mapover.py` & `gloe-0.5.4/gloe/collection/_mapover.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/conditional/_conditioner.py` & `gloe-0.5.4/gloe/conditional/_conditioner.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/ensurer/_transformer_ensurer.py` & `gloe-0.5.4/gloe/ensurer/_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/experimental/_bridge.py` & `gloe-0.5.4/gloe/experimental/_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/functional.py` & `gloe-0.5.4/gloe/functional.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/transformers.py` & `gloe-0.5.4/gloe/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe/utils.py` & `gloe-0.5.4/gloe/utils.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/gloe.egg-info/PKG-INFO` & `gloe-0.5.4/gloe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.3
+Version: 0.5.4
 Summary: Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gloe-0.5.3/gloe.egg-info/SOURCES.txt` & `gloe-0.5.4/gloe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/pyproject.toml` & `gloe-0.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gloe"
-version = "0.5.3"
+version = "0.5.4"
 authors = [
   { name="Samir Braga", email="samirchavess@gmail.com" },
 ]
 description = "Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `gloe-0.5.3/tests/lib/ensurers.py` & `gloe-0.5.4/tests/lib/ensurers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/lib/transformers.py` & `gloe-0.5.4/tests/lib/transformers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_async_transformer.py` & `gloe-0.5.4/tests/test_async_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_conditioner_transformer.py` & `gloe-0.5.4/tests/test_conditioner_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_function_transformer.py` & `gloe-0.5.4/tests/test_function_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import unittest
 from typing import cast
 
 from tests.lib.transformers import (
     square,
     square_root,
     sum_tuple2,
@@ -257,10 +258,18 @@
         Test the curried transformer
         """
 
         graph = logarithm(base=2)
         self.assertEqual(graph(2), 1)
         self.assertEqual(graph.label, "logarithm")
 
+    def test_transformers_on_a_running_event_loop(self):
+        async def run_main():
+            graph = square >> square_root
+            graph(9)
+
+        loop = asyncio.new_event_loop()
+        loop.run_until_complete(run_main())
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `gloe-0.5.3/tests/test_transformer_bridge.py` & `gloe-0.5.4/tests/test_transformer_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_transformer_collections.py` & `gloe-0.5.4/tests/test_transformer_collections.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_transformer_ensurer.py` & `gloe-0.5.4/tests/test_transformer_ensurer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_transformer_graph.py` & `gloe-0.5.4/tests/test_transformer_graph.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.3/tests/test_transformer_types.py` & `gloe-0.5.4/tests/test_transformer_types.py`

 * *Files identical despite different names*

