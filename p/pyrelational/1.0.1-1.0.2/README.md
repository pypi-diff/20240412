# Comparing `tmp/pyrelational-1.0.1.tar.gz` & `tmp/pyrelational-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrelational-1.0.1.tar", last modified: Mon Feb 19 14:17:35 2024, max compression
+gzip compressed data, was "pyrelational-1.0.2.tar", last modified: Fri Apr 12 11:04:38 2024, max compression
```

## Comparing `pyrelational-1.0.1.tar` & `pyrelational-1.0.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-19 14:17:25.000000 pyrelational-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-02-19 14:17:35.732036 pyrelational-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-02-19 14:17:25.000000 pyrelational-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.720036 pyrelational-1.0.1/pyrelational/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational/data_managers/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/data_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/data_managers/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/datasets/benchmark_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/datasets/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/datasets/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/datasets/uci_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational/informativeness/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/informativeness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/informativeness/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/informativeness/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/informativeness/task_agnostic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational/model_managers/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/model_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/model_managers/abstract_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/model_managers/ensemble_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/model_managers/lightning_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/model_managers/mcdropout_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/model_managers/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational/oracles/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/oracles/abstract_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/oracles/benchmark_oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/pipeline/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.728036 pyrelational-1.0.1/pyrelational/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/abstract_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.728036 pyrelational-1.0.1/pyrelational/strategies/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/classification/abstract_classification_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/classification/entropy_classification_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/classification/least_confidence_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/classification/marginal_confidence_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/classification/ratio_confidence_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.728036 pyrelational-1.0.1/pyrelational/strategies/regression/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/abstract_regression_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/bald_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/expected_improvement_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/least_confidence_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/mean_prediction_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/thompson_sampling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/regression/upper_confidence_bound_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.728036 pyrelational-1.0.1/pyrelational/strategies/task_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/task_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/task_agnostic/random_acquisition_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/task_agnostic/relative_distance_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/strategies/task_agnostic/representative_sampling_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-19 14:17:25.000000 pyrelational-1.0.1/pyrelational/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.724036 pyrelational-1.0.1/pyrelational.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-02-19 14:17:35.000000 pyrelational-1.0.1/pyrelational.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-02-19 14:17:35.000000 pyrelational-1.0.1/pyrelational.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 14:17:35.000000 pyrelational-1.0.1/pyrelational.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-19 14:17:35.000000 pyrelational-1.0.1/pyrelational.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-19 14:17:35.000000 pyrelational-1.0.1/pyrelational.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 14:17:35.732036 pyrelational-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-19 14:17:25.000000 pyrelational-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.728036 pyrelational-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.728036 pyrelational-1.0.1/tests/data_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/data_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/data_managers/test_data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/datasets/test_benchmark_datamanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/datasets/test_classification_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/datasets/test_regression_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/datasets/test_uci_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/tests/informativeness/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/informativeness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/informativeness/test_informativeness_scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/model_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/model_managers/test_ensemble_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/model_managers/test_mc_dropout_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/model_managers/test_model_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/oracles/test_oracles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/tests/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/pipeline/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:35.732036 pyrelational-1.0.1/tests/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/strategies/agnostic_strategy_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/strategies/classification_strategy_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/strategies/regression_strategy_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/strategies/test_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-02-19 14:17:25.000000 pyrelational-1.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.103722 pyrelational-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 11:04:26.000000 pyrelational-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-04-12 11:04:38.103722 pyrelational-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-12 11:04:26.000000 pyrelational-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.091722 pyrelational-1.0.2/pyrelational/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/data_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/data_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19773 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/data_managers/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/datasets/benchmark_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26346 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/datasets/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/datasets/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/datasets/uci_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/informativeness/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/informativeness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/informativeness/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/informativeness/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/informativeness/task_agnostic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/model_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/model_managers/abstract_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/model_managers/ensemble_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/model_managers/lightning_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6096 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/model_managers/mcdropout_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/model_managers/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/oracles/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/oracles/abstract_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/oracles/benchmark_oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/pipeline/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/abstract_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/pyrelational/strategies/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/classification/abstract_classification_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/classification/entropy_classification_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/classification/least_confidence_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/classification/marginal_confidence_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/classification/ratio_confidence_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/pyrelational/strategies/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/abstract_regression_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/bald_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/expected_improvement_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/least_confidence_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/mean_prediction_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/thompson_sampling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/regression/upper_confidence_bound_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/pyrelational/strategies/task_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/task_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/task_agnostic/random_acquisition_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/task_agnostic/relative_distance_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/strategies/task_agnostic/representative_sampling_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 11:04:26.000000 pyrelational-1.0.2/pyrelational/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.095722 pyrelational-1.0.2/pyrelational.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13991 2024-04-12 11:04:37.000000 pyrelational-1.0.2/pyrelational.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-12 11:04:38.000000 pyrelational-1.0.2/pyrelational.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:04:37.000000 pyrelational-1.0.2/pyrelational.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 11:04:37.000000 pyrelational-1.0.2/pyrelational.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 11:04:37.000000 pyrelational-1.0.2/pyrelational.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:04:38.103722 pyrelational-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 11:04:26.000000 pyrelational-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/tests/data_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/data_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/data_managers/test_data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/datasets/test_benchmark_datamanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/datasets/test_classification_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/datasets/test_regression_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/datasets/test_uci_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.099722 pyrelational-1.0.2/tests/informativeness/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/informativeness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/informativeness/test_informativeness_scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.103722 pyrelational-1.0.2/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/model_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/model_managers/test_ensemble_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/model_managers/test_mc_dropout_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/model_managers/test_model_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.103722 pyrelational-1.0.2/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/oracles/test_oracles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.103722 pyrelational-1.0.2/tests/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/pipeline/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:38.103722 pyrelational-1.0.2/tests/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/strategies/agnostic_strategy_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/strategies/classification_strategy_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/strategies/regression_strategy_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/strategies/test_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-12 11:04:26.000000 pyrelational-1.0.2/tests/test_utils.py
```

### Comparing `pyrelational-1.0.1/LICENSE` & `pyrelational-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/PKG-INFO` & `pyrelational-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrelational
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python tool box for quickly implementing active learning strategies
 Home-page: https://github.com/RelationRx/pyrelational
 Author: Relation Therapeutics
 Author-email: software@relationrx.com
 License: UNKNOWN
 Description: # PyRelationAL
