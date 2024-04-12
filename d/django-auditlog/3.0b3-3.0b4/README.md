# Comparing `tmp/django-auditlog-3.0b3.tar.gz` & `tmp/django-auditlog-3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-auditlog-3.0b3.tar", last modified: Mon Nov 20 08:17:25 2023, max compression
+gzip compressed data, was "django-auditlog-3.0b4.tar", last modified: Thu Jan  4 08:48:33 2024, max compression
```

## Comparing `django-auditlog-3.0b3.tar` & `django-auditlog-3.0b4.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.814740 django-auditlog-3.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.798740 django-auditlog-3.0b3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.802740 django-auditlog-3.0b3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14204 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2023-11-20 08:17:25.814740 django-auditlog-3.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.806740 django-auditlog-3.0b3/auditlog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/cid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.806740 django-auditlog-3.0b3/auditlog/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.806740 django-auditlog-3.0b3/auditlog/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/management/commands/auditlogflush.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/management/commands/auditlogmigratejson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.806740 django-auditlog-3.0b3/auditlog/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0002_auto_support_long_primary_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0003_logentry_remote_addr.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0004_logentry_detailed_object_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0005_logentry_additional_data_verbose_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0006_object_pk_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0007_object_pk_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0008_action_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0009_alter_logentry_additional_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0010_alter_logentry_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0011_logentry_serialized_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0012_add_logentry_action_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0013_alter_logentry_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0014_logentry_cid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/0015_alter_logentry_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    22714 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/receivers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.810740 django-auditlog-3.0b3/auditlog_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.810740 django-auditlog-3.0b3/auditlog_tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/fixtures/custom_get_cid.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/fixtures/m2m_test_fixture.json
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.810740 django-auditlog-3.0b3/auditlog_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/templates/simplemodel_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/test_two_step_json_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    93302 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/auditlog_tests/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.810740 django-auditlog-3.0b3/django_auditlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2023-11-20 08:17:25.000000 django-auditlog-3.0b3/django_auditlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-11-20 08:17:25.000000 django-auditlog-3.0b3/django_auditlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 08:17:25.000000 django-auditlog-3.0b3/django_auditlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 08:17:25.000000 django-auditlog-3.0b3/django_auditlog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-20 08:17:25.000000 django-auditlog-3.0b3/django_auditlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-20 08:17:25.000000 django-auditlog-3.0b3/django_auditlog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.810740 django-auditlog-3.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 08:17:25.814740 django-auditlog-3.0b3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/source/internals.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/source/upgrade.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17029 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 08:17:25.814740 django-auditlog-3.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-11-20 08:17:07.000000 django-auditlog-3.0b3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.325378 django-auditlog-3.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.309378 django-auditlog-3.0b4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.313378 django-auditlog-3.0b4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14792 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-01-04 08:48:33.325378 django-auditlog-3.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.317378 django-auditlog-3.0b4/auditlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/cid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.317378 django-auditlog-3.0b4/auditlog/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.317378 django-auditlog-3.0b4/auditlog/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/management/commands/auditlogflush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/management/commands/auditlogmigratejson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.321378 django-auditlog-3.0b4/auditlog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0002_auto_support_long_primary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0003_logentry_remote_addr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0004_logentry_detailed_object_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0005_logentry_additional_data_verbose_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0006_object_pk_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0007_object_pk_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0008_action_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0009_alter_logentry_additional_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0010_alter_logentry_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0011_logentry_serialized_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0012_add_logentry_action_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0013_alter_logentry_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0014_logentry_cid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/0015_alter_logentry_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23063 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.321378 django-auditlog-3.0b4/auditlog_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.321378 django-auditlog-3.0b4/auditlog_tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/fixtures/custom_get_cid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/fixtures/m2m_test_fixture.json
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10091 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.321378 django-auditlog-3.0b4/auditlog_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/templates/simplemodel_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/test_two_step_json_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95274 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/auditlog_tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.325378 django-auditlog-3.0b4/django_auditlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-01-04 08:48:33.000000 django-auditlog-3.0b4/django_auditlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-01-04 08:48:33.000000 django-auditlog-3.0b4/django_auditlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 08:48:33.000000 django-auditlog-3.0b4/django_auditlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 08:48:33.000000 django-auditlog-3.0b4/django_auditlog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-04 08:48:33.000000 django-auditlog-3.0b4/django_auditlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-04 08:48:33.000000 django-auditlog-3.0b4/django_auditlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.325378 django-auditlog-3.0b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 08:48:33.325378 django-auditlog-3.0b4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/source/internals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/source/upgrade.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17029 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 08:48:33.325378 django-auditlog-3.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-04 08:48:13.000000 django-auditlog-3.0b4/tox.ini
```

### Comparing `django-auditlog-3.0b3/.github/workflows/release.yml` & `django-auditlog-3.0b4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/.github/workflows/test.yml` & `django-auditlog-3.0b4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/.gitignore` & `django-auditlog-3.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/.pre-commit-config.yaml` & `django-auditlog-3.0b4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 ---
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.10.1
+    rev: 23.12.1
     hooks:
       - id: black
         language_version: python3.8
         args:
           - "--target-version"
           - "py38"
   - repo: https://github.com/PyCQA/flake8
     rev: "6.1.0"
     hooks:
       - id: flake8
         args: ["--max-line-length", "110"]
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.0
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
```

### Comparing `django-auditlog-3.0b3/.readthedocs.yaml` & `django-auditlog-3.0b4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/CHANGELOG.md` & `django-auditlog-3.0b4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 # Changes
 
 ## Next Release
 
