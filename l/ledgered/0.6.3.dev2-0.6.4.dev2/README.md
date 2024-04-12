# Comparing `tmp/ledgered-0.6.3.dev2.tar.gz` & `tmp/ledgered-0.6.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgered-0.6.3.dev2.tar", last modified: Tue Mar 26 17:41:53 2024, max compression
+gzip compressed data, was "ledgered-0.6.4.dev2.tar", last modified: Fri Apr 12 15:06:45 2024, max compression
```

## Comparing `ledgered-0.6.3.dev2.tar` & `ledgered-0.6.4.dev2.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.727203 ledgered-0.6.3.dev2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.715203 ledgered-0.6.3.dev2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.719203 ledgered-0.6.3.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/.github/workflows/build_and_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/.github/workflows/fast-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-26 17:41:53.727203 ledgered-0.6.3.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.719203 ledgered-0.6.3.dev2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/doc/binary.md
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/doc/manifest.md
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 17:41:53.727203 ledgered-0.6.3.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.715203 ledgered-0.6.3.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.719203 ledgered-0.6.3.dev2/src/ledgered/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/binary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/src/ledgered/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/manifest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/src/ledgered/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/src/ledgered/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/src/ledgered.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-26 17:41:53.000000 ledgered-0.6.3.dev2/src/ledgered.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.719203 ledgered-0.6.3.dev2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/tests/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/_data/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/_data/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/_data/full_correct.toml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/_data/ledger_app.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/_data/minimal.toml
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/_data/one_leaf.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/tests/functional/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/functional/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/functional/manifest/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:53.723203 ledgered-0.6.3.dev2/tests/unit/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/manifest/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/manifest/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/manifest/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/manifest/test_use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-26 17:41:42.000000 ledgered-0.6.3.dev2/tests/unit/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.710891 ledgered-0.6.4.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.698891 ledgered-0.6.4.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.702891 ledgered-0.6.4.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/.github/workflows/build_and_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/.github/workflows/fast-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-12 15:06:45.710891 ledgered-0.6.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.702891 ledgered-0.6.4.dev2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/doc/binary.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/doc/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:06:45.710891 ledgered-0.6.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.698891 ledgered-0.6.4.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.702891 ledgered-0.6.4.dev2/src/ledgered/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.706891 ledgered-0.6.4.dev2/src/ledgered/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/manifest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.706891 ledgered-0.6.4.dev2/src/ledgered/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/src/ledgered/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.710891 ledgered-0.6.4.dev2/src/ledgered.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 15:06:45.000000 ledgered-0.6.4.dev2/src/ledgered.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.698891 ledgered-0.6.4.dev2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.706891 ledgered-0.6.4.dev2/tests/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/_data/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/_data/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/_data/full_correct.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/_data/ledger_app.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/_data/minimal.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/_data/one_leaf.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.706891 ledgered-0.6.4.dev2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.706891 ledgered-0.6.4.dev2/tests/functional/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/functional/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/functional/manifest/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/functional/test_github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.706891 ledgered-0.6.4.dev2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:45.710891 ledgered-0.6.4.dev2/tests/unit/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/manifest/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/manifest/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/manifest/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/manifest/test_use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-12 15:06:36.000000 ledgered-0.6.4.dev2/tests/unit/test_serializers.py
```

### Comparing `ledgered-0.6.3.dev2/.github/workflows/build_and_tests.yml` & `ledgered-0.6.4.dev2/.github/workflows/build_and_tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,20 @@
       run: |
         pip install -U pip
         pip install -U .[dev]
 
     - name: Run tests and generate coverage
       run: pytest -v --tb=short tests/ --cov ledgered --cov-report xml
 
+    - name: Run unit tests and generate coverage
+      run: pytest -v --tb=short tests/unit --cov ledgered --cov-report xml
+
+    - name: Run functional tests and generate coverage
+      run: pytest -v --tb=short tests/functional --cov ledgered --cov-report xml --cov-append --token "${{ secrets.GITHUB_TOKEN }}"
+
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v4
       with:
         name: codecov-ledgered
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `ledgered-0.6.3.dev2/.github/workflows/codeql-analysis.yml` & `ledgered-0.6.4.dev2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/.github/workflows/fast-checks.yml` & `ledgered-0.6.4.dev2/.github/workflows/fast-checks.yml`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/CHANGELOG.md` & `ledgered-0.6.4.dev2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.7.0] - 2024-04-12
+
+### Added
+
+- Added wrapper around GitHub API to ease manipulating Ledger application repositories
+
+
 ## [0.6.3] - 2024-03-26
 
 ### Fixed
 
 - ledger-binary: NanoS SDK has a unique `target_version` section.
```

### Comparing `ledgered-0.6.3.dev2/LICENSE` & `ledgered-0.6.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/PKG-INFO` & `ledgered-0.6.4.dev2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgered
-Version: 0.6.3.dev2
+Version: 0.6.4.dev2
 Summary: Python tools, utils, libraries, to be used with Ledger cryptodevices
 Author-email: Ledger <hello@ledger.fr>
 License: MIT License
         
         Copyright (c) 2023 Ledger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pyelftools
