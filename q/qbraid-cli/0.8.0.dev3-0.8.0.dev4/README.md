# Comparing `tmp/qbraid-cli-0.8.0.dev3.tar.gz` & `tmp/qbraid_cli-0.8.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-cli-0.8.0.dev3.tar", last modified: Wed Apr 10 17:23:03 2024, max compression
+gzip compressed data, was "qbraid_cli-0.8.dev4.tar", last modified: Fri Apr 12 21:20:55 2024, max compression
```

## Comparing `qbraid-cli-0.8.0.dev3.tar` & `qbraid_cli-0.8.dev4.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.453631 qbraid-cli-0.8.0.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.421630 qbraid-cli-0.8.0.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.421630 qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.425630 qbraid-cli-0.8.0.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/MANIFEST.IN
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 17:23:03.453631 qbraid-cli-0.8.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.425630 qbraid-cli-0.8.0.dev3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.425630 qbraid-cli-0.8.0.dev3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.429630 qbraid-cli-0.8.0.dev3/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.429630 qbraid-cli-0.8.0.dev3/docs/_static/style/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/style/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/_static/style/s4defs-roles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.433630 qbraid-cli-0.8.0.dev3/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/configure.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/devices-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.433630 qbraid-cli-0.8.0.dev3/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.433630 qbraid-cli-0.8.0.dev3/qbraid_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/configure/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/credits/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/devices/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/envs/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/toggle_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/qbraid_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 17:23:03.000000 qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:23:03.453631 qbraid-cli-0.8.0.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.437631 qbraid-cli-0.8.0.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_configure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/test_configure_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/test_prompt_for_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_configure/test_validate_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_credits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_credits/test_credits_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_devices/test_devices_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_devices/test_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.441630 qbraid-cli-0.8.0.dev3/tests/test_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_activate_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_find_shell_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_print_activate_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_create_qbraid_env_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_replace_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_update_state_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_installed_envs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_is_valid_env_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_request_delete_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_validate_env_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.445630 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_disable_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_enable_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_get_package_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_handle_jobs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_run_progress_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_validate_library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tests/test_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tests/test_kernels/test_kernels_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:23:03.449631 qbraid-cli-0.8.0.dev3/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tools/split_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-10 17:22:57.000000 qbraid-cli-0.8.0.dev3/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.153820 qbraid_cli-0.8.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.125820 qbraid_cli-0.8.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.125820 qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/MANIFEST.IN
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-12 21:20:55.153820 qbraid_cli-0.8.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.129819 qbraid_cli-0.8.dev4/docs/_static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/style/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/_static/style/s4defs-roles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.133819 qbraid_cli-0.8.dev4/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/devices-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.133819 qbraid_cli-0.8.dev4/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.133819 qbraid_cli-0.8.dev4/qbraid_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 21:20:54.000000 qbraid_cli-0.8.dev4/qbraid_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/configure/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/configure/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/credits/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/devices/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/devices/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.137820 qbraid_cli-0.8.dev4/qbraid_cli/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/envs/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/qbraid_cli/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/toggle_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/jobs/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/qbraid_cli/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/kernels/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/qbraid_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 21:20:55.000000 qbraid_cli-0.8.dev4/qbraid_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:20:55.153820 qbraid_cli-0.8.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_configure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/test_configure_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/test_prompt_for_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_configure/test_validate_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_credits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_credits/test_credits_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_devices/test_devices_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_devices/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.141820 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_activate_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_find_shell_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_print_activate_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_envs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_envs/test_create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_create_qbraid_env_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_update_state_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_is_valid_env_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_request_delete_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_validate_env_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.145820 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_disable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_enable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_get_package_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_handle_jobs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_run_progress_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_validate_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tests/test_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tests/test_kernels/test_kernels_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:55.149820 qbraid_cli-0.8.dev4/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tools/split_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-12 21:20:49.000000 qbraid_cli-0.8.dev4/tools/verify_headers.py
```

### Comparing `qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_cli-0.8.dev4/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.github/workflows/docs.yml` & `qbraid_cli-0.8.dev4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.github/workflows/format.yml` & `qbraid_cli-0.8.dev4/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.github/workflows/main.yml` & `qbraid_cli-0.8.dev4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.github/workflows/publish.yml` & `qbraid_cli-0.8.dev4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.github/workflows/test-publish.yml` & `qbraid_cli-0.8.dev4/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.gitignore` & `qbraid_cli-0.8.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/.readthedocs.yml` & `qbraid_cli-0.8.dev4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/CONTRIBUTING.md` & `qbraid_cli-0.8.dev4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/Makefile` & `qbraid_cli-0.8.dev4/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/PKG-INFO` & `qbraid_cli-0.8.dev4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev3
+Version: 0.8.0.dev4
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -25,28 +25,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.12.1
 Requires-Dist: rich>=10.11.0
 Requires-Dist: jupyter_client<9.0.0,>=7.0.0
-Requires-Dist: qbraid-core>=0.1.1
+Requires-Dist: qbraid-core>=0.1.2
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
 Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: toml; extra == "docs"
 Requires-Dist: build; extra == "docs"
