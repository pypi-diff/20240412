# Comparing `tmp/declare-0.0.1.tar.gz` & `tmp/declare-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "declare-0.0.1.tar", last modified: Tue Aug 31 00:34:30 2021, max compression
+gzip compressed data, was "declare-1.0.0.tar", max compression
```

## Comparing `declare-0.0.1.tar` & `declare-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,7 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2021-08-31 00:34:30.769770 declare-0.0.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)      517 2021-08-31 00:34:30.769770 declare-0.0.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)       54 2021-08-30 21:09:07.000000 declare-0.0.1/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2021-08-31 00:34:30.765770 declare-0.0.1/declare/
--rw-rw-r--   0 chris     (1000) chris     (1000)      362 2021-08-30 23:34:06.000000 declare-0.0.1/declare/__init__.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2021-08-31 00:34:30.769770 declare-0.0.1/declare.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      517 2021-08-31 00:34:30.000000 declare-0.0.1/declare.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      247 2021-08-31 00:34:30.000000 declare-0.0.1/declare.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2021-08-31 00:34:30.000000 declare-0.0.1/declare.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       14 2021-08-31 00:34:30.000000 declare-0.0.1/declare.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2021-08-31 00:34:30.769770 declare-0.0.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      689 2021-08-30 21:19:50.000000 declare-0.0.1/setup.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2021-08-31 00:34:30.769770 declare-0.0.1/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2021-08-30 21:21:24.000000 declare-0.0.1/tests/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      254 2021-08-30 23:31:23.000000 declare-0.0.1/tests/test_base.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      430 2021-08-30 23:42:41.000000 declare-0.0.1/tests/test_controller.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      358 2021-08-30 23:39:19.000000 declare-0.0.1/tests/test_stateful.py
+-rw-r--r--   0        0        0     1069 2024-04-12 11:18:31.938782 declare-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6045 2024-04-12 11:20:03.194526 declare-1.0.0/README.md
+-rw-r--r--   0        0        0      332 2024-04-12 11:20:23.375409 declare-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      371 2024-04-12 11:18:31.948419 declare-1.0.0/src/declare/__init__.py
+-rw-r--r--   0        0        0     6013 2024-04-12 11:18:31.949028 declare-1.0.0/src/declare/_declare.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:18:31.949073 declare-1.0.0/src/declare/py.typed
+-rw-r--r--   0        0        0     6667 1970-01-01 00:00:00.000000 declare-1.0.0/PKG-INFO
```

