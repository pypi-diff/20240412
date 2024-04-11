# Comparing `tmp/holdup-5.0.0.tar.gz` & `tmp/holdup-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holdup-5.0.0.tar", last modified: Wed Apr 10 23:28:25 2024, max compression
+gzip compressed data, was "holdup-5.1.0.tar", last modified: Thu Apr 11 23:39:06 2024, max compression
```

## Comparing `holdup-5.0.0.tar` & `holdup-5.1.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.439959 holdup-5.0.0/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      735 2024-04-10 23:18:07.000000 holdup-5.0.0/.bumpversion.cfg
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1607 2024-04-10 23:18:07.000000 holdup-5.0.0/.cookiecutterrc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      174 2024-04-10 18:20:04.000000 holdup-5.0.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2019-05-22 22:01:47.000000 holdup-5.0.0/.dockerignore
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-10 18:20:04.000000 holdup-5.0.0/.editorconfig
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.432959 holdup-5.0.0/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.434959 holdup-5.0.0/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)    10795 2024-04-10 18:24:54.000000 holdup-5.0.0/.github/workflows/github-actions.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-04-10 18:27:49.000000 holdup-5.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      282 2024-04-10 18:20:04.000000 holdup-5.0.0/.readthedocs.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      162 2024-04-10 18:24:46.000000 holdup-5.0.0/AUTHORS.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2856 2024-04-10 23:17:47.000000 holdup-5.0.0/CHANGELOG.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2341 2024-04-10 18:20:04.000000 holdup-5.0.0/CONTRIBUTING.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)      482 2024-04-10 23:12:41.000000 holdup-5.0.0/Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2024-04-10 18:24:46.000000 holdup-5.0.0/LICENSE
--rw-r--r--   0 ionel     (1000) ionel     (1000)      468 2024-04-10 18:24:46.000000 holdup-5.0.0/MANIFEST.in
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7628 2024-04-10 23:28:25.439959 holdup-5.0.0/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     4834 2024-04-10 23:18:07.000000 holdup-5.0.0/README.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.434959 holdup-5.0.0/ci/
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-10 18:20:04.000000 holdup-5.0.0/ci/bootstrap.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-10 18:20:04.000000 holdup-5.0.0/ci/requirements.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.432959 holdup-5.0.0/ci/templates/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.432959 holdup-5.0.0/ci/templates/.github/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.435959 holdup-5.0.0/ci/templates/.github/workflows/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     2166 2024-04-10 18:20:04.000000 holdup-5.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.436959 holdup-5.0.0/docs/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/authors.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/changelog.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1030 2024-04-10 23:18:07.000000 holdup-5.0.0/docs/conf.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/contributing.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      244 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       86 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/installation.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/readme.rst
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.436959 holdup-5.0.0/docs/reference/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      154 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/reference/holdup.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       58 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/reference/index.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       17 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/requirements.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2024-04-10 18:20:04.000000 holdup-5.0.0/docs/spelling_wordlist.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       64 2024-04-10 18:24:46.000000 holdup-5.0.0/docs/usage.rst
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-04-10 18:20:04.000000 holdup-5.0.0/pyproject.toml
--rw-r--r--   0 ionel     (1000) ionel     (1000)      825 2024-04-10 18:24:46.000000 holdup-5.0.0/pytest.ini
--rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-04-10 23:28:25.439959 holdup-5.0.0/setup.cfg
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2907 2024-04-10 23:18:07.000000 holdup-5.0.0/setup.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.432959 holdup-5.0.0/src/
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.437959 holdup-5.0.0/src/holdup/
--rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-04-10 23:18:07.000000 holdup-5.0.0/src/holdup/__init__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      382 2024-04-10 18:25:33.000000 holdup-5.0.0/src/holdup/__main__.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)    15184 2024-04-10 18:28:38.000000 holdup-5.0.0/src/holdup/cli.py
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.438959 holdup-5.0.0/src/holdup.egg-info/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     7628 2024-04-10 23:28:25.000000 holdup-5.0.0/src/holdup.egg-info/PKG-INFO
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1021 2024-04-10 23:28:25.000000 holdup-5.0.0/src/holdup.egg-info/SOURCES.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-10 23:28:25.000000 holdup-5.0.0/src/holdup.egg-info/dependency_links.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)       43 2024-04-10 23:28:25.000000 holdup-5.0.0/src/holdup.egg-info/entry_points.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-10 23:28:03.000000 holdup-5.0.0/src/holdup.egg-info/not-zip-safe
--rw-r--r--   0 ionel     (1000) ionel     (1000)       14 2024-04-10 23:28:25.000000 holdup-5.0.0/src/holdup.egg-info/requires.txt
--rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2024-04-10 23:28:25.000000 holdup-5.0.0/src/holdup.egg-info/top_level.txt
-drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-10 23:28:25.438959 holdup-5.0.0/tests/
--rw-r--r--   0 ionel     (1000) ionel     (1000)     3024 2022-03-20 15:20:45.000000 holdup-5.0.0/tests/Dockerfile
--rw-r--r--   0 ionel     (1000) ionel     (1000)      233 2023-02-13 20:53:55.000000 holdup-5.0.0/tests/conftest.py
--rw-r--r--   0 ionel     (1000) ionel     (1000)      299 2024-04-10 23:15:17.000000 holdup-5.0.0/tests/docker-compose.yml
--rw-r--r--   0 ionel     (1000) ionel     (1000)    10435 2024-04-10 23:15:17.000000 holdup-5.0.0/tests/test_holdup.py
--rwxrwxr-x   0 ionel     (1000) ionel     (1000)      650 2019-05-26 20:51:27.000000 holdup-5.0.0/tests/test_pg.py
--rwxr-xr-x   0 ionel     (1000) ionel     (1000)      520 2024-04-10 19:37:57.000000 holdup-5.0.0/tests/test_pg.sh
--rw-r--r--   0 ionel     (1000) ionel     (1000)     1822 2024-04-10 23:15:17.000000 holdup-5.0.0/tox.ini
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.864210 holdup-5.1.0/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      735 2024-04-11 23:38:56.000000 holdup-5.1.0/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1606 2024-04-11 23:38:56.000000 holdup-5.1.0/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      174 2024-04-11 23:28:23.000000 holdup-5.1.0/.coveragerc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2019-05-22 22:01:47.000000 holdup-5.1.0/.dockerignore
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-11 23:28:23.000000 holdup-5.1.0/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.858210 holdup-5.1.0/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.861210 holdup-5.1.0/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7585 2024-04-11 23:28:43.000000 holdup-5.1.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-04-11 23:28:43.000000 holdup-5.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      282 2024-04-11 23:28:23.000000 holdup-5.1.0/.readthedocs.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      162 2024-04-11 23:28:43.000000 holdup-5.1.0/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3114 2024-04-11 23:28:43.000000 holdup-5.1.0/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2341 2024-04-11 23:28:23.000000 holdup-5.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      482 2024-04-10 23:12:41.000000 holdup-5.1.0/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1330 2024-04-11 23:28:43.000000 holdup-5.1.0/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      519 2024-04-11 23:28:43.000000 holdup-5.1.0/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7886 2024-04-11 23:39:06.864210 holdup-5.1.0/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     4834 2024-04-11 23:38:56.000000 holdup-5.1.0/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.861210 holdup-5.1.0/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-11 23:28:23.000000 holdup-5.1.0/ci/bootstrap.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-11 23:28:23.000000 holdup-5.1.0/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.858210 holdup-5.1.0/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.858210 holdup-5.1.0/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.861210 holdup-5.1.0/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2142 2024-04-11 23:28:23.000000 holdup-5.1.0/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.862210 holdup-5.1.0/docs/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       28 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/authors.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       30 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/changelog.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      967 2024-04-11 23:38:56.000000 holdup-5.1.0/docs/conf.py
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       33 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/contributing.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      219 2024-04-11 23:28:43.000000 holdup-5.1.0/docs/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2024-04-11 23:28:24.000000 holdup-5.1.0/docs/readme.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.862210 holdup-5.1.0/docs/reference/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      196 2024-04-11 23:28:43.000000 holdup-5.1.0/docs/reference/index.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       17 2024-04-11 23:28:23.000000 holdup-5.1.0/docs/requirements.txt
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      109 2024-04-11 23:28:23.000000 holdup-5.1.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      684 2024-04-10 23:05:47.000000 holdup-5.1.0/holdup.spec
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      526 2024-04-10 23:13:07.000000 holdup-5.1.0/pyinstaller.Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-04-11 23:28:23.000000 holdup-5.1.0/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      825 2024-04-11 23:28:43.000000 holdup-5.1.0/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-04-11 23:39:06.864210 holdup-5.1.0/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2907 2024-04-11 23:38:56.000000 holdup-5.1.0/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.859210 holdup-5.1.0/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.862210 holdup-5.1.0/src/holdup/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-04-11 23:38:56.000000 holdup-5.1.0/src/holdup/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      382 2024-04-11 23:28:43.000000 holdup-5.1.0/src/holdup/__main__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     8071 2024-04-11 23:25:03.000000 holdup-5.1.0/src/holdup/checks.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7329 2024-04-11 23:28:43.000000 holdup-5.1.0/src/holdup/cli.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      447 2024-04-11 23:13:41.000000 holdup-5.1.0/src/holdup/pg.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.864210 holdup-5.1.0/src/holdup.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     7886 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1031 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       43 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       14 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/requires.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        7 2024-04-11 23:39:06.000000 holdup-5.1.0/src/holdup.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:39:06.864210 holdup-5.1.0/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3024 2022-03-20 15:20:45.000000 holdup-5.1.0/tests/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      233 2023-02-13 20:53:55.000000 holdup-5.1.0/tests/conftest.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      299 2024-04-10 23:15:17.000000 holdup-5.1.0/tests/docker-compose.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)    10663 2024-04-11 23:01:11.000000 holdup-5.1.0/tests/test_holdup.py
+-rwxrwxr-x   0 ionel     (1000) ionel     (1000)      650 2019-05-26 20:51:27.000000 holdup-5.1.0/tests/test_pg.py
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)      520 2024-04-10 19:37:57.000000 holdup-5.1.0/tests/test_pg.sh
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1830 2024-04-11 23:28:43.000000 holdup-5.1.0/tox.ini
```

### Comparing `holdup-5.0.0/.bumpversion.cfg` & `holdup-5.1.0/.bumpversion.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 5.0.0
+current_version = 5.1.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `holdup-5.0.0/.cookiecutterrc` & `holdup-5.1.0/.cookiecutterrc`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     distribution_name: holdup
     email: contact@ionelmc.ro
     formatter_quote_style: double
     full_name: Ionel Cristian Mărieș
     function_name: compute
     github_actions: 'yes'
     github_actions_osx: 'yes'
