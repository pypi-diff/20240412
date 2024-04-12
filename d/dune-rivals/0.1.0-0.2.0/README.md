# Comparing `tmp/dune-rivals-0.1.0.tar.gz` & `tmp/dune_rivals-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune-rivals-0.1.0.tar", last modified: Thu Apr 11 16:04:39 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.tar", last modified: Fri Apr 12 20:07:50 2024, max compression
```

## Comparing `dune-rivals-0.1.0.tar` & `dune_rivals-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-11 16:04:39.552904 dune-rivals-0.1.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      436 2024-04-11 16:04:39.552904 dune-rivals-0.1.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-11 15:59:50.000000 dune-rivals-0.1.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-11 16:04:39.552904 dune-rivals-0.1.0/dune_rivals.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      436 2024-04-11 16:04:39.000000 dune-rivals-0.1.0/dune_rivals.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2024-04-11 16:04:39.000000 dune-rivals-0.1.0/dune_rivals.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-11 16:04:39.000000 dune-rivals-0.1.0/dune_rivals.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-04-11 16:04:39.000000 dune-rivals-0.1.0/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      527 2024-04-11 15:38:02.000000 dune-rivals-0.1.0/dune_rivals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      503 2024-04-11 16:02:33.000000 dune-rivals-0.1.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-11 16:04:39.552904 dune-rivals-0.1.0/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:07:50.547628 dune_rivals-0.2/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:07:50.547212 dune_rivals-0.2/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:07:50.546760 dune_rivals-0.2/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     7771 2024-04-12 20:02:16.000000 dune_rivals-0.2/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:07:35.000000 dune_rivals-0.2/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:07:50.547720 dune_rivals-0.2/setup.cfg
```