+Requires-Dist: m2r; extra == "docs"
+Requires-Dist: typer; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
```

### Comparing `qbraid-cli-0.8.0.dev3/README.md` & `qbraid_cli-0.8.dev4/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/Makefile` & `qbraid_cli-0.8.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/api-key.png` & `qbraid_cli-0.8.dev4/docs/_static/api-key.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/cards/jupyter.png` & `qbraid_cli-0.8.dev4/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/cards/python.png` & `qbraid_cli-0.8.dev4/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/cards/terminal.png` & `qbraid_cli-0.8.dev4/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/favicon.ico` & `qbraid_cli-0.8.dev4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/logo.png` & `qbraid_cli-0.8.dev4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/style/custom.css` & `qbraid_cli-0.8.dev4/docs/_static/style/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/_static/style/s4defs-roles.css` & `qbraid_cli-0.8.dev4/docs/_static/style/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/configure.rst` & `qbraid_cli-0.8.dev4/docs/cli/configure.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/devices-list.rst` & `qbraid_cli-0.8.dev4/docs/cli/devices-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/envs-activate.rst` & `qbraid_cli-0.8.dev4/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/envs-list.rst` & `qbraid_cli-0.8.dev4/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/envs-uninstall.rst` & `qbraid_cli-0.8.dev4/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/envs.rst` & `qbraid_cli-0.8.dev4/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/jobs-add.rst` & `qbraid_cli-0.8.dev4/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/jobs-disable.rst` & `qbraid_cli-0.8.dev4/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/jobs-enable.rst` & `qbraid_cli-0.8.dev4/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/jobs-list.rst` & `qbraid_cli-0.8.dev4/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/jobs.rst` & `qbraid_cli-0.8.dev4/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/kernels.rst` & `qbraid_cli-0.8.dev4/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/cli/qbraid.rst` & `qbraid_cli-0.8.dev4/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/conf.py` & `qbraid_cli-0.8.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/guide/overview.rst` & `qbraid_cli-0.8.dev4/docs/guide/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/index.rst` & `qbraid_cli-0.8.dev4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/docs/make.bat` & `qbraid_cli-0.8.dev4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/pyproject.toml` & `qbraid_cli-0.8.dev4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-cli"
-version = "0.8.0.dev3"
+version = "0.8.0.dev4"
 description = "Command Line Interface for interacting with all parts of the qBraid platform."
 readme = "README.md"
 authors = [{ name = "qBraid Development Team", email = "contact@qbraid.com" }]
 license = { text = "Proprietary" }
 keywords = ["qbraid", "cli", "quantum", "cloud"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -26,29 +26,29 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "typer>=0.12.1",
     "rich>=10.11.0",
     "jupyter_client>=7.0.0,<9.0.0",
-    "qbraid-core>=0.1.1",
+    "qbraid-core>=0.1.2",
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
 
 [project.optional-dependencies]
 jobs = ["amazon-braket-sdk>=1.48.1"]
 dev = ["black", "isort", "pylint", "pytest"]
-docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.21", "toml", "build"]
+docs = ["sphinx~=7.2.6", "sphinx-rtd-theme>=1.3,<2.1", "docutils<0.21", "toml", "build", "m2r", "typer"]
 
 [project.scripts]
 qbraid = "qbraid_cli.main:app"
 
 [tool.setuptools_scm]
 write_to = "qbraid_cli/_version.py"
```

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/configure/actions.py` & `qbraid_cli-0.8.dev4/qbraid_cli/configure/actions.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/configure/app.py` & `qbraid_cli-0.8.dev4/qbraid_cli/configure/app.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/credits/app.py` & `qbraid_cli-0.8.dev4/qbraid_cli/credits/app.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/devices/app.py` & `qbraid_cli-0.8.dev4/qbraid_cli/devices/app.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/devices/validation.py` & `qbraid_cli-0.8.dev4/qbraid_cli/devices/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/activate.py` & `qbraid_cli-0.8.dev4/qbraid_cli/envs/activate.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/app.py` & `qbraid_cli-0.8.dev4/qbraid_cli/envs/app.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/create.py` & `qbraid_cli-0.8.dev4/qbraid_cli/envs/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/envs/data_handling.py` & `qbraid_cli-0.8.dev4/qbraid_cli/envs/data_handling.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/exceptions.py` & `qbraid_cli-0.8.dev4/qbraid_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/handlers.py` & `qbraid_cli-0.8.dev4/qbraid_cli/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,19 @@
     """
     error_type = error_type or "Error"
     message = message or DEFAULT_ERROR_MESSAGE
     error_prefix = typer.style(f"{error_type}:", fg=typer.colors.RED, bold=True)
     full_message = f"\n{error_prefix} {message}\n"
     if include_traceback:
         tb_string = traceback.format_exc()
-        full_message += f"\n{tb_string}"
+        # TODO: find out reason for weird traceback emitted from
+        # qbraid jobs enable/disable when library not installed.
+        # For now, if matches, just don't print it.
+        if tb_string.strip() != "NoneType: None":
+            full_message += f"\n{tb_string}"
     typer.echo(full_message, err=True)
     raise typer.Exit(code=1)
 
 
 def handle_filesystem_operation(operation: Callable[[], None], path: Path) -> None:
     """
     Executes a filesystem operation with error handling.
```

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/app.py` & `qbraid_cli-0.8.dev4/qbraid_cli/jobs/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Module defining commands in the 'qbraid jobs' namespace.
 
 """
-
-import sys
 from typing import Any, Callable, Dict, Tuple
 
 import typer
 from rich.console import Console
 
 from qbraid_cli.handlers import handle_error, run_progress_task
 from qbraid_cli.jobs.toggle_braket import disable_braket, enable_braket
@@ -64,23 +62,24 @@
     library: str = typer.Argument(
         default=None,
         help="Optional: Specify a software library with quantum jobs support to check its status.",
         callback=validate_library,
     )
 ) -> None:
     """Display the state of qBraid Quantum Jobs for the current environment."""
-    state_values: Dict[str, Tuple[bool, bool]] = run_progress_get_state(library)
+    result: Tuple[str, Dict[str, Tuple[bool, bool]]] = run_progress_get_state(library)
+    python_exe, state_values = result
     state_values = dict(sorted(state_values.items()))
 
     console = Console()
     header_1, header_2 = "Library", "State"
     max_lib_length = max((len(lib) for lib in state_values.keys()), default=len(header_1))
     padding = max_lib_length + 9
 
-    console.print(f"Executable: {sys.executable}")
+    console.print(f"Executable: {python_exe}")
     console.print(f"\n{header_1:<{padding}}{header_2}", style="bold")
 
     for lib, (installed, enabled) in state_values.items():
         state_str = (
             "[green]enabled"
             if enabled and installed
             else "[red]disabled" if installed else "[grey70]unavailable"
```

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/toggle_braket.py` & `qbraid_cli-0.8.dev4/qbraid_cli/jobs/toggle_braket.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,60 +5,58 @@
 Module supporting 'qbraid jobs enable/disable braket' and commands.
 
 """
 
 import logging
 import os
 import subprocess
-import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 import typer
-from qbraid_core.system import (
-    QbraidSystemError,
-    get_active_site_packages_path,
-    get_latest_package_version,
-    get_local_package_version,
-)
 
 from qbraid_cli.exceptions import QbraidException
 from qbraid_cli.handlers import handle_error, handle_filesystem_operation, run_progress_task
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
-def get_package_data(package: str) -> Tuple[str, str, str]:
+def get_package_data(package: str) -> Tuple[str, str, str, str]:
     """Retrieve package version and location data.
 
     Args:
         package (str): The name of the package to retrieve data for.
 
     Returns:
-        Tuple[str, str, str]: The installed and latest versions of the package, and the
-                              local site-packages path where it is / would be installed.
+        Tuple[str, str, str, str]: The installed and latest versions of the package, and the
+                                   local site-packages path where it is / would be installed.
 
     Raises:
         QbraidException: If package version or location data cannot be retrieved.
 
     """
+    # pylint: disable=import-outside-toplevel
+    from qbraid_core.system import (
+        QbraidSystemError,
+        get_active_python_path,
+        get_active_site_packages_path,
+        get_latest_package_version,
+        get_local_package_version,
+    )
 
     try:
-        installed_version = get_local_package_version(package)
+        python_pathlib = get_active_python_path()
+        site_packages_path = get_active_site_packages_path(python_path=python_pathlib)
+        installed_version = get_local_package_version(package, python_path=python_pathlib)
         latest_version = get_latest_package_version(package)
     except QbraidSystemError as err:
-        raise QbraidException("Failed to retrieve package version information") from err
-
-    try:
-        site_packages_path = get_active_site_packages_path()
-    except QbraidSystemError as err:
-        raise QbraidException("Failed to retrieve site-package location") from err
+        raise QbraidException("Failed to retrieve required system and/or package metadata") from err
 
-    return installed_version, latest_version, site_packages_path
+    return installed_version, latest_version, str(site_packages_path), str(python_pathlib)
 
 
 def confirm_updates(
     mode: str,
     site_packages_path: str,
     installed_version: Optional[str] = None,
     latest_version: Optional[str] = None,
@@ -113,16 +111,14 @@
     typer.echo(f"  {core_package} location: {os.path.join(site_packages_path, core_package)}\n")
 
     user_confirmation = typer.confirm("Proceed", default=True)
     if not user_confirmation:
         typer.echo("\nqBraidSystemExit: Exiting.")
         raise typer.Exit()
 
-    typer.echo("")
-
 
 def aws_configure_dummy() -> None:
     """
     Initializes AWS configuration and credentials files with placeholder values.
 
     This function ensures the existence of AWS config and credentials files in the user's home
     directory. If these files do not already exist, it creates them and populates them with
@@ -152,58 +148,59 @@
         handle_filesystem_operation(configure_aws, aws_dir)
     except QbraidException:
         handle_error(message="Failed to configure qBraid quantum jobs.")
 
 
 def enable_braket(auto_confirm: bool = False):
     """Enable qBraid quantum jobs for Amazon Braket."""
-    installed, latest, path = run_progress_task(
+    installed, latest, path, python_exe = run_progress_task(
         get_package_data, "boto3", description="Solving environment..."
     )
 
     if not auto_confirm:
         confirm_updates("enable", path, installed_version=installed, latest_version=latest)
+    typer.echo("")
 
     aws_configure_dummy()  # TODO: possibly add another confirmation for writing aws config files
+
     try:
-        subprocess.check_call([sys.executable, "-m", "pip", "install", "--upgrade", "boto3"])
+        subprocess.check_call([python_exe, "-m", "pip", "install", "--upgrade", "boto3"])
+        subprocess.check_call([python_exe, "-m", "pip", "uninstall", "botocore", "-y", "--quiet"])
         subprocess.check_call(
-            [sys.executable, "-m", "pip", "uninstall", "botocore", "-y", "--quiet"]
+            [python_exe, "-m", "pip", "install", "git+https://github.com/qBraid/botocore.git"]
         )
-        subprocess.check_call(
-            [sys.executable, "-m", "pip", "install", "git+https://github.com/qBraid/botocore.git"]
-        )
-    except subprocess.CalledProcessError:
+    except (subprocess.CalledProcessError, FileNotFoundError):
         handle_error(message="Failed to enable qBraid quantum jobs.")
 
     typer.secho("\nSuccessfully enabled qBraid quantum jobs.", fg=typer.colors.GREEN, bold=True)
     typer.secho("\nTo disable, run: \n\n\t$ qbraid jobs disable braket\n")
 
 
 def disable_braket(auto_confirm: bool = False):
     """Disable qBraid quantum jobs for Amazon Braket."""
     package = "botocore"
-    installed, latest, path = run_progress_task(
+    installed, latest, path, python_exe = run_progress_task(
         get_package_data, package, description="Solving environment..."
     )
     package = f"{package}~={installed}" if installed < latest else package
 
     if not auto_confirm:
         confirm_updates("disable", path)
+    typer.echo("")
 
     try:
         subprocess.check_call(
             [
-                sys.executable,
+                python_exe,
                 "-m",
                 "pip",
                 "install",
                 package,
                 "--force-reinstall",
             ],
             stderr=subprocess.DEVNULL,
         )
-    except subprocess.CalledProcessError:
+    except (subprocess.CalledProcessError, FileNotFoundError):
         handle_error(message="Failed to disable qBraid quantum jobs.")
 
     typer.secho("\nSuccessfully disabled qBraid quantum jobs.", fg=typer.colors.GREEN, bold=True)
     typer.secho("\nTo enable, run: \n\n\t$ qbraid jobs enable braket\n")
```

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/jobs/validation.py` & `qbraid_cli-0.8.dev4/qbraid_cli/jobs/validation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Module for validating command arguments for qBraid Quantum Jobs.
 
 """
-
-from typing import Callable, Dict, Optional, Tuple
+import sys
+from typing import Any, Callable, Dict, Optional, Tuple
 
 import typer
-from qbraid_core.services.quantum.proxy import SUPPORTED_QJOB_LIBS, quantum_lib_proxy_state
 from rich.console import Console
 
 from qbraid_cli.handlers import handle_error, run_progress_task, validate_item
 
+LEGACY_ARGS: Dict[str, str] = {
+    "amazon_braket": "braket",
+    "aws_braket": "braket",
+}
+
 
 def validate_library(value: str) -> str:
     """Validate quantum jobs library."""
-    return validate_item(value, SUPPORTED_QJOB_LIBS, "Library")
+    # pylint:disable-next=import-outside-toplevel
+    from qbraid_core.services.quantum.proxy import SUPPORTED_QJOB_LIBS
+
+    qjobs_libs = list(SUPPORTED_QJOB_LIBS.keys())
 
+    if value in LEGACY_ARGS:
+        old_value = value
+        value = LEGACY_ARGS[value]
 
-def get_state(library: Optional[str] = None) -> Dict[str, Tuple[bool, bool]]:
+        console = Console()
+        console.print(
+            f"[red]DeprecationWarning:[/red] Argument '{old_value}' "
+            f"is deprecated. Use '{value}' instead.\n"
+        )
+
+    return validate_item(value, qjobs_libs, "Library")
+
+
+def get_state(library: Optional[str] = None) -> Tuple[str, Dict[str, Tuple[bool, bool]]]:
     """Get the state of qBraid Quantum Jobs for the specified library."""
+    from qbraid_core.services.quantum import QuantumClient
 
-    state_values = {}
+    jobs_state = QuantumClient.qbraid_jobs_state(device_lib=library)
 
-    if library:
-        libraries_to_check = [library]
-    else:
-        libraries_to_check = SUPPORTED_QJOB_LIBS
+    python_exe: str = jobs_state.get("exe", sys.executable)
+    libs_state: Dict[str, Any] = jobs_state.get("libs", {})
 
-    for lib in libraries_to_check:
-        state = quantum_lib_proxy_state(lib)
-        state_values[lib] = state["supported"], state["enabled"]
+    state_values = {
+        lib: (state["supported"], state["enabled"]) for lib, state in libs_state.items()
+    }
 
-    return state_values
+    return python_exe, state_values
 
 
-def run_progress_get_state(library: Optional[str] = None) -> Dict[str, Tuple[bool, bool]]:
+def run_progress_get_state(
+    library: Optional[str] = None,
+) -> Tuple[str, Dict[str, Tuple[bool, bool]]]:
     """Run get state function with rich progress UI."""
     return run_progress_task(
         get_state,
         library,
         description="Collecting package metadata...",
         error_message=f"Failed to collect {library} package metadata.",
     )
@@ -49,26 +69,25 @@
 
 def handle_jobs_state(
     library: str,
     action: str,  # 'enable' or 'disable'
     action_callback: Callable[[], None],
 ) -> None:
     """Handle the common logic for enabling or disabling qBraid Quantum Jobs."""
-    state_values: Dict[str, Tuple[bool, bool]] = run_progress_get_state(library)
+    _, state_values = run_progress_get_state(library)
     installed, enabled = state_values[library]
 
     if not installed:
-        handle_error(message=f"{library} not installed.")
+        handle_error(
+            message=f"{library} not installed."
+        )  # TODO: Provide command to install library?
     if (enabled and action == "enable") or (not enabled and action == "disable"):
         action_color = "green" if enabled else "red"
         console = Console()
         console.print(
             f"\nqBraid quantum jobs already [bold {action_color}]{action}d[/bold {action_color}] "
-            f"for [magenta]{library}[/magenta]."
-        )
-        console.print(
-            "To check the state of all quantum jobs libraries in this environment, "
-            "use: \n\n\t$ qbraid jobs state\n"
+            f"for [magenta]{library}[/magenta].\n\nCheck the state of all quantum jobs "
+            "libraries in this environment with: \n\n\t$ qbraid jobs state\n"
         )
         raise typer.Exit()
 
     action_callback()  # Perform the specific enable/disable action
```

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/kernels/app.py` & `qbraid_cli-0.8.dev4/qbraid_cli/kernels/app.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli/main.py` & `qbraid_cli-0.8.dev4/qbraid_cli/main.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/PKG-INFO` & `qbraid_cli-0.8.dev4/qbraid_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev3
+Version: 0.8.0.dev4
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -25,28 +25,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.12.1
 Requires-Dist: rich>=10.11.0
 Requires-Dist: jupyter_client<9.0.0,>=7.0.0
-Requires-Dist: qbraid-core>=0.1.1
+Requires-Dist: qbraid-core>=0.1.2
 Provides-Extra: jobs
 Requires-Dist: amazon-braket-sdk>=1.48.1; extra == "jobs"
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
 Requires-Dist: sphinx-rtd-theme<2.1,>=1.3; extra == "docs"
 Requires-Dist: docutils<0.21; extra == "docs"
 Requires-Dist: toml; extra == "docs"
 Requires-Dist: build; extra == "docs"
+Requires-Dist: m2r; extra == "docs"
+Requires-Dist: typer; extra == "docs"
 
 <img width="full" alt="qbraid_cli" src="https://qbraid-static.s3.amazonaws.com/logos/qbraid-cli-banner.png">
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html)
 [![PyPI version](https://img.shields.io/pypi/v/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Python verions](https://img.shields.io/pypi/pyversions/qbraid-cli.svg?color=blue)](https://pypi.org/project/qbraid-cli/)
 [![Downloads](https://static.pepy.tech/badge/qbraid-cli)](https://pepy.tech/project/qbraid-cli)
```

### Comparing `qbraid-cli-0.8.0.dev3/qbraid_cli.egg-info/SOURCES.txt` & `qbraid_cli-0.8.dev4/qbraid_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_configure/test_configure_set.py` & `qbraid_cli-0.8.dev4/tests/test_configure/test_configure_set.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_configure/test_prompt_for_config.py` & `qbraid_cli-0.8.dev4/tests/test_configure/test_prompt_for_config.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_configure/test_validate_input.py` & `qbraid_cli-0.8.dev4/tests/test_configure/test_validate_input.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_credits/test_credits_value.py` & `qbraid_cli-0.8.dev4/tests/test_credits/test_credits_value.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_devices/test_devices_list.py` & `qbraid_cli-0.8.dev4/tests/test_devices/test_devices_list.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_devices/test_validations.py` & `qbraid_cli-0.8.dev4/tests/test_devices/test_validations.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_activate_pyenv.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_activate_pyenv.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_find_shell_rc.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_find_shell_rc.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_activate/test_print_activate_command.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_activate/test_print_activate_command.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_activate.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_activate.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_create.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_create.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_list.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_app/test_envs_remove.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_app/test_envs_remove.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_create_qbraid_env_assets.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_create_qbraid_env_assets.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_replace_str.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_replace_str.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_create/test_update_state_json.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_create/test_update_state_json.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_installed_envs_data.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_installed_envs_data.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_is_valid_env_name.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_is_valid_env_name.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_request_delete_env.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_request_delete_env.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_envs/test_data_handling/test_validate_env_name.py` & `qbraid_cli-0.8.dev4/tests/test_envs/test_data_handling/test_validate_env_name.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_disable.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_disable.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 import pytest
 import typer
 from qbraid_core.services.quantum.proxy import SUPPORTED_QJOB_LIBS
 
 from qbraid_cli.jobs.app import jobs_disable
 
+qjob_libs = list(SUPPORTED_QJOB_LIBS.keys())
 
-@pytest.mark.parametrize("library", SUPPORTED_QJOB_LIBS)
+
+@pytest.mark.parametrize("library", qjob_libs)
 def test_library_validation_on_disable(library):
     """Test library validation function during the jobs disable command."""
     with (
         patch(
             "qbraid_cli.jobs.validation.validate_library", return_value=library
         ) as mock_validate_library,
         patch("typer.confirm", return_value=True),
@@ -31,15 +33,15 @@
 
 def test_error_for_unsupported_library_on_disable():
     """Test that an error is raised for an unsupported library during the jobs disable command."""
     with pytest.raises(typer.Exit):
         jobs_disable(library="unsupported_library")
 
 
-@pytest.mark.parametrize("library", SUPPORTED_QJOB_LIBS)
+@pytest.mark.parametrize("library", qjob_libs)
 def test_handle_jobs_state_integration_on_disable(library):
     """Test the handle_jobs_state function during the jobs disable command."""
     with (
         patch(f"qbraid_cli.jobs.toggle_{library}.disable_{library}"),
         patch("qbraid_cli.jobs.validation.handle_jobs_state") as mock_handle_jobs_state,
     ):
         with pytest.raises(typer.Exit):
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_enable.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_enable.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,33 @@
 
 import pytest
 import typer
 from qbraid_core.services.quantum.proxy import SUPPORTED_QJOB_LIBS
 
 from qbraid_cli.jobs.app import jobs_enable
 
+qjobs_libs = list(SUPPORTED_QJOB_LIBS.keys())
 
-@pytest.mark.parametrize("library", SUPPORTED_QJOB_LIBS)
+
+@pytest.mark.parametrize("library", qjobs_libs)
 def test_library_validation(library):
     """Test library validation function during the jobs enable command."""
     with (
         patch(f"qbraid_cli.jobs.toggle_{library}.enable_{library}") as mock_enable_library,
         patch("qbraid_cli.jobs.validation.validate_library") as mock_validate_library,
     ):
         # Assume `validate_library` callback returns True for simplicity
         mock_enable_library.return_value = None
         mock_validate_library.return_value = True
         with pytest.raises(typer.Exit):
             jobs_enable(library=library)
             mock_validate_library.assert_called_once_with(library)
 
 
-@pytest.mark.parametrize("library", SUPPORTED_QJOB_LIBS)
+@pytest.mark.parametrize("library", qjobs_libs)
 def test_enable_action_for_supported_library(library):
     """Test the enable action for supported libraries."""
     if importlib.util.find_spec(library) is None:
         with pytest.raises(typer.Exit):
             jobs_enable(library=library)
     else:
         with patch(f"qbraid_cli.jobs.toggle_{library}.enable_{library}") as mock_enable_library:
@@ -46,15 +48,15 @@
 
 def test_raise_error_for_unsupported_library():
     """Test that an error is raised for an unsupported library during the jobs enable command."""
     with pytest.raises(typer.Exit):
         jobs_enable(library="unsupported_library")
 
 
-@pytest.mark.parametrize("library", SUPPORTED_QJOB_LIBS)
+@pytest.mark.parametrize("library", qjobs_libs)
 def test_handle_jobs_state_integration(library):
     """Test the handle_jobs_state function during the jobs enable command."""
     with (
         patch("typer.confirm") as mock_confirm,
         patch(f"qbraid_cli.jobs.toggle_{library}.enable_{library}") as mock_enable_library,
         patch("qbraid_cli.jobs.validation.handle_jobs_state") as mock_handle_jobs_state,
     ):
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_list.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_app/test_jobs_state.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_app/test_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_aws_configure_dummy.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_confirm_updates.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_confirm_updates.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_disable_braket.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_disable_braket.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """
 Unit tests for the disable_braket function in the toggle_braket module.
 
 """
 
 import subprocess
-import sys
 from unittest.mock import patch
 
 import pytest
 import typer
 
 from qbraid_cli.jobs.toggle_braket import disable_braket
 
@@ -20,15 +19,15 @@
     """
     Tests that `get_package_data` and `confirm_updates` helper functions are called with
     the correct arguments when `disable_braket` is executed.
     """
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.1.0", "/some/path"),
+            return_value=("1.0.0", "1.1.0", "/some/path", "/usr/bin/python"),
         ) as mock_get_package_data_disable,
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates") as mock_confirm_updates,
     ):
         # Assume successful subprocess call
         with patch("subprocess.check_call"):
             disable_braket()
 
@@ -40,24 +39,24 @@
     """
     Tests that the correct package version is specified for reinstallation during the
     `disable_braket` function execution.
     """
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.1.0", "/some/path"),
+            return_value=("1.0.0", "1.1.0", "/some/path", "/usr/bin/python"),
         ),
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates"),
         patch("subprocess.check_call") as mock_check_call,
     ):
         disable_braket()
 
         mock_check_call.assert_called_with(
             [
-                sys.executable,
+                "/usr/bin/python",
                 "-m",
                 "pip",
                 "install",
                 "botocore~=1.0.0",  # The version is specified because installed < latest
                 "--force-reinstall",
             ],
             stderr=subprocess.DEVNULL,
@@ -68,30 +67,30 @@
     """
     Tests if `disable_braket` correctly handles subprocess execution for package reinstallation
     and raises the typer.Exit when a subprocess call fails.
     """
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.0.0", "/some/path"),
+            return_value=("1.0.0", "1.0.0", "/some/path", "/usr/bin/python"),
         ),
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates"),
         patch("subprocess.check_call", side_effect=subprocess.CalledProcessError(1, "cmd")),
         patch("qbraid_cli.handlers.handle_error"),
     ):
         with pytest.raises(typer.Exit):
             disable_braket()
 
 
 def test_success_message_displayed():
     """Tests if correct success messages are displayed to the user."""
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.0.0", "/some/path"),
+            return_value=("1.0.0", "1.0.0", "/some/path", "/usr/bin/python"),
         ),
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates"),
         patch("subprocess.check_call"),
         patch("typer.secho") as mock_secho,
     ):
         disable_braket()
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_enable_braket.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_enable_braket.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,61 +3,62 @@
 
 """
 Unit tests for the enable_braket function in the toggle_braket module.
 
 """
 
 import subprocess