-    github_actions_windows: 'yes'
+    github_actions_windows: 'no'
     license: BSD 2-Clause License
     module_name: core
     package_name: holdup
     pre_commit: 'yes'
     project_name: Holdup
     project_short_description: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
     pypi_badge: 'yes'
@@ -36,12 +36,12 @@
     setup_py_uses_setuptools_scm: 'no'
     sphinx_docs: 'yes'
     sphinx_docs_hosting: https://python-holdup.readthedocs.io/
     sphinx_doctest: 'no'
     sphinx_theme: furo
     test_matrix_separate_coverage: 'no'
     tests_inside_package: 'no'
-    version: 5.0.0
+    version: 5.1.0
     version_manager: bump2version
     website: https://blog.ionelmc.ro
     year_from: '2016'
     year_to: '2024'
```

### Comparing `holdup-5.0.0/.github/workflows/github-actions.yml` & `holdup-5.1.0/.github/workflows/github-actions.yml`

 * *Files 16% similar despite different names*

```diff
@@ -21,290 +21,194 @@
             os: 'ubuntu-latest'
           - name: 'py38-pg2 (ubuntu)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38-pg2'
             os: 'ubuntu-latest'
-          - name: 'py38-pg2 (windows)'
-            python: '3.8'
-            toxpython: 'python3.8'
-            python_arch: 'x64'
-            tox_env: 'py38-pg2'
-            os: 'windows-latest'
           - name: 'py38-pg2 (macos)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38-pg2'
             os: 'macos-latest'
           - name: 'py38-pg3 (ubuntu)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38-pg3'
             os: 'ubuntu-latest'