```

### Comparing `pyrelational-1.0.1/README.md` & `pyrelational-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/data_managers/data_manager.py` & `pyrelational-1.0.2/pyrelational/data_managers/data_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         if train_indices is None:
             if test_indices is None:
                 raise ValueError("No train or test specified, too ambiguous to set values")
             train_indices = list(remaining_indices)
         elif test_indices is None:
             test_indices = list(remaining_indices)
         elif remaining_indices:
-            warnings.warn(f"{len(remaining_indices)} indices are not found in any split")
+            warnings.warn(f"{len(remaining_indices)} indices are not found in any split", stacklevel=3)
 
         self._ensure_not_empty("train", train_indices)
         self._ensure_not_empty("test", test_indices)
         self._ensure_no_split_leaks(train_indices, validation_indices, test_indices)
         self.train_indices = train_indices
         self.validation_indices = validation_indices
         self.test_indices = test_indices
```

### Comparing `pyrelational-1.0.1/pyrelational/datasets/__init__.py` & `pyrelational-1.0.2/pyrelational/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/datasets/benchmark_datamanager.py` & `pyrelational-1.0.2/pyrelational/datasets/benchmark_datamanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Utility to create datamanagers corresponding to different AL tasks
 """
+
 import random
 from collections import defaultdict
 from typing import Any, List
 
 import numpy as np
 from sklearn.metrics import pairwise_distances
 from torch.utils.data import Dataset
```

### Comparing `pyrelational-1.0.1/pyrelational/datasets/classification.py` & `pyrelational-1.0.2/pyrelational/datasets/classification.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/datasets/regression.py` & `pyrelational-1.0.2/pyrelational/datasets/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Regression datasets that can be used for benchmarking AL strategies
 """
+
 from typing import Tuple
 
 import numpy as np
 import torch
 from sklearn.datasets import load_diabetes, make_regression
 from sklearn.model_selection import KFold
 from torch import Tensor
