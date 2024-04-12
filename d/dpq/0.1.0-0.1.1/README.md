# Comparing `tmp/dpq-0.1.0.tar.gz` & `tmp/dpq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpq-0.1.0.tar", max compression
+gzip compressed data, was "dpq-0.1.1.tar", max compression
```

## Comparing `dpq-0.1.0.tar` & `dpq-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-07 21:10:10.603839 dpq-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-07 21:10:10.603720 dpq-0.1.0/dpq/__init__.py
--rw-r--r--   0        0        0      253 2024-04-07 21:12:05.088666 dpq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dpq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3693 2024-04-12 07:53:08.845937 dpq-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2024-04-09 07:16:40.852521 dpq-0.1.1/dpq/__init__.py
+-rw-r--r--   0        0        0     5420 2024-04-12 15:14:34.552495 dpq-0.1.1/dpq/dpq.py
+-rw-r--r--   0        0        0      420 2024-04-12 15:18:46.396089 dpq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 dpq-0.1.1/PKG-INFO
```