-          - name: 'py38-pg3 (windows)'
-            python: '3.8'
-            toxpython: 'python3.8'
-            python_arch: 'x64'
-            tox_env: 'py38-pg3'
-            os: 'windows-latest'
           - name: 'py38-pg3 (macos)'
             python: '3.8'
             toxpython: 'python3.8'
             python_arch: 'x64'
             tox_env: 'py38-pg3'
             os: 'macos-latest'
           - name: 'py39-pg2 (ubuntu)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39-pg2'
             os: 'ubuntu-latest'
-          - name: 'py39-pg2 (windows)'
-            python: '3.9'
-            toxpython: 'python3.9'
-            python_arch: 'x64'
-            tox_env: 'py39-pg2'
-            os: 'windows-latest'
           - name: 'py39-pg2 (macos)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39-pg2'
             os: 'macos-latest'
           - name: 'py39-pg3 (ubuntu)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39-pg3'
             os: 'ubuntu-latest'
-          - name: 'py39-pg3 (windows)'
-            python: '3.9'
-            toxpython: 'python3.9'
-            python_arch: 'x64'
-            tox_env: 'py39-pg3'
-            os: 'windows-latest'
           - name: 'py39-pg3 (macos)'
             python: '3.9'
             toxpython: 'python3.9'
             python_arch: 'x64'
             tox_env: 'py39-pg3'
             os: 'macos-latest'
           - name: 'py310-pg2 (ubuntu)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-pg2'
             os: 'ubuntu-latest'