+## 3.0.0-beta.4 (2024-01-02)
+
+#### Improvements
+- feat: If any receiver returns False, no logging will be made. This can be useful if logging should be conditionally enabled / disabled ([#590](https://github.com/jazzband/django-auditlog/pull/590))
+- Django: Confirm Django 5.0 support ([#598](https://github.com/jazzband/django-auditlog/pull/598))
+- Django: Drop Django 4.1 support ([#598](https://github.com/jazzband/django-auditlog/pull/598))
+
 ## 3.0.0-beta.3 (2023-11-13)
 
 #### Improvements
 
 - Python: Confirm Python 3.12 support ([#572](https://github.com/jazzband/django-auditlog/pull/572))
 - feat: `thread.local` replaced with `ContextVar` to improve context managers in Django 4.2+
 
+#### Fixes
+
+- fix: Handle `ObjectDoesNotExist` in evaluation of `object_repr` ([#592](https://github.com/jazzband/django-auditlog/pull/592))
+
 ## 3.0.0-beta.2 (2023-10-05)
 
 #### Breaking Changes
 - feat: stop deleting old log entries when a model with the same pk is created (i.e. the pk value is reused) ([#559](https://github.com/jazzband/django-auditlog/pull/559))
 
 #### Fixes
 * fix: only fire the `post_log` signal when the log is created or when there is an error in the process ([#561](https://github.com/jazzband/django-auditlog/pull/561))
```

### Comparing `django-auditlog-3.0b3/CODE_OF_CONDUCT.md` & `django-auditlog-3.0b4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/LICENSE` & `django-auditlog-3.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/PKG-INFO` & `django-auditlog-3.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auditlog
-Version: 3.0b3
+Version: 3.0b4
 Summary: Audit log app for Django
 Home-page: https://github.com/jazzband/django-auditlog
 Author: Jan-Jelle Kester
 License: MIT
 Project-URL: Documentation, https://django-auditlog.readthedocs.io
 Project-URL: Source, https://github.com/jazzband/django-auditlog
 Project-URL: Tracker, https://github.com/jazzband/django-auditlog/issues
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.2
 Requires-Dist: python-dateutil>=2.7.0
```

### Comparing `django-auditlog-3.0b3/README.md` & `django-auditlog-3.0b4/README.md`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/admin.py` & `django-auditlog-3.0b4/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/cid.py` & `django-auditlog-3.0b4/auditlog/cid.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/conf.py` & `django-auditlog-3.0b4/auditlog/conf.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/context.py` & `django-auditlog-3.0b4/auditlog/context.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/diff.py` & `django-auditlog-3.0b4/auditlog/diff.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/filters.py` & `django-auditlog-3.0b4/auditlog/filters.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/management/commands/auditlogflush.py` & `django-auditlog-3.0b4/auditlog/management/commands/auditlogflush.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/management/commands/auditlogmigratejson.py` & `django-auditlog-3.0b4/auditlog/management/commands/auditlogmigratejson.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/middleware.py` & `django-auditlog-3.0b4/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/migrations/0001_initial.py` & `django-auditlog-3.0b4/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/migrations/0012_add_logentry_action_access.py` & `django-auditlog-3.0b4/auditlog/migrations/0012_add_logentry_action_access.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/migrations/0013_alter_logentry_timestamp.py` & `django-auditlog-3.0b4/auditlog/migrations/0013_alter_logentry_timestamp.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/migrations/0014_logentry_cid.py` & `django-auditlog-3.0b4/auditlog/migrations/0014_logentry_cid.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/migrations/0015_alter_logentry_changes.py` & `django-auditlog-3.0b4/auditlog/migrations/0015_alter_logentry_changes.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/mixins.py` & `django-auditlog-3.0b4/auditlog/mixins.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/models.py` & `django-auditlog-3.0b4/auditlog/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from django.utils import formats
 from django.utils import timezone as django_timezone
 from django.utils.encoding import smart_str
 from django.utils.translation import gettext_lazy as _
 
 from auditlog.diff import mask_str
 
+DEFAULT_OBJECT_REPR = "<error forming object repr>"
+
 
 class LogEntryManager(models.Manager):
     """
     Custom manager for the :py:class:`LogEntry` model.
     """
 
     def log_create(self, instance, force_log: bool = False, **kwargs):
@@ -50,15 +52,19 @@
         pk = self._get_pk_value(instance)
 
         if changes is not None or force_log:
             kwargs.setdefault(
                 "content_type", ContentType.objects.get_for_model(instance)
             )
             kwargs.setdefault("object_pk", pk)
-            kwargs.setdefault("object_repr", smart_str(instance))
+            try:
+                object_repr = smart_str(instance)
+            except ObjectDoesNotExist:
+                object_repr = DEFAULT_OBJECT_REPR
+            kwargs.setdefault("object_repr", object_repr)
             kwargs.setdefault(
                 "serialized_data", self._get_serialized_data_or_none(instance)
             )
 
             if isinstance(pk, int):
                 kwargs.setdefault("object_id", pk)
 
@@ -92,15 +98,19 @@
 
         pk = self._get_pk_value(instance)
         if changed_queryset:
             kwargs.setdefault(
                 "content_type", ContentType.objects.get_for_model(instance)
             )
             kwargs.setdefault("object_pk", pk)
-            kwargs.setdefault("object_repr", smart_str(instance))
+            try:
+                object_repr = smart_str(instance)
+            except ObjectDoesNotExist:
+                object_repr = DEFAULT_OBJECT_REPR
+            kwargs.setdefault("object_repr", object_repr)
             kwargs.setdefault("action", LogEntry.Action.UPDATE)
 
             if isinstance(pk, int):
                 kwargs.setdefault("object_id", pk)
 
             get_additional_data = getattr(instance, "get_additional_data", None)
             if callable(get_additional_data):
```

### Comparing `django-auditlog-3.0b3/auditlog/receivers.py` & `django-auditlog-3.0b4/auditlog/receivers.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,18 @@
     action, instance, sender, diff_old, diff_new, fields_to_check=None, force_log=False
 ):
     pre_log_results = pre_log.send(
         sender,
         instance=instance,
         action=action,
     )
+
+    if any(item[1] is False for item in pre_log_results):
+        return
+
     error = None
     log_created = False
     changes = None
     try:
         changes = model_instance_diff(
             diff_old, diff_new, fields_to_check=fields_to_check
         )
```

### Comparing `django-auditlog-3.0b3/auditlog/registry.py` & `django-auditlog-3.0b4/auditlog/registry.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog/signals.py` & `django-auditlog-3.0b4/auditlog/signals.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     The actual instance that's being audited.
 
 :param Action action:
     The action on the model resulting in an
     audit log entry. Type: :class:`auditlog.models.LogEntry.Action`
 
 The receivers' return values are sent to any :func:`post_log`
-signal receivers.
+signal receivers, with one exception: if any receiver returns False,
+no logging will be made. This can be useful if logging should be
+conditionally enabled / disabled
 """
 
 post_log = django.dispatch.Signal()
 """
 Whenever an audit log entry is written, this signal
 is sent after writing the log.
 This signal is also fired when there is an error in creating the log.
```

### Comparing `django-auditlog-3.0b3/auditlog_tests/models.py` & `django-auditlog-3.0b4/auditlog_tests/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,17 @@
     )
     one_to_one = models.OneToOneField(
         to="SimpleModel", on_delete=models.CASCADE, related_name="reverse_one_to_one"
     )
 
     history = AuditlogHistoryField(delete_related=True)
 
+    def __str__(self):
+        return f"RelatedModel #{self.pk} -> {self.related.id}"
+
 
 class ManyRelatedModel(models.Model):
     """
     A model with many-to-many relations.
     """
 
     recursive = models.ManyToManyField("self")
```

### Comparing `django-auditlog-3.0b3/auditlog_tests/test_commands.py` & `django-auditlog-3.0b4/auditlog_tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog_tests/test_settings.py` & `django-auditlog-3.0b4/auditlog_tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog_tests/test_two_step_json_migration.py` & `django-auditlog-3.0b4/auditlog_tests/test_two_step_json_migration.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/auditlog_tests/tests.py` & `django-auditlog-3.0b4/auditlog_tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from django.utils.encoding import smart_str
 
 from auditlog.admin import LogEntryAdmin
 from auditlog.cid import get_cid
 from auditlog.context import disable_auditlog, set_actor
 from auditlog.diff import model_instance_diff
 from auditlog.middleware import AuditlogMiddleware
-from auditlog.models import LogEntry
+from auditlog.models import DEFAULT_OBJECT_REPR, LogEntry
 from auditlog.registry import AuditlogModelRegistry, AuditLogRegistrationError, auditlog
 from auditlog.signals import post_log, pre_log
 from auditlog_tests.fixtures.custom_get_cid import get_cid as custom_get_cid
 from auditlog_tests.models import (
     AdditionalDataIncludedModel,
     AltPrimaryKeyModel,
     AutoManyRelatedModel,
@@ -432,14 +432,23 @@
             },
         )
         # Add same related obj again.
         self.obj.related.add(self.related)
         latest_log_entry = self.obj.history.first()
         self.assertEqual(log_entry.id, latest_log_entry.id)
 
+    def test_object_repr_related_deleted(self):
+        """No error is raised when __str__() raises ObjectDoesNotExist."""
+        # monkey-patching to avoid extra logic in the model
+        with mock.patch.object(self.obj.__class__, "__str__") as mock_str:
+            mock_str.side_effect = self.related.DoesNotExist("I am fake")
+            self.obj.related.add(self.related)
+            log_entry = self.obj.history.first()
+            self.assertEqual(log_entry.object_repr, DEFAULT_OBJECT_REPR)
+
 
 class MiddlewareTest(TestCase):
     """
     Test the middleware responsible for connecting and disconnecting the signals used in automatic logging.
     """
 
     def setUp(self):
@@ -1856,14 +1865,33 @@
         # simple2 DOES have these relations
         self.assertEqual(simple2.reverse_one_to_one, related)
         self.assertEqual(simple2.related_models.count(), 1)
 
         model_instance_diff(simple2, simple1)
         model_instance_diff(simple1, simple2)
 
+    def test_object_repr_related_deleted(self):
+        """No error is raised when __str__() loads a related object that has been deleted."""
+        simple = SimpleModel()
+        simple.save()
+        related = RelatedModel(related=simple, one_to_one=simple)
+        related.save()
+        related_id = related.id
+
+        related.refresh_from_db()
+        simple.delete()
+        related.delete()
+
+        log_entry = (
+            LogEntry.objects.get_for_model(RelatedModel)
+            .filter(object_id=related_id)
+            .get(action=LogEntry.Action.DELETE)
+        )
+        self.assertEqual(log_entry.object_repr, DEFAULT_OBJECT_REPR)
+
     def test_when_field_doesnt_exist(self):
         """No error is raised and the default is returned."""
         first = SimpleModel(boolean=True)
         second = SimpleModel()
 
         # then boolean should be False, as we use the default value
         # specified inside the model
@@ -2416,14 +2444,41 @@
         pre_log.connect(pre_log_receiver_extra)
         post_log.connect(post_log_receiver)
 
         self.obj = SimpleModel.objects.create(text="I am not difficult.")
 
         self.assertSignals(LogEntry.Action.CREATE)
 
+    def test_disabled_logging(self):
+        log_count = LogEntry.objects.count()
+
+        def pre_log_receiver(sender, instance, action, **_kwargs):
+            return True
+
+        def pre_log_receiver_extra(*_args, **_kwargs):
+            pass
+
+        def pre_log_receiver_disable(*_args, **_kwargs):
+            return False
+
+        pre_log.connect(pre_log_receiver)
+        pre_log.connect(pre_log_receiver_extra)
+
+        self.obj = SimpleModel.objects.create(text="I am not difficult.")
+
+        self.assertEqual(LogEntry.objects.count(), log_count + 1)
+
+        log_count = LogEntry.objects.count()
+
+        pre_log.connect(pre_log_receiver_disable)
+
+        self.obj = SimpleModel.objects.create(text="I am not difficult.")
+
+        self.assertEqual(LogEntry.objects.count(), log_count)
+
     def test_custom_signals_update(self):
         def pre_log_receiver(sender, instance, action, **_kwargs):
             self.my_pre_log_data["is_called"] = True
             self.my_pre_log_data["my_sender"] = sender
             self.my_pre_log_data["my_instance"] = instance
             self.my_pre_log_data["my_action"] = action
```

### Comparing `django-auditlog-3.0b3/django_auditlog.egg-info/PKG-INFO` & `django-auditlog-3.0b4/django_auditlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-auditlog
-Version: 3.0b3
+Version: 3.0b4
 Summary: Audit log app for Django
 Home-page: https://github.com/jazzband/django-auditlog
 Author: Jan-Jelle Kester
 License: MIT
 Project-URL: Documentation, https://django-auditlog.readthedocs.io
 Project-URL: Source, https://github.com/jazzband/django-auditlog
 Project-URL: Tracker, https://github.com/jazzband/django-auditlog/issues
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.2
 Requires-Dist: python-dateutil>=2.7.0
```

### Comparing `django-auditlog-3.0b3/django_auditlog.egg-info/SOURCES.txt` & `django-auditlog-3.0b4/django_auditlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/Makefile` & `django-auditlog-3.0b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/make.bat` & `django-auditlog-3.0b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/source/conf.py` & `django-auditlog-3.0b4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/source/index.rst` & `django-auditlog-3.0b4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/source/installation.rst` & `django-auditlog-3.0b4/docs/source/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 Instead of installing Auditlog via PyPI, you can also clone the Git repository or download the source code via GitHub.
 The repository can be found at https://github.com/jazzband/django-auditlog/.
 
 **Requirements**
 
 - Python 3.8 or higher
-- Django 3.2, 4.1 and 4.2
+- Django 3.2, 4.2 and 5.0
 
-Auditlog is currently tested with Python 3.8+ and Django 3.2, 4.1 and 4.2. The latest test report can be found
+Auditlog is currently tested with Python 3.8+ and Django 3.2, 4.2 and 5.0. The latest test report can be found
 at https://github.com/jazzband/django-auditlog/actions.
 
 Adding Auditlog to your Django application
 ------------------------------------------
 
 To use Auditlog in your application, just add ``'auditlog'`` to your project's ``INSTALLED_APPS`` setting and run
 ``manage.py migrate`` to create/upgrade the necessary database structure.
```

### Comparing `django-auditlog-3.0b3/docs/source/internals.rst` & `django-auditlog-3.0b4/docs/source/internals.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/source/upgrade.rst` & `django-auditlog-3.0b4/docs/source/upgrade.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/docs/source/usage.rst` & `django-auditlog-3.0b4/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `django-auditlog-3.0b3/setup.py` & `django-auditlog-3.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,12 +35,12 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "License :: OSI Approved :: MIT License",
     ],
 )
```

### Comparing `django-auditlog-3.0b3/tox.ini` & `django-auditlog-3.0b4/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tox]
 envlist =
     {py38,py39,py310}-django32
-    {py38,py39,py310,py311}-django{41,42}
-    {py310,py311,py312}-djangomain
+    {py38,py39,py310,py311}-django42
+    {py310,py311,py312}-django{50,main}
     py38-docs
     py38-lint
 
 [testenv]
 setenv =
   COVERAGE_FILE={toxworkdir}/.coverage.{envname}
 commands =
     coverage run --source auditlog runtests.py
     coverage xml
 deps =
     django32: Django>=3.2,<3.3
-    django41: Django>=4.1,<4.2
     django42: Django>=4.2,<4.3
+    django50: Django>=5.0,<5.1
     djangomain: https://github.com/django/django/archive/main.tar.gz
     # Test requirements
     coverage
     codecov
     freezegun
     psycopg2-binary
 passenv=
```

