# Comparing `tmp/pyproject_installer-0.5.2.tar.gz` & `tmp/pyproject_installer-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_installer-0.5.2.tar", last modified: Tue Jul 11 08:42:22 2023, max compression
+gzip compressed data, was "pyproject_installer-0.5.3.tar", last modified: Fri Apr 12 09:38:57 2024, max compression
```

## Comparing `pyproject_installer-0.5.2.tar` & `pyproject_installer-0.5.3.tar`

### file list

```diff
@@ -1,90 +1,91 @@
--rw-r--r--   0        0        0       78 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/__init__.py
--rw-r--r--   0        0        0    16053 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/__main__.py
--rw-r--r--   0        0        0      317 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/codes.py
--rw-r--r--   0        0        0      391 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/errors.py
--rw-r--r--   0        0        0       18 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/version.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/__init__.py
--rw-r--r--   0        0        0      501 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8926 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10194 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    16397 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0     3287 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39206 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18106 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16326 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/version.py
--rw-r--r--   0        0        0      396 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      172 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/build_cmd/__init__.py
--rw-r--r--   0        0        0     4477 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/build_cmd/_build.py
--rw-r--r--   0        0        0      206 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/__init__.py
--rw-r--r--   0        0        0      181 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/_deps_command.py
--rw-r--r--   0        0        0     9272 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/deps_config.py
--rw-r--r--   0        0        0      728 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/__init__.py
--rw-r--r--   0        0        0      190 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/collector.py
--rw-r--r--   0        0        0     2358 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/hatch.py
--rw-r--r--   0        0        0     1306 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/metadata.py
--rw-r--r--   0        0        0     1361 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pdm.py
--rw-r--r--   0        0        0      825 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep517.py
--rw-r--r--   0        0        0      679 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep518.py
--rw-r--r--   0        0        0     1062 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
--rw-r--r--   0        0        0     2481 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/poetry.py
--rw-r--r--   0        0        0     2239 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/tox.py
--rw-r--r--   0        0        0       73 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/install_cmd/__init__.py
--rw-r--r--   0        0        0     6215 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/install_cmd/_install.py
--rw-r--r--   0        0        0      270 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/__init__.py
--rw-r--r--   0        0        0     9335 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/build_backend.py
--rw-r--r--   0        0        0      913 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/entry_points.py
--rw-r--r--   0        0        0      193 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/normalization.py
--rw-r--r--   0        0        0     1811 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/scripts.py
--rw-r--r--   0        0        0    10893 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/wheel.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/backend_helper/__init__.py
--rw-r--r--   0        0        0     5872 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/lib/backend_helper/backend_caller.py
--rw-r--r--   0        0        0       65 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/__init__.py
--rw-r--r--   0        0        0      430 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/_run_command.py
--rw-r--r--   0        0        0     7104 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/_run_env.py
--rw-r--r--   0        0        0      172 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/__init__.py
--rw-r--r--   0        0        0      367 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/common.py
--rw-r--r--   0        0        0     2092 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/config.py
--rw-r--r--   0        0        0     8581 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/metadata.py
--rw-r--r--   0        0        0     5559 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/sdist.py
--rw-r--r--   0        0        0     6922 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/wheel.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      396 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     7856 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     5082 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     4144 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/test_backends.py
--rw-r--r--   0        0        0     1719 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/test_buildable.py
--rw-r--r--   0        0        0     2238 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/integration/test_config_settings.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/__init__.py
--rw-r--r--   0        0        0    31635 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_main.py
--rw-r--r--   0        0        0       92 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_version.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/__init__.py
--rw-r--r--   0        0        0      509 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/conftest.py
--rw-r--r--   0        0        0    15784 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/test_backend_caller.py
--rw-r--r--   0        0        0    12189 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/test_builder.py
--rw-r--r--   0        0        0     8179 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_build/test_pyproject_parser.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/__init__.py
--rw-r--r--   0        0        0      495 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/conftest.py
--rw-r--r--   0        0        0    30288 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/test_collectors.py
--rw-r--r--   0        0        0    25247 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_deps/test_deps_config.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_install/__init__.py
--rw-r--r--   0        0        0    17931 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_install/test_installer.py
--rw-r--r--   0        0        0        0 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_run/__init__.py
--rw-r--r--   0        0        0    18875 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/tests/unit/test_run/test_env.py
--rw-r--r--   0        0        0    17234 2023-07-11 08:42:22.000000 pyproject_installer-0.5.2/PKG-INFO
--rw-r--r--   0        0        0     3464 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/pyproject.toml
--rw-r--r--   0        0        0    16282 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/README.md
--rw-r--r--   0        0        0     1024 2023-07-11 08:41:33.000000 pyproject_installer-0.5.2/LICENSE
+-rw-r--r--   0        0        0       78 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/__init__.py
+-rw-r--r--   0        0        0    16054 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/__main__.py
+-rw-r--r--   0        0        0      317 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/codes.py
+-rw-r--r--   0        0        0      391 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/errors.py
+-rw-r--r--   0        0        0       18 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/version.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/__init__.py
+-rw-r--r--   0        0        0      496 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0     2933 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39784 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16236 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      172 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/build_cmd/__init__.py
+-rw-r--r--   0        0        0     4471 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/build_cmd/_build.py
+-rw-r--r--   0        0        0      206 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/_deps_command.py
+-rw-r--r--   0        0        0     9272 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/deps_config.py
+-rw-r--r--   0        0        0      789 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/collector.py
+-rw-r--r--   0        0        0     2358 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/hatch.py
+-rw-r--r--   0        0        0     1306 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/metadata.py
+-rw-r--r--   0        0        0     1361 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pdm.py
+-rw-r--r--   0        0        0      825 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pep517.py
+-rw-r--r--   0        0        0      679 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pep518.py
+-rw-r--r--   0        0        0     1062 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
+-rw-r--r--   0        0        0     1685 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pipenv.py
+-rw-r--r--   0        0        0     2481 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/poetry.py
+-rw-r--r--   0        0        0     2239 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/tox.py
+-rw-r--r--   0        0        0       73 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/install_cmd/__init__.py
+-rw-r--r--   0        0        0     6266 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/install_cmd/_install.py
+-rw-r--r--   0        0        0      181 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/__init__.py
+-rw-r--r--   0        0        0     9335 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/build_backend.py
+-rw-r--r--   0        0        0      913 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/entry_points.py
+-rw-r--r--   0        0        0      193 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/normalization.py
+-rw-r--r--   0        0        0     1811 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/scripts.py
+-rw-r--r--   0        0        0    10893 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/wheel.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/backend_helper/__init__.py
+-rw-r--r--   0        0        0     5873 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/lib/backend_helper/backend_caller.py
+-rw-r--r--   0        0        0       65 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/run_cmd/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/run_cmd/_run_command.py
+-rw-r--r--   0        0        0     7104 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/src/pyproject_installer/run_cmd/_run_env.py
+-rw-r--r--   0        0        0      173 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/common.py
+-rw-r--r--   0        0        0     2092 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/config.py
+-rw-r--r--   0        0        0     8581 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/metadata.py
+-rw-r--r--   0        0        0     5560 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/sdist.py
+-rw-r--r--   0        0        0     6923 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/wheel.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      396 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/__init__.py
+-rw-r--r--   0        0        0     7970 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5086 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4144 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/integration/test_backends.py
+-rw-r--r--   0        0        0     1720 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/integration/test_buildable.py
+-rw-r--r--   0        0        0     2236 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/integration/test_config_settings.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0    31857 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_main.py
+-rw-r--r--   0        0        0       92 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_version.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_build/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_build/conftest.py
+-rw-r--r--   0        0        0    16003 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_build/test_backend_caller.py
+-rw-r--r--   0        0        0    12359 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_build/test_builder.py
+-rw-r--r--   0        0        0     8180 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_build/test_pyproject_parser.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_deps/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_deps/conftest.py
+-rw-r--r--   0        0        0    33331 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_deps/test_collectors.py
+-rw-r--r--   0        0        0    25247 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_deps/test_deps_config.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_install/__init__.py
+-rw-r--r--   0        0        0    19647 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_install/test_installer.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_run/__init__.py
+-rw-r--r--   0        0        0    18943 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/tests/unit/test_run/test_env.py
+-rw-r--r--   0        0        0    17436 2024-04-12 09:38:57.000000 pyproject_installer-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     3510 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    16433 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/README.md
+-rw-r--r--   0        0        0     1024 2024-04-12 09:38:35.000000 pyproject_installer-0.5.3/LICENSE
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/__main__.py` & `pyproject_installer-0.5.3/src/pyproject_installer/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     - editable builds(PEP660) are not supported
 
 Install features:
     - install without bytecompilation
     - RECORD is dropped (PEP627)
     - signature verification of signed wheel is not supported
 """
+
 from pathlib import Path
 import argparse
 import json
 import logging
 import sys
 
 from . import __version__ as project_version
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_elffile.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_manylinux.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_manylinux.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import collections
 import contextlib
 import functools
 import os
 import re
 import sys
 import warnings
-from typing import Dict, Generator, Iterator, NamedTuple, Optional, Tuple
+from typing import Dict, Generator, Iterator, NamedTuple, Optional, Sequence, Tuple
 
 from ._elffile import EIClass, EIData, ELFFile, EMachine
 
 EF_ARM_ABIMASK = 0xFF000000
 EF_ARM_ABI_VER5 = 0x05000000
 EF_ARM_ABI_FLOAT_HARD = 0x00000400
 
@@ -46,20 +46,29 @@
             f is not None
             and f.capacity == EIClass.C32
             and f.encoding == EIData.Lsb
             and f.machine == EMachine.I386
         )
 
 
-def _have_compatible_abi(executable: str, arch: str) -> bool:
-    if arch == "armv7l":
+def _have_compatible_abi(executable: str, archs: Sequence[str]) -> bool:
+    if "armv7l" in archs:
         return _is_linux_armhf(executable)
-    if arch == "i686":
+    if "i686" in archs:
         return _is_linux_i686(executable)
-    return arch in {"x86_64", "aarch64", "ppc64", "ppc64le", "s390x"}
+    allowed_archs = {
+        "x86_64",
+        "aarch64",
+        "ppc64",
+        "ppc64le",
+        "s390x",
+        "loongarch64",
+        "riscv64",
+    }
+    return any(arch in allowed_archs for arch in archs)
 
 
 # If glibc ever changes its major version, we need to know what the last
 # minor version was, so we can build the complete list of all versions.
 # For now, guess what the highest minor version might be, assume it will
 # be 50 for testing. Once this actually happens, update the dictionary
 # with the actual value.
@@ -77,15 +86,15 @@
     """
     # os.confstr is quite a bit faster than ctypes.DLL. It's also less likely
     # to be broken or missing. This strategy is used in the standard library
     # platform module.
     # https://github.com/python/cpython/blob/fcf1d003bf4f0100c/Lib/platform.py#L175-L183
     try:
         # Should be a string like "glibc 2.17".
