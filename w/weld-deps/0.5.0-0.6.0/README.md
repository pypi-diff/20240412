# Comparing `tmp/weld_deps-0.5.0.tar.gz` & `tmp/weld_deps-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weld_deps-0.5.0.tar", max compression
+gzip compressed data, was "weld_deps-0.6.0.tar", max compression
```

## Comparing `weld_deps-0.5.0.tar` & `weld_deps-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-12 06:34:07.110074 weld_deps-0.5.0/LICENSE
--rw-r--r--   0        0        0      333 2024-04-12 06:34:24.490205 weld_deps-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-12 06:34:07.114074 weld_deps-0.5.0/weld_deps/__init__.py
--rw-r--r--   0        0        0     5879 2024-04-12 06:34:07.114074 weld_deps-0.5.0/weld_deps/dep.py
--rw-r--r--   0        0        0      423 2024-04-12 06:34:07.114074 weld_deps-0.5.0/weld_deps/examples/pack1/beet.yaml
--rw-r--r--   0        0        0        0 2024-04-12 06:34:07.114074 weld_deps-0.5.0/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
--rw-r--r--   0        0        0     1729 2024-04-12 06:34:07.114074 weld_deps-0.5.0/weld_deps/main.py
--rw-r--r--   0        0        0     4855 2024-04-12 06:34:07.114074 weld_deps-0.5.0/weld_deps/utils.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 06:39:32.802835 weld_deps-0.6.0/LICENSE
+-rw-r--r--   0        0        0      333 2024-04-12 06:39:46.971051 weld_deps-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-12 06:39:32.802835 weld_deps-0.6.0/weld_deps/__init__.py
+-rw-r--r--   0        0        0     5879 2024-04-12 06:39:32.802835 weld_deps-0.6.0/weld_deps/dep.py
+-rw-r--r--   0        0        0      423 2024-04-12 06:39:32.802835 weld_deps-0.6.0/weld_deps/examples/pack1/beet.yaml
+-rw-r--r--   0        0        0        0 2024-04-12 06:39:32.802835 weld_deps-0.6.0/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
+-rw-r--r--   0        0        0     1729 2024-04-12 06:39:32.802835 weld_deps-0.6.0/weld_deps/main.py
+-rw-r--r--   0        0        0     4855 2024-04-12 06:39:32.802835 weld_deps-0.6.0/weld_deps/utils.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.6.0/PKG-INFO
```

### Comparing `weld_deps-0.5.0/LICENSE` & `weld_deps-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weld_deps-0.5.0/weld_deps/dep.py` & `weld_deps-0.6.0/weld_deps/dep.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.5.0/weld_deps/main.py` & `weld_deps-0.6.0/weld_deps/main.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.5.0/weld_deps/utils.py` & `weld_deps-0.6.0/weld_deps/utils.py`

 * *Files identical despite different names*

