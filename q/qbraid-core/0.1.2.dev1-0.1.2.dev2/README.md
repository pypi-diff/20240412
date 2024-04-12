# Comparing `tmp/qbraid-core-0.1.2.dev1.tar.gz` & `tmp/qbraid-core-0.1.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.2.dev1.tar", last modified: Thu Apr 11 23:06:32 2024, max compression
+gzip compressed data, was "qbraid-core-0.1.2.dev2.tar", last modified: Fri Apr 12 00:32:48 2024, max compression
```

## Comparing `qbraid-core-0.1.2.dev1.tar` & `qbraid-core-0.1.2.dev2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.308509 qbraid-core-0.1.2.dev1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.312509 qbraid-core-0.1.2.dev1/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.316510 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.316510 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.316510 qbraid-core-0.1.2.dev1/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 23:06:32.000000 qbraid-core-0.1.2.dev1/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_create_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_create_local_venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_delete_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_installed_envs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_replace_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_system_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_system_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tests/test_update_install_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:06:32.320510 qbraid-core-0.1.2.dev1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-11 23:06:28.000000 qbraid-core-0.1.2.dev1/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.389665 qbraid-core-0.1.2.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.373665 qbraid-core-0.1.2.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.373665 qbraid-core-0.1.2.dev2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.377665 qbraid-core-0.1.2.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-12 00:32:48.389665 qbraid-core-0.1.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.377665 qbraid-core-0.1.2.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.377665 qbraid-core-0.1.2.dev2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.377665 qbraid-core-0.1.2.dev2/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.377665 qbraid-core-0.1.2.dev2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.377665 qbraid-core-0.1.2.dev2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.381665 qbraid-core-0.1.2.dev2/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 00:32:48.000000 qbraid-core-0.1.2.dev2/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.381665 qbraid-core-0.1.2.dev2/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.381665 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.381665 qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.385665 qbraid-core-0.1.2.dev2/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.385665 qbraid-core-0.1.2.dev2/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-12 00:32:48.000000 qbraid-core-0.1.2.dev2/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-12 00:32:48.000000 qbraid-core-0.1.2.dev2/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:32:48.000000 qbraid-core-0.1.2.dev2/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 00:32:48.000000 qbraid-core-0.1.2.dev2/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 00:32:48.000000 qbraid-core-0.1.2.dev2/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:32:48.389665 qbraid-core-0.1.2.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.385665 qbraid-core-0.1.2.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.385665 qbraid-core-0.1.2.dev2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_create_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_create_local_venv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_delete_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_system_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_system_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tests/test_update_install_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:32:48.385665 qbraid-core-0.1.2.dev2/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-12 00:32:44.000000 qbraid-core-0.1.2.dev2/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-core-0.1.2.dev2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-core-0.1.2.dev2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.github/workflows/docs.yml` & `qbraid-core-0.1.2.dev2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.github/workflows/format.yml` & `qbraid-core-0.1.2.dev2/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.github/workflows/main.yml` & `qbraid-core-0.1.2.dev2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.github/workflows/publish.yml` & `qbraid-core-0.1.2.dev2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.github/workflows/test-publish.yml` & `qbraid-core-0.1.2.dev2/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/.gitignore` & `qbraid-core-0.1.2.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/LICENSE` & `qbraid-core-0.1.2.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/PKG-INFO` & `qbraid-core-0.1.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.2.dev1
+Version: 0.1.2.dev2
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.2.dev1/README.md` & `qbraid-core-0.1.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/Makefile` & `qbraid-core-0.1.2.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/cards/jupyter.png` & `qbraid-core-0.1.2.dev2/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/cards/python.png` & `qbraid-core-0.1.2.dev2/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/cards/terminal.png` & `qbraid-core-0.1.2.dev2/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/css/custom.css` & `qbraid-core-0.1.2.dev2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/css/s4defs-roles.css` & `qbraid-core-0.1.2.dev2/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/favicon.ico` & `qbraid-core-0.1.2.dev2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/_static/logo.png` & `qbraid-core-0.1.2.dev2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/conf.py` & `qbraid-core-0.1.2.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/index.rst` & `qbraid-core-0.1.2.dev2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/docs/make.bat` & `qbraid-core-0.1.2.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/pyproject.toml` & `qbraid-core-0.1.2.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.2.dev1"
+version = "0.1.2.dev2"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
```

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/__init__.py` & `qbraid-core-0.1.2.dev2/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/_compat.py` & `qbraid-core-0.1.2.dev2/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/client.py` & `qbraid-core-0.1.2.dev2/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/config.py` & `qbraid-core-0.1.2.dev2/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/exceptions.py` & `qbraid-core-0.1.2.dev2/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/registry.py` & `qbraid-core-0.1.2.dev2/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/retry.py` & `qbraid-core-0.1.2.dev2/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/__init__.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/client.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/create.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/paths.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/state.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/environments/validate.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/__init__.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/adapter.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/client.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 import sys
 from typing import Any, Dict, List, Optional
 
 from qbraid_core.client import QbraidClient
 from qbraid_core.exceptions import RequestsApiError
 from qbraid_core.registry import register_client
+from qbraid_core.system import get_active_python_path
 
 from .exceptions import QuantumServiceRequestError
 from .proxy import SUPPORTED_QJOB_LIBS, quantum_lib_proxy_state
 
 
 @register_client()
 class QuantumClient(QbraidClient):
@@ -125,29 +126,32 @@
     def create_job(self, data: Dict[str, Any]) -> Dict[str, Any]:
         """Creates a new quantum job with the given data."""
         try:
             return self.session.post("/quantum-jobs", json=data).json()
         except RequestsApiError as err:
             raise QuantumServiceRequestError("Failed to create job") from err
 
-    def qbraid_jobs_state(self, device_lib: Optional[str] = None) -> Dict[str, Any]:
+    @staticmethod
+    def qbraid_jobs_state(device_lib: Optional[str] = None) -> Dict[str, Any]:
         """
         Checks if qBraid Quantum Jobs are enabled in the current environment for the
         specified device library.
 
         Args:
             device_lib (Optional[str]): The name of the quantum device library. If None,
                                         checks all supported libraries.
 
         Returns:
             Dict[str, Any]: A dictionary containing the system's executable path and the states
                             of libraries relevant to qBraid Quantum Jobs. The libraries' states
                             include whether they are supported and enabled.
         """
-        environment_state = {"exe": sys.executable}
+        python_exe = get_active_python_path()
+        environment_state = {"exe": str(python_exe)}
+
         check_libs = [device_lib] if device_lib else SUPPORTED_QJOB_LIBS
 
         libs_state = {lib: quantum_lib_proxy_state(lib) for lib in check_libs}
 
         environment_state["libs"] = libs_state
 
         return environment_state
```

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/services/quantum/proxy.py` & `qbraid-core-0.1.2.dev2/qbraid_core/services/quantum/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,22 +121,18 @@
     }
 
     if device_lib not in SUPPORTED_QJOB_LIBS:
         raise ValueError(f"Unsupported quantum job library. Expected one of {SUPPORTED_QJOB_LIBS}")
 
     if device_lib == "braket":
         supported, enabled = _check_proxy_braket()