```

### Comparing `pyrelational-1.0.1/pyrelational/datasets/uci_datasets.py` & `pyrelational-1.0.2/pyrelational/datasets/uci_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Class to help download and do the initial processing of dataset on the UCI database
 """
+
 import os
 import urllib.request
 import zipfile
 from os import path
 
 import numpy as np
 import pandas as pd
```

### Comparing `pyrelational-1.0.1/pyrelational/informativeness/classification.py` & `pyrelational-1.0.2/pyrelational/informativeness/classification.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/informativeness/regression.py` & `pyrelational-1.0.2/pyrelational/informativeness/regression.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/informativeness/task_agnostic.py` & `pyrelational-1.0.2/pyrelational/informativeness/task_agnostic.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Array = Union[Tensor, NDArray[Any], List[Any]]
 
 
 def relative_distance(
     query_set: Union[Array, DataLoader[Any]],
     reference_set: Union[Array, DataLoader[Any]],
     metric: Optional[Union[str, Callable[..., Any]]] = "euclidean",
-    axis: int = -1,
+    axis: int = 1,
 ) -> Tensor:
     """
     Function that return the minimum distance, according to input metric, from each sample in the query_set to the
     samples in the reference set.
 
     :param query_set: input containing the features of samples in the queryable pool. query set should either be an
         array-like object or a pytorch dataloader whose first element in each bactch is a featurisation of the samples
```

### Comparing `pyrelational-1.0.1/pyrelational/model_managers/abstract_model_manager.py` & `pyrelational-1.0.2/pyrelational/model_managers/abstract_model_manager.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/model_managers/ensemble_model_manager.py` & `pyrelational-1.0.2/pyrelational/model_managers/ensemble_model_manager.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/model_managers/lightning_model_manager.py` & `pyrelational-1.0.2/pyrelational/model_managers/lightning_model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,15 @@
 
         self._current_model = model
 
     def test(self, loader: DataLoader[Any]) -> Dict[str, float]:
         if not self.is_trained():
             raise ValueError("No current model, call 'train(train_loader, valid_loader)' to train the model first")
         trainer, _ = self.init_trainer()
-        ret: Dict[str, float] = trainer.test(self._current_model, dataloaders=loader)[0]
-        return ret
+        return dict(trainer.test(self._current_model, dataloaders=loader)[0])
 
     def __call__(self, loader: DataLoader[Any]) -> torch.Tensor:
         """
         Call function which outputs model predictions from dataloader
 
         :param loader: pytorch dataloader
         :return: model predictions of shape (number of samples in loader,1)
```

### Comparing `pyrelational-1.0.1/pyrelational/model_managers/mcdropout_model_manager.py` & `pyrelational-1.0.2/pyrelational/model_managers/mcdropout_model_manager.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/model_managers/model_utils.py` & `pyrelational-1.0.2/pyrelational/model_managers/model_utils.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/oracles/abstract_oracle.py` & `pyrelational-1.0.2/pyrelational/oracles/abstract_oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file contains the implementation of an abstract oracle interface for PyRelationAL
 """
+
 from abc import ABC, abstractmethod
 from typing import Any, List
 
 from pyrelational.data_managers.data_manager import DataManager
 
 
 class Oracle(ABC):
```

### Comparing `pyrelational-1.0.1/pyrelational/oracles/benchmark_oracle.py` & `pyrelational-1.0.2/pyrelational/oracles/benchmark_oracle.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/pipeline/pipeline.py` & `pyrelational-1.0.2/pyrelational/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module defines the acquisition manager which utilises
 the data manager, sampling functions, and model to create acquisition
 functions and general arbiters of the active learning pipeline
 """
+
 import logging
-from abc import ABC
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
 from torch.utils.data import DataLoader
@@ -17,15 +17,15 @@
 from pyrelational.oracles.abstract_oracle import Oracle
 from pyrelational.oracles.benchmark_oracle import BenchmarkOracle
 from pyrelational.strategies.abstract_strategy import Strategy
 
 logger = logging.getLogger()
 
 
-class Pipeline(ABC):
+class Pipeline:
     """
     The pipeline facilitates the communication between
 
         - DataManager
         - ModelManager,
         - Strategy,
         - Oracle (Optional)
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/abstract_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/abstract_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module defines the interface for an abstract active learning strategy
 which is composed of defining a `__call__` function which
 suggests observations to be labelled. In the default case the `__call__`
 is the composition of a informativeness function which assigns a measure of
 informativeness to unlabelled observations and a selection algorithm which chooses
 what observations to present to the oracle
 """
+
 import inspect
 import logging
 from abc import ABC
 from typing import Any, Callable, Dict, List
 
 from pyrelational.data_managers import DataManager
 from pyrelational.model_managers import ModelManager
@@ -44,26 +45,25 @@
     """
 
     def __init__(self, *args: Any, **kwargs: Any):
         super(Strategy, self).__init__()
 
     __call__: Callable[..., List[int]] = _call_unimplemented
 