-          - name: 'py310-pg2 (windows)'
-            python: '3.10'
-            toxpython: 'python3.10'
-            python_arch: 'x64'
-            tox_env: 'py310-pg2'
-            os: 'windows-latest'
           - name: 'py310-pg2 (macos)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-pg2'
             os: 'macos-latest'
           - name: 'py310-pg3 (ubuntu)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-pg3'
             os: 'ubuntu-latest'
-          - name: 'py310-pg3 (windows)'
-            python: '3.10'
-            toxpython: 'python3.10'
-            python_arch: 'x64'
-            tox_env: 'py310-pg3'
-            os: 'windows-latest'
           - name: 'py310-pg3 (macos)'
             python: '3.10'
             toxpython: 'python3.10'
             python_arch: 'x64'
             tox_env: 'py310-pg3'
             os: 'macos-latest'
           - name: 'py311-pg2 (ubuntu)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-pg2'
             os: 'ubuntu-latest'
-          - name: 'py311-pg2 (windows)'
-            python: '3.11'
-            toxpython: 'python3.11'
-            python_arch: 'x64'
-            tox_env: 'py311-pg2'
-            os: 'windows-latest'
           - name: 'py311-pg2 (macos)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-pg2'
             os: 'macos-latest'
           - name: 'py311-pg3 (ubuntu)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-pg3'
             os: 'ubuntu-latest'
-          - name: 'py311-pg3 (windows)'
-            python: '3.11'
-            toxpython: 'python3.11'
-            python_arch: 'x64'
-            tox_env: 'py311-pg3'
-            os: 'windows-latest'
           - name: 'py311-pg3 (macos)'
             python: '3.11'
             toxpython: 'python3.11'
             python_arch: 'x64'
             tox_env: 'py311-pg3'
             os: 'macos-latest'
           - name: 'py312-pg2 (ubuntu)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312-pg2'
             os: 'ubuntu-latest'
-          - name: 'py312-pg2 (windows)'
-            python: '3.12'
-            toxpython: 'python3.12'
-            python_arch: 'x64'
-            tox_env: 'py312-pg2'
-            os: 'windows-latest'
           - name: 'py312-pg2 (macos)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312-pg2'
             os: 'macos-latest'
           - name: 'py312-pg3 (ubuntu)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312-pg3'
             os: 'ubuntu-latest'
