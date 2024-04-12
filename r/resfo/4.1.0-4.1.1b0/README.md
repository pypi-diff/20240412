# Comparing `tmp/resfo-4.1.0.tar.gz` & `tmp/resfo-4.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resfo-4.1.0.tar", last modified: Tue Jan  9 07:58:29 2024, max compression
+gzip compressed data, was "resfo-4.1.1b0.tar", last modified: Fri Apr 12 10:39:05 2024, max compression
```

## Comparing `resfo-4.1.0.tar` & `resfo-4.1.1b0.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.368987 resfo-4.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.356987 resfo-4.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.360987 resfo-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-09 07:58:20.000000 resfo-4.1.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-09 07:58:20.000000 resfo-4.1.0/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-09 07:58:20.000000 resfo-4.1.0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-09 07:58:20.000000 resfo-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-09 07:58:20.000000 resfo-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-09 07:58:20.000000 resfo-4.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-01-09 07:58:20.000000 resfo-4.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-01-09 07:58:20.000000 resfo-4.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-01-09 07:58:20.000000 resfo-4.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-01-09 07:58:29.368987 resfo-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-01-09 07:58:20.000000 resfo-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-09 07:58:20.000000 resfo-4.1.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-09 07:58:20.000000 resfo-4.1.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.360987 resfo-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.360987 resfo-4.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/api_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/example_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-01-09 07:58:20.000000 resfo-4.1.0/docs/source/the_file_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-09 07:58:20.000000 resfo-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-01-09 07:58:29.368987 resfo-4.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.356987 resfo-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.364987 resfo-4.1.0/src/resfo/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.364987 resfo-4.1.0/src/resfo/_formatted/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_formatted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_formatted/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_formatted/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.364987 resfo-4.1.0/src/resfo/_unformatted/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_unformatted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_unformatted/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_unformatted/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/_unformatted/write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/array_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-01-09 07:58:20.000000 resfo-4.1.0/src/resfo/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.368987 resfo-4.1.0/src/resfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-01-09 07:58:29.000000 resfo-4.1.0/src/resfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-09 07:58:29.000000 resfo-4.1.0/src/resfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 07:58:29.000000 resfo-4.1.0/src/resfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-09 07:58:29.000000 resfo-4.1.0/src/resfo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-09 07:58:29.000000 resfo-4.1.0/src/resfo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:29.368987 resfo-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_formatted_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_formatted_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_formatted_read_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_formatted_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_read_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_type_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_unformatted_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_unformatted_read_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_unformatted_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-01-09 07:58:20.000000 resfo-4.1.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-01-09 07:58:20.000000 resfo-4.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.865104 resfo-4.1.1b0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.853104 resfo-4.1.1b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.857104 resfo-4.1.1b0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.857104 resfo-4.1.1b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 10:39:01.000000 resfo-4.1.1b0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-12 10:39:01.000000 resfo-4.1.1b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-12 10:39:01.000000 resfo-4.1.1b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-04-12 10:39:01.000000 resfo-4.1.1b0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-12 10:39:05.865104 resfo-4.1.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-12 10:39:01.000000 resfo-4.1.1b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-12 10:39:01.000000 resfo-4.1.1b0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 10:39:01.000000 resfo-4.1.1b0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.857104 resfo-4.1.1b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.857104 resfo-4.1.1b0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/api_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/example_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-04-12 10:39:01.000000 resfo-4.1.1b0/docs/source/the_file_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-12 10:39:01.000000 resfo-4.1.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 10:39:05.865104 resfo-4.1.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.853104 resfo-4.1.1b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.861104 resfo-4.1.1b0/src/resfo/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.861104 resfo-4.1.1b0/src/resfo/_formatted/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_formatted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_formatted/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_formatted/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.861104 resfo-4.1.1b0/src/resfo/_unformatted/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_unformatted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_unformatted/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_unformatted/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/_unformatted/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/array_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-12 10:39:01.000000 resfo-4.1.1b0/src/resfo/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.865104 resfo-4.1.1b0/src/resfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-12 10:39:05.000000 resfo-4.1.1b0/src/resfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-12 10:39:05.000000 resfo-4.1.1b0/src/resfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:39:05.000000 resfo-4.1.1b0/src/resfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 10:39:05.000000 resfo-4.1.1b0/src/resfo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 10:39:05.000000 resfo-4.1.1b0/src/resfo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:05.865104 resfo-4.1.1b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_formatted_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_formatted_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_formatted_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_formatted_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_type_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_unformatted_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_unformatted_read_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_unformatted_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 10:39:01.000000 resfo-4.1.1b0/tox.ini
```

### Comparing `resfo-4.1.0/.github/workflows/publish_to_pypi.yml` & `resfo-4.1.1b0/.github/workflows/publish_to_pypi.yml`

 * *Files 21% similar despite different names*

```diff
@@ -5,21 +5,22 @@
     tags:
       - '*'
 
 jobs:
   build-n-publish:
     name: Build and publish Python 🐍 distributions 📦 to PyPI
     runs-on: ubuntu-latest