-    def suggest(self, num_annotate: int, *args: Any, **kwargs: Any) -> List[int]:
+    def suggest(self, num_annotate: int, **kwargs: Any) -> List[int]:
         """
         Filter kwargs and feed arguments to the __call__ method to return unlabelled observations to be labelled
         as a list of dataset indices.
 
         :param num_annotate: number of samples to annotate
-        :param args: any arguments needed by private suggest method
         :param kwargs: any kwargs (filtered to match internal suggest inputs)
         :return: list of indices of samples to query from oracle
         """
         filtered_kwargs = self._filter_kwargs(**kwargs)
-        return self(num_annotate=num_annotate, *args, **filtered_kwargs)
+        return self(num_annotate=num_annotate, **filtered_kwargs)
 
     @staticmethod
     def train_and_infer(data_manager: DataManager, model_manager: ModelManager[Any, Any]) -> Any:
         """
         Train the model on the currently labelled subset of the data and produces an output that can be used in
         model uncertainty based strategies.
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/classification/abstract_classification_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/classification/abstract_classification_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/classification/entropy_classification_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/classification/entropy_classification_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Active learning using entropy based confidence uncertainty measure
 between classes in the posterior predictive distribution to
 choose which observations to propose to the oracle
 """
+
 from torch import Tensor
 
 from pyrelational.informativeness import classification_entropy
 from pyrelational.strategies.classification.abstract_classification_strategy import (
     ClassificationStrategy,
 )
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/classification/least_confidence_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/classification/least_confidence_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Active learning using least confidence uncertainty measure
 between classes in the posterior predictive distribution to
 choose which observations to propose to the oracle
 """
+
 from torch import Tensor
 
 from pyrelational.informativeness import classification_least_confidence
 from pyrelational.strategies.classification.abstract_classification_strategy import (
     ClassificationStrategy,
 )
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/classification/marginal_confidence_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/classification/marginal_confidence_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Active learning using marginal confidence uncertainty measure
 between classes in the posterior predictive distribution to
 choose which observations to propose to the oracle
 """
+
 from torch import Tensor
 
 from pyrelational.informativeness import classification_margin_confidence
 from pyrelational.strategies.classification.abstract_classification_strategy import (
     ClassificationStrategy,
 )
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/classification/ratio_confidence_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/classification/ratio_confidence_strategy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Active learning using ratio based confidence uncertainty measure
 between classes in the posterior predictive distribution to
 choose which observations to propose to the oracle
 """
+
 from torch import Tensor
 
 from pyrelational.informativeness import classification_ratio_confidence
 from pyrelational.strategies.classification.abstract_classification_strategy import (
     ClassificationStrategy,
 )
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/__init__.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/abstract_regression_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/abstract_regression_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/bald_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/bald_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/expected_improvement_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/expected_improvement_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/mean_prediction_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/mean_prediction_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/thompson_sampling_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/thompson_sampling_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/regression/upper_confidence_bound_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/regression/upper_confidence_bound_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/task_agnostic/random_acquisition_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/task_agnostic/random_acquisition_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Defines and implements a random acquisition active learning strategy.
 """
+
 from typing import List
 
 import numpy as np
 
 from pyrelational.data_managers import DataManager
 from pyrelational.strategies.abstract_strategy import Strategy
```

### Comparing `pyrelational-1.0.1/pyrelational/strategies/task_agnostic/relative_distance_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/task_agnostic/relative_distance_strategy.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/pyrelational/strategies/task_agnostic/representative_sampling_strategy.py` & `pyrelational-1.0.2/pyrelational/strategies/task_agnostic/representative_sampling_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Representative sampling based active learning strategy
 """
+
 from typing import Any, List, Union
 
 import numpy as np
 import torch
 from sklearn.base import ClusterMixin
 
 from pyrelational.data_managers import DataManager
```

### Comparing `pyrelational-1.0.1/pyrelational.egg-info/PKG-INFO` & `pyrelational-1.0.2/pyrelational.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrelational
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python tool box for quickly implementing active learning strategies
 Home-page: https://github.com/RelationRx/pyrelational
 Author: Relation Therapeutics
 Author-email: software@relationrx.com
 License: UNKNOWN
 Description: # PyRelationAL
```

### Comparing `pyrelational-1.0.1/pyrelational.egg-info/SOURCES.txt` & `pyrelational-1.0.2/pyrelational.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/setup.py` & `pyrelational-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,16 @@
 """
 pip install -e .
 """
 
 setup_requires = ["pytest-runner"]
 tests_require = ["pytest", "pytest-cov", "mock"]
 
-install_requires = [
-    "numpy>=1.22.0",
-    "pandas>=1.3.0",
-    "lightning>=1.8.6",
-    "torch>=1.9.0",
-    "scikit-learn>=1.0.2",
-    "tabulate>=0.7.0",
-    "pyreadr>=0.4.4",
-    "xlrd>=2.0.1",
-    "openpyxl>=3.0.9",
-]
-
+with open("requirements/base_requirements.txt", "r") as req:
+    install_requires = [line.strip() for line in req if line.strip()]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 version: Dict[str, str] = {}
 with open("pyrelational/version.py") as fp:
     exec(fp.read(), version)
```

### Comparing `pyrelational-1.0.1/tests/data_managers/test_data_manager.py` & `pyrelational-1.0.2/tests/data_managers/test_data_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for data manager
 """
