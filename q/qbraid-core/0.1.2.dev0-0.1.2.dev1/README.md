# Comparing `tmp/qbraid-core-0.1.2.dev0.tar.gz` & `tmp/qbraid-core-0.1.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.2.dev0.tar", last modified: Thu Apr 11 20:00:37 2024, max compression
+gzip compressed data, was "qbraid-core-0.1.2.dev1.tar", last modified: Thu Apr 11 23:06:32 2024, max compression
```

## Comparing `qbraid-core-0.1.2.dev0.tar` & `qbraid-core-0.1.2.dev1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.798846 qbraid-core-0.1.2.dev0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.802847 qbraid-core-0.1.2.dev0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.802847 qbraid-core-0.1.2.dev0/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.802847 qbraid-core-0.1.2.dev0/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.806846 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.806846 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.806846 qbraid-core-0.1.2.dev0/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 20:00:37.000000 qbraid-core-0.1.2.dev0/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_create_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_create_local_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_delete_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_installed_envs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_replace_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_system_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_system_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tests/test_update_install_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:00:37.810846 qbraid-core-0.1.2.dev0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-11 20:00:33.000000 qbraid-core-0.1.2.dev0/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.316510 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.316510 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.316510 qbraid-core-0.1.2.dev1/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_create_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_create_local_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_delete_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_system_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_system_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_update_install_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.github/workflows/docs.yml` & `qbraid-core-0.1.2.dev1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.github/workflows/format.yml` & `qbraid-core-0.1.2.dev1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.github/workflows/main.yml` & `qbraid-core-0.1.2.dev1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.github/workflows/publish.yml` & `qbraid-core-0.1.2.dev1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.github/workflows/test-publish.yml` & `qbraid-core-0.1.2.dev1/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/.gitignore` & `qbraid-core-0.1.2.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/LICENSE` & `qbraid-core-0.1.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/PKG-INFO` & `qbraid-core-0.1.2.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.2.dev0
+Version: 0.1.2.dev1
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.2.dev0/README.md` & `qbraid-core-0.1.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/Makefile` & `qbraid-core-0.1.2.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/cards/jupyter.png` & `qbraid-core-0.1.2.dev1/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/cards/python.png` & `qbraid-core-0.1.2.dev1/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/cards/terminal.png` & `qbraid-core-0.1.2.dev1/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/css/custom.css` & `qbraid-core-0.1.2.dev1/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/css/s4defs-roles.css` & `qbraid-core-0.1.2.dev1/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/favicon.ico` & `qbraid-core-0.1.2.dev1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/_static/logo.png` & `qbraid-core-0.1.2.dev1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/conf.py` & `qbraid-core-0.1.2.dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/index.rst` & `qbraid-core-0.1.2.dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/docs/make.bat` & `qbraid-core-0.1.2.dev1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/pyproject.toml` & `qbraid-core-0.1.2.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.2.dev0"
+version = "0.1.2.dev1"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
```

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/__init__.py` & `qbraid-core-0.1.2.dev1/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/_compat.py` & `qbraid-core-0.1.2.dev1/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/client.py` & `qbraid-core-0.1.2.dev1/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/config.py` & `qbraid-core-0.1.2.dev1/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/exceptions.py` & `qbraid-core-0.1.2.dev1/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/registry.py` & `qbraid-core-0.1.2.dev1/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/retry.py` & `qbraid-core-0.1.2.dev1/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/__init__.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/client.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/create.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/paths.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/state.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/environments/validate.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/__init__.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/adapter.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/client.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/services/quantum/proxy.py` & `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,59 @@
 
 """
 Module for checking state of qBraid Quantum Jobs proxies.
 
 """
 
 import logging
+from importlib.metadata import PackageNotFoundError, distribution
 from pathlib import Path
 from typing import Dict, Optional, Tuple, Union
 
 from qbraid_core.system import get_active_site_packages_path, get_venv_site_packages_path
 
 from .exceptions import QbraidException
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_QJOB_LIBS = ["braket"]
 
 
+def _check_proxy_braket() -> Tuple[bool, bool]:
+    """
+    Determine the braket proxy state by checking that amazon-braket-sdk,
+    boto3, and botocore are installed and that botocore is the qBraid fork.
+
+    Returns:
+        Tuple[bool, bool]: A tuple of two booleans indicating whether qBraid
+                           Quantum Jobs are supported and enabled, respectively.
+
+    """
+    packages = ["amazon-braket-sdk", "boto3", "botocore"]
+
+    supported = True
+    enabled = False
+
+    botocore_data = None
+    for package in packages:
+        try:
+            dist = distribution(package)
+            if package == "botocore":
+                botocore_data = dist.metadata
+        except PackageNotFoundError:
+            return False, False
+
+    if botocore_data:
+        homepage = botocore_data.get("Home-page", "")
+        if "github.com/qBraid/botocore" in homepage:
+            enabled = True
+
+    return supported, enabled
+
+
 def _check_proxy(
     proxy_spec: Tuple[str, ...], slug_path: Optional[Path] = None
 ) -> Tuple[bool, bool, Path]:
     """
     Checks if the specified proxy file exists and contains the string 'qbraid'.
 
     Args:
@@ -36,16 +69,15 @@
         'qbraid', False otherwise. The sitepackages path gives the location of the site-packages
         directory where the proxy file is located.
     """
     site_packages_path = None
 
     try:
         if slug_path is None:
-            site_packages: str = get_active_site_packages_path()
-            site_packages_path = Path(site_packages)
+            site_packages_path = get_active_site_packages_path()
         else:
             site_packages_path = get_venv_site_packages_path(slug_path / "pyenv")
     except QbraidException as err:
         logger.debug(err)
         return False, False, site_packages_path
 
     target_file_path = site_packages_path.joinpath(*proxy_spec)
@@ -88,17 +120,22 @@
         "enabled": False,
     }
 
     if device_lib not in SUPPORTED_QJOB_LIBS:
         raise ValueError(f"Unsupported quantum job library. Expected one of {SUPPORTED_QJOB_LIBS}")
 
     if device_lib == "braket":
-        proxy_lib = "botocore"
-        proxy_spec = (proxy_lib, "httpsession.py")
-        supported, enabled, path = _check_proxy(proxy_spec, **kwargs)
+        supported, enabled = _check_proxy_braket()
+        if supported and enabled:
+            pathlib = get_active_site_packages_path()
+            path = str(pathlib)
+        else:
+            proxy_lib = "botocore"
+            proxy_spec = (proxy_lib, "httpsession.py")
+            supported, enabled, path = _check_proxy(proxy_spec, **kwargs)
 
     # add more device libraries here as needed
 
     state["proxy_lib"] = proxy_lib
     state["supported"] = supported
     state["enabled"] = enabled
     state["path"] = str(path)
```

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/sessions.py` & `qbraid-core-0.1.2.dev1/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/system/__init__.py` & `qbraid-core-0.1.2.dev1/qbraid_core/system/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
    is_exe
    is_valid_python
    get_python_version_from_cfg
    get_python_version_from_exe
    get_venv_site_packages_path
    get_active_site_packages_path
