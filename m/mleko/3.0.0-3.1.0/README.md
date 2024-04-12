# Comparing `tmp/mleko-3.0.0.tar.gz` & `tmp/mleko-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-3.0.0.tar", max compression
+gzip compressed data, was "mleko-3.1.0.tar", max compression
```

## Comparing `mleko-3.0.0.tar` & `mleko-3.1.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    10947 2024-04-05 08:27:13.105788 mleko-3.0.0/LICENSE
--rw-r--r--   0        0        0     4728 2024-04-05 08:27:13.105788 mleko-3.0.0/README.md
--rw-r--r--   0        0        0     1976 2024-04-05 08:27:41.730234 mleko-3.0.0/mleko/__init__.py
--rw-r--r--   0        0        0      585 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    16986 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0     1563 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     1012 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
--rw-r--r--   0        0        0     2989 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1333 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/dict_fingerprinter.py
--rw-r--r--   0        0        0     5578 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
--rw-r--r--   0        0        0    14262 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
--rw-r--r--   0        0        0     1219 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0     1360 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/__init__.py
--rw-r--r--   0        0        0      650 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/base_cache_handler.py
--rw-r--r--   0        0        0     1102 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/joblib_cache_handler.py
--rw-r--r--   0        0        0     1196 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/pickle_cache_handler.py
--rw-r--r--   0        0        0     1508 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/handlers/vaex_cache_handler.py
--rw-r--r--   0        0        0     8312 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      805 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      492 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    15173 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     5640 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/data_schema.py
--rw-r--r--   0        0        0     1614 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0    11612 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     7661 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     5156 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5439 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7257 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5803 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      569 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/base_filter.py
--rw-r--r--   0        0        0     3927 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/expression_filter.py
--rw-r--r--   0        0        0     7236 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/filter/imblearn_resampling_filter.py
--rw-r--r--   0        0        0     1197 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     6118 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    20008 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0    12998 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      680 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     4254 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     6732 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0     1612 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/__init__.py
--rw-r--r--   0        0        0     9362 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/base_transformer.py
--rw-r--r--   0        0        0     6882 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/composite_transformer.py
--rw-r--r--   0        0        0     4743 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/frequency_encoder_transformer.py
--rw-r--r--   0        0        0    11525 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/label_encoder_transformer.py
--rw-r--r--   0        0        0     3744 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py
--rw-r--r--   0        0        0     4150 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/dataset/transform/min_max_scaler_transformer.py
--rw-r--r--   0        0        0      388 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/model/__init__.py
--rw-r--r--   0        0        0    15073 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/model/base_model.py
--rw-r--r--   0        0        0    10169 2024-04-05 08:27:13.109788 mleko-3.0.0/mleko/model/lgbm_model.py
--rw-r--r--   0        0        0      413 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/model/tune/__init__.py
--rw-r--r--   0        0        0     3767 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/model/tune/base_tuner.py
--rw-r--r--   0        0        0    15426 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/model/tune/optuna_tuner.py
--rw-r--r--   0        0        0      645 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4497 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     9723 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      874 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     3832 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     6151 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2994 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/filter_step.py
--rw-r--r--   0        0        0     2780 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     7816 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/model_step.py
--rw-r--r--   0        0        0     2903 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0     5744 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/transform_step.py
--rw-r--r--   0        0        0     3430 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/pipeline/steps/tune_step.py
--rw-r--r--   0        0        0        0 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/py.typed
--rw-r--r--   0        0        0      766 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     9753 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3431 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      743 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1414 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2837 2024-04-05 08:27:13.113788 mleko-3.0.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2608 2024-04-05 08:27:41.730234 mleko-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-04-12 11:13:42.978676 mleko-3.1.0/LICENSE
+-rw-r--r--   0        0        0     4728 2024-04-12 11:13:42.978676 mleko-3.1.0/README.md
+-rw-r--r--   0        0        0     1976 2024-04-12 11:14:14.766808 mleko-3.1.0/mleko/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    16986 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0     1563 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     1012 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py
+-rw-r--r--   0        0        0     2989 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1333 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/dict_fingerprinter.py
+-rw-r--r--   0        0        0     5578 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py
+-rw-r--r--   0        0        0    14262 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py
+-rw-r--r--   0        0        0     1219 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0     1360 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/__init__.py
+-rw-r--r--   0        0        0      650 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/base_cache_handler.py
+-rw-r--r--   0        0        0     1102 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/joblib_cache_handler.py
+-rw-r--r--   0        0        0     1196 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/pickle_cache_handler.py
+-rw-r--r--   0        0        0     1508 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/handlers/vaex_cache_handler.py
+-rw-r--r--   0        0        0     8312 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      805 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      492 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1613 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    15173 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     6611 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/data_schema.py
+-rw-r--r--   0        0        0     1614 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0    11612 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     7661 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     5156 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5439 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7257 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5803 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      569 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/__init__.py
+-rw-r--r--   0        0        0     1615 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/base_filter.py
+-rw-r--r--   0        0        0     3927 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/expression_filter.py
+-rw-r--r--   0        0        0     7236 2024-04-12 11:13:42.982676 mleko-3.1.0/mleko/dataset/filter/imblearn_resampling_filter.py
+-rw-r--r--   0        0        0     1197 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     6118 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    20008 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0    12998 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      680 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     4254 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     6732 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1612 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     9362 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     6882 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4743 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0    11533 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3744 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4150 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      388 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/__init__.py
+-rw-r--r--   0        0        0    18804 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/base_model.py
+-rw-r--r--   0        0        0    10745 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/lgbm_model.py
+-rw-r--r--   0        0        0      413 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/tune/__init__.py
+-rw-r--r--   0        0        0     3767 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/tune/base_tuner.py
+-rw-r--r--   0        0        0    15426 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/model/tune/optuna_tuner.py
+-rw-r--r--   0        0        0      645 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4497 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     9723 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      874 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     3832 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     6151 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2994 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/filter_step.py
+-rw-r--r--   0        0        0     2780 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     7816 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/model_step.py
+-rw-r--r--   0        0        0     2903 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     5744 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0     3430 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/pipeline/steps/tune_step.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/py.typed
+-rw-r--r--   0        0        0      766 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     9753 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3431 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      743 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1414 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     3641 2024-04-12 11:13:42.986676 mleko-3.1.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2608 2024-04-12 11:14:14.766808 mleko-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 mleko-3.1.0/PKG-INFO
```

### Comparing `mleko-3.0.0/LICENSE` & `mleko-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/README.md` & `mleko-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/__init__.py` & `mleko-3.1.0/mleko/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 By integrating these features, `mleko` serves as a comprehensive toolkit for machine learning
 practitioners looking to build robust models efficiently.
 """
 
 from __future__ import annotations
 
 
-__version__ = "3.0.0"
+__version__ = "3.1.0"
```

### Comparing `mleko-3.0.0/mleko/cache/__init__.py` & `mleko-3.1.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/cache_mixin.py` & `mleko-3.1.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/__init__.py` & `mleko-3.1.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/callable_source_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/dict_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/dict_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/optuna_pruner_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/optuna_sampler_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-3.1.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/handlers/__init__.py` & `mleko-3.1.0/mleko/cache/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/handlers/base_cache_handler.py` & `mleko-3.1.0/mleko/cache/handlers/base_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/handlers/joblib_cache_handler.py` & `mleko-3.1.0/mleko/cache/handlers/joblib_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/handlers/pickle_cache_handler.py` & `mleko-3.1.0/mleko/cache/handlers/pickle_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/handlers/vaex_cache_handler.py` & `mleko-3.1.0/mleko/cache/handlers/vaex_cache_handler.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/cache/lru_cache_mixin.py` & `mleko-3.1.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/__init__.py` & `mleko-3.1.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/convert/base_converter.py` & `mleko-3.1.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-3.1.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/data_schema.py` & `mleko-3.1.0/mleko/dataset/data_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for DataSchema class, used for storing type information about the dataset."""
 
 from __future__ import annotations
 
 import copy
 from typing import Literal
 
