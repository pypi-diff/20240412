# Comparing `tmp/SeqTools-1.4.0.tar.gz` & `tmp/seqtools-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeqTools-1.4.0.tar", last modified: Thu Nov 23 21:14:41 2023, max compression
+gzip compressed data, was "seqtools-1.4.1.tar", last modified: Fri Apr 12 20:48:26 2024, max compression
```

## Comparing `SeqTools-1.4.0.tar` & `seqtools-1.4.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.058519 SeqTools-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.046519 SeqTools-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.050519 SeqTools-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-11-23 21:14:34.000000 SeqTools-1.4.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-11-23 21:14:34.000000 SeqTools-1.4.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-23 21:14:34.000000 SeqTools-1.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-11-23 21:14:34.000000 SeqTools-1.4.0/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2023-11-23 21:14:34.000000 SeqTools-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-11-23 21:14:34.000000 SeqTools-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-11-23 21:14:41.058519 SeqTools-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2023-11-23 21:14:34.000000 SeqTools-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.058519 SeqTools-1.4.0/SeqTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-11-23 21:14:41.000000 SeqTools-1.4.0/SeqTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-11-23 21:14:41.000000 SeqTools-1.4.0/SeqTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 21:14:41.000000 SeqTools-1.4.0/SeqTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-23 21:14:41.000000 SeqTools-1.4.0/SeqTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-23 21:14:41.000000 SeqTools-1.4.0/SeqTools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.050519 SeqTools-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.054519 SeqTools-1.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    35627 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/batch.svg
--rw-r--r--   0 runner    (1001) docker     (127)    51469 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/bird.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    55059 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/collate.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40911 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/concatenate.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20605 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/cycle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    80243 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/dog.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    70459 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/duck.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    32701 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/gather.svg
--rw-r--r--   0 runner    (1001) docker     (127)    66815 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/hedgehog.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47329 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/interleave.svg
--rw-r--r--   0 runner    (1001) docker     (127)    56834 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/owl.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    30710 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/prefetch.svg
--rw-r--r--   0 runner    (1001) docker     (127)   113762 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/rooster.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25638 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/smap.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41181 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/split.svg
--rw-r--r--   0 runner    (1001) docker     (127)    44276 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/switch.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18659 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/_static/uniter.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.054519 SeqTools-1.4.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/examples/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/examples/dataloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/examples/errors_and_debugging.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/examples/preprocessing_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2023-11-23 21:14:34.000000 SeqTools-1.4.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-11-23 21:14:34.000000 SeqTools-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.058519 SeqTools-1.4.0/seqtools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.058519 SeqTools-1.4.0/seqtools/C/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/C/refcountedbuffer.c
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/C/refcountedbuffer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/buffering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15563 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    18214 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10782 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2023-11-23 21:14:34.000000 SeqTools-1.4.0/seqtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 21:14:41.058519 SeqTools-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-23 21:14:34.000000 SeqTools-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 21:14:41.058519 SeqTools-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-11-23 21:14:34.000000 SeqTools-1.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.325880 seqtools-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.313880 seqtools-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.313880 seqtools-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-12 20:48:23.000000 seqtools-1.4.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-12 20:48:23.000000 seqtools-1.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 20:48:23.000000 seqtools-1.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-12 20:48:23.000000 seqtools-1.4.1/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-12 20:48:23.000000 seqtools-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 20:48:23.000000 seqtools-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-12 20:48:26.325880 seqtools-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-12 20:48:23.000000 seqtools-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.325880 seqtools-1.4.1/SeqTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-12 20:48:26.000000 seqtools-1.4.1/SeqTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-12 20:48:26.000000 seqtools-1.4.1/SeqTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:48:26.000000 seqtools-1.4.1/SeqTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 20:48:26.000000 seqtools-1.4.1/SeqTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 20:48:26.000000 seqtools-1.4.1/SeqTools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.317880 seqtools-1.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.321880 seqtools-1.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    35627 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/batch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    51469 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/bird.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    55059 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/collate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40911 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/concatenate.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/cycle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    80243 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/dog.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    70459 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/duck.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/gather.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    66815 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/hedgehog.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    47329 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/interleave.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    56834 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/owl.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    30710 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/prefetch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   113762 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/rooster.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    25638 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/smap.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41181 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/split.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    44276 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18659 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/_static/uniter.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.321880 seqtools-1.4.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/examples/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/examples/dataloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/examples/errors_and_debugging.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/examples/preprocessing_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-12 20:48:23.000000 seqtools-1.4.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-12 20:48:23.000000 seqtools-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.325880 seqtools-1.4.1/seqtools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.325880 seqtools-1.4.1/seqtools/C/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/C/refcountedbuffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/C/refcountedbuffer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/buffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18214 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10782 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-12 20:48:23.000000 seqtools-1.4.1/seqtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:48:26.325880 seqtools-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 20:48:23.000000 seqtools-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:48:26.325880 seqtools-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-12 20:48:23.000000 seqtools-1.4.1/tests/test_utils.py
```

### Comparing `SeqTools-1.4.0/.github/workflows/release.yml` & `seqtools-1.4.1/.github/workflows/release.yml`

 * *Files 10% similar despite different names*

```diff
@@ -5,52 +5,55 @@
   workflow_dispatch:
 
 jobs:
   build-wheels:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-22.04, windows-2022, macos-12]
