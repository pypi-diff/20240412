# Comparing `tmp/ktianc-0.1.1.tar.gz` & `tmp/ktianc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktianc-0.1.1.tar", max compression
+gzip compressed data, was "ktianc-0.3.0.tar", max compression
```

## Comparing `ktianc-0.1.1.tar` & `ktianc-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-26 07:29:13.734004 ktianc-0.1.1/ktianc/__init__.py
--rw-r--r--   0        0        0       41 2024-03-26 08:13:42.825134 ktianc-0.1.1/ktianc/main.py
--rw-r--r--   0        0        0      325 2024-03-26 08:15:06.886415 ktianc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       27 2024-03-26 07:46:24.001329 ktianc-0.1.1/README.md
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 ktianc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      463 2024-04-12 01:49:56.837756 ktianc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2633 2024-04-02 06:15:47.144933 ktianc-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 07:29:13.734004 ktianc-0.3.0/src/__init__.py
+-rw-r--r--   0        0        0      436 2024-04-12 01:49:00.528066 ktianc-0.3.0/src/main.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 ktianc-0.3.0/PKG-INFO
```

