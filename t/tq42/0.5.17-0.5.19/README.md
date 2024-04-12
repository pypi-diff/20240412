# Comparing `tmp/tq42-0.5.17.tar.gz` & `tmp/tq42-0.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tq42-0.5.17.tar", max compression
+gzip compressed data, was "tq42-0.5.19.tar", max compression
```

## Comparing `tq42-0.5.17.tar` & `tq42-0.5.19.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11357 2024-04-04 11:48:55.440611 tq42-0.5.17/LICENSE
--rw-r--r--   0        0        0     6029 2024-04-04 11:48:55.440611 tq42-0.5.17/README.md
--rw-r--r--   0        0        0      897 2024-04-04 11:48:55.464610 tq42-0.5.17/pyproject.toml
--rw-r--r--   0        0        0       76 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/__init__.py
--rwxr-xr-x   0        0        0      977 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/__main__.py
--rw-r--r--   0        0        0     2990 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/algorithm.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/cli_functions.py
--rw-r--r--   0        0        0     1017 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/compute_group.py
--rw-r--r--   0        0        0     1053 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/experiment_group.py
--rw-r--r--   0        0        0     1478 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/experiment_run_group.py
--rw-r--r--   0        0        0      420 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/organization_group.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/output_format/__init__.py
--rw-r--r--   0        0        0     3243 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/output_format/formatter.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/parsers/__init__.py
--rw-r--r--   0        0        0     2688 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/parsers/params_checker.py
--rw-r--r--   0        0        0     5891 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/parsers/tq42parser.py
--rw-r--r--   0        0        0      783 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/project_dataset_group.py
--rw-r--r--   0        0        0      719 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/project_group.py
--rw-r--r--   0        0        0     1201 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/tq42_all.py
--rw-r--r--   0        0        0     3500 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/cli/tq42_help.py
--rw-r--r--   0        0        0     7682 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/client.py
--rw-r--r--   0        0        0     2091 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/compute.py
--rw-r--r--   0        0        0     2734 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/dataset.py
--rw-r--r--   0        0        0     2311 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/exception_handling.py
--rw-r--r--   0        0        0     1854 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/exceptions.py
--rw-r--r--   0        0        0     3974 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/experiment.py
--rw-r--r--   0        0        0     5969 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/experiment_run.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/__init__.py
--rw-r--r--   0        0        0      573 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/conftest.py
--rw-r--r--   0        0        0     3396 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/functional_test_config.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/__init__.py
--rw-r--r--   0        0        0     1474 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_cli.py
--rw-r--r--   0        0        0     1523 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_compute_group.py
--rw-r--r--   0        0        0     1190 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py
--rw-r--r--   0        0        0     2404 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py
--rw-r--r--   0        0        0      678 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_organization_group.py
--rw-r--r--   0        0        0     1222 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_project_group.py
--rw-r--r--   0        0        0      689 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/test_functional_cache_utils.py
--rw-r--r--   0        0        0     5721 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/test_functional_tq42_api.py
--rw-r--r--   0        0        0     1371 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/test_polling_function.py
--rw-r--r--   0        0        0      437 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/functional_tests/test_test_config.py
--rw-r--r--   0        0        0     3038 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/organization.py
--rw-r--r--   0        0        0     5355 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/project.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/cli/__init__.py
--rw-r--r--   0        0        0     4861 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/cli/test_output_format.py
--rw-r--r--   0        0        0     6185 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/cli/test_tq42_help.py
--rw-r--r--   0        0        0     3787 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/cli/test_tq42_help_flags.py
--rw-r--r--   0        0        0      892 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_cache_utils.py
--rw-r--r--   0        0        0      806 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_compute.py
--rw-r--r--   0        0        0     2202 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_config_environment.py
--rw-r--r--   0        0        0     1890 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_dirs.py
--rw-r--r--   0        0        0      825 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_example.py
--rw-r--r--   0        0        0     1475 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_imports.py
--rw-r--r--   0        0        0      159 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_package_version.py
--rw-r--r--   0        0        0     7800 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_tq42_api.py
--rw-r--r--   0        0        0     7617 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_tq42_error_handling.py
--rw-r--r--   0        0        0     8028 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/test_utils.py
--rwxr-xr-x   0        0        0       48 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/testdata/README.md
--rw-r--r--   0        0        0      147 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/testdata/config.json
--rwxr-xr-x   0        0        0      460 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/testdata/test_convert_colon_separated_string_to_dict.txt
--rwxr-xr-x   0        0        0      210 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/tests/testdata/test_utils_get_id.txt
--rw-r--r--   0        0        0        0 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/__init__.py
--rw-r--r--   0        0        0      547 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/constants.py
--rw-r--r--   0        0        0     1256 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/dirs.py
--rw-r--r--   0        0        0     1828 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/environment_utils.py
--rw-r--r--   0        0        0      365 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/file_handling.py
--rw-r--r--   0        0        0      147 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/text_files/config.json
--rwxr-xr-x   0        0        0      132 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/text_files/cpu_configs.json
--rwxr-xr-x   0        0        0      829 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/text_files/hardware_configs.json
--rw-r--r--   0        0        0    14166 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/text_files/help.json
--rw-r--r--   0        0        0     2342 2024-04-04 11:48:55.464610 tq42-0.5.17/tq42/utils/text_files/help_flags.json
--rw-r--r--   0        0        0      491 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/text_files/insufficient_permission_error.txt
--rw-r--r--   0        0        0      130 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/text_files/invalid_arguments_error.txt
--rw-r--r--   0        0        0      191 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/text_files/local_permission_error.txt
--rw-r--r--   0        0        0      470 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/text_files/no_default_error.txt
--rwxr-xr-x   0        0        0      657 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/text_files/tq42_commands.txt
--rw-r--r--   0        0        0      411 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/text_files/unauthenticated_error.txt
--rw-r--r--   0        0        0     2112 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/token_manager.py
--rw-r--r--   0        0        0     3647 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/utils.py
--rw-r--r--   0        0        0      966 2024-04-04 11:48:55.468610 tq42-0.5.17/tq42/utils/utils_for_cache.py
--rw-r--r--   0        0        0     6648 1970-01-01 00:00:00.000000 tq42-0.5.17/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 12:56:03.669864 tq42-0.5.19/LICENSE
+-rw-r--r--   0        0        0     6029 2024-04-12 12:56:03.669864 tq42-0.5.19/README.md
+-rw-r--r--   0        0        0      749 2024-04-12 12:56:03.693863 tq42-0.5.19/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/__init__.py
+-rwxr-xr-x   0        0        0      977 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/__main__.py
+-rw-r--r--   0        0        0     2990 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/algorithm.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/cli_functions.py
+-rw-r--r--   0        0        0     1017 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/compute_group.py
+-rw-r--r--   0        0        0     1053 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/experiment_group.py
+-rw-r--r--   0        0        0     1478 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/experiment_run_group.py
+-rw-r--r--   0        0        0      420 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/organization_group.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/output_format/__init__.py
+-rw-r--r--   0        0        0     3243 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/output_format/formatter.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/parsers/__init__.py
+-rw-r--r--   0        0        0     2688 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/parsers/params_checker.py
+-rw-r--r--   0        0        0     5891 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/parsers/tq42parser.py
+-rw-r--r--   0        0        0      783 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/project_dataset_group.py
+-rw-r--r--   0        0        0      719 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/project_group.py
+-rw-r--r--   0        0        0     1201 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/tq42_all.py
+-rw-r--r--   0        0        0     3500 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/cli/tq42_help.py
+-rw-r--r--   0        0        0     7998 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/client.py
+-rw-r--r--   0        0        0     2091 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/compute.py
+-rw-r--r--   0        0        0     2734 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/dataset.py
+-rw-r--r--   0        0        0     2311 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/exception_handling.py
+-rw-r--r--   0        0        0     1854 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/exceptions.py
+-rw-r--r--   0        0        0     3974 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/experiment.py
+-rw-r--r--   0        0        0     5969 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/experiment_run.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/conftest.py
+-rw-r--r--   0        0        0     3396 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/functional_test_config.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/__init__.py
+-rw-r--r--   0        0        0     1474 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_cli.py
+-rw-r--r--   0        0        0     1523 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_compute_group.py
+-rw-r--r--   0        0        0     1190 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py
+-rw-r--r--   0        0        0     2404 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py
+-rw-r--r--   0        0        0      678 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_organization_group.py
+-rw-r--r--   0        0        0     1222 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_project_group.py
+-rw-r--r--   0        0        0      689 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_functional_cache_utils.py
+-rw-r--r--   0        0        0     5721 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_functional_tq42_api.py
+-rw-r--r--   0        0        0     1371 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_polling_function.py
+-rw-r--r--   0        0        0      437 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/functional_tests/test_test_config.py
+-rw-r--r--   0        0        0     3038 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/organization.py
+-rw-r--r--   0        0        0     5355 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/project.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/__init__.py
+-rw-r--r--   0        0        0     4861 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/test_output_format.py
+-rw-r--r--   0        0        0     6185 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/test_tq42_help.py
+-rw-r--r--   0        0        0     3787 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/cli/test_tq42_help_flags.py
+-rw-r--r--   0        0        0      892 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_cache_utils.py
+-rw-r--r--   0        0        0      806 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_compute.py
+-rw-r--r--   0        0        0     2202 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_config_environment.py
+-rw-r--r--   0        0        0     1890 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_dirs.py
+-rw-r--r--   0        0        0      825 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_example.py
+-rw-r--r--   0        0        0     1475 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_imports.py
+-rw-r--r--   0        0        0      159 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_package_version.py
+-rw-r--r--   0        0        0     7800 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_tq42_api.py
+-rw-r--r--   0        0        0     7617 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_tq42_error_handling.py
+-rw-r--r--   0        0        0    10198 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/test_utils.py
+-rwxr-xr-x   0        0        0       48 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/README.md
+-rw-r--r--   0        0        0      147 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/config.json
+-rwxr-xr-x   0        0        0      460 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/test_convert_colon_separated_string_to_dict.txt
+-rwxr-xr-x   0        0        0      210 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/tests/testdata/test_utils_get_id.txt
+-rw-r--r--   0        0        0        0 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/__init__.py
+-rw-r--r--   0        0        0      547 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/constants.py
+-rw-r--r--   0        0        0     1256 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/dirs.py
+-rw-r--r--   0        0        0     1828 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/environment_utils.py
+-rw-r--r--   0        0        0      365 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/file_handling.py
+-rw-r--r--   0        0        0      147 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/config.json
+-rwxr-xr-x   0        0        0      132 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/cpu_configs.json
+-rwxr-xr-x   0        0        0      829 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/hardware_configs.json
+-rw-r--r--   0        0        0    14166 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/help.json
+-rw-r--r--   0        0        0     2342 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/help_flags.json
+-rw-r--r--   0        0        0      491 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/insufficient_permission_error.txt
+-rw-r--r--   0        0        0      130 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/invalid_arguments_error.txt
+-rw-r--r--   0        0        0      191 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/local_permission_error.txt
+-rw-r--r--   0        0        0      470 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/no_default_error.txt
+-rwxr-xr-x   0        0        0      657 2024-04-12 12:56:03.693863 tq42-0.5.19/tq42/utils/text_files/tq42_commands.txt
+-rw-r--r--   0        0        0      411 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/text_files/unauthenticated_error.txt
+-rw-r--r--   0        0        0     2284 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/token_manager.py
+-rw-r--r--   0        0        0     4469 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/utils.py
+-rw-r--r--   0        0        0      966 2024-04-12 12:56:03.697864 tq42-0.5.19/tq42/utils/utils_for_cache.py
+-rw-r--r--   0        0        0     6690 1970-01-01 00:00:00.000000 tq42-0.5.19/PKG-INFO
```

### Comparing `tq42-0.5.17/LICENSE` & `tq42-0.5.19/LICENSE`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/README.md` & `tq42-0.5.19/README.md`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/__main__.py` & `tq42-0.5.19/tq42/__main__.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/algorithm.py` & `tq42-0.5.19/tq42/algorithm.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/cli_functions.py` & `tq42-0.5.19/tq42/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/compute_group.py` & `tq42-0.5.19/tq42/cli/compute_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/experiment_group.py` & `tq42-0.5.19/tq42/cli/experiment_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/experiment_run_group.py` & `tq42-0.5.19/tq42/cli/experiment_run_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/output_format/formatter.py` & `tq42-0.5.19/tq42/cli/output_format/formatter.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/parsers/params_checker.py` & `tq42-0.5.19/tq42/cli/parsers/params_checker.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/parsers/tq42parser.py` & `tq42-0.5.19/tq42/cli/parsers/tq42parser.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/project_dataset_group.py` & `tq42-0.5.19/tq42/cli/project_dataset_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/project_group.py` & `tq42-0.5.19/tq42/cli/project_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/tq42_all.py` & `tq42-0.5.19/tq42/cli/tq42_all.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/cli/tq42_help.py` & `tq42-0.5.19/tq42/cli/tq42_help.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/client.py` & `tq42-0.5.19/tq42/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import webbrowser
 from datetime import datetime
 import grpc
 import requests