+from mleko.cache.fingerprinters.dict_fingerprinter import DictFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 
 
 logger = CustomLogger()
 """The logger for the module."""
 
 DataType = Literal["numerical", "categorical", "boolean", "datetime", "timedelta"]
@@ -49,14 +50,40 @@
             "numerical": sorted(list(numerical)),
             "categorical": sorted(list(categorical)),
             "boolean": sorted(list(boolean)),
             "datetime": sorted(list(datetime)),
             "timedelta": sorted(list(timedelta)),
         }
 
+    def __eq__(self, other: object) -> bool:
+        """Check if two DataSchema objects are equal.
+
+        Args:
+            other: Object to compare with.
+
+        Returns:
+            True if the two DataSchema objects are equal, False otherwise.
+        """
+        return isinstance(other, DataSchema) and DictFingerprinter().fingerprint(
+            self.to_dict()
+        ) == DictFingerprinter().fingerprint(other.to_dict())
+
+    def __hash__(self) -> int:
+        """Get the hash of the DataSchema.
+
+        Warning:
+            This method is not intended to be used for stable hashing across runs. Please
+            refer to the `DictFingerprinter` class in the `mleko.utils.fingerprinter` module
+            for stable hashing of the DataSchema.
+
+        Returns:
+            Hash of the DataSchema.
+        """
+        return hash(DictFingerprinter().fingerprint(self.to_dict()))
+
     def __repr__(self) -> str:
         """Get the string representation of DataSchema.
 
         Returns:
             String representation of DataSchema.
         """
         features_str = ", ".join(f"{dtype}={features}" for dtype, features in self.features.items() if features)
