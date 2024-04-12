# Comparing `tmp/pyBrainai-1.4.1.0.tar.gz` & `tmp/pyBrainai-1.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBrainai-1.4.1.0.tar", last modified: Tue Apr  9 10:01:34 2024, max compression
+gzip compressed data, was "pyBrainai-1.4.1.1.tar", last modified: Fri Apr 12 10:17:54 2024, max compression
```

## Comparing `pyBrainai-1.4.1.0.tar` & `pyBrainai-1.4.1.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/
--rw-rw-r--   0 root         (0) root         (0)     1088 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      728 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      223 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/
--rw-rw-r--   0 root         (0) root         (0)     2989 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2659 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/_openai_scripts.py
--rw-rw-r--   0 root         (0) root         (0)    27749 2024-04-09 09:56:37.000000 pyBrainai-1.4.1.0/brainai/api_requestor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/api_resources/
--rw-rw-r--   0 root         (0) root         (0)     1099 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/api_resources/abstract/
--rw-rw-r--   0 root         (0) root         (0)      659 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5628 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2677 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/createable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     1676 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/deletable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)    10530 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/engine_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2785 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/listable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     5810 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/nested_resource_class_methods.py
--rw-rw-r--   0 root         (0) root         (0)     3590 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/paginatable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      551 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/abstract/updateable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     7955 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/audio.py
--rw-rw-r--   0 root         (0) root         (0)     4182 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/brainos_completion.py
--rw-rw-r--   0 root         (0) root         (0)     2988 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/chat_completion.py
--rw-rw-r--   0 root         (0) root         (0)     1668 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/completion.py
--rw-rw-r--   0 root         (0) root         (0)      560 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/customer.py
--rw-rw-r--   0 root         (0) root         (0)     4177 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/deployment.py
--rw-rw-r--   0 root         (0) root         (0)     2025 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/edit.py
--rw-rw-r--   0 root         (0) root         (0)     3536 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/embedding.py
--rw-rw-r--   0 root         (0) root         (0)     1718 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/engine.py
--rw-rw-r--   0 root         (0) root         (0)      925 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/error_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/api_resources/experimental/
--rw-rw-r--   0 root         (0) root         (0)      108 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/experimental/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      286 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/experimental/completion_config.py
--rw-rw-r--   0 root         (0) root         (0)     8728 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/file.py
--rw-rw-r--   0 root         (0) root         (0)     5480 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/fine_tune.py
--rw-rw-r--   0 root         (0) root         (0)     2354 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/api_resources/fine_tuning.py
--rw-rw-r--   0 root         (0) root         (0)     8631 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/image.py
--rw-rw-r--   0 root         (0) root         (0)      175 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/model.py
--rw-rw-r--   0 root         (0) root         (0)     1425 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/api_resources/moderation.py
--rw-rw-r--   0 root         (0) root         (0)    11147 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/brainai_object.py
--rw-rw-r--   0 root         (0) root         (0)      870 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/brainai_response.py
--rw-rw-r--   0 root         (0) root         (0)    50559 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.0/brainai/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/datalib/
--rw-rw-r--   0 root         (0) root         (0)      666 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/datalib/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      277 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/datalib/common.py
--rw-rw-r--   0 root         (0) root         (0)      336 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/datalib/numpy_helper.py
--rw-rw-r--   0 root         (0) root         (0)      345 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.0/brainai/datalib/pandas_helper.py
--rw-rw-r--   0 root         (0) root         (0)     8851 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/embeddings_utils.py
--rw-rw-r--   0 root         (0) root         (0)     4485 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/error.py
--rw-rw-r--   0 root         (0) root         (0)      445 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/object_classes.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/test/
--rw-rw-r--   0 root         (0) root         (0)      654 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12225 2024-04-09 09:47:58.000000 pyBrainai-1.4.1.0/brainai/test/brainos_test.py
--rw-rw-r--   0 root         (0) root         (0)     2141 2024-04-09 09:41:03.000000 pyBrainai-1.4.1.0/brainai/test/models_test.py
--rw-rw-r--   0 root         (0) root         (0)     4176 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/test/other_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/brainai/tests/asyncio/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/asyncio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2464 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/asyncio/test_endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     3691 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_api_requestor.py
--rw-rw-r--   0 root         (0) root         (0)     3001 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_endpoints.py
--rw-rw-r--   0 root         (0) root         (0)     1209 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1459 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_file_cli.py
--rw-rw-r--   0 root         (0) root         (0)     2073 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_long_examples_validator.py
--rw-rw-r--   0 root         (0) root         (0)     6737 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_url_composition.py
--rw-rw-r--   0 root         (0) root         (0)     1851 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/tests/test_util.py
--rw-rw-r--   0 root         (0) root         (0)     1240 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/brainai/upload_progress.py
--rw-rw-r--   0 root         (0) root         (0)     5540 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/util.py
--rw-rw-r--   0 root         (0) root         (0)    35135 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.0/brainai/validators.py
--rw-rw-r--   0 root         (0) root         (0)       17 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.0/brainai/version.py
--rw-rw-r--   0 root         (0) root         (0)    10692 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.0/brainai/wandb_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/pyBrainai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      728 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2262 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-09 10:01:34.000000 pyBrainai-1.4.1.0/pyBrainai.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      510 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 10:01:34.515308 pyBrainai-1.4.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/
+-rw-rw-r--   0 root         (0) root         (0)     1088 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      223 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/
+-rw-rw-r--   0 root         (0) root         (0)     2989 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.1/brainai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2659 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.1/brainai/_openai_scripts.py
+-rw-rw-r--   0 root         (0) root         (0)    27749 2024-04-09 09:56:37.000000 pyBrainai-1.4.1.1/brainai/api_requestor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/api_resources/
+-rw-rw-r--   0 root         (0) root         (0)     1099 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/api_resources/abstract/
+-rw-rw-r--   0 root         (0) root         (0)      659 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5628 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     2677 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/createable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     1676 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/deletable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)    10530 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/engine_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     2785 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/listable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     5810 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/nested_resource_class_methods.py
+-rw-rw-r--   0 root         (0) root         (0)     3590 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/paginatable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      551 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/abstract/updateable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     7955 2024-04-12 10:15:23.000000 pyBrainai-1.4.1.1/brainai/api_resources/audio.py
+-rw-rw-r--   0 root         (0) root         (0)     4182 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/brainos_completion.py
+-rw-rw-r--   0 root         (0) root         (0)     2988 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/chat_completion.py
+-rw-rw-r--   0 root         (0) root         (0)     1668 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/completion.py
+-rw-rw-r--   0 root         (0) root         (0)      560 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/customer.py
+-rw-rw-r--   0 root         (0) root         (0)     4177 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/deployment.py
+-rw-rw-r--   0 root         (0) root         (0)     2025 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/edit.py
+-rw-rw-r--   0 root         (0) root         (0)     3536 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/embedding.py
+-rw-rw-r--   0 root         (0) root         (0)     1718 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/engine.py
+-rw-rw-r--   0 root         (0) root         (0)      925 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/error_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/api_resources/experimental/
+-rw-rw-r--   0 root         (0) root         (0)      108 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/experimental/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      286 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/experimental/completion_config.py
+-rw-rw-r--   0 root         (0) root         (0)     8728 2024-04-12 10:15:24.000000 pyBrainai-1.4.1.1/brainai/api_resources/file.py
+-rw-rw-r--   0 root         (0) root         (0)     5480 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/fine_tune.py
+-rw-rw-r--   0 root         (0) root         (0)     2354 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/fine_tuning.py
+-rw-rw-r--   0 root         (0) root         (0)     8631 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/image.py
+-rw-rw-r--   0 root         (0) root         (0)      175 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/model.py
+-rw-rw-r--   0 root         (0) root         (0)     1425 2024-04-12 10:15:25.000000 pyBrainai-1.4.1.1/brainai/api_resources/moderation.py
+-rw-rw-r--   0 root         (0) root         (0)    11147 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.1/brainai/brainai_object.py
+-rw-rw-r--   0 root         (0) root         (0)      870 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.1/brainai/brainai_response.py
+-rw-rw-r--   0 root         (0) root         (0)    50559 2024-04-09 09:17:57.000000 pyBrainai-1.4.1.1/brainai/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/datalib/
+-rw-rw-r--   0 root         (0) root         (0)      666 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/datalib/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      277 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.1/brainai/datalib/common.py
+-rw-rw-r--   0 root         (0) root         (0)      336 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.1/brainai/datalib/numpy_helper.py
+-rw-rw-r--   0 root         (0) root         (0)      345 2024-04-09 09:17:58.000000 pyBrainai-1.4.1.1/brainai/datalib/pandas_helper.py
+-rw-rw-r--   0 root         (0) root         (0)     8851 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/embeddings_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     4485 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.1/brainai/error.py
+-rw-rw-r--   0 root         (0) root         (0)      445 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.1/brainai/object_classes.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/test/
+-rw-rw-r--   0 root         (0) root         (0)      654 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/test/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    12225 2024-04-09 09:47:58.000000 pyBrainai-1.4.1.1/brainai/test/brainos_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2141 2024-04-09 09:41:03.000000 pyBrainai-1.4.1.1/brainai/test/models_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4176 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/test/other_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/brainai/tests/asyncio/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/asyncio/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2464 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/asyncio/test_endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     3691 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_api_requestor.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_endpoints.py
+-rw-rw-r--   0 root         (0) root         (0)     1209 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1459 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_file_cli.py
+-rw-rw-r--   0 root         (0) root         (0)     2073 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_long_examples_validator.py
+-rw-rw-r--   0 root         (0) root         (0)     6737 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_url_composition.py
+-rw-rw-r--   0 root         (0) root         (0)     1851 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/tests/test_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1240 2024-04-09 09:18:00.000000 pyBrainai-1.4.1.1/brainai/upload_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     5540 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/util.py
+-rw-rw-r--   0 root         (0) root         (0)    35135 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.1/brainai/validators.py
+-rw-rw-r--   0 root         (0) root         (0)       17 2024-04-09 09:17:56.000000 pyBrainai-1.4.1.1/brainai/version.py
+-rw-rw-r--   0 root         (0) root         (0)    10692 2024-04-09 09:17:59.000000 pyBrainai-1.4.1.1/brainai/wandb_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/pyBrainai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      728 2024-04-12 10:17:54.000000 pyBrainai-1.4.1.1/pyBrainai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-12 10:17:54.000000 pyBrainai-1.4.1.1/pyBrainai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 10:17:54.000000 pyBrainai-1.4.1.1/pyBrainai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-12 10:17:54.000000 pyBrainai-1.4.1.1/pyBrainai.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      510 2024-04-12 10:15:33.000000 pyBrainai-1.4.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 10:17:54.663153 pyBrainai-1.4.1.1/setup.cfg
```

### Comparing `pyBrainai-1.4.1.0/LICENSE` & `pyBrainai-1.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/PKG-INFO` & `pyBrainai-1.4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBrainai
-Version: 1.4.1.0
+Version: 1.4.1.1
 Summary: Python version of brainai SDK
 Author-email: yaojianqu <game781120@126.com>
 Project-URL: Homepage, https://github.com/yaojianqu/py-brainai-sdk
 Project-URL: Issues, https://github.com/yaojianqu/py-brainai-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyBrainai-1.4.1.0/brainai/__init__.py` & `pyBrainai-1.4.1.1/brainai/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/_openai_scripts.py` & `pyBrainai-1.4.1.1/brainai/_openai_scripts.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_requestor.py` & `pyBrainai-1.4.1.1/brainai/api_requestor.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/__init__.py` & `pyBrainai-1.4.1.1/brainai/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/__init__.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/createable_api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/deletable_api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/engine_api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/engine_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/listable_api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/nested_resource_class_methods.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/paginatable_api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/paginatable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/abstract/updateable_api_resource.py` & `pyBrainai-1.4.1.1/brainai/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/audio.py` & `pyBrainai-1.4.1.1/brainai/api_resources/audio.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/brainos_completion.py` & `pyBrainai-1.4.1.1/brainai/api_resources/brainos_completion.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/chat_completion.py` & `pyBrainai-1.4.1.1/brainai/api_resources/chat_completion.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/completion.py` & `pyBrainai-1.4.1.1/brainai/api_resources/completion.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/customer.py` & `pyBrainai-1.4.1.1/brainai/api_resources/customer.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/deployment.py` & `pyBrainai-1.4.1.1/brainai/api_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/edit.py` & `pyBrainai-1.4.1.1/brainai/api_resources/edit.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/embedding.py` & `pyBrainai-1.4.1.1/brainai/api_resources/embedding.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/engine.py` & `pyBrainai-1.4.1.1/brainai/api_resources/engine.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/error_object.py` & `pyBrainai-1.4.1.1/brainai/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/file.py` & `pyBrainai-1.4.1.1/brainai/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/fine_tune.py` & `pyBrainai-1.4.1.1/brainai/api_resources/fine_tune.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/fine_tuning.py` & `pyBrainai-1.4.1.1/brainai/api_resources/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/image.py` & `pyBrainai-1.4.1.1/brainai/api_resources/image.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/api_resources/moderation.py` & `pyBrainai-1.4.1.1/brainai/api_resources/moderation.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/brainai_object.py` & `pyBrainai-1.4.1.1/brainai/brainai_object.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/brainai_response.py` & `pyBrainai-1.4.1.1/brainai/brainai_response.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/cli.py` & `pyBrainai-1.4.1.1/brainai/cli.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/datalib/__init__.py` & `pyBrainai-1.4.1.1/brainai/datalib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/embeddings_utils.py` & `pyBrainai-1.4.1.1/brainai/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/error.py` & `pyBrainai-1.4.1.1/brainai/error.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/test/__init__.py` & `pyBrainai-1.4.1.1/brainai/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/test/brainos_test.py` & `pyBrainai-1.4.1.1/brainai/test/brainos_test.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/test/models_test.py` & `pyBrainai-1.4.1.1/brainai/test/models_test.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/test/other_test.py` & `pyBrainai-1.4.1.1/brainai/test/other_test.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/asyncio/test_endpoints.py` & `pyBrainai-1.4.1.1/brainai/tests/asyncio/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_api_requestor.py` & `pyBrainai-1.4.1.1/brainai/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_endpoints.py` & `pyBrainai-1.4.1.1/brainai/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_exceptions.py` & `pyBrainai-1.4.1.1/brainai/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_file_cli.py` & `pyBrainai-1.4.1.1/brainai/tests/test_file_cli.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_long_examples_validator.py` & `pyBrainai-1.4.1.1/brainai/tests/test_long_examples_validator.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_url_composition.py` & `pyBrainai-1.4.1.1/brainai/tests/test_url_composition.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/tests/test_util.py` & `pyBrainai-1.4.1.1/brainai/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/upload_progress.py` & `pyBrainai-1.4.1.1/brainai/upload_progress.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/util.py` & `pyBrainai-1.4.1.1/brainai/util.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/validators.py` & `pyBrainai-1.4.1.1/brainai/validators.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/brainai/wandb_logger.py` & `pyBrainai-1.4.1.1/brainai/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pyBrainai-1.4.1.0/pyBrainai.egg-info/PKG-INFO` & `pyBrainai-1.4.1.1/pyBrainai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBrainai
-Version: 1.4.1.0
+Version: 1.4.1.1
 Summary: Python version of brainai SDK
 Author-email: yaojianqu <game781120@126.com>
 Project-URL: Homepage, https://github.com/yaojianqu/py-brainai-sdk
 Project-URL: Issues, https://github.com/yaojianqu/py-brainai-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyBrainai-1.4.1.0/pyBrainai.egg-info/SOURCES.txt` & `pyBrainai-1.4.1.1/pyBrainai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

