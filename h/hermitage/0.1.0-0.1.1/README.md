# Comparing `tmp/hermitage-0.1.0.tar.gz` & `tmp/hermitage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage-0.1.0.tar", max compression
+gzip compressed data, was "hermitage-0.1.1.tar", max compression
```

## Comparing `hermitage-0.1.0.tar` & `hermitage-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-01-29 14:06:18.529729 hermitage-0.1.0/hermitage/__init__.py
--rw-r--r--   0        0        0       26 2024-01-29 14:06:44.218174 hermitage-0.1.0/hermitage/main.py
--rw-r--r--   0        0        0      271 2024-01-29 14:06:08.173472 hermitage-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 hermitage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage-0.1.1/README.md
+-rw-r--r--   0        0        0      261 2024-04-02 15:23:42.889428 hermitage-0.1.1/hermitage/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.889513 hermitage-0.1.1/hermitage/definition/__init__.py
+-rw-r--r--   0        0        0    11824 2024-04-02 15:23:42.889642 hermitage-0.1.1/hermitage/definition/contracts.py
+-rw-r--r--   0        0        0       44 2024-04-02 15:23:42.889741 hermitage-0.1.1/hermitage/mappers/__init__.py
+-rw-r--r--   0        0        0     1035 2024-04-11 07:57:07.718429 hermitage-0.1.1/hermitage/mappers/invoice.py
+-rw-r--r--   0        0        0       31 2024-04-02 15:23:42.889934 hermitage-0.1.1/hermitage/parsers/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-05 16:44:15.856958 hermitage-0.1.1/hermitage/parsers/query.py
+-rw-r--r--   0        0        0      271 2024-04-12 12:56:03.500345 hermitage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 hermitage-0.1.1/PKG-INFO
```