+
 import copy
 from unittest import TestCase
 
 import pytest
 import torch
 from parameterized import parameterized
```

### Comparing `pyrelational-1.0.1/tests/datasets/test_benchmark_datamanager.py` & `pyrelational-1.0.2/tests/datasets/test_benchmark_datamanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for benchmark datamanager functions
 """
+
 from unittest import TestCase
 
 from pyrelational.datasets import BreastCancerDataset, DiabetesDataset
 from pyrelational.datasets.benchmark_datamanager import (
     create_classification_cold_start,
     create_regression_cold_start,
     create_warm_start,
```

### Comparing `pyrelational-1.0.1/tests/datasets/test_classification_datasets.py` & `pyrelational-1.0.2/tests/datasets/test_classification_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for classification datasets
 """
+
 from typing import Type, Union
 from unittest import TestCase
 
 from parameterized import parameterized
 
 from pyrelational.datasets import (
     BreastCancerDataset,
```

### Comparing `pyrelational-1.0.1/tests/datasets/test_regression_datasets.py` & `pyrelational-1.0.2/tests/datasets/test_regression_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for pyrelational.datasets.regression datasets
 """
+
 from typing import Type, Union
 from unittest import TestCase
 
 from parameterized import parameterized
 
 from pyrelational.datasets import (
     DiabetesDataset,
```

### Comparing `pyrelational-1.0.1/tests/datasets/test_uci_datasets.py` & `pyrelational-1.0.2/tests/datasets/test_uci_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for uci dataset downloader
 """
+
 import os
 import shutil
 from unittest import TestCase
 
 from parameterized import parameterized_class
 
 from pyrelational.datasets import UCIDatasets
```

### Comparing `pyrelational-1.0.1/tests/informativeness/test_informativeness_scores.py` & `pyrelational-1.0.2/tests/informativeness/test_informativeness_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for uncertainty sampling methods
 """
+
 import math
 from typing import Union
 from unittest import TestCase
 
 import pytest
 import torch
 from parameterized import parameterized
```

### Comparing `pyrelational-1.0.1/tests/model_managers/test_ensemble_model_manager.py` & `pyrelational-1.0.2/tests/model_managers/test_ensemble_model_manager.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/model_managers/test_mc_dropout_model_manager.py` & `pyrelational-1.0.2/tests/model_managers/test_mc_dropout_model_manager.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/model_managers/test_model_managers.py` & `pyrelational-1.0.2/tests/model_managers/test_model_managers.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/oracles/test_oracles.py` & `pyrelational-1.0.2/tests/oracles/test_oracles.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/pipeline/test_pipeline.py` & `pyrelational-1.0.2/tests/pipeline/test_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for active learning manager
 """
+
 from typing import Type
 from unittest import TestCase
 
 import pytest
 from parameterized import parameterized_class
 
 from pyrelational.model_managers.mcdropout_model_manager import (
```

### Comparing `pyrelational-1.0.1/tests/strategies/agnostic_strategy_test_cases.py` & `pyrelational-1.0.2/tests/strategies/agnostic_strategy_test_cases.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/strategies/classification_strategy_test_cases.py` & `pyrelational-1.0.2/tests/strategies/classification_strategy_test_cases.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/strategies/regression_strategy_test_cases.py` & `pyrelational-1.0.2/tests/strategies/regression_strategy_test_cases.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/strategies/test_strategies.py` & `pyrelational-1.0.2/tests/strategies/test_strategies.py`

 * *Files identical despite different names*

### Comparing `pyrelational-1.0.1/tests/test_utils.py` & `pyrelational-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

