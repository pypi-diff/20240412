# Comparing `tmp/exasol_script_languages_container_ci_setup-1.2.0.tar.gz` & `tmp/exasol_script_languages_container_ci_setup-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_script_languages_container_ci_setup-1.2.0.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_ci_setup-1.2.1.tar", max compression
```

## Comparing `exasol_script_languages_container_ci_setup-1.2.0.tar` & `exasol_script_languages_container_ci_setup-1.2.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1063 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/LICENSE
--rw-r--r--   0        0        0      376 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/__init__.py
--rw-r--r--   0        0        0       50 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/cli.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/__init__.py
--rw-r--r--   0        0        0     1264 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py
--rw-r--r--   0        0        0     1261 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py
--rw-r--r--   0        0        0     1484 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py
--rw-r--r--   0        0        0     1508 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py
--rw-r--r--   0        0        0     1542 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py
--rw-r--r--   0        0        0     1205 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/health.py
--rw-r--r--   0        0        0     1590 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py
--rw-r--r--   0        0        0     2225 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py
--rw-r--r--   0        0        0     2554 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py
--rw-r--r--   0        0        0     1108 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py
--rw-r--r--   0        0        0     1128 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py
--rw-r--r--   0        0        0     1471 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py
--rw-r--r--   0        0        0      173 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/common.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/options/__init__.py
--rw-r--r--   0        0        0      148 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/options/aws_options.py
--rw-r--r--   0        0        0      727 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/options/logging.py
--rw-r--r--   0        0        0     3173 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/health_check.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/__init__.py
--rw-r--r--   0        0        0     8175 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/aws_access.py
--rw-r--r--   0        0        0     8752 2023-07-05 08:52:07.323896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/deployer.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/__init__.py
--rw-r--r--   0        0        0     2023 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/aws_client.py
--rw-r--r--   0        0        0     1958 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/cloudformation_service.py
--rw-r--r--   0        0        0     1750 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/codebuild_service.py
--rw-r--r--   0        0        0        0 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/__init__.py
--rw-r--r--   0        0        0     2973 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/cloudformation.py
--rw-r--r--   0        0        0     1881 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/codebuild.py
--rw-r--r--   0        0        0      683 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/common.py
--rw-r--r--   0        0        0      509 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/secretsmanager.py
--rw-r--r--   0        0        0      882 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/secretsmanager_service.py
--rw-r--r--   0        0        0     1976 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/ci_build.py
--rw-r--r--   0        0        0     2827 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py
--rw-r--r--   0        0        0      716 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py
--rw-r--r--   0        0        0     1711 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/release_build.py
--rw-r--r--   0        0        0      327 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/render_template.py
--rw-r--r--   0        0        0      950 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py
--rw-r--r--   0        0        0      971 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py
--rw-r--r--   0        0        0     7640 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/run_start_build.py
--rw-r--r--   0        0        0     1584 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/source_credentials.py
--rwxr-xr-x   0        0        0      131 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/main.py
--rw-r--r--   0        0        0     2265 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml
--rw-r--r--   0        0        0      237 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/buildspec_batch_entry.yaml
--rw-r--r--   0        0        0      222 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/buildspec_hull.yaml
--rw-r--r--   0        0        0      950 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/config_schema.json
--rw-r--r--   0        0        0     1354 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml
--rw-r--r--   0        0        0     4094 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml
--rw-r--r--   0        0        0     3926 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml
--rw-r--r--   0        0        0      359 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/slc_source_credential.yaml
--rw-r--r--   0        0        0      771 2023-07-05 08:52:07.327896 exasol_script_languages_container_ci_setup-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci_setup-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/LICENSE
+-rw-r--r--   0        0        0      376 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1264 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py
+-rw-r--r--   0        0        0     1261 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py
+-rw-r--r--   0        0        0     1484 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py
+-rw-r--r--   0        0        0     1508 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py
+-rw-r--r--   0        0        0     1542 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py
+-rw-r--r--   0        0        0     1205 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/health.py
+-rw-r--r--   0        0        0     1590 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py
+-rw-r--r--   0        0        0     2225 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py
+-rw-r--r--   0        0        0     2554 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py
+-rw-r--r--   0        0        0     1108 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py
+-rw-r--r--   0        0        0     1128 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py
+-rw-r--r--   0        0        0     1471 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py
+-rw-r--r--   0        0        0      173 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/common.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/options/__init__.py
+-rw-r--r--   0        0        0      148 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/options/aws_options.py
+-rw-r--r--   0        0        0      727 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/options/logging.py
+-rw-r--r--   0        0        0     3173 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/health_check.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/__init__.py
+-rw-r--r--   0        0        0     8175 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/aws_access.py
+-rw-r--r--   0        0        0     8752 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/deployer.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/__init__.py
+-rw-r--r--   0        0        0     2023 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/aws_client.py
+-rw-r--r--   0        0        0     1958 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/cloudformation_service.py
+-rw-r--r--   0        0        0     1750 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/codebuild_service.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/__init__.py
+-rw-r--r--   0        0        0     2973 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/cloudformation.py
+-rw-r--r--   0        0        0     1881 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/codebuild.py
+-rw-r--r--   0        0        0      683 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/common.py
+-rw-r--r--   0        0        0      509 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/secretsmanager.py
+-rw-r--r--   0        0        0      882 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/secretsmanager_service.py
+-rw-r--r--   0        0        0     1976 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/ci_build.py
+-rw-r--r--   0        0        0     2827 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py
+-rw-r--r--   0        0        0      716 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py
+-rw-r--r--   0        0        0     1711 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/release_build.py
+-rw-r--r--   0        0        0      327 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/render_template.py
+-rw-r--r--   0        0        0      950 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py
+-rw-r--r--   0        0        0      971 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py
+-rw-r--r--   0        0        0     7640 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/run_start_build.py
+-rw-r--r--   0        0        0     1584 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/source_credentials.py
+-rwxr-xr-x   0        0        0      131 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/main.py
+-rw-r--r--   0        0        0     2265 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml
+-rw-r--r--   0        0        0      237 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/buildspec_batch_entry.yaml
+-rw-r--r--   0        0        0      222 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/buildspec_hull.yaml
+-rw-r--r--   0        0        0      950 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/config_schema.json
+-rw-r--r--   0        0        0     1354 2024-04-12 10:17:59.032101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml
+-rw-r--r--   0        0        0     4094 2024-04-12 10:17:59.036101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml
+-rw-r--r--   0        0        0     3926 2024-04-12 10:17:59.036101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml
+-rw-r--r--   0        0        0      359 2024-04-12 10:17:59.036101 exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/slc_source_credential.yaml
+-rw-r--r--   0        0        0      771 2024-04-12 10:17:59.036101 exasol_script_languages_container_ci_setup-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 exasol_script_languages_container_ci_setup-1.2.1/PKG-INFO
```

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/LICENSE` & `exasol_script_languages_container_ci_setup-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/deploy_ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/deploy_release_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/deploy_source_credentials.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/generate_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/generate_release_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/health.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/health.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/start_ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/start_release_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/start_test_release_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/validate_ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/validate_release_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/commands/validate_source_credentials.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/cli/options/logging.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/cli/options/logging.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/health_check.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/health_check.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/aws_access.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/aws_access.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/deployer.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/deployer.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/aws_client.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/aws_client.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/cloudformation_service.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/cloudformation_service.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/codebuild_service.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/codebuild_service.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/cloudformation.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/cloudformation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/codebuild.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/codebuild.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/common.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/datamodels/common.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/aws/wrapper/secretsmanager_service.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/aws/wrapper/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/ci_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/ci_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/generate_buildspec_common.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/github_draft_release_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/release_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/release_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/run_generate_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/run_generate_release_buildspec.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/run_start_build.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/run_start_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/lib/source_credentials.py` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/lib/source_credentials.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/build_buildspec.yaml`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/config_schema.json` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/config_schema.json`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/release_build_buildspec.yaml`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/slc_code_build.yaml`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml` & `exasol_script_languages_container_ci_setup-1.2.1/exasol_script_languages_container_ci_setup/templates/slc_code_release_build.yaml`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/pyproject.toml` & `exasol_script_languages_container_ci_setup-1.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "exasol-script-languages-container-ci-setup"
-version = "1.2.0"
+version = "1.2.1"
 description = "Manages AWS cloud CI build infrastructure."
 
 license = "MIT"
 
 authors = [
     "Thomas Uebensee <ext.thomas.uebensee@exasol.com>"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4.0"
 click = "^8.1.3"
 jinja2 = ">=3.1.0"
 exasol_error_reporting_python = "^0.3.0"
-exasol-script-languages-container-ci = "^1.3.0"
+exasol-script-languages-container-ci = "^1.3.4"
 boto3 = "1.26.163"
 botocore = "1.29.163"
 jsonschema = "^4.17.3"
 PyGithub = "^1.55.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
```

### Comparing `exasol_script_languages_container_ci_setup-1.2.0/PKG-INFO` & `exasol_script_languages_container_ci_setup-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-ci-setup
-Version: 1.2.0
+Version: 1.2.1
 Summary: Manages AWS cloud CI build infrastructure.
 License: MIT
 Author: Thomas Uebensee
 Author-email: ext.thomas.uebensee@exasol.com
 Requires-Python: >=3.8.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,11 +12,11 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (>=1.55.0,<2.0.0)
 Requires-Dist: boto3 (==1.26.163)
 Requires-Dist: botocore (==1.29.163)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: exasol-script-languages-container-ci (>=1.3.0,<2.0.0)
+Requires-Dist: exasol-script-languages-container-ci (>=1.3.4,<2.0.0)
 Requires-Dist: exasol_error_reporting_python (>=0.3.0,<0.4.0)
 Requires-Dist: jinja2 (>=3.1.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
```