```

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/__init__.py` & `mleko-3.1.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-3.1.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-3.1.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-3.1.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-3.1.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-3.1.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-3.1.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/filter/__init__.py` & `mleko-3.1.0/mleko/dataset/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/filter/base_filter.py` & `mleko-3.1.0/mleko/dataset/filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/filter/expression_filter.py` & `mleko-3.1.0/mleko/dataset/filter/expression_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/filter/imblearn_resampling_filter.py` & `mleko-3.1.0/mleko/dataset/filter/imblearn_resampling_filter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/ingest/__init__.py` & `mleko-3.1.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/ingest/base_ingester.py` & `mleko-3.1.0/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-3.1.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-3.1.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/split/__init__.py` & `mleko-3.1.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/split/base_splitter.py` & `mleko-3.1.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/split/expression_splitter.py` & `mleko-3.1.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/split/random_splitter.py` & `mleko-3.1.0/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/transform/__init__.py` & `mleko-3.1.0/mleko/dataset/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/transform/base_transformer.py` & `mleko-3.1.0/mleko/dataset/transform/base_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/transform/composite_transformer.py` & `mleko-3.1.0/mleko/dataset/transform/composite_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/transform/frequency_encoder_transformer.py` & `mleko-3.1.0/mleko/dataset/transform/frequency_encoder_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/transform/label_encoder_transformer.py` & `mleko-3.1.0/mleko/dataset/transform/label_encoder_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Module for the label encoder transformer."""
 
 from __future__ import annotations
 
-import json
 import re
 from pathlib import Path
 from typing import Hashable
 
 import vaex
 import vaex.array_types
 
+from mleko.cache.fingerprinters import DictFingerprinter
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column
 
 from .base_transformer import BaseTransformer
 
@@ -191,15 +191,15 @@
         Returns:
             A hashable object that uniquely identifies the transformer.
         """
         return (
             super()._fingerprint(),
             self._allow_unseen,
             self._encode_null,
-            json.dumps(self._label_dict, sort_keys=True) if self._label_dict is not None else None,
+            DictFingerprinter().fingerprint(self._label_dict),
         )
 
     def _fit_using_label_dict(self, feature: str, observed_labels: list[str]) -> bool:
         """Attempts to fit the label dictionary for the specified feature.
 
         If the label dictionary is not provided or the feature is not in the label dictionary, the function will
         return False. Otherwise, it will fit the label dictionary and return True.
```

### Comparing `mleko-3.0.0/mleko/dataset/transform/max_abs_scaler_transformer.py` & `mleko-3.1.0/mleko/dataset/transform/max_abs_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/dataset/transform/min_max_scaler_transformer.py` & `mleko-3.1.0/mleko/dataset/transform/min_max_scaler_transformer.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/model/base_model.py` & `mleko-3.1.0/mleko/model/base_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Module for the base model class."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, Hashable, Union
 