-import sys
 from unittest.mock import call, patch
 
 import pytest
 import typer
 
 from qbraid_cli.jobs.toggle_braket import enable_braket
 
 
 def test_helper_function_invocations():
     """Test that `enable_braket` correctly calls its helper functions."""
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.2.0", "/some/path"),
+            return_value=("1.0.0", "1.2.0", "/some/path", "/usr/bin/python"),
         ) as mock_get_package_data,
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates") as mock_confirm_updates,
         patch("qbraid_cli.jobs.toggle_braket.aws_configure_dummy") as mock_aws_configure_dummy,
     ):
         with patch("subprocess.check_call"):
             enable_braket()
 
         mock_get_package_data.assert_called_once_with("boto3")
         mock_confirm_updates.assert_called()
         mock_aws_configure_dummy.assert_called_once()
 
 
 def test_subprocess_calls():
     """Test the subprocess calls within `enable_braket`."""
+    mock_python_path = "/usr/bin/python"
+
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.2.0", "/some/path"),
+            return_value=("1.0.0", "1.2.0", "/some/path", mock_python_path),
         ),
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates"),
         patch("qbraid_cli.jobs.toggle_braket.aws_configure_dummy"),
         patch("subprocess.check_call") as mock_check_call,
     ):
         enable_braket()
 
         # Expected subprocess calls in order
         expected_calls = [
-            call([sys.executable, "-m", "pip", "install", "--upgrade", "boto3"]),
-            call([sys.executable, "-m", "pip", "uninstall", "botocore", "-y", "--quiet"]),
+            call([mock_python_path, "-m", "pip", "install", "--upgrade", "boto3"]),
+            call([mock_python_path, "-m", "pip", "uninstall", "botocore", "-y", "--quiet"]),
             call(
                 [
-                    sys.executable,
+                    mock_python_path,
                     "-m",
                     "pip",
                     "install",
                     "git+https://github.com/qBraid/botocore.git",
                 ]
             ),
         ]
