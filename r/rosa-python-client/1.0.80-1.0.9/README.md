# Comparing `tmp/rosa_python_client-1.0.80.tar.gz` & `tmp/rosa_python_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.80.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.9.tar", max compression
```

## Comparing `rosa_python_client-1.0.80.tar` & `rosa_python_client-1.0.9.tar`

### file list

```diff
@@ -1,9 +1,5 @@
--rw-r--r--   0        0        0      865 2024-04-12 08:07:56.935917 rosa_python_client-1.0.80/README.md
--rw-r--r--   0        0        0     1412 2024-04-12 08:08:01.382882 rosa_python_client-1.0.80/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 08:07:56.936917 rosa_python_client-1.0.80/rosa/__init__.py
--rw-r--r--   0        0        0    11119 2024-04-12 08:07:56.936917 rosa_python_client-1.0.80/rosa/cli.py
--rw-r--r--   0        0        0        0 2024-04-12 08:07:56.936917 rosa_python_client-1.0.80/rosa/tests/__init__.py
--rw-r--r--   0        0        0      843 2024-04-12 08:07:56.936917 rosa_python_client-1.0.80/rosa/tests/conftest.py
--rw-r--r--   0        0        0       30 2024-04-12 08:07:56.936917 rosa_python_client-1.0.80/rosa/tests/const.py
--rw-r--r--   0        0        0     1031 2024-04-12 08:07:56.937917 rosa_python_client-1.0.80/rosa/tests/test_parse_command.py
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 rosa_python_client-1.0.80/PKG-INFO
+-rw-r--r--   0        0        0      511 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/README.md
+-rw-r--r--   0        0        0      353 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/rosa/__init__.py
+-rw-r--r--   0        0        0     8586 2023-06-14 13:03:12.785023 rosa_python_client-1.0.9/rosa/cli.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 rosa_python_client-1.0.9/PKG-INFO
```