-from tq42.utils import dirs, file_handling
+from tq42.utils import dirs, file_handling, utils
 from tq42.utils.token_manager import TokenManager
 from tq42.exception_handling import handle_generic_sdk_errors
 import time
 
 from com.terraquantum.experiment.v1.experiment import (
     experiment_service_pb2_grpc as pb2_exp_grpc,
 )
@@ -177,24 +177,35 @@
                 data=data_token,
                 headers=self.environment.headers,
             )
             json_token = response_token.json()
             # If we received an access token, print it and break out of the loop
             if "access_token" in json_token:
                 access_token = json_token["access_token"]
-                file_handling.write_to_file(self.token_file_path, access_token)
+
+                save_location = utils.save_token(
+                    service_name="access_token",
+                    backup_save_path=self.token_file_path,
+                    token=access_token,
+                )
+
                 print(
-                    f"Authentication is successful, access token is saved in file: {self.token_file_path}"
+                    f"Authentication is successful, access token is saved in: {save_location}."
                 )
+
                 env_set = environment_default_set(client=self)
                 print(env_set)
 
             if "refresh_token" in json_token:
                 refresh_token = json_token["refresh_token"]
-                file_handling.write_to_file(self.refresh_token_file_path, refresh_token)
+                utils.save_token(
+                    service_name="refresh_token",
+                    backup_save_path=self.refresh_token_file_path,
+                    token=refresh_token,
+                )
                 current_datetime = datetime.now()
                 file_handling.write_to_file(self.timestamp_file_path, current_datetime)
                 break
 
             # Otherwise, wait for the specified interval before polling again
             time.sleep(interval)
 
