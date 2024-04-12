# Comparing `tmp/dumbo_runlim-0.2.5.tar.gz` & `tmp/dumbo_runlim-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_runlim-0.2.5.tar", max compression
+gzip compressed data, was "dumbo_runlim-0.2.6.tar", max compression
```

## Comparing `dumbo_runlim-0.2.5.tar` & `dumbo_runlim-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-03-12 08:28:59.154903 dumbo_runlim-0.2.5/LICENSE
--rw-r--r--   0        0        0       14 2024-03-12 08:28:59.154903 dumbo_runlim-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-03-12 08:28:59.154903 dumbo_runlim-0.2.5/dumbo_runlim/__init__.py
--rw-r--r--   0        0        0      102 2024-03-12 08:28:59.154903 dumbo_runlim-0.2.5/dumbo_runlim/__main__.py
--rw-r--r--   0        0        0     2475 2024-03-13 08:40:24.415657 dumbo_runlim-0.2.5/dumbo_runlim/cli.py
--rw-r--r--   0        0        0        0 2024-03-12 08:28:59.154903 dumbo_runlim-0.2.5/dumbo_runlim/experiments/__init__.py
--rw-r--r--   0        0        0      299 2024-03-12 15:56:24.333800 dumbo_runlim-0.2.5/dumbo_runlim/experiments/example.py
--rw-r--r--   0        0        0      975 2024-03-13 09:00:41.667543 dumbo_runlim-0.2.5/dumbo_runlim/experiments/ucorexplain.py
--rw-r--r--   0        0        0     8768 2024-03-13 08:40:24.419656 dumbo_runlim-0.2.5/dumbo_runlim/utils.py
--rw-r--r--   0        0        0      467 2024-03-13 08:58:13.249183 dumbo_runlim-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 dumbo_runlim-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-23 16:20:25.294556 dumbo_runlim-0.2.6/LICENSE
+-rw-r--r--   0        0        0       14 2023-12-23 16:20:25.294556 dumbo_runlim-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-12-23 16:19:03.028140 dumbo_runlim-0.2.6/dumbo_runlim/__init__.py
+-rw-r--r--   0        0        0      102 2024-03-09 07:30:56.525269 dumbo_runlim-0.2.6/dumbo_runlim/__main__.py
+-rw-r--r--   0        0        0     2475 2024-03-12 21:35:19.350072 dumbo_runlim-0.2.6/dumbo_runlim/cli.py
+-rw-r--r--   0        0        0        0 2024-03-09 07:24:54.509832 dumbo_runlim-0.2.6/dumbo_runlim/experiments/__init__.py
+-rw-r--r--   0        0        0      299 2024-03-09 12:00:37.999878 dumbo_runlim-0.2.6/dumbo_runlim/experiments/example.py
+-rw-r--r--   0        0        0      975 2024-03-13 13:11:55.500475 dumbo_runlim-0.2.6/dumbo_runlim/experiments/ucorexplain.py
+-rw-r--r--   0        0        0      967 2024-04-12 16:50:16.340524 dumbo_runlim-0.2.6/dumbo_runlim/experiments/xasp.py
+-rw-r--r--   0        0        0     8768 2024-03-12 21:43:17.604642 dumbo_runlim-0.2.6/dumbo_runlim/utils.py
+-rw-r--r--   0        0        0      467 2024-04-12 16:50:16.364524 dumbo_runlim-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 dumbo_runlim-0.2.6/PKG-INFO
```

### Comparing `dumbo_runlim-0.2.5/LICENSE` & `dumbo_runlim-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_runlim-0.2.5/dumbo_runlim/cli.py` & `dumbo_runlim-0.2.6/dumbo_runlim/cli.py`

 * *Files identical despite different names*

### Comparing `dumbo_runlim-0.2.5/dumbo_runlim/experiments/ucorexplain.py` & `dumbo_runlim-0.2.6/dumbo_runlim/experiments/ucorexplain.py`

 * *Files identical despite different names*

### Comparing `dumbo_runlim-0.2.5/dumbo_runlim/utils.py` & `dumbo_runlim-0.2.6/dumbo_runlim/utils.py`

 * *Files identical despite different names*