+    permissions:
+      id-token: write
+    environment: release
     steps:
     - uses: actions/checkout@master
     - name: Set up Python 3.9
       uses: actions/setup-python@v3
       with:
         python-version: 3.9
     - name: Install pypa/build
       run: python -m pip install build
     - name: Build a binary wheel and a source tarball
       run: python -m build --sdist --wheel --outdir dist/ .
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.RESFO_PYPI_SECRET }}
```

### Comparing `resfo-4.1.0/.github/workflows/testing.yml` & `resfo-4.1.1b0/.github/workflows/testing.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   tests:
     name: "Python ${{ matrix.python-version }}"
     runs-on: "ubuntu-latest"
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `resfo-4.1.0/CODE_OF_CONDUCT.md` & `resfo-4.1.1b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/CONTRIBUTING.md` & `resfo-4.1.1b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/LICENSE.md` & `resfo-4.1.1b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/PKG-INFO` & `resfo-4.1.1b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: resfo
-Version: 4.1.0
+Version: 4.1.1b0
 Summary: A (lazy) parser and writer for reservoir simulator fortran output format.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/equinor/resfo
 Project-URL: Repository, https://github.com/equinor/resfo
 Project-URL: Documentation, https://resfo.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/equinor/resfo/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy<2
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Provides-Extra: dev
@@ -66,7 +68,25 @@
 >>> "COORD"
 >>> "ZCORN"
 >>> "ACTNUM"
 >>> "MAPAXES"
 ```
 
 For more information, see [the docs](http://resfo.rtfd.io).
+
+
+How to contribute
+=================
+
+The easiest way to set up a nice development environment for resfo is to use tox (can be installed via `pip install tox` or
+`sudo apt install tox` on ubuntu), then all testing and linting can be ran with
+
+```bash
+tox
+```
+
+You can also set up `pre-commit` to ensure style checks are done as you commit:
+
+```bash
+pip install pre-commit
+pre-commit install
+```
```

### Comparing `resfo-4.1.0/README.md` & `resfo-4.1.1b0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -37,7 +37,25 @@
 >>> "COORD"
 >>> "ZCORN"
 >>> "ACTNUM"
 >>> "MAPAXES"
 ```
 
 For more information, see [the docs](http://resfo.rtfd.io).
+
+
+How to contribute
+=================
+
+The easiest way to set up a nice development environment for resfo is to use tox (can be installed via `pip install tox` or
+`sudo apt install tox` on ubuntu), then all testing and linting can be ran with
+
+```bash
+tox
+```
+
+You can also set up `pre-commit` to ensure style checks are done as you commit:
+
+```bash
+pip install pre-commit
+pre-commit install
+```
```

### Comparing `resfo-4.1.0/SECURITY.md` & `resfo-4.1.1b0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/docs/source/developer_guide.rst` & `resfo-4.1.1b0/docs/source/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/docs/source/error_handling.rst` & `resfo-4.1.1b0/docs/source/error_handling.rst`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/docs/source/example_usage.rst` & `resfo-4.1.1b0/docs/source/example_usage.rst`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/docs/source/index.rst` & `resfo-4.1.1b0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/docs/source/the_file_format.rst` & `resfo-4.1.1b0/docs/source/the_file_format.rst`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/pyproject.toml` & `resfo-4.1.1b0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 classifiers=[
     "Development Status :: 1 - Planning",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = ["numpy<2"]
 dynamic=["version"]
 
 authors = [
     {name="Equinor", email="fg_sib-scout@equinor.com"},
 ]
```

### Comparing `resfo-4.1.0/src/resfo/_formatted/read.py` & `resfo-4.1.1b0/src/resfo/_formatted/read.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/_formatted/write.py` & `resfo-4.1.1b0/src/resfo/_formatted/write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/_unformatted/common.py` & `resfo-4.1.1b0/src/resfo/_unformatted/common.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/_unformatted/read.py` & `resfo-4.1.1b0/src/resfo/_unformatted/read.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/_unformatted/write.py` & `resfo-4.1.1b0/src/resfo/_unformatted/write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/array_entry.py` & `resfo-4.1.1b0/src/resfo/array_entry.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/format.py` & `resfo-4.1.1b0/src/resfo/format.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/read.py` & `resfo-4.1.1b0/src/resfo/read.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/types.py` & `resfo-4.1.1b0/src/resfo/types.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo/write.py` & `resfo-4.1.1b0/src/resfo/write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/src/resfo.egg-info/PKG-INFO` & `resfo-4.1.1b0/src/resfo.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: resfo
-Version: 4.1.0
+Version: 4.1.1b0
 Summary: A (lazy) parser and writer for reservoir simulator fortran output format.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/equinor/resfo
 Project-URL: Repository, https://github.com/equinor/resfo
 Project-URL: Documentation, https://resfo.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/equinor/resfo/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: numpy<2
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx-rtd-theme; extra == "doc"
 Provides-Extra: dev
@@ -66,7 +68,25 @@
 >>> "COORD"
 >>> "ZCORN"
 >>> "ACTNUM"
 >>> "MAPAXES"
 ```
 
 For more information, see [the docs](http://resfo.rtfd.io).
+
+
+How to contribute
+=================
+
+The easiest way to set up a nice development environment for resfo is to use tox (can be installed via `pip install tox` or
+`sudo apt install tox` on ubuntu), then all testing and linting can be ran with
+
+```bash
+tox
+```
+
+You can also set up `pre-commit` to ensure style checks are done as you commit:
+
+```bash
+pip install pre-commit
+pre-commit install
+```
```

### Comparing `resfo-4.1.0/src/resfo.egg-info/SOURCES.txt` & `resfo-4.1.1b0/src/resfo.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 LICENSE.md
 README.md
 SECURITY.md
 conftest.py
 pyproject.toml
 setup.cfg
 tox.ini
+.github/ISSUE_TEMPLATE/bug_report.md
 .github/workflows/lint.yml
 .github/workflows/publish_to_pypi.yml
 .github/workflows/testing.yml
 docs/requirements.txt
 docs/source/api_doc.rst
 docs/source/conf.py
 docs/source/developer_guide.rst
@@ -38,14 +39,15 @@
 src/resfo/_formatted/read.py
 src/resfo/_formatted/write.py
 src/resfo/_unformatted/__init__.py
 src/resfo/_unformatted/common.py
 src/resfo/_unformatted/read.py
 src/resfo/_unformatted/write.py
 tests/__init__.py
+tests/conftest.py
 tests/generators.py
 tests/test_error_handling.py
 tests/test_formatted_common.py
 tests/test_formatted_read.py
 tests/test_formatted_read_write.py
 tests/test_formatted_write.py
 tests/test_read_write.py
```

### Comparing `resfo-4.1.0/tests/generators.py` & `resfo-4.1.1b0/tests/generators.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_error_handling.py` & `resfo-4.1.1b0/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_formatted_common.py` & `resfo-4.1.1b0/tests/test_formatted_common.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_formatted_read.py` & `resfo-4.1.1b0/tests/test_formatted_read.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_formatted_read_write.py` & `resfo-4.1.1b0/tests/test_formatted_read_write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_formatted_write.py` & `resfo-4.1.1b0/tests/test_formatted_write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_read_write.py` & `resfo-4.1.1b0/tests/test_read_write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_type_resolution.py` & `resfo-4.1.1b0/tests/test_type_resolution.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_types.py` & `resfo-4.1.1b0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_unformatted_read.py` & `resfo-4.1.1b0/tests/test_unformatted_read.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_unformatted_read_write.py` & `resfo-4.1.1b0/tests/test_unformatted_read_write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_unformatted_write.py` & `resfo-4.1.1b0/tests/test_unformatted_write.py`

 * *Files identical despite different names*

### Comparing `resfo-4.1.0/tests/test_update.py` & `resfo-4.1.1b0/tests/test_update.py`

 * *Files identical despite different names*