@@ -212,9 +223,11 @@
     @property
     def refresh_token_file_path(self):
         return self.token_manager.refresh_token_file_path
 
     @property
     def metadata(self):
         self.token_manager.renew_expring_token()
-        token = file_handling.read_file(self.token_file_path)
+        token = utils.get_token(
+            service_name="access_token", backup_save_path=self.token_file_path
+        )
         return (("authorization", "Bearer " + token),)
```

### Comparing `tq42-0.5.17/tq42/compute.py` & `tq42-0.5.19/tq42/compute.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/dataset.py` & `tq42-0.5.19/tq42/dataset.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/exception_handling.py` & `tq42-0.5.19/tq42/exception_handling.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/exceptions.py` & `tq42-0.5.19/tq42/exceptions.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/experiment.py` & `tq42-0.5.19/tq42/experiment.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/experiment_run.py` & `tq42-0.5.19/tq42/experiment_run.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/conftest.py` & `tq42-0.5.19/tq42/functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/functional_test_config.py` & `tq42-0.5.19/tq42/functional_tests/functional_test_config.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_cli.py` & `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_cli.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_compute_group.py` & `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_compute_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py` & `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py` & `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_organization_group.py` & `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_organization_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/invoke_cli/test_functional_project_group.py` & `tq42-0.5.19/tq42/functional_tests/invoke_cli/test_functional_project_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/test_functional_cache_utils.py` & `tq42-0.5.19/tq42/functional_tests/test_functional_cache_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/test_functional_tq42_api.py` & `tq42-0.5.19/tq42/functional_tests/test_functional_tq42_api.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/functional_tests/test_polling_function.py` & `tq42-0.5.19/tq42/functional_tests/test_polling_function.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/organization.py` & `tq42-0.5.19/tq42/organization.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/project.py` & `tq42-0.5.19/tq42/project.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/cli/test_output_format.py` & `tq42-0.5.19/tq42/tests/cli/test_output_format.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/cli/test_tq42_help.py` & `tq42-0.5.19/tq42/tests/cli/test_tq42_help.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/cli/test_tq42_help_flags.py` & `tq42-0.5.19/tq42/tests/cli/test_tq42_help_flags.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_cache_utils.py` & `tq42-0.5.19/tq42/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_compute.py` & `tq42-0.5.19/tq42/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_config_environment.py` & `tq42-0.5.19/tq42/tests/test_config_environment.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_dirs.py` & `tq42-0.5.19/tq42/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_example.py` & `tq42-0.5.19/tq42/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_imports.py` & `tq42-0.5.19/tq42/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_tq42_api.py` & `tq42-0.5.19/tq42/tests/test_tq42_api.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_tq42_error_handling.py` & `tq42-0.5.19/tq42/tests/test_tq42_error_handling.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/tests/test_utils.py` & `tq42-0.5.19/tq42/tests/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import unittest
+import os
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 from unittest import mock
+from keyring.errors import InitError, NoKeyringError
 
 from tq42 import exceptions
 from tq42.utils import dirs, utils, file_handling
 from tq42.utils.token_manager import TokenManager
 import json
 from tq42.client import ConfigEnvironment, TQ42Client
 from tq42.exceptions import NoMatchingAttributeError