-        version_string: str = getattr(os, "confstr")("CS_GNU_LIBC_VERSION")
+        version_string: Optional[str] = os.confstr("CS_GNU_LIBC_VERSION")
         assert version_string is not None
         _, version = version_string.rsplit()
     except (AssertionError, AttributeError, OSError, ValueError):
         # os.confstr() or CS_GNU_LIBC_VERSION not available (or a bad value)...
         return None
     return version
 
@@ -163,21 +172,21 @@
     version_str = _glibc_version_string()
     if version_str is None:
         return (-1, -1)
     return _parse_glibc_version(version_str)
 
 
 # From PEP 513, PEP 600
-def _is_compatible(name: str, arch: str, version: _GLibCVersion) -> bool:
+def _is_compatible(arch: str, version: _GLibCVersion) -> bool:
     sys_glibc = _get_glibc_version()
     if sys_glibc < version:
         return False
     # Check for presence of _manylinux module.
     try:
-        import _manylinux  # noqa
+        import _manylinux
     except ImportError:
         return True
     if hasattr(_manylinux, "manylinux_compatible"):
         result = _manylinux.manylinux_compatible(version[0], version[1], arch)
         if result is not None:
             return bool(result)
         return True
@@ -199,42 +208,53 @@
     # CentOS 6 w/ glibc 2.12 (PEP 571)
     (2, 12): "manylinux2010",
     # CentOS 5 w/ glibc 2.5 (PEP 513)
     (2, 5): "manylinux1",
 }
 
 
-def platform_tags(linux: str, arch: str) -> Iterator[str]:
-    if not _have_compatible_abi(sys.executable, arch):
+def platform_tags(archs: Sequence[str]) -> Iterator[str]:
+    """Generate manylinux tags compatible to the current platform.
+
+    :param archs: Sequence of compatible architectures.
+        The first one shall be the closest to the actual architecture and be the part of
+        platform tag after the ``linux_`` prefix, e.g. ``x86_64``.
+        The ``linux_`` prefix is assumed as a prerequisite for the current platform to
+        be manylinux-compatible.
+
+    :returns: An iterator of compatible manylinux tags.
+    """
+    if not _have_compatible_abi(sys.executable, archs):
         return
     # Oldest glibc to be supported regardless of architecture is (2, 17).
     too_old_glibc2 = _GLibCVersion(2, 16)
-    if arch in {"x86_64", "i686"}:
+    if set(archs) & {"x86_64", "i686"}:
         # On x86/i686 also oldest glibc to be supported is (2, 5).
         too_old_glibc2 = _GLibCVersion(2, 4)
     current_glibc = _GLibCVersion(*_get_glibc_version())
     glibc_max_list = [current_glibc]
     # We can assume compatibility across glibc major versions.
     # https://sourceware.org/bugzilla/show_bug.cgi?id=24636
     #
     # Build a list of maximum glibc versions so that we can
     # output the canonical list of all glibc from current_glibc
     # down to too_old_glibc2, including all intermediary versions.
     for glibc_major in range(current_glibc.major - 1, 1, -1):
         glibc_minor = _LAST_GLIBC_MINOR[glibc_major]
         glibc_max_list.append(_GLibCVersion(glibc_major, glibc_minor))
-    for glibc_max in glibc_max_list:
-        if glibc_max.major == too_old_glibc2.major:
-            min_minor = too_old_glibc2.minor
-        else:
-            # For other glibc major versions oldest supported is (x, 0).
-            min_minor = -1
-        for glibc_minor in range(glibc_max.minor, min_minor, -1):
-            glibc_version = _GLibCVersion(glibc_max.major, glibc_minor)
-            tag = "manylinux_{}_{}".format(*glibc_version)
-            if _is_compatible(tag, arch, glibc_version):
-                yield linux.replace("linux", tag)
-            # Handle the legacy manylinux1, manylinux2010, manylinux2014 tags.
-            if glibc_version in _LEGACY_MANYLINUX_MAP:
-                legacy_tag = _LEGACY_MANYLINUX_MAP[glibc_version]
-                if _is_compatible(legacy_tag, arch, glibc_version):
-                    yield linux.replace("linux", legacy_tag)
+    for arch in archs:
+        for glibc_max in glibc_max_list:
+            if glibc_max.major == too_old_glibc2.major:
+                min_minor = too_old_glibc2.minor
+            else:
+                # For other glibc major versions oldest supported is (x, 0).
+                min_minor = -1
+            for glibc_minor in range(glibc_max.minor, min_minor, -1):
+                glibc_version = _GLibCVersion(glibc_max.major, glibc_minor)
+                tag = "manylinux_{}_{}".format(*glibc_version)
+                if _is_compatible(arch, glibc_version):
+                    yield f"{tag}_{arch}"
+                # Handle the legacy manylinux1, manylinux2010, manylinux2014 tags.
+                if glibc_version in _LEGACY_MANYLINUX_MAP:
+                    legacy_tag = _LEGACY_MANYLINUX_MAP[glibc_version]
+                    if _is_compatible(arch, glibc_version):
+                        yield f"{legacy_tag}_{arch}"
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_musllinux.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_musllinux.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 linked against musl, and what musl version is used.
 """
 
 import functools
 import re
 import subprocess
 import sys
-from typing import Iterator, NamedTuple, Optional
+from typing import Iterator, NamedTuple, Optional, Sequence
 
 from ._elffile import ELFFile
 
 
 class _MuslVersion(NamedTuple):
     major: int
     minor: int
@@ -43,32 +43,35 @@
     try:
         with open(executable, "rb") as f:
             ld = ELFFile(f).interpreter
     except (OSError, TypeError, ValueError):
         return None
     if ld is None or "musl" not in ld:
         return None
-    proc = subprocess.run([ld], stderr=subprocess.PIPE, universal_newlines=True)
+    proc = subprocess.run([ld], stderr=subprocess.PIPE, text=True)
     return _parse_musl_version(proc.stderr)
 
 
-def platform_tags(arch: str) -> Iterator[str]:
+def platform_tags(archs: Sequence[str]) -> Iterator[str]:
     """Generate musllinux tags compatible to the current platform.
 
