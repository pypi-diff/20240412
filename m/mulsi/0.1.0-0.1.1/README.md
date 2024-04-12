# Comparing `tmp/mulsi-0.1.0.tar.gz` & `tmp/mulsi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mulsi-0.1.0.tar", max compression
+gzip compressed data, was "mulsi-0.1.1.tar", max compression
```

## Comparing `mulsi-0.1.0.tar` & `mulsi-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0     1088 2024-01-31 21:19:50.899523 mulsi-0.1.0/LICENSE
--rw-r--r--   0        0        0       82 2024-01-31 21:19:50.899523 mulsi-0.1.0/README.md
--rw-r--r--   0        0        0      803 2024-01-31 21:19:50.899523 mulsi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       65 2024-01-31 21:19:50.899523 mulsi-0.1.0/src/mulsi/__init__.py
--rw-r--r--   0        0        0     4569 2024-01-31 21:19:50.899523 mulsi-0.1.0/src/mulsi/hook.py
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 mulsi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-12 20:48:26.813043 mulsi-0.1.1/LICENSE
+-rw-r--r--   0        0        0       82 2024-04-12 20:48:26.813043 mulsi-0.1.1/README.md
+-rw-r--r--   0        0        0     1247 2024-04-12 20:48:26.817044 mulsi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/__init__.py
+-rw-r--r--   0        0        0     3104 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/adversarial.py
+-rw-r--r--   0        0        0     5486 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/hook.py
+-rw-r--r--   0        0        0     3154 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/probe.py
+-rw-r--r--   0        0        0     2097 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/processor.py
+-rw-r--r--   0        0        0     1058 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/reader.py
+-rw-r--r--   0        0        0     4043 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/representation.py
+-rw-r--r--   0        0        0     2206 2024-04-12 20:48:26.817044 mulsi-0.1.1/src/mulsi/wrapper.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 mulsi-0.1.1/PKG-INFO
```

### Comparing `mulsi-0.1.0/LICENSE` & `mulsi-0.1.1/LICENSE`

 * *Files identical despite different names*