-          - name: 'py312-pg3 (windows)'
-            python: '3.12'
-            toxpython: 'python3.12'
-            python_arch: 'x64'
-            tox_env: 'py312-pg3'
-            os: 'windows-latest'
           - name: 'py312-pg3 (macos)'
             python: '3.12'
             toxpython: 'python3.12'
             python_arch: 'x64'
             tox_env: 'py312-pg3'
             os: 'macos-latest'
           - name: 'pypy38-pg2 (ubuntu)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38-pg2'
             os: 'ubuntu-latest'
-          - name: 'pypy38-pg2 (windows)'
-            python: 'pypy-3.8'
-            toxpython: 'pypy3.8'
-            python_arch: 'x64'
-            tox_env: 'pypy38-pg2'
-            os: 'windows-latest'
           - name: 'pypy38-pg2 (macos)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38-pg2'
             os: 'macos-latest'
           - name: 'pypy38-pg3 (ubuntu)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38-pg3'
             os: 'ubuntu-latest'
-          - name: 'pypy38-pg3 (windows)'
-            python: 'pypy-3.8'
-            toxpython: 'pypy3.8'
-            python_arch: 'x64'
-            tox_env: 'pypy38-pg3'
-            os: 'windows-latest'
           - name: 'pypy38-pg3 (macos)'
             python: 'pypy-3.8'
             toxpython: 'pypy3.8'
             python_arch: 'x64'
             tox_env: 'pypy38-pg3'
             os: 'macos-latest'
           - name: 'pypy39-pg2 (ubuntu)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39-pg2'
             os: 'ubuntu-latest'
-          - name: 'pypy39-pg2 (windows)'
-            python: 'pypy-3.9'
-            toxpython: 'pypy3.9'
-            python_arch: 'x64'
-            tox_env: 'pypy39-pg2'
-            os: 'windows-latest'
           - name: 'pypy39-pg2 (macos)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39-pg2'
             os: 'macos-latest'
           - name: 'pypy39-pg3 (ubuntu)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39-pg3'
             os: 'ubuntu-latest'
-          - name: 'pypy39-pg3 (windows)'
-            python: 'pypy-3.9'
-            toxpython: 'pypy3.9'
-            python_arch: 'x64'
-            tox_env: 'pypy39-pg3'
-            os: 'windows-latest'
           - name: 'pypy39-pg3 (macos)'
             python: 'pypy-3.9'
             toxpython: 'pypy3.9'
             python_arch: 'x64'
             tox_env: 'pypy39-pg3'
             os: 'macos-latest'
           - name: 'pypy310-pg2 (ubuntu)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310-pg2'
             os: 'ubuntu-latest'
-          - name: 'pypy310-pg2 (windows)'
-            python: 'pypy-3.10'
-            toxpython: 'pypy3.10'
-            python_arch: 'x64'
-            tox_env: 'pypy310-pg2'
-            os: 'windows-latest'
           - name: 'pypy310-pg2 (macos)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310-pg2'
             os: 'macos-latest'
           - name: 'pypy310-pg3 (ubuntu)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310-pg3'
             os: 'ubuntu-latest'
-          - name: 'pypy310-pg3 (windows)'
-            python: 'pypy-3.10'
-            toxpython: 'pypy3.10'
-            python_arch: 'x64'
-            tox_env: 'pypy310-pg3'
-            os: 'windows-latest'
           - name: 'pypy310-pg3 (macos)'
             python: 'pypy-3.10'
             toxpython: 'pypy3.10'
             python_arch: 'x64'
             tox_env: 'pypy310-pg3'
             os: 'macos-latest'
     steps:
```

### Comparing `holdup-5.0.0/.pre-commit-config.yaml` & `holdup-5.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/CHANGELOG.rst` & `holdup-5.1.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 
 Changelog
 =========
 
+5.1.0 (2024-04-12)
+------------------
+
+* Fixed buggy handling when http checks are specified with a port.
+* Changed User-Agent header and stripped port from Host header for http checks.
+* Refactored a bunch of code into a separate ``holdup.checks`` module.
+
 5.0.0 (2024-04-11)
 ------------------
 
 * Added a static binary in the Github release (built with Pyinstaller on Alpine, as a static bin).
 * Dropped support for Python 3.7 and added in Python 3.12 in the test suite.
 
 4.0.0 (2023-02-14)