-    :param arch: Should be the part of platform tag after the ``linux_``
-        prefix, e.g. ``x86_64``. The ``linux_`` prefix is assumed as a
-        prerequisite for the current platform to be musllinux-compatible.
+    :param archs: Sequence of compatible architectures.
+        The first one shall be the closest to the actual architecture and be the part of
+        platform tag after the ``linux_`` prefix, e.g. ``x86_64``.
+        The ``linux_`` prefix is assumed as a prerequisite for the current platform to
+        be musllinux-compatible.
 
     :returns: An iterator of compatible musllinux tags.
     """
     sys_musl = _get_musl_version(sys.executable)
     if sys_musl is None:  # Python not dynamically linked against musl.
         return
-    for minor in range(sys_musl.minor, -1, -1):
-        yield f"musllinux_{sys_musl.major}_{minor}_{arch}"
+    for arch in archs:
+        for minor in range(sys_musl.minor, -1, -1):
+            yield f"musllinux_{sys_musl.major}_{minor}_{arch}"
 
 
 if __name__ == "__main__":  # pragma: no cover
     import sysconfig
 
     plat = sysconfig.get_platform()
     assert plat.startswith("linux-"), "not linux"
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_parser.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,21 @@
     return parsed_specifiers
 
 
 # --------------------------------------------------------------------------------------
 # Recursive descent parser for marker expression
 # --------------------------------------------------------------------------------------
 def parse_marker(source: str) -> MarkerList:
-    return _parse_marker(Tokenizer(source, rules=DEFAULT_RULES))
+    return _parse_full_marker(Tokenizer(source, rules=DEFAULT_RULES))
+
+
+def _parse_full_marker(tokenizer: Tokenizer) -> MarkerList:
+    retval = _parse_marker(tokenizer)
+    tokenizer.expect("END", expected="end of marker expression")
+    return retval
 
 
 def _parse_marker(tokenizer: Tokenizer) -> MarkerList:
     """
     marker = marker_atom (BOOLOP marker_atom)+
     """
     expression = [_parse_marker_atom(tokenizer)]
@@ -314,18 +320,15 @@
     else:
         tokenizer.raise_syntax_error(
             message="Expected a marker variable or quoted string"
         )
 
 
 def process_env_var(env_var: str) -> Variable:
-    if (
-        env_var == "platform_python_implementation"
-        or env_var == "python_implementation"
-    ):
+    if env_var in ("platform_python_implementation", "python_implementation"):
         return Variable("platform_python_implementation")
     else:
         return Variable(env_var)
 
 
 def process_python_str(python_str: str) -> Value:
     value = ast.literal_eval(python_str)
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_structures.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/_tokenizer.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/markers.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/requirements.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/requirements.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
-import urllib.parse
-from typing import Any, List, Optional, Set
+from typing import Any, Iterator, Optional, Set
 
 from ._parser import parse_requirement as _parse_requirement
 from ._tokenizer import ParserSyntaxError
 from .markers import Marker, _normalize_extra_values
 from .specifiers import SpecifierSet
+from .utils import canonicalize_name
 
 
 class InvalidRequirement(ValueError):
     """
     An invalid requirement was found, users should refer to PEP 508.
     """
 
@@ -33,63 +33,58 @@
     def __init__(self, requirement_string: str) -> None:
         try:
             parsed = _parse_requirement(requirement_string)
         except ParserSyntaxError as e:
             raise InvalidRequirement(str(e)) from e
 
         self.name: str = parsed.name
-        if parsed.url:
-            parsed_url = urllib.parse.urlparse(parsed.url)
-            if parsed_url.scheme == "file":
-                if urllib.parse.urlunparse(parsed_url) != parsed.url:
-                    raise InvalidRequirement("Invalid URL given")
-            elif not (parsed_url.scheme and parsed_url.netloc) or (
-                not parsed_url.scheme and not parsed_url.netloc
-            ):
-                raise InvalidRequirement(f"Invalid URL: {parsed.url}")
-            self.url: Optional[str] = parsed.url
-        else:
-            self.url = None
-        self.extras: Set[str] = set(parsed.extras if parsed.extras else [])
+        self.url: Optional[str] = parsed.url or None
+        self.extras: Set[str] = set(parsed.extras or [])
         self.specifier: SpecifierSet = SpecifierSet(parsed.specifier)
         self.marker: Optional[Marker] = None
         if parsed.marker is not None:
             self.marker = Marker.__new__(Marker)
             self.marker._markers = _normalize_extra_values(parsed.marker)
 
-    def __str__(self) -> str:
-        parts: List[str] = [self.name]
+    def _iter_parts(self, name: str) -> Iterator[str]:
+        yield name
 
         if self.extras:
             formatted_extras = ",".join(sorted(self.extras))
-            parts.append(f"[{formatted_extras}]")
+            yield f"[{formatted_extras}]"
 
         if self.specifier:
-            parts.append(str(self.specifier))
+            yield str(self.specifier)
 
         if self.url:
-            parts.append(f"@ {self.url}")
+            yield f"@ {self.url}"
             if self.marker:
-                parts.append(" ")
+                yield " "
 
         if self.marker:
-            parts.append(f"; {self.marker}")
+            yield f"; {self.marker}"
 
-        return "".join(parts)
+    def __str__(self) -> str:
+        return "".join(self._iter_parts(self.name))
 
     def __repr__(self) -> str:
         return f"<Requirement('{self}')>"
 
     def __hash__(self) -> int:
-        return hash((self.__class__.__name__, str(self)))
+        return hash(
+            (
+                self.__class__.__name__,
+                *self._iter_parts(canonicalize_name(self.name)),
+            )
+        )
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Requirement):
             return NotImplemented
 
         return (
-            self.name == other.name
+            canonicalize_name(self.name) == canonicalize_name(other.name)
             and self.extras == other.extras
             and self.specifier == other.specifier
             and self.url == other.url
             and self.marker == other.marker
         )
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/specifiers.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/specifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,25 +7,15 @@
     from packaging.specifiers import Specifier, SpecifierSet, InvalidSpecifier
     from packaging.version import Version
 """
 
 import abc
 import itertools
 import re
