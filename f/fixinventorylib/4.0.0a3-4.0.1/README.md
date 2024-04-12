# Comparing `tmp/fixinventorylib-4.0.0a3.tar.gz` & `tmp/fixinventorylib-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorylib-4.0.0a3.tar", last modified: Wed Feb 28 15:43:06 2024, max compression
+gzip compressed data, was "fixinventorylib-4.0.1.tar", last modified: Thu Mar 14 14:09:46 2024, max compression
```

## Comparing `fixinventorylib-4.0.0a3.tar` & `fixinventorylib-4.0.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.906131 fixinventorylib-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-28 15:43:06.906131 fixinventorylib-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.902131 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-28 15:43:06.000000 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-02-28 15:43:06.000000 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:43:06.000000 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:39:34.000000 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-28 15:43:06.000000 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-28 15:43:06.000000 fixinventorylib-4.0.0a3/fixinventorylib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.894131 fixinventorylib-4.0.0a3/fixlib/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.894131 fixinventorylib-4.0.0a3/fixlib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.894131 fixinventorylib-4.0.0a3/fixlib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    49892 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.898131 fixinventorylib-4.0.0a3/fixlib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/durations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.898131 fixinventorylib-4.0.0a3/fixlib/graph/
--rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17747 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.898131 fixinventorylib-4.0.0a3/fixlib/log/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/proc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)    33802 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    19996 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.898131 fixinventorylib-4.0.0a3/fixlib/web/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.902131 fixinventorylib-4.0.0a3/fixlib/web/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/fixlib/x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-28 15:43:06.906131 fixinventorylib-4.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:43:06.902131 fixinventorylib-4.0.0a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-28 15:38:39.000000 fixinventorylib-4.0.0a3/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.521453 fixinventorylib-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-14 14:09:46.521453 fixinventorylib-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.521453 fixinventorylib-4.0.1/fixinventorylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-14 14:09:46.000000 fixinventorylib-4.0.1/fixinventorylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-14 14:09:46.000000 fixinventorylib-4.0.1/fixinventorylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:09:46.000000 fixinventorylib-4.0.1/fixinventorylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:06:18.000000 fixinventorylib-4.0.1/fixinventorylib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-14 14:09:46.000000 fixinventorylib-4.0.1/fixinventorylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-14 14:09:46.000000 fixinventorylib-4.0.1/fixinventorylib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.513453 fixinventorylib-4.0.1/fixlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.513453 fixinventorylib-4.0.1/fixlib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.513453 fixinventorylib-4.0.1/fixlib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49892 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.513453 fixinventorylib-4.0.1/fixlib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6881 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16100 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.513453 fixinventorylib-4.0.1/fixlib/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)    28662 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17747 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.517453 fixinventorylib-4.0.1/fixlib/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33802 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.517453 fixinventorylib-4.0.1/fixlib/web/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.517453 fixinventorylib-4.0.1/fixlib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31503 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/fixlib/x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-14 14:09:46.521453 fixinventorylib-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:09:46.521453 fixinventorylib-4.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17394 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-14 14:05:23.000000 fixinventorylib-4.0.1/test/test_x509.py
```

### Comparing `fixinventorylib-4.0.0a3/PKG-INFO` & `fixinventorylib-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorylib
-Version: 4.0.0a3
+Version: 4.0.1
 Summary: Fix Inventory common library.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fixinventory/tree/main/fixlib
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
@@ -73,12 +73,12 @@
 * [License](#license)
 
 
 ## Overview
 This is the Fix Inventory common library. Any functionality that is required by more than one of [our components](https://github.com/someengineering/fixinventory#component-list) will be put in here.
 
 ## Contact
-If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/fixinventory/issues/new).
+If you have any questions feel free to [join our Discord](https://discord.gg/fixsecurity) or [open a GitHub issue](https://github.com/someengineering/fixinventory/issues/new).
 
 
 ## License
 See [LICENSE](../LICENSE) for details.
```

### Comparing `fixinventorylib-4.0.0a3/README.md` & `fixinventorylib-4.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 * [License](#license)
 
 
 ## Overview
 This is the Fix Inventory common library. Any functionality that is required by more than one of [our components](https://github.com/someengineering/fixinventory#component-list) will be put in here.
 
 ## Contact
-If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/fixinventory/issues/new).
+If you have any questions feel free to [join our Discord](https://discord.gg/fixsecurity) or [open a GitHub issue](https://github.com/someengineering/fixinventory/issues/new).
 
 
 ## License
 See [LICENSE](../LICENSE) for details.
```

### Comparing `fixinventorylib-4.0.0a3/fixinventorylib.egg-info/PKG-INFO` & `fixinventorylib-4.0.1/fixinventorylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorylib
-Version: 4.0.0a3
+Version: 4.0.1
 Summary: Fix Inventory common library.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fixinventory/tree/main/fixlib
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
@@ -73,12 +73,12 @@
 * [License](#license)
 
 
 ## Overview
 This is the Fix Inventory common library. Any functionality that is required by more than one of [our components](https://github.com/someengineering/fixinventory#component-list) will be put in here.
 
 ## Contact
-If you have any questions feel free to [join our Discord](https://discord.gg/someengineering) or [open a GitHub issue](https://github.com/someengineering/fixinventory/issues/new).
+If you have any questions feel free to [join our Discord](https://discord.gg/fixsecurity) or [open a GitHub issue](https://github.com/someengineering/fixinventory/issues/new).
 
 
 ## License
 See [LICENSE](../LICENSE) for details.
```

### Comparing `fixinventorylib-4.0.0a3/fixinventorylib.egg-info/SOURCES.txt` & `fixinventorylib-4.0.1/fixinventorylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/args.py` & `fixinventorylib-4.0.1/fixlib/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 
 # removed from types in 3.0-3.9: introduced again in 3.10
 NoneType = type(None)
 
 
 def convert(value: Any, type_goal: Union[type, Callable[[Any], Any]]) -> Any:
-    if type_goal is NoneType:  # type: ignore
+    if type_goal is NoneType:
         return value
     elif isinstance(type_goal, type):
         try:
             if type_goal in (str, int, float, complex):
                 return type_goal(value)
             elif type_goal is bool:
                 return value.lower() in ("true", "1", "yes")
```

### Comparing `fixinventorylib-4.0.0a3/fixlib/asynchronous/utils.py` & `fixinventorylib-4.0.1/fixlib/asynchronous/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/asynchronous/web/runner.py` & `fixinventorylib-4.0.1/fixlib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/asynchronous/web/ws_handler.py` & `fixinventorylib-4.0.1/fixlib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/baseplugin.py` & `fixinventorylib-4.0.1/fixlib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/baseresources.py` & `fixinventorylib-4.0.1/fixlib/baseresources.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/config.py` & `fixinventorylib-4.0.1/fixlib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,15 @@
                     log.error(f"Invalid config override {override}")
                     continue
                 config_key, config_value = override.split("=", 1)
                 if "." not in config_key:
                     log.error(f"Invalid config override {config_key}")
                     continue
 
+                config_key = config_key.replace("resoto", "fix")  # backwards compatibility
                 config_keys = config_key.split(".")
                 num_keys = len(config_keys)
                 config_part = running_config.data
                 set_value = False
 
                 # By default we cast the override value to the type of the current
                 # value. This works for most cases including dictionary values.
```

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/__init__.py` & `fixinventorylib-4.0.1/fixlib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/actions.py` & `fixinventorylib-4.0.1/fixlib/core/actions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/ca.py` & `fixinventorylib-4.0.1/fixlib/core/ca.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from fixlib.jwt import decode_jwt_from_headers, encode_jwt_to_headers
 from cryptography.x509.base import Certificate
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 from tempfile import TemporaryDirectory
 from threading import Lock, Event, Thread, Condition
 from fixlib.logger import log
 from fixlib.event import add_event_listener, Event as FixEvent, EventType
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from jwt.exceptions import InvalidSignatureError
 
 
 class FingerprintError(Exception):
     pass
 
 
@@ -193,15 +193,15 @@
     def __certificates_watcher(self) -> None:
         while True:
             with self.__exit:
                 if self.__loaded.is_set():
                     for cert in (self.__ca_cert, self.__cert):
                         if (
                             isinstance(cert, Certificate)
-                            and cert.not_valid_after < datetime.utcnow() - self.renew_before
+                            and cert.not_valid_after_utc < datetime.now(timezone.utc) - self.renew_before
                         ):
                             self.reload()
                             break
                     self.__refresh_files_on_disk()
                 if self.__exit.wait(60):
                     break
```

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/config.py` & `fixinventorylib-4.0.1/fixlib/core/config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/custom_command.py` & `fixinventorylib-4.0.1/fixlib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/events.py` & `fixinventorylib-4.0.1/fixlib/core/events.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/model_check.py` & `fixinventorylib-4.0.1/fixlib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/model_export.py` & `fixinventorylib-4.0.1/fixlib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/progress.py` & `fixinventorylib-4.0.1/fixlib/core/progress.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/search.py` & `fixinventorylib-4.0.1/fixlib/core/search.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/core/tasks.py` & `fixinventorylib-4.0.1/fixlib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/durations.py` & `fixinventorylib-4.0.1/fixlib/durations.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/event.py` & `fixinventorylib-4.0.1/fixlib/event.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/graph/__init__.py` & `fixinventorylib-4.0.1/fixlib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/graph/graph_extensions.py` & `fixinventorylib-4.0.1/fixlib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/json.py` & `fixinventorylib-4.0.1/fixlib/json.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/json_bender.py` & `fixinventorylib-4.0.1/fixlib/json_bender.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/jwt.py` & `fixinventorylib-4.0.1/fixlib/jwt.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/lock.py` & `fixinventorylib-4.0.1/fixlib/lock.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/logger.py` & `fixinventorylib-4.0.1/fixlib/logger.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/parse_util.py` & `fixinventorylib-4.0.1/fixlib/parse_util.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/proc.py` & `fixinventorylib-4.0.1/fixlib/proc.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/threading.py` & `fixinventorylib-4.0.1/fixlib/threading.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/tree.py` & `fixinventorylib-4.0.1/fixlib/tree.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/utils.py` & `fixinventorylib-4.0.1/fixlib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -569,7 +569,18 @@
 
     if isinstance(elem, Sequence):
         return tuple([freeze(v) for v in elem])
     elif isinstance(elem, Mapping):
         return frozendict({k: freeze(v) for k, v in elem.items()})
     else:
         return elem
+
+
+def ensure_bw_compat() -> None:
+    for i, arg in enumerate(sys.argv):
+        if arg.startswith("--resoto"):
+            sys.argv[i] = "--fix" + arg[len("--resoto") :]
+
+    old_env_vars = [key for key in os.environ if key.startswith("RESOTO")]
+    for old_env_var in old_env_vars:
+        new_env_var = old_env_var.replace("RESOTO", "FIX")
+        os.environ[new_env_var] = os.environ.pop(old_env_var)
```

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/__init__.py` & `fixinventorylib-4.0.1/fixlib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/metrics.py` & `fixinventorylib-4.0.1/fixlib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/android-chrome-192x192.png` & `fixinventorylib-4.0.1/fixlib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/android-chrome-512x512.png` & `fixinventorylib-4.0.1/fixlib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/apple-touch-icon.png` & `fixinventorylib-4.0.1/fixlib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/favicon-16x16.png` & `fixinventorylib-4.0.1/fixlib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/favicon-32x32.png` & `fixinventorylib-4.0.1/fixlib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/index.html` & `fixinventorylib-4.0.1/fixlib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/mstile-150x150.png` & `fixinventorylib-4.0.1/fixlib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/web/static/picnic.min.css` & `fixinventorylib-4.0.1/fixlib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/fixlib/x509.py` & `fixinventorylib-4.0.1/fixlib/x509.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,18 +281,20 @@
 def load_cert_from_bytes(cert: bytes) -> Certificate:
     return x509.load_pem_x509_certificate(cert, default_backend())
 
 
 def load_key_from_bytes(
     key: bytes, passphrase: Optional[str] = None, skip_rsa_key_validation: bool = False
 ) -> RSAPrivateKey:
-    backend = default_backend()
-    if passphrase is not None:
-        passphrase = passphrase.encode()  # type: ignore
-    return backend.load_pem_private_key(key, passphrase, skip_rsa_key_validation)  # type: ignore
+    passphrase_bytes: Optional[bytes] = passphrase.encode() if passphrase is not None else None
+    private_key = serialization.load_pem_private_key(
+        key, passphrase_bytes, unsafe_skip_rsa_key_validation=skip_rsa_key_validation
+    )
+    assert isinstance(private_key, RSAPrivateKey)
+    return private_key
 
 
 def make_ip(ip: str) -> Union[IPv4Address, IPv6Address, IPv4Network, IPv6Network]:
     if "/" in ip:
         return ip_network(ip)
     else:
         return ip_address(ip)
```

### Comparing `fixinventorylib-4.0.0a3/pyproject.toml` & `fixinventorylib-4.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventorylib"
-version = "4.0.0a3"
+version = "4.0.1"
 authors = [{ name = "Some Engineering Inc." }]
 description = "Fix Inventory common library."
 license = { text = "AGPLv3" }
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
```

### Comparing `fixinventorylib-4.0.0a3/test/test_args.py` & `fixinventorylib-4.0.1/test/test_args.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_baseresources.py` & `fixinventorylib-4.0.1/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_config.py` & `fixinventorylib-4.0.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_graph.py` & `fixinventorylib-4.0.1/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_graph_extensions.py` & `fixinventorylib-4.0.1/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_json.py` & `fixinventorylib-4.0.1/test/test_json.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_jwt.py` & `fixinventorylib-4.0.1/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_plugin.py` & `fixinventorylib-4.0.1/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_tree.py` & `fixinventorylib-4.0.1/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_utils.py` & `fixinventorylib-4.0.1/test/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import unittest
 import threading
 import time
 import copy
+import os
+from unittest.mock import patch
 from datetime import datetime
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     from backports.zoneinfo import ZoneInfo
 from tempfile import TemporaryDirectory
@@ -16,17 +18,18 @@
     rrdata_as_dict,
     get_local_tzinfo,
     utc_str,
     replace_env_vars,
     merge_json_elements,
     drop_deleted_attributes,
     freeze,
+    stdin_generator,
+    ensure_bw_compat,
 )
 from fixlib.baseresources import BaseResource
-from fixlib.utils import stdin_generator
 from attrs import define
 from typing import ClassVar
 import pytest
 import sys
 import tempfile
 from contextlib import contextmanager
 from frozendict import frozendict
@@ -474,7 +477,35 @@
     flat_dict = {"foo": "bar"}
     assert freeze(flat_dict) == frozendict(flat_dict)
     # nested too
     nested_dict = {"foo": flat_dict}
     assert freeze(nested_dict) == frozendict({"foo": frozendict(flat_dict)})
     # and a list to tupple
     assert freeze([1, 2]) == (1, 2)
+
+
+def test_ensure_bw_compat_cli_args():
+    with patch("sys.argv", ["program_name", "--resotocore-uri", "some_value", "--another-arg"]):
+        ensure_bw_compat()
+        assert sys.argv == ["program_name", "--fixcore-uri", "some_value", "--another-arg"]
+
+
+def test_ensure_bw_compat_env_vars_single_replacement():
+    with patch.dict("os.environ", {"RESOTOCORE_URI": "123", "OTHER_ENV_VAR": "abc"}):
+        ensure_bw_compat()
+        assert "FIXCORE_URI" in os.environ
+        assert os.environ["FIXCORE_URI"] == "123"
+        assert "OTHER_ENV_VAR" in os.environ
+
+
+def test_ensure_bw_compat_env_vars_multiple_replacements():
+    with patch.dict("os.environ", {"RESOTOWORKER_RESOTOCORE_URI": "123"}):
+        ensure_bw_compat()
+        assert "FIXWORKER_FIXCORE_URI" in os.environ
+        assert os.environ["FIXWORKER_FIXCORE_URI"] == "123"
+
+
+def test_ensure_bw_compat_no_changes_needed():
+    with patch("sys.argv", ["program_name", "--another-arg"]), patch.dict("os.environ", {"OTHER_ENV_VAR": "abc"}):
+        ensure_bw_compat()
+        assert sys.argv == ["program_name", "--another-arg"]
+        assert "OTHER_ENV_VAR" in os.environ
```

### Comparing `fixinventorylib-4.0.0a3/test/test_web.py` & `fixinventorylib-4.0.1/test/test_web.py`

 * *Files identical despite different names*

### Comparing `fixinventorylib-4.0.0a3/test/test_x509.py` & `fixinventorylib-4.0.1/test/test_x509.py`

 * *Files identical despite different names*