```

### Comparing `holdup-5.0.0/CONTRIBUTING.rst` & `holdup-5.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/LICENSE` & `holdup-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/PKG-INFO` & `holdup-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holdup
-Version: 5.0.0
+Version: 5.1.0
 Summary: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
 Home-page: https://github.com/ionelmc/python-holdup
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-holdup.readthedocs.io/
 Project-URL: Changelog, https://python-holdup.readthedocs.io/en/latest/changelog.html
@@ -135,14 +135,21 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+5.1.0 (2024-04-12)
+------------------
+
+* Fixed buggy handling when http checks are specified with a port.
+* Changed User-Agent header and stripped port from Host header for http checks.
+* Refactored a bunch of code into a separate ``holdup.checks`` module.
+
 5.0.0 (2024-04-11)
 ------------------
 
 * Added a static binary in the Github release (built with Pyinstaller on Alpine, as a static bin).
 * Dropped support for Python 3.7 and added in Python 3.12 in the test suite.
 
 4.0.0 (2023-02-14)
```

### Comparing `holdup-5.0.0/README.rst` & `holdup-5.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/holdup
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/holdup.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/holdup
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-holdup/v5.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-holdup/v5.1.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ionelmc/python-holdup/compare/v5.0.0...master
+    :target: https://github.com/ionelmc/python-holdup/compare/v5.1.0...master
 
 
 
 .. end-badges
 
 A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services
 (like almost everything).
```

### Comparing `holdup-5.0.0/ci/bootstrap.py` & `holdup-5.1.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/ci/templates/.github/workflows/github-actions.yml` & `holdup-5.1.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 {% else %}
 {% set python %}{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% set cpython %}cp{{ prefix[2:] }}{% endset %}
 {% set toxpython %}python{{ prefix[2] }}.{{ prefix[3:] }}{% endset %}
 {% endif %}
 {% for os, python_arch in [
     ['ubuntu', 'x64'],
-    ['windows', 'x64'],
     ['macos', 'x64'],
 ] %}
           - name: '{{ env }} ({{ os }})'
             python: '{{ python }}'
             toxpython: '{{ toxpython }}'
             python_arch: '{{ python_arch }}'
             tox_env: '{{ env }}'
```

### Comparing `holdup-5.0.0/docs/conf.py` & `holdup-5.1.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,29 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "Holdup"
 year = "2016-2024"
 author = "Ionel Cristian Mărieș"
 copyright = f"{year}, {author}"
-version = release = "5.0.0"
+version = release = "5.1.0"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
-    "issue": ("https://github.com/ionelmc/python-holdup/issues/%s", "#"),
-    "pr": ("https://github.com/ionelmc/python-holdup/pull/%s", "PR #"),
+    "issue": ("https://github.com/ionelmc/python-holdup/issues/%s", "#%s"),
+    "pr": ("https://github.com/ionelmc/python-holdup/pull/%s", "PR #%s"),
 }
+html_theme = "furo"
 
 html_theme_options = {
     "githuburl": "https://github.com/ionelmc/python-holdup/",
 }
 
 html_use_smartypants = True
 html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
-html_sidebars = {
-    "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
-}
 html_short_title = f"{project}-{version}"
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
```

### Comparing `holdup-5.0.0/pyproject.toml` & `holdup-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/pytest.ini` & `holdup-5.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/setup.py` & `holdup-5.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="holdup",
-    version="5.0.0",
+    version="5.1.0",
     license="BSD-2-Clause",
     description="A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Ionel Cristian Mărieș",
