# Comparing `tmp/RoffIO-1.0.2.tar.gz` & `tmp/RoffIO-1.0.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoffIO-1.0.2.tar", last modified: Mon Feb 12 11:13:01 2024, max compression
+gzip compressed data, was "RoffIO-1.0.3b1.tar", last modified: Fri Apr 12 11:11:13 2024, max compression
```

## Comparing `RoffIO-1.0.2.tar` & `RoffIO-1.0.3b1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.080930 RoffIO-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.068930 RoffIO-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.072930 RoffIO-1.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-12 11:12:50.000000 RoffIO-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.072930 RoffIO-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-12 11:12:50.000000 RoffIO-1.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-12 11:12:50.000000 RoffIO-1.0.2/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-12 11:12:50.000000 RoffIO-1.0.2/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-12 11:12:50.000000 RoffIO-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-12 11:12:50.000000 RoffIO-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-02-12 11:12:50.000000 RoffIO-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-12 11:12:50.000000 RoffIO-1.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-12 11:12:50.000000 RoffIO-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-02-12 11:13:01.080930 RoffIO-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-02-12 11:12:50.000000 RoffIO-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-12 11:12:50.000000 RoffIO-1.0.2/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-12 11:12:50.000000 RoffIO-1.0.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-12 11:13:01.080930 RoffIO-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-12 11:12:50.000000 RoffIO-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.068930 RoffIO-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.080930 RoffIO-1.0.2/src/RoffIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-02-12 11:13:01.000000 RoffIO-1.0.2/src/RoffIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-12 11:13:01.000000 RoffIO-1.0.2/src/RoffIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 11:13:01.000000 RoffIO-1.0.2/src/RoffIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-12 11:13:01.000000 RoffIO-1.0.2/src/RoffIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-12 11:13:01.000000 RoffIO-1.0.2/src/RoffIO.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.072930 RoffIO-1.0.2/src/_roffio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/endianess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/lazy_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/reading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.076930 RoffIO-1.0.2/src/_roffio/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/binary_roff_body_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/combinators.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/roff_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/text_roff_body_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/tokenizer/token_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/_roffio/writing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.076930 RoffIO-1.0.2/src/roffio/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/roffio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-12 11:12:50.000000 RoffIO-1.0.2/src/roffio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.076930 RoffIO-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 11:13:01.080930 RoffIO-1.0.2/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/generators/roff_file_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/generators/roff_tag_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_binary_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_endianess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_lazy_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_read_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_text_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_tokenizer_combinators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tests/test_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-12 11:12:50.000000 RoffIO-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.876332 RoffIO-1.0.3b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.880332 RoffIO-1.0.3b1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.880332 RoffIO-1.0.3b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.876332 RoffIO-1.0.3b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/src/RoffIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2024-04-12 11:11:13.000000 RoffIO-1.0.3b1/src/RoffIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-12 11:11:13.000000 RoffIO-1.0.3b1/src/RoffIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:11:13.000000 RoffIO-1.0.3b1/src/RoffIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 11:11:13.000000 RoffIO-1.0.3b1/src/RoffIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 11:11:13.000000 RoffIO-1.0.3b1/src/RoffIO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.880332 RoffIO-1.0.3b1/src/_roffio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/endianess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/lazy_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/reading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/src/_roffio/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/binary_roff_body_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/roff_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/text_roff_body_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/tokenizer/token_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11485 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/_roffio/writing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/src/roffio/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/roffio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/src/roffio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:13.884332 RoffIO-1.0.3b1/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/generators/roff_file_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/generators/roff_tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_binary_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_endianess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_lazy_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_text_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_tokenizer_combinators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tests/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 11:11:09.000000 RoffIO-1.0.3b1/tox.ini
```

### Comparing `RoffIO-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `RoffIO-1.0.3b1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/.github/workflows/testing.yml` & `RoffIO-1.0.3b1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/CODE_OF_CONDUCT.md` & `RoffIO-1.0.3b1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/CONTRIBUTING.md` & `RoffIO-1.0.3b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/LICENSE.md` & `RoffIO-1.0.3b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/PKG-INFO` & `RoffIO-1.0.3b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoffIO
-Version: 1.0.2
+Version: 1.0.3b1
 Summary: A (lazy) parser and writer for the Roxar Open File Format (ROFF).
 Home-page: https://github.com/equinor/roffio
 Author: Equinor
 Author-email: fg_sib-scout@equinor.com
 License: LGPL-3.0
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `RoffIO-1.0.2/README.md` & `RoffIO-1.0.3b1/README.md`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/SECURITY.md` & `RoffIO-1.0.3b1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/setup.py` & `RoffIO-1.0.3b1/setup.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/RoffIO.egg-info/PKG-INFO` & `RoffIO-1.0.3b1/src/RoffIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoffIO
-Version: 1.0.2
+Version: 1.0.3b1
 Summary: A (lazy) parser and writer for the Roxar Open File Format (ROFF).
 Home-page: https://github.com/equinor/roffio
 Author: Equinor
 Author-email: fg_sib-scout@equinor.com
 License: LGPL-3.0
 Platform: any
 Classifier: Development Status :: 1 - Planning
```

### Comparing `RoffIO-1.0.2/src/RoffIO.egg-info/SOURCES.txt` & `RoffIO-1.0.3b1/src/RoffIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/endianess_handler.py` & `RoffIO-1.0.3b1/src/_roffio/endianess_handler.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/lazy_tuple.py` & `RoffIO-1.0.3b1/src/_roffio/lazy_tuple.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/parser.py` & `RoffIO-1.0.3b1/src/_roffio/parser.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/reading.py` & `RoffIO-1.0.3b1/src/_roffio/reading.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/__init__.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/abstract_roff_body_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/binary_roff_body_tokenizer.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/binary_roff_body_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/combinators.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/combinators.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/common.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/common.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/roff_tokenizer.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/roff_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/text_roff_body_tokenizer.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/text_roff_body_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/token.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/token.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/tokenizer/token_kind.py` & `RoffIO-1.0.3b1/src/_roffio/tokenizer/token_kind.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/src/_roffio/writing.py` & `RoffIO-1.0.3b1/src/_roffio/writing.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/generators/roff_file_contents.py` & `RoffIO-1.0.3b1/tests/generators/roff_file_contents.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_binary_tokenizer.py` & `RoffIO-1.0.3b1/tests/test_binary_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_endianess_handler.py` & `RoffIO-1.0.3b1/tests/test_endianess_handler.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_parse.py` & `RoffIO-1.0.3b1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_read_write.py` & `RoffIO-1.0.3b1/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_text_tokenizer.py` & `RoffIO-1.0.3b1/tests/test_text_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_tokenizer.py` & `RoffIO-1.0.3b1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_tokenizer_combinators.py` & `RoffIO-1.0.3b1/tests/test_tokenizer_combinators.py`

 * *Files identical despite different names*

### Comparing `RoffIO-1.0.2/tests/test_write.py` & `RoffIO-1.0.3b1/tests/test_write.py`

 * *Files identical despite different names*