+   get_active_python_path
    get_local_package_path
    get_local_package_version
    get_latest_package_version
    replace_str
    echo_log
 
 Exceptions
@@ -40,14 +41,15 @@
 
    QbraidSystemError
    UnknownFileSystemObjectError
 
 """
 from .exceptions import QbraidSystemError, UnknownFileSystemObjectError
 from .executables import (
+    get_active_python_path,
     get_python_version_from_cfg,
     get_python_version_from_exe,
     is_exe,
     is_valid_python,
 )
 from .generic import echo_log, replace_str
 from .packages import (
```

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/system/executables.py` & `qbraid-core-0.1.2.dev1/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/system/generic.py` & `qbraid-core-0.1.2.dev1/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/system/packages.py` & `qbraid-core-0.1.2.dev1/qbraid_core/system/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import ast
 import logging
 import site
 import subprocess
 import sys
 from importlib.metadata import PackageNotFoundError, version
 from pathlib import Path
+from typing import Optional
 
 import requests
 
 from .exceptions import QbraidSystemError
 from .executables import (
     get_active_python_path,
     get_python_version_from_cfg,
@@ -58,23 +59,23 @@
         raise QbraidSystemError("Unable to determine Python version from the virtual environment.")
 
     major_minor_version = ".".join(python_version.split(".")[:2])
     lib_python_dir = venv_path / f"lib/python{major_minor_version}"
     return lib_python_dir / "site-packages"
 
 
-def get_active_site_packages_path() -> Path:
+def get_active_site_packages_path(python_path: Optional[Path] = None) -> Path:
     """
     Retrieves the site-packages path of the current Python environment,
     respecting active virtual environments, as well.
 
     """
 
     current_python_path = Path(sys.executable)
-    shell_python_path = get_active_python_path()
+    shell_python_path = python_path or get_active_python_path()
 
     if shell_python_path == current_python_path:
         site_packages_paths = [Path(path) for path in site.getsitepackages()]
 
     else:
         try:
             result = subprocess.run(
```

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core/system/threader.py` & `qbraid-core-0.1.2.dev1/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core.egg-info/PKG-INFO` & `qbraid-core-0.1.2.dev1/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.2.dev0
+Version: 0.1.2.dev1
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.2.dev0/qbraid_core.egg-info/SOURCES.txt` & `qbraid-core-0.1.2.dev1/qbraid_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/fixtures/environments.py` & `qbraid-core-0.1.2.dev1/tests/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_client.py` & `qbraid-core-0.1.2.dev1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_compat.py` & `qbraid-core-0.1.2.dev1/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_config.py` & `qbraid-core-0.1.2.dev1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_create_environment.py` & `qbraid-core-0.1.2.dev1/tests/test_create_environment.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_create_local_venv.py` & `qbraid-core-0.1.2.dev1/tests/test_create_local_venv.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_delete_environment.py` & `qbraid-core-0.1.2.dev1/tests/test_delete_environment.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_environments.py` & `qbraid-core-0.1.2.dev1/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_installed_envs_data.py` & `qbraid-core-0.1.2.dev1/tests/test_installed_envs_data.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_replace_str.py` & `qbraid-core-0.1.2.dev1/tests/test_replace_str.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_session.py` & `qbraid-core-0.1.2.dev1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_system_executables.py` & `qbraid-core-0.1.2.dev1/tests/test_system_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_system_packages.py` & `qbraid-core-0.1.2.dev1/tests/test_system_packages.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tests/test_update_install_status.py` & `qbraid-core-0.1.2.dev1/tests/test_update_install_status.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev0/tools/verify_headers.py` & `qbraid-core-0.1.2.dev1/tools/verify_headers.py`

 * *Files identical despite different names*