```

### Comparing `holdup-5.0.0/src/holdup.egg-info/PKG-INFO` & `holdup-5.1.0/src/holdup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holdup
-Version: 5.0.0
+Version: 5.1.0
 Summary: A tool to wait for services and execute command. Useful for Docker containers that depend on slow to start services (like almost everything).
 Home-page: https://github.com/ionelmc/python-holdup
 Author: Ionel Cristian Mărieș
 Author-email: contact@ionelmc.ro
 License: BSD-2-Clause
 Project-URL: Documentation, https://python-holdup.readthedocs.io/
 Project-URL: Changelog, https://python-holdup.readthedocs.io/en/latest/changelog.html
@@ -135,14 +135,21 @@
 
             PYTEST_ADDOPTS=--cov-append tox
 
 
 Changelog
 =========
 
+5.1.0 (2024-04-12)
+------------------
+
+* Fixed buggy handling when http checks are specified with a port.
+* Changed User-Agent header and stripped port from Host header for http checks.
+* Refactored a bunch of code into a separate ``holdup.checks`` module.
+
 5.0.0 (2024-04-11)
 ------------------
 
 * Added a static binary in the Github release (built with Pyinstaller on Alpine, as a static bin).
 * Dropped support for Python 3.7 and added in Python 3.12 in the test suite.
 
 4.0.0 (2023-02-14)
```

### Comparing `holdup-5.0.0/src/holdup.egg-info/SOURCES.txt` & `holdup-5.1.0/src/holdup.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,37 +8,38 @@
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 Dockerfile
 LICENSE
 MANIFEST.in
 README.rst
+holdup.spec
+pyinstaller.Dockerfile
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
 .github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
-docs/installation.rst
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
-docs/usage.rst
-docs/reference/holdup.rst
 docs/reference/index.rst
 src/holdup/__init__.py
 src/holdup/__main__.py
+src/holdup/checks.py
 src/holdup/cli.py
+src/holdup/pg.py
 src/holdup.egg-info/PKG-INFO
 src/holdup.egg-info/SOURCES.txt
 src/holdup.egg-info/dependency_links.txt
 src/holdup.egg-info/entry_points.txt
 src/holdup.egg-info/not-zip-safe
 src/holdup.egg-info/requires.txt
 src/holdup.egg-info/top_level.txt
```

### Comparing `holdup-5.0.0/tests/Dockerfile` & `holdup-5.1.0/tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/tests/test_holdup.py` & `holdup-5.1.0/tests/test_holdup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # ruff: noqa: PTH110, PTH120, PTH123
 import os
+import shutil
 import socket
 import threading
-from distutils import spawn
 
 import pytest
 
 pytest_plugins = ("pytester",)
 
 
 def has_docker():
-    return spawn.find_executable("docker") and spawn.find_executable("docker-compose")
+    return shutil.which("docker")
 
 
 @pytest.fixture(params=[[], ["--", "python", "-c", 'print("success !")']])
 def extra(request):
     return request.param
 
 
@@ -51,49 +51,59 @@
     tcp.close()
     unix_path.unlink()
 
 
 @pytest.mark.parametrize("status", [200, 404])
 @pytest.mark.parametrize("proto", ["http", "https"])
 def test_http(testdir, extra, status, proto):
-    result = testdir.run("holdup", "-T", "5", "-t", "5.1", f"{proto}://httpbin.org/status/{status}", *extra)
+    result = testdir.run("holdup", "-T", "5", "-t", "5.1", f"{proto}://httpbingo.org/status/{status}", *extra)
+    if extra:
+        if status == 200:
+            result.stdout.fnmatch_lines(["success !"])
+        else:
+            result.stderr.fnmatch_lines(["*HTTP Error 404*"])
+
+
+@pytest.mark.parametrize("status", [200, 404])
+def test_http_port(testdir, extra, status):
+    result = testdir.run("holdup", "-T", "5", "-t", "5.1", f"http://httpbingo.org:80/status/{status}", *extra)
     if extra:
         if status == 200:
             result.stdout.fnmatch_lines(["success !"])
         else:
             result.stderr.fnmatch_lines(["*HTTP Error 404*"])
 
 
 @pytest.mark.parametrize("auth", ["basic-auth", "digest-auth/auth"])
 @pytest.mark.parametrize("proto", ["http", "https"])
 def test_http_auth(testdir, extra, auth, proto):