@@ -223,7 +225,58 @@
         alternative_json_path = dirs.testdata("config.json")
         tq42 = TQ42Client(alternative_json_path)
         self.assertEqual(tq42.config_file, alternative_json_path)
 
     def test_find_oneof_field_name(self):
         res = utils.find_oneof_field_name("ToyMetadataProto")
         self.assertEqual(res, "toy_metadata")
+
+    def test_save_get_token_with_keyring_enabled(self):
+        # keyring is working on Mac Sonoma 14.4 and Windows 11
+        token_file_path = os.path.join(dirs.testdata(), "keyring_test.json")
+        utils.save_token(
+            service_name="access_token",
+            backup_save_path=token_file_path,
+            token="test_token",
+        )
+        token = utils.get_token(
+            service_name="access_token", backup_save_path=token_file_path
+        )
+        self.assertEqual(token, "test_token")
+
+    @mock.patch("keyring.set_password")
+    @mock.patch("keyring.get_password")
+    def test_save_get_token_has_InitError(self, mock_set_password, mock_get_password):
+        # keyring not working on Ubuntu 20.04.6LTS and causes InitError exception
+        token_file_path = os.path.join(dirs.testdata(), "keyring_test.json")
+        mock_set_password.side_effect = InitError()
+        mock_get_password.side_effect = InitError()
+        utils.save_token(
+            service_name="access_token",
+            backup_save_path=token_file_path,
+            token="test_token",
+        )
+        token = utils.get_token(
+            service_name="access_token", backup_save_path=token_file_path
+        )
+        os.remove(token_file_path)
+        self.assertEqual(token, "test_token")
+
+    @mock.patch("keyring.set_password")
+    @mock.patch("keyring.get_password")
+    def test_save_get_token_has_NoKeyringError(
+        self, mock_set_password, mock_get_password
+    ):
+        # keyring not working on Debian and Redhat, NoKeyringError is raised
+        token_file_path = os.path.join(dirs.testdata(), "keyring_test.json")
+        mock_set_password.side_effect = NoKeyringError()
+        mock_get_password.side_effect = NoKeyringError()
+        utils.save_token(
+            service_name="access_token",
+            backup_save_path=token_file_path,
+            token="test_token",
+        )
+        token = utils.get_token(
+            service_name="access_token", backup_save_path=token_file_path
+        )
+        os.remove(token_file_path)
+        self.assertEqual(token, "test_token")
```

### Comparing `tq42-0.5.17/tq42/utils/constants.py` & `tq42-0.5.19/tq42/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/dirs.py` & `tq42-0.5.19/tq42/utils/dirs.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/environment_utils.py` & `tq42-0.5.19/tq42/utils/environment_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/text_files/hardware_configs.json` & `tq42-0.5.19/tq42/utils/text_files/hardware_configs.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/text_files/help.json` & `tq42-0.5.19/tq42/utils/text_files/help.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/text_files/help_flags.json` & `tq42-0.5.19/tq42/utils/text_files/help_flags.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/text_files/tq42_commands.txt` & `tq42-0.5.19/tq42/utils/text_files/tq42_commands.txt`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/tq42/utils/token_manager.py` & `tq42-0.5.19/tq42/utils/token_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tq42.utils import dirs, file_handling
+from tq42.utils import dirs, file_handling, utils
 from datetime import datetime
 import requests
 
 
 class TokenManager:
     def __init__(self, environment, alt_config_folder):
         self.alt_config_folder = alt_config_folder
@@ -35,20 +35,26 @@
         if diff.total_seconds() > renew_limit:
             self.request_new_access_token()
             return True
 
         return False
 
     def request_new_access_token(self):
-        refresh_token = file_handling.read_file(self.refresh_token_file_path)
+        refresh_token = utils.get_token(
+            service_name="refresh_token", backup_save_path=self.refresh_token_file_path
+        )
         data = self.environment.refresh_token_data(refresh_token)
         response = requests.post(
             self.environment.auth_url_token,
             data=data,
             headers=self.environment.headers,
         )
         json_response = response.json()
         if "access_token" in json_response:
             access_token = json_response["access_token"]
-            file_handling.write_to_file(self.token_file_path, access_token)
+            utils.save_token(
+                service_name="access_token",
+                backup_save_path=self.token_file_path,
+                token=access_token,
+            )
             current_datetime = datetime.now()
             file_handling.write_to_file(self.timestamp_file_path, current_datetime)
```