-        if supported and enabled:
-            pathlib = get_active_site_packages_path()
-            path = str(pathlib)
-        else:
+        if supported and not enabled:
             proxy_lib = "botocore"
             proxy_spec = (proxy_lib, "httpsession.py")
-            supported, enabled, path = _check_proxy(proxy_spec, **kwargs)
+            supported, enabled, _ = _check_proxy(proxy_spec, **kwargs)
 
     # add more device libraries here as needed
 
     state["proxy_lib"] = proxy_lib
     state["supported"] = supported
     state["enabled"] = enabled
-    state["path"] = str(path)
     return state
```

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/sessions.py` & `qbraid-core-0.1.2.dev2/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/system/__init__.py` & `qbraid-core-0.1.2.dev2/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/system/executables.py` & `qbraid-core-0.1.2.dev2/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/system/generic.py` & `qbraid-core-0.1.2.dev2/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/system/packages.py` & `qbraid-core-0.1.2.dev2/qbraid_core/system/packages.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core/system/threader.py` & `qbraid-core-0.1.2.dev2/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core.egg-info/PKG-INFO` & `qbraid-core-0.1.2.dev2/qbraid_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.2.dev1
+Version: 0.1.2.dev2
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.2.dev1/qbraid_core.egg-info/SOURCES.txt` & `qbraid-core-0.1.2.dev2/qbraid_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/fixtures/environments.py` & `qbraid-core-0.1.2.dev2/tests/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_client.py` & `qbraid-core-0.1.2.dev2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_compat.py` & `qbraid-core-0.1.2.dev2/tests/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_config.py` & `qbraid-core-0.1.2.dev2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_create_environment.py` & `qbraid-core-0.1.2.dev2/tests/test_create_environment.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_create_local_venv.py` & `qbraid-core-0.1.2.dev2/tests/test_create_local_venv.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_delete_environment.py` & `qbraid-core-0.1.2.dev2/tests/test_delete_environment.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_environments.py` & `qbraid-core-0.1.2.dev2/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_installed_envs_data.py` & `qbraid-core-0.1.2.dev2/tests/test_installed_envs_data.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_replace_str.py` & `qbraid-core-0.1.2.dev2/tests/test_replace_str.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_session.py` & `qbraid-core-0.1.2.dev2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_system_executables.py` & `qbraid-core-0.1.2.dev2/tests/test_system_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_system_packages.py` & `qbraid-core-0.1.2.dev2/tests/test_system_packages.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tests/test_update_install_status.py` & `qbraid-core-0.1.2.dev2/tests/test_update_install_status.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.2.dev1/tools/verify_headers.py` & `qbraid-core-0.1.2.dev2/tools/verify_headers.py`

 * *Files identical despite different names*