-    result = testdir.run("holdup", "-T", "5", "-t", "5.1", f"{proto}://usr:pwd@httpbin.org/{auth}/usr/pwd", *extra)
+    result = testdir.run("holdup", "-T", "5", "-t", "5.1", f"{proto}://usr:pwd@httpbingo.org/{auth}/usr/pwd", *extra)
     if extra:
         result.stdout.fnmatch_lines(["success !"])
 
 
 def test_http_insecure_with_option(testdir):
     result = testdir.run("holdup", "-t", "2", "--insecure", "https://self-signed.badssl.com/")
     assert result.ret == 0
 
 
 def test_http_insecure_with_proto(testdir):
     result = testdir.run("holdup", "-t", "2", "https+insecure://self-signed.badssl.com/")
     assert result.ret == 0
 
 
-def test_any(testdir, tmp_path_factory, extra):
+def test_any1(testdir, tmp_path_factory, extra):
     tcp = socket.socket()
     tcp.bind(("127.0.0.1", 0))
     _, port = tcp.getsockname()
 
     uds = socket.socket(socket.AF_UNIX)
 
     tmp_path = tmp_path_factory.getbasetemp()
-    unix_path = tmp_path / "sock"
+    unix_path = tmp_path / "s"
     path_path = tmp_path / "miss"
     uds.bind(str(unix_path))
     uds.listen(1)
     result = testdir.run("holdup", "-v", "-t", "0.5", f"tcp://localhost:{port}/,path://{path_path},unix://{unix_path}", *extra)
     if extra:
         result.stdout.fnmatch_lines(
             [
@@ -109,22 +119,21 @@
         )
     assert result.ret == 0
     tcp.close()
     uds.close()
     unix_path.unlink()
 
 
-def test_any2(testdir, tmp_path_factory, extra):
+def test_any2(testdir, tmp_path, extra):
     tcp = socket.socket()
     tcp.bind(("127.0.0.1", 0))
     _, port = tcp.getsockname()
 
     uds = socket.socket(socket.AF_UNIX)
-    tmp_path = tmp_path_factory.getbasetemp()
-    unix_path = tmp_path / "sock"
+    unix_path = tmp_path / "s"
     path_path = tmp_path / "miss"
     uds.bind(str(unix_path))
     uds.listen(1)
     result = testdir.run("holdup", "-v", "-t", "0.5", f"path://{path_path},unix://{unix_path},tcp://localhost:{port}/", *extra)
     if extra:
         result.stdout.fnmatch_lines(
             [
@@ -240,15 +249,15 @@
 def test_eval_falsey(testdir):
     result = testdir.run("holdup", "-t", "0", "eval://None")
     result.stderr.fnmatch_lines(["holdup: Failed checks: 'eval://None' -> Failed to evaluate 'None'. Result None is falsey. Aborting!"])
     assert result.ret == 1
 
 
 def test_eval_distutils(testdir, extra):
-    result = testdir.run("holdup", 'eval://__import__("distutils.spawn").spawn.find_executable("find")', *extra)
+    result = testdir.run("holdup", 'eval://__import__("shutil").which("find")', *extra)
     if extra:
         result.stdout.fnmatch_lines(["success !"])
     assert result.ret == 0
 
 
 def test_eval_comma(testdir, extra):
     result = testdir.run("holdup", 'eval://os.path.join("foo", "bar")', *extra)
```

### Comparing `holdup-5.0.0/tests/test_pg.py` & `holdup-5.1.0/tests/test_pg.py`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/tests/test_pg.sh` & `holdup-5.1.0/tests/test_pg.sh`

 * *Files identical despite different names*

### Comparing `holdup-5.0.0/tox.ini` & `holdup-5.1.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     *
 usedevelop = false
 deps =
     pytest
     pytest-cov
     pg3: psycopg
     {py38,py39,py310,py311,py312}-pg2: psycopg2-binary
-    {pypy38,pypy39}-pg2: psycopg2cffi
+    {pypy38,pypy39,pypy310}-pg2: psycopg2cffi
 commands =
     {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv tests}
 
 [testenv:check]
 deps =
     docutils
     check-manifest
```