+import pandas as pd
 import vaex
 
 from mleko.cache.fingerprinters import DictFingerprinter, VaexFingerprinter
 from mleko.cache.handlers import JOBLIB_CACHE_HANDLER, VAEX_DATAFRAME_CACHE_HANDLER
 from mleko.cache.lru_cache_mixin import LRUCacheMixin
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
+from mleko.utils.vaex_helpers import HashableVaexDataFrame, get_columns
 
 
 logger = CustomLogger()
 """The logger for the module."""
 
 HyperparametersType = Dict[
     str,
@@ -41,45 +44,61 @@
     specified DataFrame and transforms the specified features in the DataFrame.
     """
 
     def __init__(
         self,
         features: list[str] | tuple[str, ...] | None,
         ignore_features: list[str] | tuple[str, ...] | None,
+        memoized_dataset_cache_size: int | None,
         cache_directory: str | Path,
         cache_size: int,
     ) -> None:
         """Initializes the model and ensures the destination directory exists.
 
         Note:
             The `features` and `ignore_features` arguments are mutually exclusive. If both are specified, a
             `ValueError` is raised.
 
+        Warning:
+            The `memoized_dataset_cache_size` parameter is experimental and should be used with caution. It refers to
+            the number of datasets to keep in memory for speeding up repeated training. This can be useful when
+            hyperparameter tuning or cross-validation is performed, as the dataset does not need to be loaded from disk
+            every time. However, this can lead to memory issues if the dataset is too large. Specify 0 to disable the
+            cache. When finished with the fitting and transforming, please call the `_clear_dataset_cache` method to
+            clear the cache and free up memory.
+
         Args:
             features: List of feature names to be used by the model. If None, the default is all features
                 applicable to the model.
             ignore_features: List of feature names to be ignored by the model. If None, the default is to
                 ignore no features.
+            memoized_dataset_cache_size: The number of datasets to keep in memory for speeding up repeated training.
+                When finished with the fitting and transforming, please call the `_clear_dataset_cache` method to clear
+                the cache and free up memory. Specify 0 to disable the cache.
             cache_directory: Directory where the cache will be stored locally.
             cache_size: The maximum number of entries to keep in the cache.
 
         Raises:
             ValueError: If both `features` and `ignore_features` are specified.
         """
         super().__init__(cache_directory, cache_size)
+        self._memoized_dataset_cache_size = memoized_dataset_cache_size
+
         if features is not None and ignore_features is not None:
             msg = "Both `features` and `ignore_features` have been specified. The arguments are mutually exclusive."
             logger.error(msg)
             raise ValueError(msg)
 
         self._model = None
         self._hyperparameters: HyperparametersType = {}
         self._features: tuple[str, ...] | None = tuple(features) if features is not None else None
         self._ignore_features: tuple[str, ...] = tuple(ignore_features) if ignore_features is not None else tuple()
 
+        self._memoized_load_dataset = lru_cache(maxsize=self._memoized_dataset_cache_size)(self._memoized_load_dataset)
+
     def fit(
         self,
         data_schema: DataSchema,
         train_dataframe: vaex.DataFrame,
         validation_dataframe: vaex.DataFrame | None = None,
         hyperparameters: HyperparametersType | None = None,
         cache_group: str | None = None,
@@ -248,14 +267,18 @@
                 VAEX_DATAFRAME_CACHE_HANDLER,
             ],
             disable_cache=disable_cache,
         )
         self._assign_model(model)
         return model, metrics, df_train, df_validation
 
+    def clear_load_dataset_cache(self) -> None:
+        """Clears the cache for the `_memoized_load_dataset` method."""
+        self._memoized_load_dataset.cache_clear()  # type: ignore
+
     def _fit_transform(
         self,
         data_schema: DataSchema,
         train_dataframe: vaex.DataFrame,
         validation_dataframe: vaex.DataFrame | None = None,
         hyperparameters: HyperparametersType | None = None,
     ) -> tuple[Any, dict[str, dict[str, list[Any]]], vaex.DataFrame, vaex.DataFrame | None]:
@@ -303,14 +326,68 @@
         """
         return sorted(
             set(self._default_features(data_schema)) - set(self._ignore_features)
             if self._features is None
             else self._features
         )
 
+    def _load_dataset(
+        self,
+        data_schema: DataSchema,
+        dataframe: vaex.DataFrame,
+        additional_features: list[str] | None = None,
+    ) -> pd.DataFrame:
+        """Load the dataset into memory.
+
+        Warning:
+            This method should be used with caution, as it loads the entire dataset into memory as a pandas DataFrame.
+
+        Args:
+            data_schema: The data schema of the dataframe.
+            dataframe: The dataframe to load.
+            additional_features: Additional features to load, such as the target feature.
+
+        Returns:
+            A pandas DataFrame with the loaded data.
+        """
+        feature_names = self._feature_set(data_schema)
+        df = get_columns(dataframe, feature_names + (additional_features if additional_features else [])).to_pandas_df()
+        return df  # type: ignore
+
+    def _memoized_load_dataset(
+        self,
+        data_schema: DataSchema,
+        dataframe: HashableVaexDataFrame,
+        additional_features: tuple[str, ...] | None = None,
+        name: str | None = None,
+    ) -> pd.DataFrame:
+        """Load the dataset into memory and memoize the result.
+
+        Warning:
+            This method should be used with caution, as it loads the entire dataset into memory as a pandas DataFrame.
+            The returned DataFrame will be memoized using the `functools.lru_cache` to avoid reloading the
+            dataset multiple times. The cache size is set to the `memoized_dataset_cache_size` attribute.
+
+        Args:
+            data_schema: The data schema of the dataframe.
+            dataframe: The dataframe to load, wrapped in a `HashableVaexDataFrame` object.
+            additional_features: Additional features to load, such as the target feature.
+            name: Name of the dataset to be used in the log message.
+
+        Returns:
+            A pandas DataFrame with the loaded data.
+        """
+        if name is not None:
+            name = f"{name.strip()} "
+        else:
+            name = ""
+
+        logger.info(f"Loading the {name}dataset into memory.")
+        return self._load_dataset(data_schema, dataframe.df, list(additional_features) if additional_features else None)
+
     @abstractmethod
     def _fit(
         self,
         data_schema: DataSchema,
         train_dataframe: vaex.DataFrame,
         validation_dataframe: vaex.DataFrame | None = None,
         hyperparameters: HyperparametersType | None = None,
```

### Comparing `mleko-3.0.0/mleko/model/lgbm_model.py` & `mleko-3.1.0/mleko/model/lgbm_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pandas as pd
 import vaex
 from lightgbm.sklearn import _LGBM_ScikitEvalMetricType
 
 from mleko.dataset.data_schema import DataSchema
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
-from mleko.utils.vaex_helpers import get_columns
+from mleko.utils.vaex_helpers import HashableVaexDataFrame
 
 from .base_model import BaseModel, HyperparametersType
 
 
 logger = CustomLogger()
 """The logger for the module."""
 
@@ -59,36 +59,47 @@
         model: lgb.LGBMClassifier | lgb.LGBMRegressor,
         eval_metric: _LGBM_ScikitEvalMetricType | None = None,
         log_eval_period: int | None = 10,
         features: list[str] | tuple[str, ...] | None = None,
         ignore_features: list[str] | tuple[str, ...] | None = None,
         random_state: int | None = 42,
         verbosity: int = logging.INFO,
+        memoized_dataset_cache_size: int | None = 0,
         cache_directory: str | Path = "data/lgbm-model",
         cache_size: int = 1,
     ) -> None:
         """Initialize the LightGBM model with the given hyperparameters.
 
         Note:
             Features and ignore_features are mutually exclusive. If both are provided, a `ValueError` will be raised.
             By default, all features are used. If ignore_features is provided, all features except the ones in
             ignore_features will be used. If features is provided, only the features in features will be used.
 
+        Warning:
+            The `memoized_dataset_cache_size` parameter is experimental and should be used with caution. It refers to
+            the number of datasets to keep in memory for speeding up repeated training. This can be useful when
+            hyperparameter tuning or cross-validation is performed, as the dataset does not need to be loaded from disk
+            every time. However, this can lead to memory issues if the dataset is too large. Specify 0 to disable the
+            cache. When finished with the fitting and transforming, please call the `_clear_dataset_cache` method to
+            clear the cache and free up memory.
 
         Args:
             target: The name of the target feature.
             model: The LightGBM model to be used.
             eval_metric: Evaluation metric(s) to be used as list of strings or a single string. Refer to
                 https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html#lightgbm.LGBMClassifier.fit
                 to see the list of available metrics and how to define custom metrics.
             log_eval_period: The period to log the evaluation results.
             features: The names of the features to be used as input for the model.
             ignore_features: The names of the features to be ignored.
             random_state: The random state to be used for reproducibility.
             verbosity: The verbosity level of the logger, will be passed to the LightGBM model.
+            memoized_dataset_cache_size: The number of datasets to keep in memory for speeding up repeated training.
+                When finished with the fitting and transforming, please call the `_clear_dataset_cache` method to clear
+                the cache and free up memory. Specify 0 to disable the cache.
             cache_directory: The target directory where the model will be saved.
             cache_size: The maximum number of entries to keep in the cache.
 
         Examples:
             >>> import vaex
             >>> from mleko.model import LGBMModel
             >>> from lightgbm import LGBMClassifier
@@ -101,15 +112,15 @@
             ...     target="class_",
             ...     model=LGBMClassifier(n_estimators=100),
             ...     random_state=42,
             ...     features=["sepal_width", "petal_length", "petal_width"],
             ... )
             >>> booster, df_train_pred, df_test_pred = model.fit_transform(data_schema, df_train, df_test, {})
         """
-        super().__init__(features, ignore_features, cache_directory, cache_size)
+        super().__init__(features, ignore_features, memoized_dataset_cache_size, cache_directory, cache_size)
         lgb.register_logger(logger)
 
         self._target = target
         self._model = model
         self._eval_metric = eval_metric
         self._log_eval_period = log_eval_period
         self._random_state = random_state
@@ -147,23 +158,31 @@
 
         if self._target in self._feature_set(data_schema):
             msg = f"Target feature {self._target} is in the feature set."
             logger.error(msg)
             raise ValueError(msg)
 
         validation_datasets: list[tuple[str, pd.DataFrame, pd.Series]] = []
-        logger.info("Loading the training dataset into memory.")
-        train_df = self._load_dataset(data_schema, train_dataframe)
+        train_df = self._memoized_load_dataset(
+            data_schema,
+            HashableVaexDataFrame(train_dataframe),
+            (self._target,),
+            name="training",
+        )
         X_train = train_df[self._feature_set(data_schema)]
         y_train = train_df[self._target]
         validation_datasets.append(("train", X_train, y_train))
 
         if validation_dataframe is not None:
-            logger.info("Loading the validation dataset into memory.")
-            validation_df = self._load_dataset(data_schema, validation_dataframe)
+            validation_df = self._memoized_load_dataset(
+                data_schema,
+                HashableVaexDataFrame(validation_dataframe),
+                (self._target,),
+                name="validation",
+            )
             X_validation = validation_df[self._feature_set(data_schema)]
             y_validation = validation_df[self._target]
             validation_datasets.append(("validation", X_validation, y_validation))
 
         if hyperparameters is None:
             hyperparameters = {}
 
@@ -200,17 +219,15 @@
         Args:
             data_schema: The data schema of the dataframe.
             dataframe: The dataframe to transform.
 
         Returns:
             The transformed dataframe.
         """
-        logger.info("Loading the dataset into memory.")
-        feature_names = self._feature_set(data_schema)
-        dataset = get_columns(dataframe, feature_names).to_pandas_df()
+        dataset = self._memoized_load_dataset(data_schema, HashableVaexDataFrame(dataframe))
         df = dataframe.copy()
 
         logger.info("Transforming the dataset.")
         if isinstance(self._model, lgb.LGBMClassifier):
             probs: np.ndarray = self._model.predict_proba(dataset)  # type: ignore
             for i, prob in enumerate(probs.T):
                 df[f"probability_{i}"] = prob
@@ -238,21 +255,7 @@
             data_schema: The data schema of the dataframes.
 
         Returns:
             The default set of features.
         """
         features = data_schema.get_features(["numerical", "boolean", "categorical"])
         return tuple(str(feature) for feature in features)
-
-    def _load_dataset(self, data_schema: DataSchema, dataframe: vaex.DataFrame) -> pd.DataFrame:
-        """Load the dataset into memory.
-
-        Args:
-            data_schema: The data schema of the dataframe.
-            dataframe: The dataframe to load.
-
-        Returns:
-            A pandas DataFrame with the loaded data.
-        """
-        feature_names = self._feature_set(data_schema)
-        df: pd.DataFrame = get_columns(dataframe, feature_names + [self._target]).to_pandas_df()  # type: ignore
-        return df
```

### Comparing `mleko-3.0.0/mleko/model/tune/base_tuner.py` & `mleko-3.1.0/mleko/model/tune/base_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/model/tune/optuna_tuner.py` & `mleko-3.1.0/mleko/model/tune/optuna_tuner.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/__init__.py` & `mleko-3.1.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/data_container.py` & `mleko-3.1.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/pipeline.py` & `mleko-3.1.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/pipeline_step.py` & `mleko-3.1.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/__init__.py` & `mleko-3.1.0/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/convert_step.py` & `mleko-3.1.0/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-3.1.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/filter_step.py` & `mleko-3.1.0/mleko/pipeline/steps/filter_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/ingest_step.py` & `mleko-3.1.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/model_step.py` & `mleko-3.1.0/mleko/pipeline/steps/model_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/split_step.py` & `mleko-3.1.0/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/transform_step.py` & `mleko-3.1.0/mleko/pipeline/steps/transform_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/pipeline/steps/tune_step.py` & `mleko-3.1.0/mleko/pipeline/steps/tune_step.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/utils/__init__.py` & `mleko-3.1.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/utils/custom_logger.py` & `mleko-3.1.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/utils/decorators.py` & `mleko-3.1.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/utils/file_helpers.py` & `mleko-3.1.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/utils/tqdm_helpers.py` & `mleko-3.1.0/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-3.0.0/mleko/utils/vaex_helpers.py` & `mleko-3.1.0/mleko/utils/vaex_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """This module contains helper functions for working with `vaex` DataFrames."""
 
 from __future__ import annotations
 
+from dataclasses import dataclass
+
 import vaex
 
 
 def get_column(df: vaex.DataFrame, column: str) -> vaex.Expression:
     """Get specified column from a DataFrame as an Expression.
 
     Args:
@@ -84,7 +86,33 @@
     """
     idx_name = "index"
     df[idx_name] = vaex.vrange(0, df.shape[0])
     index = get_column(df, idx_name)
     selection = get_filtered_df(df, index.isin(indices))
     selection.delete_virtual_column(idx_name)
     return selection.extract()
+
+
+@dataclass(frozen=True)
+class HashableVaexDataFrame:
+    """An immutable hashable wrapper around a `vaex.DataFrame`."""
+
+    df: vaex.DataFrame
+
+    def __eq__(self, other) -> bool:
+        """Check if two `HashableVaexDataFrame` objects are equal.
+
+        Args:
+            other: `HashableVaexDataFrame` object to compare with.
+
+        Returns:
+            True if the two `HashableVaexDataFrame` objects are equal, False otherwise.
+        """
+        return isinstance(other, HashableVaexDataFrame) and self.df.fingerprint() == other.df.fingerprint()
+
+    def __hash__(self) -> int:
+        """Get the hash of the `HashableVaexDataFrame`.
+
+        Returns:
+            Hash of the `HashableVaexDataFrame`.
+        """
+        return hash(self.df.fingerprint())
```

### Comparing `mleko-3.0.0/pyproject.toml` & `mleko-3.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "3.0.0"
+version = "3.1.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/klarna-incubator/mleko"
 repository = "https://github.com/klarna-incubator/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-3.0.0/PKG-INFO` & `mleko-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 3.0.0
+Version: 3.1.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/klarna-incubator/mleko
 License: Apache-2.0
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.1,<3.11.dev0
 Classifier: Development Status :: 4 - Beta
```