### Comparing `tq42-0.5.17/tq42/utils/utils.py` & `tq42-0.5.19/tq42/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import importlib
 import json
 from typing import Union
+import keyring
 
 from com.terraquantum.experiment.v1.experimentrun import (
     create_experiment_run_request_pb2 as create_exp_run,
 )
 from com.terraquantum.experiment.v1.experimentrun.experiment_run_pb2 import (
     HardwareProto,
 )
 from com.terraquantum.experiment.v1.experimentrun.algorithm import shared_pb2
 
 import tq42.utils.dirs as dirs
+from tq42.utils import file_handling
 from tq42.exceptions import NoMatchingAttributeError
+from keyring.errors import NoKeyringError, InitError
 
 
 def get_id(input):
     input = str(input)
     inputs = input.strip().splitlines()
     for input in inputs:
         pair_result = input.split(":")
@@ -99,7 +102,33 @@
         request_id=None,
         algorithm=algo,
         experiment_id=exp_id,
         hardware=hardware,
         **keyword_args,
     )
     return experiment_request
+
+
+def save_token(service_name: str, backup_save_path: str, token: str) -> str:
+    try:
+        save_location = "keyring"
+        keyring.set_password(
+            service_name=service_name,
+            username="username",
+            password=token,
+        )
+        return save_location
+
+    except (NoKeyringError, InitError):
+        file_handling.write_to_file(backup_save_path, token)
+        return backup_save_path
+
+
+def get_token(service_name: str, backup_save_path: str) -> str:
+    try:
+        return keyring.get_password(
+            service_name=service_name,
+            username="username",
+        )
+
+    except (NoKeyringError, InitError):
+        return file_handling.read_file(backup_save_path)
```

### Comparing `tq42-0.5.17/tq42/utils/utils_for_cache.py` & `tq42-0.5.19/tq42/utils/utils_for_cache.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.17/PKG-INFO` & `tq42-0.5.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tq42
-Version: 0.5.17
+Version: 0.5.19
 Summary: tq42 sdk
 Author: Terra Quantum AG
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: keyring (>=25.0.0,<26.0.0)
 Requires-Dist: pytest (>=7.4.4,<8.0.0)
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: tq42_grpc_client (==1.0.77)
+Requires-Dist: tq42_grpc_client (==1.0.93)
 Description-Content-Type: text/markdown
 
 ![](images/TQ42_Logo_Black_Teal.svg)
 
 # Introduction to TQ42
 The TQ42 Python SDK puts the power in your hands to accelerate delivery of custom, high-impact solutions. After installing the SDK and authenticating, access algorithms such as TetraOpt – a global optimization library based on tensor train (TT) decomposition.
```

