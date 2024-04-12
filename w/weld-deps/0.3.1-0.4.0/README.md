# Comparing `tmp/weld_deps-0.3.1.tar.gz` & `tmp/weld_deps-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weld_deps-0.3.1.tar", max compression
+gzip compressed data, was "weld_deps-0.4.0.tar", max compression
```

## Comparing `weld_deps-0.3.1.tar` & `weld_deps-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-12 06:28:50.824636 weld_deps-0.3.1/LICENSE
--rw-r--r--   0        0        0      333 2024-04-12 06:29:06.032597 weld_deps-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-12 06:28:50.824636 weld_deps-0.3.1/weld_deps/__init__.py
--rw-r--r--   0        0        0     5879 2024-04-12 06:28:50.824636 weld_deps-0.3.1/weld_deps/dep.py
--rw-r--r--   0        0        0      423 2024-04-12 06:28:50.824636 weld_deps-0.3.1/weld_deps/examples/pack1/beet.yaml
--rw-r--r--   0        0        0        0 2024-04-12 06:28:50.824636 weld_deps-0.3.1/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
--rw-r--r--   0        0        0     1729 2024-04-12 06:28:50.824636 weld_deps-0.3.1/weld_deps/main.py
--rw-r--r--   0        0        0     4855 2024-04-12 06:28:50.824636 weld_deps-0.3.1/weld_deps/utils.py
--rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 06:30:16.954829 weld_deps-0.4.0/LICENSE
+-rw-r--r--   0        0        0      333 2024-04-12 06:30:31.514862 weld_deps-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-12 06:30:16.954829 weld_deps-0.4.0/weld_deps/__init__.py
+-rw-r--r--   0        0        0     5879 2024-04-12 06:30:16.954829 weld_deps-0.4.0/weld_deps/dep.py
+-rw-r--r--   0        0        0      423 2024-04-12 06:30:16.954829 weld_deps-0.4.0/weld_deps/examples/pack1/beet.yaml
+-rw-r--r--   0        0        0        0 2024-04-12 06:30:16.954829 weld_deps-0.4.0/weld_deps/examples/pack1/src/data/pack1/functions/test.mcfunction
+-rw-r--r--   0        0        0     1729 2024-04-12 06:30:16.954829 weld_deps-0.4.0/weld_deps/main.py
+-rw-r--r--   0        0        0     4855 2024-04-12 06:30:16.954829 weld_deps-0.4.0/weld_deps/utils.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 weld_deps-0.4.0/PKG-INFO
```

### Comparing `weld_deps-0.3.1/LICENSE` & `weld_deps-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weld_deps-0.3.1/weld_deps/dep.py` & `weld_deps-0.4.0/weld_deps/dep.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.3.1/weld_deps/main.py` & `weld_deps-0.4.0/weld_deps/main.py`

 * *Files identical despite different names*

### Comparing `weld_deps-0.3.1/weld_deps/utils.py` & `weld_deps-0.4.0/weld_deps/utils.py`

 * *Files identical despite different names*