+Requires-Dist: pygithub
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
 # Ledgered
 
 [![codecov](https://codecov.io/gh/LedgerHQ/ledgered/graph/badge.svg?token=0mwgQwrusz)](https://codecov.io/gh/LedgerHQ/ledgered)
```

### Comparing `ledgered-0.6.3.dev2/README.md` & `ledgered-0.6.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/doc/binary.md` & `ledgered-0.6.4.dev2/doc/binary.md`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/doc/manifest.md` & `ledgered-0.6.4.dev2/doc/manifest.md`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/pyproject.toml` & `ledgered-0.6.4.dev2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "Operating System :: MacOS :: MacOS X",
 ]
 dynamic = [ "version" ]
 requires-python = ">=3.7"
 dependencies = [
     "toml",
     "pyelftools",
+    "pygithub",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov"
 ]
```

### Comparing `ledgered-0.6.3.dev2/src/ledgered/binary.py` & `ledgered-0.6.4.dev2/src/ledgered/binary.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered/manifest/app.py` & `ledgered-0.6.4.dev2/src/ledgered/manifest/app.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered/manifest/cli.py` & `ledgered-0.6.4.dev2/src/ledgered/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered/manifest/manifest.py` & `ledgered-0.6.4.dev2/src/ledgered/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered/manifest/tests.py` & `ledgered-0.6.4.dev2/src/ledgered/manifest/tests.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered/manifest/use_cases.py` & `ledgered-0.6.4.dev2/src/ledgered/manifest/use_cases.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered/serializers.py` & `ledgered-0.6.4.dev2/src/ledgered/serializers.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/src/ledgered.egg-info/PKG-INFO` & `ledgered-0.6.4.dev2/src/ledgered.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledgered
-Version: 0.6.3.dev2
+Version: 0.6.4.dev2
 Summary: Python tools, utils, libraries, to be used with Ledger cryptodevices
 Author-email: Ledger <hello@ledger.fr>
 License: MIT License
         
         Copyright (c) 2023 Ledger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: toml
 Requires-Dist: pyelftools
+Requires-Dist: pygithub
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 
 # Ledgered
 
 [![codecov](https://codecov.io/gh/LedgerHQ/ledgered/graph/badge.svg?token=0mwgQwrusz)](https://codecov.io/gh/LedgerHQ/ledgered)
```

### Comparing `ledgered-0.6.3.dev2/src/ledgered.egg-info/SOURCES.txt` & `ledgered-0.6.4.dev2/src/ledgered.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 .github/workflows/codeql-analysis.yml
 .github/workflows/fast-checks.yml
 doc/binary.md
 doc/manifest.md
 src/ledgered/__init__.py
 src/ledgered/__version__.py
 src/ledgered/binary.py
+src/ledgered/github.py
 src/ledgered/serializers.py
 src/ledgered.egg-info/PKG-INFO
 src/ledgered.egg-info/SOURCES.txt
 src/ledgered.egg-info/dependency_links.txt
 src/ledgered.egg-info/entry_points.txt
 src/ledgered.egg-info/requires.txt
 src/ledgered.egg-info/top_level.txt
@@ -31,17 +32,20 @@
 tests/_data/Cargo.toml
 tests/_data/Makefile
 tests/_data/full_correct.toml
 tests/_data/ledger_app.toml
 tests/_data/minimal.toml
 tests/_data/one_leaf.toml
 tests/functional/__init__.py
+tests/functional/conftest.py
+tests/functional/test_github.py
 tests/functional/manifest/__init__.py
 tests/functional/manifest/test_cli.py
 tests/unit/__init__.py
 tests/unit/test_binary.py
+tests/unit/test_github.py
 tests/unit/test_serializers.py
 tests/unit/manifest/__init__.py
 tests/unit/manifest/test_app.py
 tests/unit/manifest/test_manifest.py
 tests/unit/manifest/test_tests.py
 tests/unit/manifest/test_use_cases.py
```

### Comparing `ledgered-0.6.3.dev2/tests/functional/manifest/test_cli.py` & `ledgered-0.6.4.dev2/tests/functional/manifest/test_cli.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/tests/unit/manifest/test_app.py` & `ledgered-0.6.4.dev2/tests/unit/manifest/test_app.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/tests/unit/manifest/test_manifest.py` & `ledgered-0.6.4.dev2/tests/unit/manifest/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/tests/unit/manifest/test_tests.py` & `ledgered-0.6.4.dev2/tests/unit/manifest/test_tests.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/tests/unit/manifest/test_use_cases.py` & `ledgered-0.6.4.dev2/tests/unit/manifest/test_use_cases.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/tests/unit/test_binary.py` & `ledgered-0.6.4.dev2/tests/unit/test_binary.py`

 * *Files identical despite different names*

### Comparing `ledgered-0.6.3.dev2/tests/unit/test_serializers.py` & `ledgered-0.6.4.dev2/tests/unit/test_serializers.py`

 * *Files identical despite different names*