@@ -65,15 +66,15 @@
 
 
 def test_subprocess_error_handling():
     """ "Test if the program exits correctly using typer.Exit"""
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.2.0", "/some/path"),
+            return_value=("1.0.0", "1.2.0", "/some/path", "/usr/bin/python"),
         ),
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates"),
         patch("qbraid_cli.jobs.toggle_braket.aws_configure_dummy"),
         patch(
             "subprocess.check_call",
             side_effect=subprocess.CalledProcessError(returncode=1, cmd="cmd"),
         ),
@@ -83,15 +84,15 @@
 
 
 def test_success_feedback():
     """Test feedback for successful execution"""
     with (
         patch(
             "qbraid_cli.jobs.toggle_braket.get_package_data",
-            return_value=("1.0.0", "1.2.0", "/some/path"),
+            return_value=("1.0.0", "1.2.0", "/some/path", "/usr/bin/python"),
         ),
         patch("qbraid_cli.jobs.toggle_braket.confirm_updates"),
         patch("qbraid_cli.jobs.toggle_braket.aws_configure_dummy"),
         patch("subprocess.check_call"),
         patch("typer.secho") as mock_secho,
     ):
         enable_braket()
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_toggle_braket/test_get_package_data.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_toggle_braket/test_get_package_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,143 +19,167 @@
     Verify that the function returns the correct tuple of installed version,
     latest version, and site-packages path for a known package.
     """
     package_name = "example_package"
     expected_installed_version = "1.0.0"
     expected_latest_version = "1.0.1"
     expected_site_packages_path = "/usr/local/lib/python3.9/site-packages"
+    expected_python_exe = "/usr/local/bin/python"
 
     with (
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_local_package_version",
+            "qbraid_core.system.get_local_package_version",
             return_value=expected_installed_version,
         ),
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_latest_package_version",
+            "qbraid_core.system.get_latest_package_version",
             return_value=expected_latest_version,
         ),
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_active_site_packages_path",
+            "qbraid_core.system.get_active_site_packages_path",
             return_value=expected_site_packages_path,
         ),
+        patch(
+            "qbraid_core.system.get_active_python_path",
+            return_value=expected_python_exe,
+        ),
     ):
-        installed_version, latest_version, site_packages_path = get_package_data(package_name)
+        installed_version, latest_version, site_packages_path, python_exe = get_package_data(
+            package_name
+        )
 
         assert installed_version == expected_installed_version
         assert latest_version == expected_latest_version
         assert site_packages_path == expected_site_packages_path
+        assert python_exe == expected_python_exe
 
 
 def test_error_during_local_version_retrieval():
     """
     Ensure the function raises a QbraidException when either get_local_package_version or
     get_latest_package_version fails.
     """
     package_name = "faulty_package"
     with (
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_local_package_version",
+            "qbraid_core.system.get_local_package_version",
             side_effect=QbraidSystemError("Error"),
         ),
-        patch("qbraid_cli.jobs.toggle_braket.get_latest_package_version") as mock_latest_version,
+        patch("qbraid_core.system.get_latest_package_version") as mock_latest_version,
     ):
         mock_latest_version.return_value = (
             "1.0.1"  # This won't be reached but is set for completeness
         )
         with pytest.raises(QbraidException) as exc_info:
             get_package_data(package_name)
-        assert "Failed to retrieve package version information" in str(exc_info.value)
+        assert "Failed to retrieve required system and/or package metadata" in str(exc_info.value)
 
 
 def test_error_during_latest_version_retrieval():
     """
     Check if the function correctly raises a QbraidException
     when get_active_site_packages_path fails.
     """
     package_name = "faulty_package"
     with (
-        patch("qbraid_cli.jobs.toggle_braket.get_local_package_version") as mock_local_version,
+        patch("qbraid_core.system.get_local_package_version") as mock_local_version,
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_latest_package_version",
+            "qbraid_core.system.get_latest_package_version",
             side_effect=QbraidSystemError("Error"),
         ),
     ):
         mock_local_version.return_value = "1.0.0"  # This is expected to be successful
         with pytest.raises(QbraidException) as exc_info:
             get_package_data(package_name)
-        assert "Failed to retrieve package version information" in str(exc_info.value)
+        assert "Failed to retrieve required system and/or package metadata" in str(exc_info.value)
 
 
 def test_non_existent_package():
     """
     Confirm that the function behaves as expected
     (either by returning versions as None or raising an exception),
     when a non-existent package is queried.
     """
     package_name = "imaginary_package"
-    expected_installed_version = (
-        None  # Assuming the function returns None for non-existent packages
-    )
+    expected_installed_version = None
     expected_latest_version = None
-    expected_site_packages_path = (
-        "/usr/local/lib/python3.10/site-packages"  # This should still be retrievable
-    )
+    expected_site_packages_path = "/usr/local/lib/python3.10/site-packages"
+    expected_python_exe = "/usr/local/bin/python"
 
     with (
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_local_package_version",
+            "qbraid_core.system.get_local_package_version",
             return_value=expected_installed_version,
         ),
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_latest_package_version",
+            "qbraid_core.system.get_latest_package_version",
             return_value=expected_latest_version,
         ),
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_active_site_packages_path",
+            "qbraid_core.system.get_active_site_packages_path",
             return_value=expected_site_packages_path,
         ),
+        patch(
+            "qbraid_core.system.get_active_python_path",
+            return_value=expected_python_exe,
+        ),
     ):
-        installed_version, latest_version, site_packages_path = get_package_data(package_name)
+        installed_version, latest_version, site_packages_path, python_exe = get_package_data(
+            package_name
+        )
 
         assert (
             installed_version == expected_installed_version
         ), "Installed version should be None for a non-existent package"
         assert (
             latest_version == expected_latest_version
         ), "Latest version should be None for a non-existent package"
         assert (
             site_packages_path == expected_site_packages_path
         ), "The site-packages path should still be retrievable"
+        assert (
+            python_exe == expected_python_exe
+        ), "The python executable should still be retrievable"
 
 
 def test_package_no_updates_available():
     """Verify the function correctly identifies when the installed version is the latest."""
     package_name = "up_to_date_package"
     expected_installed_version = "1.0.1"
     expected_latest_version = "1.0.1"  # Installed version is the latest
     expected_site_packages_path = "/usr/local/lib/python3.10/site-packages"
+    expected_python_exe = "/usr/local/bin/python"
 
     with (
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_local_package_version",
+            "qbraid_core.system.get_local_package_version",
             return_value=expected_installed_version,
         ),
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_latest_package_version",
+            "qbraid_core.system.get_latest_package_version",
             return_value=expected_latest_version,
         ),
         patch(
-            "qbraid_cli.jobs.toggle_braket.get_active_site_packages_path",
+            "qbraid_core.system.get_active_site_packages_path",
             return_value=expected_site_packages_path,
         ),
+        patch(
+            "qbraid_core.system.get_active_python_path",
+            return_value=expected_python_exe,
+        ),
     ):
-        installed_version, latest_version, site_packages_path = get_package_data(package_name)
+        installed_version, latest_version, site_packages_path, python_exe = get_package_data(
+            package_name
+        )
 
         assert (
             installed_version == expected_installed_version
         ), "Installed version should match the expected version"
         assert (
             latest_version == expected_latest_version
         ), "Latest version should match the installed version indicating no updates"
         assert (
             site_packages_path == expected_site_packages_path
         ), "The site-packages path should be correctly retrieved"
+        assert (
+            python_exe == expected_python_exe
+        ), "The python executable should still be retrievable"
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_get_state.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_get_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,38 +9,54 @@
 from unittest.mock import patch
 
 import pytest
 
 from qbraid_cli.jobs.validation import get_state
 
 
-@patch("qbraid_cli.jobs.validation.quantum_lib_proxy_state")
+@patch("qbraid_core.services.quantum.QuantumClient.qbraid_jobs_state")
 def test_get_state_specific_library(mock_qbraid_jobs_state):
     """Test the get_state function for a specific library."""
+    library = "braket"
+    python_exe = "/usr/bin/python"
+    supported, enabled = True, False
     mock_qbraid_jobs_state.return_value = {
-        "proxy_lib": "botocore",
-        "supported": True,
-        "enabled": False,
+        "exe": python_exe,
+        "libs": {
+            library: {
+                "supported": supported,
+                "enabled": enabled,
+            }
+        },
     }
-    library = "braket"
-    expected = {library: (True, False)}
-
     result = get_state(library)
-    mock_qbraid_jobs_state.assert_called_once_with(library)
+    expected = (python_exe, {library: (supported, enabled)})
+    mock_qbraid_jobs_state.assert_called_once_with(device_lib=library)
     assert result == expected, f"Expected state for {library} to be correctly returned"
 
 
 @pytest.mark.parametrize(
     "library,mock_return,expected",
     [
-        ("braket", {"proxy_lib": "botocore", "supported": True, "enabled": False}, (True, False)),
-        ("test", {"proxy_lib": "other", "supported": False, "enabled": False}, (False, False)),
+        (
+            "braket",
+            {"exe": "/usr/bin/python", "libs": {"braket": {"supported": True, "enabled": False}}},
+            (True, False),
+        ),
+        (
+            "test",
+            {"exe": "/usr/bin/python", "libs": {"test": {"supported": False, "enabled": False}}},
+            (False, False),
+        ),
     ],
 )
-@patch("qbraid_cli.jobs.validation.quantum_lib_proxy_state")
+@patch("qbraid_core.services.quantum.QuantumClient.qbraid_jobs_state")
 def test_get_state_multiple_libraries(mock_qbraid_jobs_state, library, mock_return, expected):
     """Test the get_state function when there are multiple libraries."""
     mock_qbraid_jobs_state.return_value = mock_return
 
     result = get_state(library)
-    mock_qbraid_jobs_state.assert_called_once_with(library)
-    assert result == {library: expected}, f"Expected state for {library} to be correctly returned"
+    mock_qbraid_jobs_state.assert_called_once_with(device_lib=library)
+    assert result == (
+        "/usr/bin/python",
+        {library: expected},
+    ), f"Expected state for {library} to be correctly returned"
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_handle_jobs_state.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_handle_jobs_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,46 +13,49 @@
 
 from qbraid_cli.jobs.validation import handle_jobs_state
 
 
 def test_handle_jobs_state_not_installed():
     """Test handle_jobs_state when the library is not installed."""
     with patch(
-        "qbraid_cli.jobs.validation.run_progress_get_state", return_value={"braket": (False, False)}
+        "qbraid_cli.jobs.validation.run_progress_get_state",
+        return_value=("/usr/local/bin/python", {"braket": (False, False)}),
     ):
 
         action_callback = MagicMock()
 
         with pytest.raises(typer.Exit):
 
             assert "Error" in handle_jobs_state("braket", "enable", action_callback).output
 
 
 @patch("rich.console.Console.print")
 def test_handle_jobs_state_already_correct_state(mock_console_print):
     """Test handle_jobs_state when the library is already in the correct state."""
 
     with patch(
-        "qbraid_cli.jobs.validation.run_progress_get_state", return_value={"braket": (True, True)}
+        "qbraid_cli.jobs.validation.run_progress_get_state",
+        return_value=("/usr/local/bin/python", {"braket": (True, True)}),
     ):
 
         action_callback = MagicMock()
 
         with pytest.raises(typer.Exit):
             handle_jobs_state("braket", "enable", action_callback)
 
         # Verify console.print is called with the expected messages
-        assert mock_console_print.call_count == 2
+        assert mock_console_print.call_count == 1
         action_callback.assert_not_called()
 
 
 def test_handle_jobs_state_action_needed():
     """Test handle_jobs_state when the library is not in the correct state."""
     with patch(
-        "qbraid_cli.jobs.validation.run_progress_get_state", return_value={"braket": (True, False)}
+        "qbraid_cli.jobs.validation.run_progress_get_state",
+        return_value=("/usr/local/bin/python", {"braket": (True, False)}),
     ):
 
         action_callback = MagicMock()
 
         with patch("rich.console.Console.print") as mock_console_print:
             handle_jobs_state("braket", "enable", action_callback)
```

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_run_progress_get_state.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_run_progress_get_state.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_jobs/test_validation/test_validate_library.py` & `qbraid_cli-0.8.dev4/tests/test_jobs/test_validation/test_validate_library.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tests/test_kernels/test_kernels_list.py` & `qbraid_cli-0.8.dev4/tests/test_kernels/test_kernels_list.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tools/split_rst.py` & `qbraid_cli-0.8.dev4/tools/split_rst.py`

 * *Files identical despite different names*

### Comparing `qbraid-cli-0.8.0.dev3/tools/verify_headers.py` & `qbraid_cli-0.8.dev4/tools/verify_headers.py`

 * *Files identical despite different names*