-from typing import (
-    Callable,
-    Iterable,
-    Iterator,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import Callable, Iterable, Iterator, List, Optional, Tuple, TypeVar, Union
 
 from .utils import canonicalize_version
 from .version import Version
 
 UnparsedVersion = Union[Version, str]
 UnparsedVersionVar = TypeVar("UnparsedVersionVar", bound=UnparsedVersion)
 CallableOperator = Callable[[Version, str], bool]
@@ -379,15 +369,15 @@
         # is that ~=2.2 is equivalent to >=2.2,==2.*. This allows us to
         # implement this in terms of the other specifiers instead of
         # implementing it ourselves. The only thing we need to do is construct
         # the other specifiers.
 
         # We want everything but the last item in the version, but we want to
         # ignore suffix segments.
-        prefix = ".".join(
+        prefix = _version_join(
             list(itertools.takewhile(_is_not_suffix, _version_split(spec)))[:-1]
         )
 
         # Add the prefix notation to the end of our string
         prefix += ".*"
 
         return self._get_operator(">=")(prospective, spec) and self._get_operator("==")(
@@ -400,21 +390,21 @@
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
             normalized_prospective = canonicalize_version(
                 prospective.public, strip_trailing_zero=False
             )
             # Get the normalized version string ignoring the trailing .*
             normalized_spec = canonicalize_version(spec[:-2], strip_trailing_zero=False)
-            # Split the spec out by dots, and pretend that there is an implicit
-            # dot in between a release segment and a pre-release segment.
+            # Split the spec out by bangs and dots, and pretend that there is
+            # an implicit dot in between a release segment and a pre-release segment.
             split_spec = _version_split(normalized_spec)
 
-            # Split the prospective version out by dots, and pretend that there
-            # is an implicit dot in between a release segment and a pre-release
-            # segment.
+            # Split the prospective version out by bangs and dots, and pretend
+            # that there is an implicit dot in between a release segment and
+            # a pre-release segment.
             split_prospective = _version_split(normalized_prospective)
 
             # 0-pad the prospective version before shortening it to get the correct
             # shortened version.
             padded_prospective, _ = _pad_version(split_prospective, split_spec)
 
             # Shorten the prospective version to be the same length as the spec
@@ -640,24 +630,46 @@
                 yield version
 
 
 _prefix_regex = re.compile(r"^([0-9]+)((?:a|b|c|rc)[0-9]+)$")
 
 
 def _version_split(version: str) -> List[str]:
+    """Split version into components.
+
+    The split components are intended for version comparison. The logic does
+    not attempt to retain the original version string, so joining the
+    components back with :func:`_version_join` may not produce the original
+    version string.
+    """
     result: List[str] = []
-    for item in version.split("."):
+
+    epoch, _, rest = version.rpartition("!")
+    result.append(epoch or "0")
+
+    for item in rest.split("."):
         match = _prefix_regex.search(item)
         if match:
             result.extend(match.groups())
         else:
             result.append(item)
     return result
 
 
+def _version_join(components: List[str]) -> str:
+    """Join split version components into a version string.
+
+    This function assumes the input came from :func:`_version_split`, where the
+    first component must be the epoch (either empty or numeric), and all other
+    components numeric.
+    """
+    epoch, *rest = components
+    return f"{epoch}!{'.'.join(rest)}"
+
+
 def _is_not_suffix(segment: str) -> bool:
     return not any(
         segment.startswith(prefix) for prefix in ("dev", "a", "b", "rc", "post")
     )
 
 
 def _pad_version(left: List[str], right: List[str]) -> Tuple[List[str], List[str]]:
@@ -671,15 +683,18 @@
     left_split.append(left[len(left_split[0]) :])
     right_split.append(right[len(right_split[0]) :])
 
     # Insert our padding
     left_split.insert(1, ["0"] * max(0, len(right_split[0]) - len(left_split[0])))
     right_split.insert(1, ["0"] * max(0, len(left_split[0]) - len(right_split[0])))
 
-    return (list(itertools.chain(*left_split)), list(itertools.chain(*right_split)))
+    return (
+        list(itertools.chain.from_iterable(left_split)),
+        list(itertools.chain.from_iterable(right_split)),
+    )
 
 
 class SpecifierSet(BaseSpecifier):
     """This class abstracts handling of a set of version specifiers.
 
     It can be passed a single specifier (``>=3.0``), a comma-separated list of
     specifiers (``>=3.0,!=3.1``), or no specifier at all.
@@ -703,22 +718,16 @@
             raised.
         """
 
         # Split on `,` to break each individual specifier into it's own item, and
         # strip each item to remove leading/trailing whitespace.
         split_specifiers = [s.strip() for s in specifiers.split(",") if s.strip()]
 
-        # Parsed each individual specifier, attempting first to make it a
-        # Specifier.
-        parsed: Set[Specifier] = set()
-        for specifier in split_specifiers:
-            parsed.add(Specifier(specifier))
-
-        # Turn our parsed specifiers into a frozen set and save them for later.
-        self._specs = frozenset(parsed)
+        # Make each individual specifier a Specifier and save in a frozen set for later.
+        self._specs = frozenset(map(Specifier, split_specifiers))
 
         # Store our prereleases value so we can use it later to determine if
         # we accept prereleases or not.
         self._prereleases = prereleases
 
     @property
     def prereleases(self) -> Optional[bool]:
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/tags.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import logging
 import platform
+import re
+import struct
 import subprocess
 import sys
 import sysconfig
 from importlib.machinery import EXTENSION_SUFFIXES
 from typing import (
     Dict,
     FrozenSet,
@@ -33,15 +35,15 @@
     "cpython": "cp",
     "pypy": "pp",
     "ironpython": "ip",
     "jython": "jy",
 }
 
 
-_32_BIT_INTERPRETER = sys.maxsize <= 2**32
+_32_BIT_INTERPRETER = struct.calcsize("P") == 4
 
 
 class Tag:
     """
     A representation of the tag triple for a wheel.
 
     Instances are considered immutable and thus are hashable. Equality checking
@@ -119,56 +121,70 @@
     return value
 
 
 def _normalize_string(string: str) -> str:
     return string.replace(".", "_").replace("-", "_").replace(" ", "_")
 
 
-def _abi3_applies(python_version: PythonVersion) -> bool:
+def _is_threaded_cpython(abis: List[str]) -> bool:
+    """
+    Determine if the ABI corresponds to a threaded (`--disable-gil`) build.
+
+    The threaded builds are indicated by a "t" in the abiflags.
+    """
+    if len(abis) == 0:
+        return False
+    # expect e.g., cp313
+    m = re.match(r"cp\d+(.*)", abis[0])
+    if not m:
+        return False
+    abiflags = m.group(1)
+    return "t" in abiflags
+
+
+def _abi3_applies(python_version: PythonVersion, threading: bool) -> bool:
     """
     Determine if the Python version supports abi3.
 
-    PEP 384 was first implemented in Python 3.2.
+    PEP 384 was first implemented in Python 3.2. The threaded (`--disable-gil`)
+    builds do not support abi3.
     """
-    return len(python_version) > 1 and tuple(python_version) >= (3, 2)
+    return len(python_version) > 1 and tuple(python_version) >= (3, 2) and not threading
 
 
 def _cpython_abis(py_version: PythonVersion, warn: bool = False) -> List[str]:
     py_version = tuple(py_version)  # To allow for version comparison.
     abis = []
     version = _version_nodot(py_version[:2])
-    debug = pymalloc = ucs4 = ""
+    threading = debug = pymalloc = ucs4 = ""
     with_debug = _get_config_var("Py_DEBUG", warn)
     has_refcount = hasattr(sys, "gettotalrefcount")
     # Windows doesn't set Py_DEBUG, so checking for support of debug-compiled
     # extension modules is the best option.
     # https://github.com/pypa/pip/issues/3383#issuecomment-173267692
     has_ext = "_d.pyd" in EXTENSION_SUFFIXES
     if with_debug or (with_debug is None and (has_refcount or has_ext)):
         debug = "d"
+    if py_version >= (3, 13) and _get_config_var("Py_GIL_DISABLED", warn):
+        threading = "t"
     if py_version < (3, 8):
         with_pymalloc = _get_config_var("WITH_PYMALLOC", warn)
         if with_pymalloc or with_pymalloc is None:
             pymalloc = "m"
         if py_version < (3, 3):
             unicode_size = _get_config_var("Py_UNICODE_SIZE", warn)
             if unicode_size == 4 or (
                 unicode_size is None and sys.maxunicode == 0x10FFFF
             ):
                 ucs4 = "u"
     elif debug:
         # Debug builds can also load "normal" extension modules.
         # We can also assume no UCS-4 or pymalloc requirement.
-        abis.append(f"cp{version}")
-    abis.insert(
-        0,
-        "cp{version}{debug}{pymalloc}{ucs4}".format(
-            version=version, debug=debug, pymalloc=pymalloc, ucs4=ucs4
-        ),
-    )
+        abis.append(f"cp{version}{threading}")
+    abis.insert(0, f"cp{version}{threading}{debug}{pymalloc}{ucs4}")
     return abis
 
 
 def cpython_tags(
     python_version: Optional[PythonVersion] = None,
     abis: Optional[Iterable[str]] = None,
     platforms: Optional[Iterable[str]] = None,
@@ -208,19 +224,22 @@
         except ValueError:
             pass
 
     platforms = list(platforms or platform_tags())
     for abi in abis:
         for platform_ in platforms:
             yield Tag(interpreter, abi, platform_)
-    if _abi3_applies(python_version):
+
+    threading = _is_threaded_cpython(abis)
+    use_abi3 = _abi3_applies(python_version, threading)
+    if use_abi3:
         yield from (Tag(interpreter, "abi3", platform_) for platform_ in platforms)
     yield from (Tag(interpreter, "none", platform_) for platform_ in platforms)
 
-    if _abi3_applies(python_version):
+    if use_abi3:
         for minor_version in range(python_version[1] - 1, 1, -1):
             for platform_ in platforms:
                 interpreter = "cp{version}".format(
                     version=_version_nodot((python_version[0], minor_version))
                 )
                 yield Tag(interpreter, "abi3", platform_)
 
@@ -402,15 +421,15 @@
                     "-sS",
                     "-c",
                     "import platform; print(platform.mac_ver()[0])",
                 ],
                 check=True,
                 env={"SYSTEM_VERSION_COMPAT": "0"},
                 stdout=subprocess.PIPE,
-                universal_newlines=True,
+                text=True,
             ).stdout
             version = cast("MacVersion", tuple(map(int, version_str.split(".")[:2])))
     else:
         version = version
     if arch is None:
         arch = _mac_arch(cpu_arch)
     else:
@@ -465,23 +484,29 @@
                     minor=compat_version[1],
                     binary_format=binary_format,
                 )
 
 
 def _linux_platforms(is_32bit: bool = _32_BIT_INTERPRETER) -> Iterator[str]:
     linux = _normalize_string(sysconfig.get_platform())
+    if not linux.startswith("linux_"):
+        # we should never be here, just yield the sysconfig one and return
+        yield linux
+        return
     if is_32bit:
         if linux == "linux_x86_64":
             linux = "linux_i686"
         elif linux == "linux_aarch64":
-            linux = "linux_armv7l"
+            linux = "linux_armv8l"
     _, arch = linux.split("_", 1)
-    yield from _manylinux.platform_tags(linux, arch)
-    yield from _musllinux.platform_tags(arch)
-    yield linux
+    archs = {"armv8l": ["armv8l", "armv7l"]}.get(arch, [arch])
+    yield from _manylinux.platform_tags(archs)
+    yield from _musllinux.platform_tags(archs)
+    for arch in archs:
+        yield f"linux_{arch}"
 
 
 def _generic_platforms() -> Iterator[str]:
     yield _normalize_string(sysconfig.get_platform())
 
 
 def platform_tags() -> Iterator[str]:
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/utils.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,37 +8,54 @@
 from .tags import Tag, parse_tag
 from .version import InvalidVersion, Version
 
 BuildTag = Union[Tuple[()], Tuple[int, str]]
 NormalizedName = NewType("NormalizedName", str)
 
 
+class InvalidName(ValueError):
+    """
+    An invalid distribution name; users should refer to the packaging user guide.
+    """
+
+
 class InvalidWheelFilename(ValueError):
     """
     An invalid wheel filename was found, users should refer to PEP 427.
     """
 
 
 class InvalidSdistFilename(ValueError):
     """
     An invalid sdist filename was found, users should refer to the packaging user guide.
     """
 
 
+# Core metadata spec for `Name`
+_validate_regex = re.compile(
+    r"^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$", re.IGNORECASE
+)
 _canonicalize_regex = re.compile(r"[-_.]+")
+_normalized_regex = re.compile(r"^([a-z0-9]|[a-z0-9]([a-z0-9-](?!--))*[a-z0-9])$")
 # PEP 427: The build number must start with a digit.
 _build_tag_regex = re.compile(r"(\d+)(.*)")
 
 
-def canonicalize_name(name: str) -> NormalizedName:
+def canonicalize_name(name: str, *, validate: bool = False) -> NormalizedName:
+    if validate and not _validate_regex.match(name):
+        raise InvalidName(f"name is invalid: {name!r}")
     # This is taken from PEP 503.
     value = _canonicalize_regex.sub("-", name).lower()
     return cast(NormalizedName, value)
 
 
+def is_normalized_name(name: str) -> bool:
+    return _normalized_regex.match(name) is not None
+
+
 def canonicalize_version(
     version: Union[Version, str], *, strip_trailing_zero: bool = True
 ) -> str:
     """
     This is very similar to Version.__str__, but has one subtle difference
     with the way it handles the release segment.
     """
@@ -96,19 +113,26 @@
     if dashes not in (4, 5):
         raise InvalidWheelFilename(
             f"Invalid wheel filename (wrong number of parts): {filename}"
         )
 
     parts = filename.split("-", dashes - 2)
     name_part = parts[0]
-    # See PEP 427 for the rules on escaping the project name
+    # See PEP 427 for the rules on escaping the project name.
     if "__" in name_part or re.match(r"^[\w\d._]*$", name_part, re.UNICODE) is None:
         raise InvalidWheelFilename(f"Invalid project name: {filename}")
     name = canonicalize_name(name_part)
-    version = Version(parts[1])
+
+    try:
+        version = Version(parts[1])
+    except InvalidVersion as e:
+        raise InvalidWheelFilename(
+            f"Invalid wheel filename (invalid version): {filename}"
+        ) from e
+
     if dashes == 5:
         build_part = parts[2]
         build_match = _build_tag_regex.match(build_part)
         if build_match is None:
             raise InvalidWheelFilename(
                 f"Invalid build number: {build_part} in '{filename}'"
             )
@@ -133,9 +157,16 @@
     # We are requiring a PEP 440 version, which cannot contain dashes,
     # so we split on the last dash.
     name_part, sep, version_part = file_stem.rpartition("-")
     if not sep:
         raise InvalidSdistFilename(f"Invalid sdist filename: {filename}")
 
     name = canonicalize_name(name_part)
-    version = Version(version_part)
+
+    try:
+        version = Version(version_part)
+    except InvalidVersion as e:
+        raise InvalidSdistFilename(
+            f"Invalid sdist filename (invalid version): {filename}"
+        ) from e
+
     return (name, version)
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/packaging/version.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/packaging/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,45 +3,47 @@
 # for complete details.
 """
 .. testsetup::
 
     from packaging.version import parse, Version
 """
 
-import collections
 import itertools
 import re
-from typing import Any, Callable, Optional, SupportsInt, Tuple, Union
+from typing import Any, Callable, NamedTuple, Optional, SupportsInt, Tuple, Union
 
 from ._structures import Infinity, InfinityType, NegativeInfinity, NegativeInfinityType
 
 __all__ = ["VERSION_PATTERN", "parse", "Version", "InvalidVersion"]
 
-InfiniteTypes = Union[InfinityType, NegativeInfinityType]
-PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
-SubLocalType = Union[InfiniteTypes, int, str]
-LocalType = Union[
+LocalType = Tuple[Union[int, str], ...]
+
+CmpPrePostDevType = Union[InfinityType, NegativeInfinityType, Tuple[str, int]]
+CmpLocalType = Union[
     NegativeInfinityType,
-    Tuple[
-        Union[
-            SubLocalType,
-            Tuple[SubLocalType, str],
-            Tuple[NegativeInfinityType, SubLocalType],
-        ],
-        ...,
-    ],
+    Tuple[Union[Tuple[int, str], Tuple[NegativeInfinityType, Union[int, str]]], ...],
 ]
 CmpKey = Tuple[
-    int, Tuple[int, ...], PrePostDevType, PrePostDevType, PrePostDevType, LocalType
+    int,
+    Tuple[int, ...],
+    CmpPrePostDevType,
+    CmpPrePostDevType,
+    CmpPrePostDevType,
+    CmpLocalType,
 ]
 VersionComparisonMethod = Callable[[CmpKey, CmpKey], bool]
 
-_Version = collections.namedtuple(
-    "_Version", ["epoch", "release", "dev", "pre", "post", "local"]
-)
+
+class _Version(NamedTuple):
+    epoch: int
+    release: Tuple[int, ...]
+    dev: Optional[Tuple[str, int]]
+    pre: Optional[Tuple[str, int]]
+    post: Optional[Tuple[str, int]]
+    local: Optional[LocalType]
 
 
 def parse(version: str) -> "Version":
     """Parse the given version string.
 
     >>> parse('1.0.dev1')
     <Version('1.0.dev1')>
@@ -113,15 +115,15 @@
 _VERSION_PATTERN = r"""
     v?
     (?:
         (?:(?P<epoch>[0-9]+)!)?                           # epoch
         (?P<release>[0-9]+(?:\.[0-9]+)*)                  # release segment
         (?P<pre>                                          # pre-release
             [-_\.]?
-            (?P<pre_l>(a|b|c|rc|alpha|beta|pre|preview))
+            (?P<pre_l>alpha|a|beta|b|preview|pre|c|rc)
             [-_\.]?
             (?P<pre_n>[0-9]+)?
         )?
         (?P<post>                                         # post release
             (?:-(?P<post_n1>[0-9]+))
             |
             (?:
@@ -265,16 +267,15 @@
         """The epoch of the version.
 
         >>> Version("2.0.0").epoch
         0
         >>> Version("1!2.0.0").epoch
         1
         """
-        _epoch: int = self._version.epoch
-        return _epoch
+        return self._version.epoch
 
     @property
     def release(self) -> Tuple[int, ...]:
         """The components of the "release" segment of the version.
 
         >>> Version("1.2.3").release
         (1, 2, 3)
@@ -282,32 +283,30 @@
         (2, 0, 0)
         >>> Version("1!2.0.0.post0").release
         (2, 0, 0)
 
         Includes trailing zeroes but not the epoch or any pre-release / development /
         post-release suffixes.
         """
-        _release: Tuple[int, ...] = self._version.release
-        return _release
+        return self._version.release
 
     @property
     def pre(self) -> Optional[Tuple[str, int]]:
         """The pre-release segment of the version.
 
         >>> print(Version("1.2.3").pre)
         None
         >>> Version("1.2.3a1").pre
         ('a', 1)
         >>> Version("1.2.3b1").pre
         ('b', 1)
         >>> Version("1.2.3rc1").pre
         ('rc', 1)
         """
-        _pre: Optional[Tuple[str, int]] = self._version.pre
-        return _pre
+        return self._version.pre
 
     @property
     def post(self) -> Optional[int]:
         """The post-release number of the version.
 
         >>> print(Version("1.2.3").post)
         None
@@ -447,15 +446,15 @@
         >>> Version("1").micro
         0
         """
         return self.release[2] if len(self.release) >= 3 else 0
 
 
 def _parse_letter_version(
-    letter: str, number: Union[str, bytes, SupportsInt]
+    letter: Optional[str], number: Union[str, bytes, SupportsInt, None]
 ) -> Optional[Tuple[str, int]]:
 
     if letter:
         # We consider there to be an implicit 0 in a pre-release if there is
         # not a numeral associated with it.
         if number is None:
             number = 0
@@ -485,15 +484,15 @@
 
     return None
 
 
 _local_version_separators = re.compile(r"[\._-]")
 
 
-def _parse_local_version(local: str) -> Optional[LocalType]:
+def _parse_local_version(local: Optional[str]) -> Optional[LocalType]:
     """
     Takes a string like abc.1.twelve and turns it into ("abc", 1, "twelve").
     """
     if local is not None:
         return tuple(
             part.lower() if not part.isdigit() else int(part)
             for part in _local_version_separators.split(local)
@@ -503,15 +502,15 @@
 
 def _cmpkey(
     epoch: int,
     release: Tuple[int, ...],
     pre: Optional[Tuple[str, int]],
     post: Optional[Tuple[str, int]],
     dev: Optional[Tuple[str, int]],
-    local: Optional[Tuple[SubLocalType]],
+    local: Optional[LocalType],
 ) -> CmpKey:
 
     # When we compare a release version, we want to compare it with all of the
     # trailing zeros removed. So we'll use a reverse the list, drop all the now
     # leading zeros until we come to something non zero, then take the rest
     # re-reverse it back into the correct order and make it a tuple and use
     # that for our sorting key.
@@ -520,39 +519,39 @@
     )
 
     # We need to "trick" the sorting algorithm to put 1.0.dev0 before 1.0a0.
     # We'll do this by abusing the pre segment, but we _only_ want to do this
     # if there is not a pre or a post segment. If we have one of those then
     # the normal sorting rules will handle this case correctly.
     if pre is None and post is None and dev is not None:
-        _pre: PrePostDevType = NegativeInfinity
+        _pre: CmpPrePostDevType = NegativeInfinity
     # Versions without a pre-release (except as noted above) should sort after
     # those with one.
     elif pre is None:
         _pre = Infinity
     else:
         _pre = pre
 
     # Versions without a post segment should sort before those with one.
     if post is None:
-        _post: PrePostDevType = NegativeInfinity
+        _post: CmpPrePostDevType = NegativeInfinity
 
     else:
         _post = post
 
     # Versions without a development segment should sort after those with one.
     if dev is None:
-        _dev: PrePostDevType = Infinity
+        _dev: CmpPrePostDevType = Infinity
 
     else:
         _dev = dev
 
     if local is None:
         # Versions without a local segment should sort before those with one.
-        _local: LocalType = NegativeInfinity
+        _local: CmpLocalType = NegativeInfinity
     else:
         # Versions with a local segment need that segment parsed to implement
         # the sorting rules in PEP440.
         # - Alpha numeric segments sort before numeric segments
         # - Alpha numeric segments sort lexicographically
         # - Numeric segments sort numerically
         # - Shorter versions sort before longer versions when the prefixes
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/_vendor/tomli/_re.py` & `pyproject_installer-0.5.3/src/pyproject_installer/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/build_cmd/_build.py` & `pyproject_installer-0.5.3/src/pyproject_installer/build_cmd/_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     hook = "prepare_metadata_for_build_wheel"
     logger.info("Building metadata with %s", hook)
     with build_out_tmpdir(srcdir, hook, config, verbose) as (
         distinfo_dir,
         tmp_path,
     ):
-        if distinfo_dir != "":
+        if distinfo_dir:
             metadata_path_src = tmp_path / distinfo_dir / metadata_filename
             # Python 3.8 syntax
             with metadata_path_src.open(
                 mode="rb"
             ) as fsrc, metadata_path_dest.open(mode="wb") as fdst:
                 shutil.copyfileobj(fsrc, fdst)
             return metadata_filename
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/deps_config.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/deps_config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/__init__.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .pep518 import Pep518Collector
 from .pip_reqfile import PipReqFileCollector
 from .metadata import MetadataCollector
 from .poetry import PoetryCollector
 from .tox import ToxCollector
 from .hatch import HatchCollector
 from .pdm import PdmCollector
+from .pipenv import PipenvCollector
 
 
 __all__ = ["get_collector", "SUPPORTED_COLLECTORS"]
 
 SUPPORTED_COLLECTORS = {
     cls.name: cls
     for cls in [
@@ -17,14 +18,15 @@
         Pep518Collector,
         MetadataCollector,
         PipReqFileCollector,
         PoetryCollector,
         ToxCollector,
         HatchCollector,
         PdmCollector,
+        PipenvCollector,
     ]
 }
 
 
 def get_collector(name):
     try:
         return SUPPORTED_COLLECTORS[name]
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/hatch.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/hatch.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/metadata.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pdm.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pdm.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep517.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pep517.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pep518.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pep518.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/poetry.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/poetry.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/deps_cmd/collectors/tox.py` & `pyproject_installer-0.5.3/src/pyproject_installer/deps_cmd/collectors/tox.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/install_cmd/_install.py` & `pyproject_installer-0.5.3/src/pyproject_installer/install_cmd/_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,29 +64,29 @@
             # PEP427
             # In wheel, scripts are packaged in
             # {distribution}-{version}.data/scripts/. If the first line of a
             # file in scripts/ starts with exactly b'#!python', rewrite to
             # point to the correct interpreter.
             for s in f.iterdir():
                 if s.is_file() and not s.is_symlink():
+                    script_path = rootdir / s.name
                     with s.open(mode="rb") as sf:
                         if sf.read(len(MAGIC_SHEBANG)) == MAGIC_SHEBANG:
                             sf.seek(0)
                             sf.readline()  # discard shebang
-                            script_path = rootdir / s.name
                             with script_path.open(mode="wb") as fsf:
                                 fsf.write(
                                     (
                                         build_shebang(sys.executable) + "\n"
                                     ).encode("utf-8")
                                 )
                                 shutil.copyfileobj(sf, fsf)
-                            script_path.chmod(
-                                script_path.stat().st_mode | 0o555
-                            )
+                    # make any file in scripts directory executable
+                    # (can be a compiled binary for example)
+                    script_path.chmod(script_path.stat().st_mode | 0o555)
 
         shutil.rmtree(data_path / f)
 
     shutil.rmtree(data_path)
 
 
 def validate_wheel_path(wheel_path):
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/lib/build_backend.py` & `pyproject_installer-0.5.3/src/pyproject_installer/lib/build_backend.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/lib/entry_points.py` & `pyproject_installer-0.5.3/src/pyproject_installer/lib/entry_points.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/lib/scripts.py` & `pyproject_installer-0.5.3/src/pyproject_installer/lib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/lib/wheel.py` & `pyproject_installer-0.5.3/src/pyproject_installer/lib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/lib/backend_helper/backend_caller.py` & `pyproject_installer-0.5.3/src/pyproject_installer/lib/backend_helper/backend_caller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Intended to be run in subprocess to call build backend's hooks.
 Must not have dependencies other than stdlib.
 """
+
 from importlib import import_module
 from pathlib import Path
 import argparse
 import logging
 import os
 import json
 import sys
```

### Comparing `pyproject_installer-0.5.2/src/pyproject_installer/run_cmd/_run_env.py` & `pyproject_installer-0.5.3/src/pyproject_installer/run_cmd/_run_env.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/backend/config.py` & `pyproject_installer-0.5.3/backend/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/backend/metadata.py` & `pyproject_installer-0.5.3/backend/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/backend/sdist.py` & `pyproject_installer-0.5.3/backend/sdist.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 1. Parse PEP621 metadata
 2. Parse dynamic version(`version_file`) with ast
 3. Make archive:
    - search in `package_dir` and `include_dirs_sdist`
    - include *.py for now
    - exclude __pycache__ and .pyc
 """
+
 from io import BytesIO
 from pathlib import Path
 import logging
 import os
 import tarfile
 import time
```

### Comparing `pyproject_installer-0.5.2/backend/wheel.py` & `pyproject_installer-0.5.3/backend/wheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 1. Parse PEP621 metadata
 2. Parse dynamic version(`version_file`) with ast
 3. Make archive:
    - search in `package_dir`
    - include *.py for now
    - exclude __pycache__ and .pyc
 """
+
 from base64 import urlsafe_b64encode
 from io import TextIOWrapper, BytesIO
 from pathlib import Path
 from zipfile import ZipFile, ZipInfo, ZIP_DEFLATED
 import csv
 import hashlib
 import logging
```

### Comparing `pyproject_installer-0.5.2/backend/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.3/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/backend/_vendor/tomli/_re.py` & `pyproject_installer-0.5.3/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/tests/conftest.py` & `pyproject_installer-0.5.3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,18 @@
     def update_record(self):
         with StringIO(newline="") as ws:
             writer = csv.writer(ws, lineterminator="\n")
             records = [
                 (
                     f,
                     "sha256={}".format(
-                        digest_for_record("sha256", v.encode("utf8"))
+                        digest_for_record(
+                            "sha256",
+                            v if isinstance(v, bytes) else v.encode("utf8"),
+                        )
                     ),
                     0,
                 )
                 for f, v in self._contents.items()
                 if f != self.record_key
             ]
             records.append((self.record_key, "", 0))
```

### Comparing `pyproject_installer-0.5.2/tests/integration/conftest.py` & `pyproject_installer-0.5.3/tests/integration/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 @pytest.fixture
 def setuptools_project(pyproject):
     pyproject_path = pyproject(
         textwrap.dedent(
             """\
             [build-system]
-            requires = ["setuptools"]
+            requires = ["setuptools>=64"]
             build-backend = "setuptools.build_meta"
             """
         )
     )
     (pyproject_path / "setup.cfg").write_text(
         textwrap.dedent(
             """\
```

### Comparing `pyproject_installer-0.5.2/tests/integration/test_backends.py` & `pyproject_installer-0.5.3/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/tests/integration/test_buildable.py` & `pyproject_installer-0.5.3/tests/integration/test_buildable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Check if pyproject_installer is buildable by other tools like `build` or `pip`
 """
+
 import subprocess
 
 
 from pyproject_installer import __version__ as installer_version
 
 
 def install_pkg(context, pkg, ignore_installed=True):
```

### Comparing `pyproject_installer-0.5.2/tests/integration/test_config_settings.py` & `pyproject_installer-0.5.3/tests/integration/test_config_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
     virt_env_installer, setuptools_project, install_build_deps, wheeldir
 ):
     """
     1. Create virtual environment with installed pyproject_installer
     2. Create pyproject with setuptools build backend
     3. Install build requirements with pip
     4. Build with custom config_settings (today's setuptools respects
-       `--global-option` key)
+       `--build-option` key)
     """
     python = virt_env_installer.env_exec_cmd
     install_build_deps(python, srcdir=setuptools_project)
     build_args = [
         python,
         "-m",
         "pyproject_installer",
         "build",
         "--backend-config-settings",
         json.dumps(
             {
-                "--global-option": [
+                "--build-option": [
                     "--python-tag=test_tag",
                     "--build-number=123",
                     "--plat-name=test_plat",
                 ],
             }
         ),
         "--outdir",
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_main.py` & `pyproject_installer-0.5.3/tests/unit/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,24 +48,26 @@
 
 
 def test_version():
     result = subprocess.run(
         args=[sys.executable, "-m", "pyproject_installer", "--version"],
         capture_output=True,
     )
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     assert result.stdout.rstrip().decode("utf-8") == project_version
     assert result.stderr == b""
 
 
 def test_help():
     result = subprocess.run(
         args=[sys.executable, "-m", "pyproject_installer", "--help"],
         capture_output=True,
     )
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     assert result.stdout.rstrip().startswith(
         b"usage: python -m pyproject_installer "
     )
     assert result.stderr == b""
 
 
@@ -133,14 +135,15 @@
 
             __main__.setup_logging(verbose=True)
             logging.getLogger().{level}("{level}")
         """
     )
     cmd = [sys.executable, "-c", code]
     result = subprocess.run(args=cmd, capture_output=True)
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     if destination == "stderr":
         log_out = result.stderr
         log_no_out = result.stdout
     else:
         log_out = result.stdout
         log_no_out = result.stderr
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_build/test_backend_caller.py` & `pyproject_installer-0.5.3/tests/unit/test_build/test_backend_caller.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 
 
 def test_help():
     result = subprocess.run(
         args=[sys.executable, "-m", BACKEND_CALLER_MOD, "--help"],
         capture_output=True,
     )
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     assert result.stdout.rstrip().startswith(b"usage: backend_caller.py ")
     assert result.stderr == b""
 
 
 def test_invalid_hook_choice():
     invalid_hook = "invalid_hook_name"
@@ -131,15 +132,15 @@
     expected_err_msg = (
         "argument hook_name: invalid choice: '{}' (choose from {})\n"
     ).format(
         invalid_hook,
         ", ".join([f"{x!r}" for x in backend_caller.SUPPORTED_HOOKS]),
     )
 
-    assert result.returncode != 0
+    assert result.returncode
     assert expected_err_msg.encode("utf-8") in result.stderr
     assert result.stdout == b""
 
 
 def test_invalid_hook_args():
     with pytest.raises(
         ValueError,
@@ -216,14 +217,15 @@
 
             backend_caller.setup_logging(verbose=True)
             backend_caller.logger.{level}("{level}")
         """
     )
     cmd = [sys.executable, "-c", code]
     result = subprocess.run(args=cmd, capture_output=True)
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     if destination == "stderr":
         log_out = result.stderr
         log_no_out = result.stdout
     else:
         log_out = result.stdout
         log_no_out = result.stderr
@@ -458,14 +460,15 @@
     hook_result = backend_caller.call_hook(
         be.name,
         backend_path=None,
         hook=hook,
         hook_args=[str(wheeldir)],
         hook_kwargs={},
     )
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-string
     assert hook_result == ""
 
 
 def test_prepare_metadata_for_build_wheel(build_backend, wheeldir):
     be = build_backend("be")
     hook = "prepare_metadata_for_build_wheel"
     hook_result = backend_caller.call_hook(
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_build/test_builder.py` & `pyproject_installer-0.5.3/tests/unit/test_build/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,19 @@
 
     outdir = pyproject_path / "dist"
     outdir.mkdir()
 
     build_wheel(pyproject_path, outdir=outdir)
 
 
-@pytest.mark.skipif(os.geteuid() == 0, reason="Requires unprivileged user")
+@pytest.mark.skipif(
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
+    os.geteuid() == 0,
+    reason="Requires unprivileged user",
+)
 def test_uncreatable_outdir(mock_build, pyproject):
     """Check error if outdir is uncreatable(e.g. not enough permissions)"""
     pyproject_path = pyproject()
 
     outdir = Path("/uncreatable_dir")
     with pytest.raises(
         ValueError,
@@ -371,15 +375,19 @@
     assert not expected_outdir.exists()
 
     build_metadata(pyproject_path, outdir=outdir)
 
     assert expected_outdir.exists()
 
 
-@pytest.mark.skipif(os.geteuid() == 0, reason="Requires unprivileged user")
+@pytest.mark.skipif(
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
+    os.geteuid() == 0,
+    reason="Requires unprivileged user",
+)
 def test_metadata_uncreatable_outdir(pyproject_metadata):
     """Check error if outdir is uncreatable(e.g. not enough permissions)"""
     pyproject_path = pyproject_metadata()
 
     outdir = Path("/uncreatable_dir")
     with pytest.raises(
         ValueError,
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_build/test_pyproject_parser.py` & `pyproject_installer-0.5.3/tests/unit/test_build/test_pyproject_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for parser of pyproject.toml"""
+
 import json
 import textwrap
 import sys
 
 import pytest
 
 from pyproject_installer.build_cmd import build_wheel
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_deps/test_collectors.py` & `pyproject_installer-0.5.3/tests/unit/test_deps/test_collectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,24 +75,24 @@
         monkeypatch.chdir(tmpdir)
         return reqfile_path
 
     return _pip_reqfile
 
 
 @pytest.fixture
-def poetry_deps(tmpdir, monkeypatch):
-    """poetry deps"""
+def pipenv_deps(tmpdir, monkeypatch):
+    """pipenv deps"""
 
-    def _poetry_deps(content):
-        pyproject_toml_path = tmpdir / "pyproject.toml"
-        pyproject_toml_path.write_text(content, encoding="utf-8")
+    def _pipenv_deps(content):
+        pipfile_path = tmpdir / "Pipfile"
+        pipfile_path.write_text(content, encoding="utf-8")
         monkeypatch.chdir(tmpdir)
-        return pyproject_toml_path
+        return pipfile_path
 
-    return _poetry_deps
+    return _pipenv_deps
 
 
 @pytest.fixture
 def tox_deps(tmpdir, monkeypatch):
     """tox deps in specified format"""
 
     def _tox_deps(config_type, testenv, deps):
@@ -161,14 +161,27 @@
         config_path.write_text("\n".join(contents) + "\n", encoding="utf-8")
         monkeypatch.chdir(tmpdir)
         return config_path
 
     return _pdm_deps
 
 
+@pytest.fixture
+def poetry_deps(tmpdir, monkeypatch):
+    """poetry deps"""
+
+    def _poetry_deps(content):
+        pyproject_toml_path = tmpdir / "pyproject.toml"
+        pyproject_toml_path.write_text(content, encoding="utf-8")
+        monkeypatch.chdir(tmpdir)
+        return pyproject_toml_path
+
+    return _poetry_deps
+
+
 PEP508_DEPS_DATA = (
     ([], []),
     (["foo"], ["foo"]),
     (["foo == 1.0"], ["foo==1.0"]),
     (
         ["foo @ https://example.com/foo.zip"],
         ["foo@ https://example.com/foo.zip"],
@@ -974,7 +987,97 @@
     with pytest.raises(ValueError) as exc:
         deps_command("sync", depsconfig_path, srcnames=[])
     expected_err = f"Pdm dependencies are not configured for group: {group}"
     assert str(exc.value) == expected_err
 
     actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
     assert actual_conf == input_conf
+
+
+@pytest.mark.parametrize(
+    "deps_data",
+    (
+        ([], []),
+        (['_foo = "*"'], []),
+        (['foo = "*"'], ["foo"]),
+        (['foo = "1.0"'], ["foo"]),
+        (['foo = { git = "https://example.com/bar.git" }'], ["foo"]),
+        (['foo = { version = "1.0" }'], ["foo"]),
+        (
+            ['foo = { git = "https://example.com/bar.git", version = "1.0" }'],
+            ["foo"],
+        ),
+        (
+            ['foo = {version = "1.0", markers = "python_version <= \'3.4\'"}'],
+            ['foo; python_version <= "3.4"'],
+        ),
+        (
+            ['foo = {version = "1.0", markers = "invalid_marker == \'3.4\'"}'],
+            ["foo"],
+        ),
+        (['foo = "*"', 'bar = "*"'], ["bar", "foo"]),
+        (['bar = "*"', 'foo = "*"'], ["bar", "foo"]),
+        (['Foo = "*"'], ["Foo"]),
+        (['foo = "1.0"', 'bar = "1.0"'], ["bar", "foo"]),
+        (['foo = {version = "*", sys_platform = "== \'win32\'"}'], ["foo"]),
+    ),
+)
+def test_pipenv_collector(deps_data, pipenv_deps, depsconfig):
+    """Collection of pipenv deps"""
+    # prepare source config
+    srcname = "foo"
+    collector = "pipenv"
+    category = "packages"
+
+    in_reqs, out_reqs = deps_data
+
+    pipenv_content = f"[{category}]\n"
+    pipenv_content += "\n".join(in_reqs) + "\n"
+    pipenv_path = pipenv_deps(pipenv_content)
+
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(pipenv_path), category],
+            },
+        },
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    deps_command("sync", depsconfig_path, srcnames=[])
+
+    expected_conf = deepcopy(input_conf)
+    if out_reqs:
+        expected_conf["sources"][srcname]["deps"] = out_reqs
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == expected_conf
+
+
+def test_pipenv_collector_missing_category(pipenv_deps, depsconfig):
+    """Collection of pipenv's deps with missing category"""
+    # prepare source config
+    srcname = "foo"
+    collector = "pipenv"
+    category = "packages"
+
+    pipenv_path = pipenv_deps("\n")
+
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(pipenv_path), category],
+            },
+        },
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    with pytest.raises(ValueError) as exc:
+        deps_command("sync", depsconfig_path, srcnames=[])
+    expected_err = (
+        f"pipenv dependencies are not configured for category: {category}"
+    )
+    assert expected_err in str(exc.value)
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_deps/test_deps_config.py` & `pyproject_installer-0.5.3/tests/unit/test_deps/test_deps_config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.2/tests/unit/test_install/test_installer.py` & `pyproject_installer-0.5.3/tests/unit/test_install/test_installer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 import os
 import logging
+import shutil
 import sys
 import subprocess
 import sysconfig
+import textwrap
 
 import pytest
 
 from pyproject_installer.errors import WheelFileError
 from pyproject_installer.install_cmd import install_wheel
 from pyproject_installer.install_cmd._install import (
     get_installation_scheme,
@@ -39,14 +41,31 @@
             for f in files:
                 actual_filelist.add(Path(root) / f)
 
         return actual_filelist
 
 
 @pytest.fixture
+def compiled_binary(tmpdir):
+    gcc_exe = shutil.which("gcc")
+    if gcc_exe is None:
+        pytest.skip("Requires gcc to compile a test binary")
+
+    def _compiled_binary(exec_name, content):
+        output_bin = tmpdir / exec_name
+        source_c = tmpdir / f"{exec_name}.c"
+        source_c.write_text(content)
+        gcc_cmd = [gcc_exe, "-o", output_bin, source_c]
+        subprocess.check_call(gcc_cmd)
+        return output_bin
+
+    return _compiled_binary
+
+
+@pytest.fixture
 def installed_wheel(tmpdir):
     def _installed_wheel(*args, **kwargs):
         destdir = tmpdir / "destdir"
         destdir.mkdir()
         return InstalledWheel(destdir, *args, **kwargs)
 
     return _installed_wheel
@@ -75,15 +94,19 @@
     bad_whl.touch(exist_ok=False)
     with pytest.raises(
         WheelFileError, match=f"Error reading wheel {bad_whl}: "
     ):
         install_wheel(bad_whl, destdir=destdir)
 
 
-@pytest.mark.skipif(os.geteuid() == 0, reason="Requires unprivileged user")
+@pytest.mark.skipif(
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
+    os.geteuid() == 0,
+    reason="Requires unprivileged user",
+)
 def test_unaccessible_destdir(wheel):
     with pytest.raises(ValueError, match="Unable to create path for destdir"):
         install_wheel(wheel(), destdir=Path("/unaccessible/dest/dir"))
 
 
 @pytest.mark.parametrize(
     "wheel_name",
@@ -330,17 +353,17 @@
             wheel(contents=contents), destdir=installed_wheel().destdir
         )
 
 
 @pytest.mark.parametrize("ep_spec", ("foo", "foo.bar"))
 def test_invalid_entry_points(ep_spec, wheel_contents, wheel, installed_wheel):
     contents = wheel_contents()
-    contents[
-        "foo-1.0.dist-info/entry_points.txt"
-    ] = f"[console_scripts]\nbar = {ep_spec}\n"
+    contents["foo-1.0.dist-info/entry_points.txt"] = (
+        f"[console_scripts]\nbar = {ep_spec}\n"
+    )
     with pytest.raises(ValueError, match="Invalid entry_points specification"):
         install_wheel(
             wheel(contents=contents), destdir=installed_wheel().destdir
         )
 
 
 @pytest.mark.parametrize("purelib", (True, False), ids=("purelib", "platlib"))
@@ -406,17 +429,17 @@
 @pytest.mark.parametrize(
     "strip_dist_info", (None, True, False), ids=("default", "strip", "no_strip")
 )
 def test_installation_filelist(
     strip_dist_info, wheel_contents, wheel, installed_wheel
 ):
     contents = wheel_contents()
-    contents[
-        "foo-1.0.dist-info/entry_points.txt"
-    ] = "[console_scripts]\nbar = foo:main\n"
+    contents["foo-1.0.dist-info/entry_points.txt"] = (
+        "[console_scripts]\nbar = foo:main\n"
+    )
 
     dest_wheel = installed_wheel()
     kwargs = {"destdir": dest_wheel.destdir}
     if strip_dist_info is not None:
         kwargs["strip_dist_info"] = strip_dist_info
 
     install_wheel(wheel(contents=contents), **kwargs)
@@ -517,14 +540,49 @@
     install_wheel(wheel(contents=contents), destdir=dest_wheel.destdir)
     script = dest_wheel.scripts / "bar"
 
     expected_content = f"{expected_shebang}\nprint('Hello, World!')\n"
     assert script.read_text() == expected_content
 
     result = subprocess.run([script], capture_output=True)
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
+    assert result.returncode == 0
+    assert result.stdout == b"Hello, World!\n"
+    assert result.stderr == b""
+
+
+def test_data_binary_scripts(
+    compiled_binary, wheel_contents, wheel, installed_wheel
+):
+    """
+    Test that compiled binary can be executed on installation
+    """
+    binary_name = "foo_binary"
+    binary_path = compiled_binary(
+        binary_name,
+        textwrap.dedent(
+            """\
+            #include <stdio.h>
+            int main() {
+               printf("Hello, World!\\n");
+            }
+            """
+        ),
+    )
+
+    contents = wheel_contents()
+    contents[f"foo-1.0.data/scripts/{binary_name}"] = binary_path.read_bytes()
+
+    dest_wheel = installed_wheel()
+
+    install_wheel(wheel(contents=contents), destdir=dest_wheel.destdir)
+    script = dest_wheel.scripts / binary_name
+
+    result = subprocess.run([script], capture_output=True)
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     assert result.stdout == b"Hello, World!\n"
     assert result.stderr == b""
 
 
 @pytest.mark.parametrize(
     "sub_execs",
@@ -543,17 +601,17 @@
     mocker, sub_execs, wheel_contents, wheel, installed_wheel
 ):
     sys_exec, expected_shebang = sub_execs
     mocker.patch(
         "pyproject_installer.install_cmd._install.sys.executable", sys_exec
     )
     contents = wheel_contents()
-    contents[
-        "foo-1.0.dist-info/entry_points.txt"
-    ] = "[console_scripts]\nbar = foo:main\n"
+    contents["foo-1.0.dist-info/entry_points.txt"] = (
+        "[console_scripts]\nbar = foo:main\n"
+    )
 
     dest_wheel = installed_wheel()
 
     install_wheel(wheel(contents=contents), destdir=dest_wheel.destdir)
     script = dest_wheel.scripts / "bar"
 
     expected_content = SCRIPT_TEMPLATE.format(
@@ -562,10 +620,11 @@
     assert script.read_text() == expected_content
 
     new_env = os.environ.copy()
     new_env["PYTHONPATH"] = (
         str(dest_wheel.sitedir) + os.pathsep + new_env.get("PYTHONPATH", "")
     )
     result = subprocess.run([script], capture_output=True, env=new_env)
+    # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
     assert result.returncode == 0
     assert result.stdout == b"Hello, World!\n"
     assert result.stderr == b""
```

### Comparing `pyproject_installer-0.5.2/tests/unit/test_run/test_env.py` & `pyproject_installer-0.5.3/tests/unit/test_run/test_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         contents = wheel_contents(distr=distr)
         contents[f"{distr}/__init__.py"] = textwrap.dedent(
             f"""\
                 def main():
                     print("Hello, World! ({script_name})")
             """
         )
-        contents[
-            f"{contents.distinfo}/entry_points.txt"
-        ] = f"[console_scripts]\n{script_name} = {distr}:main\n"
+        contents[f"{contents.distinfo}/entry_points.txt"] = (
+            f"[console_scripts]\n{script_name} = {distr}:main\n"
+        )
 
         return wheel(name=f"{distr}-1.0-py3-none-any.whl", contents=contents)
 
     return _build_wheel
 
 
 @pytest.fixture
@@ -355,16 +355,16 @@
     for out in outs:
         assert f"Command's {out}:\n{out}\n" in str(exc.value)
 
     for noout in [x for x in ["stdout", "stderr"] if x not in outs]:
         assert f"Command's {noout}:\n" not in str(exc.value)
 
     captured = capfd.readouterr()
-    assert captured.out == ""
-    assert captured.err == ""
+    assert not captured.out
+    assert not captured.err
 
 
 @pytest.mark.parametrize(
     "outs",
     (["stdout"], ["stderr"], ["stdout", "stderr"]),
     ids=idf_outs,
 )
@@ -390,15 +390,15 @@
 
     assert "Command's std" not in str(exc.value)
 
     captured = capfd.readouterr()
     for out in outs:
         assert getattr(captured, out[3:]) == f"{out}\n"
     for noout in [x for x in ["stdout", "stderr"] if x not in outs]:
-        assert getattr(captured, noout[3:]) == ""
+        assert not getattr(captured, noout[3:])
 
 
 @pytest.mark.parametrize(
     "outs",
     (["stdout"], ["stderr"], ["stdout", "stderr"]),
     ids=idf_outs,
 )
@@ -422,16 +422,16 @@
     for out in outs:
         assert getattr(res, out).decode("utf-8") == f"{out}\n"
 
     for noout in [x for x in ["stdout", "stderr"] if x not in outs]:
         assert getattr(res, noout) == b""
 
     captured = capfd.readouterr()
-    assert captured.out == ""
-    assert captured.err == ""
+    assert not captured.out
+    assert not captured.err
 
 
 @pytest.mark.parametrize(
     "outs",
     (["stdout"], ["stderr"], ["stdout", "stderr"]),
     ids=idf_outs,
 )
@@ -455,15 +455,15 @@
     assert res.stdout is None
     assert res.stderr is None
 
     captured = capfd.readouterr()
     for out in outs:
         assert getattr(captured, out[3:]) == f"{out}\n"
     for noout in [x for x in ["stdout", "stderr"] if x not in outs]:
-        assert getattr(captured, noout[3:]) == ""
+        assert not getattr(captured, noout[3:])
 
 
 @pytest.fixture(
     params=(x for x in product(range(2), repeat=3) if x != (0, 0, 0)),
     ids=idf_console_data,
 )
 def console_scripts_data(request, mock_ssps, mock_usps):
@@ -539,14 +539,15 @@
         if pythonpath:
             m.setenv("PYTHONPATH", pythonpath, prepend=os.pathsep)
         res = run_command(
             vsp_wheel,
             command=[command],
             capture_output=True,
         )
+        # pylint: disable-next=use-implicit-booleaness-not-comparison-to-zero
         assert res.returncode == 0
         expected_out = f"Hello, World! ({command})"
         assert res.stdout.strip().decode("utf-8") == expected_out
         assert res.stderr == b""
 
     expected_fails = [
         console_scripts_data[ps]
```

### Comparing `pyproject_installer-0.5.2/PKG-INFO` & `pyproject_installer-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-installer
-Version: 0.5.2
+Version: 0.5.3
 Summary: Pyproject installer
 Author-email: Stanislav Levin <slev@altlinux.org>
 License: MIT
 Project-URL: source,https://github.com/stanislavlevin/pyproject_installer
 Project-URL: tracker,https://github.com/stanislavlevin/pyproject_installer/issues
 Keywords: packaging,PEP517,build,install
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # pyproject-installer
 
 This tool is intended for build, install, run or management of dependencies
@@ -258,26 +259,26 @@
 <em><strong>example</strong></em>: python -m pyproject_installer deps show build
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: add
-<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox, poetry, hatch or pdm have limited support.
+<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox, poetry, hatch, pdm or pipenv have limited support.
 <em><strong>example</strong></em>: python -m pyproject_installer deps add --help
 </pre>
 
 Positional arguments:
 <pre>
 <em><strong>description</strong></em>: source name
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: source type
-<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox, hatch, pdm
+<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox, hatch, pdm, pipenv
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: specific configuration options for source
 <em><strong>default</strong></em>: []
 </pre>
 
@@ -302,14 +303,17 @@
 python -m pyproject_installer deps add check poetry dev
 
 Configuration of source of <strong>hatch</strong> requirements:
 python -m pyproject_installer deps add check hatch hatch.toml test
 
 Configuration of source of <strong>pdm</strong> requirements:
 python -m pyproject_installer deps add check pdm test
+
+Configuration of source of <strong>pipenv</strong> requirements:
+python -m pyproject_installer deps add check pipenv Pipfile packages
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: sync
 <em><strong>description</strong></em>: sync stored requirements to configured sources
```

### Comparing `pyproject_installer-0.5.2/pyproject.toml` & `pyproject_installer-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "Operating System :: Unix",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries",
 ]
 dynamic = ["version"]
 
 [project.urls]
 source = "https://github.com/stanislavlevin/pyproject_installer"
 tracker = "https://github.com/stanislavlevin/pyproject_installer/issues"
```

### Comparing `pyproject_installer-0.5.2/README.md` & `pyproject_installer-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -235,26 +235,26 @@
 <em><strong>example</strong></em>: python -m pyproject_installer deps show build
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: add
-<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox, poetry, hatch or pdm have limited support.
+<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox, poetry, hatch, pdm or pipenv have limited support.
 <em><strong>example</strong></em>: python -m pyproject_installer deps add --help
 </pre>
 
 Positional arguments:
 <pre>
 <em><strong>description</strong></em>: source name
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: source type
-<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox, hatch, pdm
+<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox, hatch, pdm, pipenv
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: specific configuration options for source
 <em><strong>default</strong></em>: []
 </pre>
 
@@ -279,14 +279,17 @@
 python -m pyproject_installer deps add check poetry dev
 
 Configuration of source of <strong>hatch</strong> requirements:
 python -m pyproject_installer deps add check hatch hatch.toml test
 
 Configuration of source of <strong>pdm</strong> requirements:
 python -m pyproject_installer deps add check pdm test
+
+Configuration of source of <strong>pipenv</strong> requirements:
+python -m pyproject_installer deps add check pipenv Pipfile packages
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: sync
 <em><strong>description</strong></em>: sync stored requirements to configured sources
```

### Comparing `pyproject_installer-0.5.2/LICENSE` & `pyproject_installer-0.5.3/LICENSE`

 * *Files identical despite different names*