+        os: [ubuntu-22.04, windows-2022, macos-13, macos-14]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.14.1
+        uses: pypa/cibuildwheel@v2.17.0
 
       - name: Store wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: dist
-          path: wheelhouse/*.whl
+          name: wheels-${{ matrix.os }}
+          path: ./wheelhouse/*.whl
+          overwrite: true
 
   build-sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Build sdist
         run: pipx run build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: dist
+          name: wheels-sdist
           path: dist/*.tar.gz
+          overwrite: true
 
   upload-pypi:
     needs: [build-wheels, build-sdist]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Download dist
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
-          name: dist
+          pattern: wheels-*
           path: dist
+          merge-multiple: true
 
       - name: Store whether the current ref is on main
         id: check-ref-on-main
         run: |
           git fetch --all --filter=tree:0
           printf "ref_on_main=%s\n" \
             $(git branch -a --contains ${{ github.ref_name }} --format "%(refname:short)" \
```

### Comparing `SeqTools-1.4.0/.github/workflows/tests.yml` & `seqtools-1.4.1/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     runs-on: ubuntu-latest
 
     steps:
       - name: ufmt
         uses: omnilib/ufmt@action-v1
         with:
           path: seqtools
-          python-version: "3.11"
+          python-version: "3.10"
 
   unit-tests:
     runs-on: ubuntu-latest
     needs: check-formatting
 
     strategy:
       matrix:
```

### Comparing `SeqTools-1.4.0/CHANGELOG.txt` & `seqtools-1.4.1/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/LICENSE.txt` & `seqtools-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/PKG-INFO` & `seqtools-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeqTools
-Version: 1.4.0
+Version: 1.4.1
 Summary: A library for transparent transformation of indexable containers (lists, etc.)
 Author-email: Nicolas Granger <nicolas.granger.m@gmail.com>
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: PyPi, https://pypi.org/project/SeqTools
 Project-URL: Documentation, http://seqtools-doc.readthedocs.io
 Project-URL: Repository, https://github.com/nlgranger/SeqTools
 Keywords: mapping,lazy,delayed,pipeline,processing
```

### Comparing `SeqTools-1.4.0/README.rst` & `seqtools-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/SeqTools.egg-info/PKG-INFO` & `seqtools-1.4.1/SeqTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeqTools
-Version: 1.4.0
+Version: 1.4.1
 Summary: A library for transparent transformation of indexable containers (lists, etc.)
 Author-email: Nicolas Granger <nicolas.granger.m@gmail.com>
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: PyPi, https://pypi.org/project/SeqTools
 Project-URL: Documentation, http://seqtools-doc.readthedocs.io
 Project-URL: Repository, https://github.com/nlgranger/SeqTools
 Keywords: mapping,lazy,delayed,pipeline,processing
```

### Comparing `SeqTools-1.4.0/SeqTools.egg-info/SOURCES.txt` & `seqtools-1.4.1/SeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/batch.svg` & `seqtools-1.4.1/docs/_static/batch.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/bird.jpg` & `seqtools-1.4.1/docs/_static/bird.jpg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/collate.svg` & `seqtools-1.4.1/docs/_static/collate.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/concatenate.svg` & `seqtools-1.4.1/docs/_static/concatenate.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/cycle.svg` & `seqtools-1.4.1/docs/_static/cycle.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/dog.jpg` & `seqtools-1.4.1/docs/_static/dog.jpg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/duck.jpg` & `seqtools-1.4.1/docs/_static/duck.jpg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/gather.svg` & `seqtools-1.4.1/docs/_static/gather.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/hedgehog.jpg` & `seqtools-1.4.1/docs/_static/hedgehog.jpg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/interleave.svg` & `seqtools-1.4.1/docs/_static/interleave.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/owl.jpg` & `seqtools-1.4.1/docs/_static/owl.jpg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/prefetch.svg` & `seqtools-1.4.1/docs/_static/prefetch.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/rooster.jpg` & `seqtools-1.4.1/docs/_static/rooster.jpg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/smap.svg` & `seqtools-1.4.1/docs/_static/smap.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/split.svg` & `seqtools-1.4.1/docs/_static/split.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/switch.svg` & `seqtools-1.4.1/docs/_static/switch.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/_static/uniter.svg` & `seqtools-1.4.1/docs/_static/uniter.svg`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/conf.py` & `seqtools-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/examples/dataloader.py` & `seqtools-1.4.1/docs/examples/dataloader.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/examples/dataloader.rst` & `seqtools-1.4.1/docs/examples/dataloader.rst`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/examples/errors_and_debugging.ipynb` & `seqtools-1.4.1/docs/examples/errors_and_debugging.ipynb`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/examples/preprocessing_pipeline.ipynb` & `seqtools-1.4.1/docs/examples/preprocessing_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/index.rst` & `seqtools-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/reference.rst` & `seqtools-1.4.1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/docs/tutorial.rst` & `seqtools-1.4.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/pyproject.toml` & `seqtools-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/C/refcountedbuffer.c` & `seqtools-1.4.1/seqtools/C/refcountedbuffer.c`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/__init__.py` & `seqtools-1.4.1/seqtools/__init__.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/buffering.py` & `seqtools-1.4.1/seqtools/buffering.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/errors.py` & `seqtools-1.4.1/seqtools/errors.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/evaluation.py` & `seqtools-1.4.1/seqtools/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         # set cleanup hooks
         weakref.finalize(
             self, ProcessBacked.cleanup, self.job_queue, self.workers, worker_monitor
         )
 
     @staticmethod
-    def cleanup(job_queue, workers: list[multiprocessing.Process], monitor):
+    def cleanup(job_queue, workers, monitor):
         for _ in workers:
             job_queue.put((-1, -1))
         for w in workers:
             if w.is_alive():
                 w.join(1)
                 if w.is_alive():
                     w.kill()
@@ -231,29 +231,32 @@
                 success = False
             else:
                 success = True
 
             # serialize it
             try:
                 if shm_slot_start is None:
-                    payload = pkl.dumps(value, protocol=-1)
+                    payload = pkl.dumps(value, protocol=pkl.HIGHEST_PROTOCOL)
                 else:
                     buffers_limits.clear()
                     shm_offset = shm_slot_start
                     shm_slot_stop = shm_slot_start + shm_slot_size
                     payload = pkl.dumps(
-                        value, protocol=-1, buffer_callback=buffer_callback
+                        value,
+                        protocol=pkl.HIGHEST_PROTOCOL,
+                        buffer_callback=buffer_callback,
                     )
 
             except Exception as e:  # gracefully recover failed serialization
                 if success:
                     success = False
-                    msg = "failed to send item {} to parent process, ".format(
-                        idx
-                    ) + "is it picklable? Error message was:\n{}".format(e)
+                    msg = (
+                        f"failed to send item {idx} to parent process, "
+                        + "is it picklable? Error message was:\n{e}"
+                    )
                     payload = pkl.dumps(ValueError(msg))
                 else:  # serialize error message because error can't be pickled
                     payload = pkl.dumps(str(value))
 
             # send it
             try:
                 result_pipe.send(
```

### Comparing `SeqTools-1.4.0/seqtools/indexing.py` & `seqtools-1.4.1/seqtools/indexing.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/instrument.py` & `seqtools-1.4.1/seqtools/instrument.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/mapping.py` & `seqtools-1.4.1/seqtools/mapping.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/serialization.py` & `seqtools-1.4.1/seqtools/serialization.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/shape.py` & `seqtools-1.4.1/seqtools/shape.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/seqtools/utils.py` & `seqtools-1.4.1/seqtools/utils.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_evaluation.py` & `seqtools-1.4.1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_indexing.py` & `seqtools-1.4.1/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_instrument.py` & `seqtools-1.4.1/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_mapping.py` & `seqtools-1.4.1/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_memory.py` & `seqtools-1.4.1/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_serialization.py` & `seqtools-1.4.1/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_shape.py` & `seqtools-1.4.1/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `SeqTools-1.4.0/tests/test_utils.py` & `seqtools-1.4.1/tests/test_utils.py`

 * *Files identical despite different names*

