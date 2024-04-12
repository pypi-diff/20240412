# Comparing `tmp/datumaro-1.6.0rc0.tar.gz` & `tmp/datumaro-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.6.0rc0.tar", last modified: Fri Oct  6 09:42:26 2023, max compression
+gzip compressed data, was "datumaro-1.6.0rc1.tar", last modified: Fri Jan 12 02:42:38 2024, max compression
```

## Comparing `datumaro-1.6.0rc0.tar` & `datumaro-1.6.0rc1.tar`

### file list

```diff
@@ -1,386 +1,395 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.527422 datumaro-1.6.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)   391964 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2023-10-06 09:42:26.527422 datumaro-1.6.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/requirements-default.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.483422 datumaro-1.6.0rc0/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.483422 datumaro-1.6.0rc0/rust/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/rust/src/coco_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/rust/src/page_maps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/rust/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 09:42:26.527422 datumaro-1.6.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.475422 datumaro-1.6.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.483422 datumaro-1.6.0rc0/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.483422 datumaro-1.6.0rc0/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.487422 datumaro-1.6.0rc0/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.487422 datumaro-1.6.0rc0/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9340 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.487422 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.487422 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.487422 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.491422 datumaro-1.6.0rc0/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.491422 datumaro-1.6.0rc0/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.491422 datumaro-1.6.0rc0/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13260 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (127)    34942 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25024 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/contexts/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30021 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    25867 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12020 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14785 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19651 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19989 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.495422 datumaro-1.6.0rc0/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41170 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.499422 datumaro-1.6.0rc0/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/merge/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    24403 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    13417 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    89678 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22880 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.499422 datumaro-1.6.0rc0/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.499422 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.499422 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    37755 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/configurable_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.503422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.503422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    12457 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)    21483 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23596 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33535 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/page_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16020 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21501 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19503 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18774 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.507422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17906 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (127)    15150 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.511422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    38738 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16317 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31405 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/framework_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.515422 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/interpreters/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    48169 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32124 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.519422 datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.523422 datumaro-1.6.0rc0/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    49413 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    45116 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.523422 datumaro-1.6.0rc0/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12034 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/multi_procs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-06 09:42:14.000000 datumaro-1.6.0rc0/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 09:42:26.483422 datumaro-1.6.0rc0/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-06 09:42:26.000000 datumaro-1.6.0rc0/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)   391964 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/requirements-default.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.764831 datumaro-1.6.0rc1/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/coco_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/datum_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/json_section_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/page_maps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.756832 datumaro-1.6.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.772832 datumaro-1.6.0rc1/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.772832 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.772832 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.780831 datumaro-1.6.0rc1/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.780831 datumaro-1.6.0rc1/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.780831 datumaro-1.6.0rc1/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34942 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34020 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25867 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41283 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14069 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89834 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23625 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.788832 datumaro-1.6.0rc1/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.788832 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.788832 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/configurable_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.792832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21483 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24679 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19062 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38738 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/framework_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49095 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.820832 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49413 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.820832 datumaro-1.6.0rc1/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/import_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/multi_procs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.6.0rc0/3rd-party.txt` & `datumaro-1.6.0rc1/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/LICENSE` & `datumaro-1.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/PKG-INFO` & `datumaro-1.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.0rc0
+Version: 1.6.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,41 +29,41 @@
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: pandas>=1.1.5
-Requires-Dist: openvino==2023.1.0
+Requires-Dist: openvino>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
 Requires-Dist: protobuf<4
 Requires-Dist: tabulate
 Requires-Dist: ovmsclient
 Requires-Dist: tritonclient[all]
 Requires-Dist: scikit-learn
 Requires-Dist: json-stream
 Requires-Dist: opencv-python
 Provides-Extra: tf
 Requires-Dist: tensorflow; extra == "tf"
 Provides-Extra: tfds
-Requires-Dist: tensorflow-datasets; extra == "tfds"
+Requires-Dist: tensorflow-datasets<4.9.3; extra == "tfds"
 Provides-Extra: tf-gpu
 Requires-Dist: tensorflow-gpu; extra == "tf-gpu"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: torchvision; extra == "torch"
 Provides-Extra: default
-Requires-Dist: dvc>=3.0.0; extra == "default"
+Requires-Dist: dvc==3.30.1; extra == "default"
 Requires-Dist: fsspec<=2022.11.0; python_version < "3.8" and extra == "default"
 Requires-Dist: GitPython!=3.1.25,>=3.1.18; extra == "default"
 Requires-Dist: openvino-telemetry>=2022.1.0; extra == "default"
-Requires-Dist: openvino-dev==2023.1.0; extra == "default"
+Requires-Dist: openvino-dev>=2023.2.0; extra == "default"
 
 # Dataset Management Framework (Datumaro)
 
 [![Build status](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml/badge.svg)](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml)
 [![codecov](https://codecov.io/gh/openvinotoolkit/datumaro/branch/develop/graph/badge.svg?token=FG25VU096Q)](https://codecov.io/gh/openvinotoolkit/datumaro)
 
 A framework and CLI tool to build, transform, and analyze datasets.
@@ -105,15 +105,15 @@
   - [Open Images](https://storage.googleapis.com/openimages/web/download.html)
   - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/index.html)
     (`classification`, `detection`, `segmentation`, `action_classification`, `person_layout`)
   - [TF Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/using_your_own_dataset.md)
     (`bboxes`, `masks`)
   - [YOLO](https://github.com/AlexeyAB/darknet#how-to-train-pascal-voc-data) (`bboxes`)
 
-  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/supported_formats).
+  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/formats).
 - Dataset building
   - Merging multiple datasets into one
   - Dataset filtering by a custom criteria:
     - remove polygons of a certain class
     - remove images without annotations of a specific class
     - remove `occluded` annotations from images
     - keep only vertically-oriented images
```

### Comparing `datumaro-1.6.0rc0/README.md` & `datumaro-1.6.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   - [Open Images](https://storage.googleapis.com/openimages/web/download.html)
   - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/index.html)
     (`classification`, `detection`, `segmentation`, `action_classification`, `person_layout`)
   - [TF Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/using_your_own_dataset.md)
     (`bboxes`, `masks`)
   - [YOLO](https://github.com/AlexeyAB/darknet#how-to-train-pascal-voc-data) (`bboxes`)
 
-  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/supported_formats).
+  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/formats).
 - Dataset building
   - Merging multiple datasets into one
   - Dataset filtering by a custom criteria:
     - remove polygons of a certain class
     - remove images without annotations of a specific class
     - remove `occluded` annotations from images
     - keep only vertically-oriented images
```

### Comparing `datumaro-1.6.0rc0/pyproject.toml` & `datumaro-1.6.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 omit = [
     "src/datumaro/__main__.py",
     "src/datumaro/version.py",
     "tests/*",
 ]
 
 [tool.cibuildwheel]
+# reference docs - https://cibuildwheel.readthedocs.io/en/stable/options/#build-skip
 build = "cp38-*_x86_64 cp39-*_x86_64 cp310-*_x86_64 cp311-*_x86_64 cp38-*_amd64 cp39-*_amd64 cp310-*_amd64 cp311-*_amd64"
+skip = "*macos*"
 
 [tool.cibuildwheel.linux]
 before-all = [
     "curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs -o rustup-init.sh",
     "sh ./rustup-init.sh -y --default-toolchain stable --profile minimal"
 ]
 
@@ -45,14 +47,17 @@
     # Don't complain if tests don't hit defensive assertion code:
     'raise AssertionError',
     'raise NotImplementedError',
 
     # Don't complain if non-runnable code isn't run:
     'if 0:',
     'if __name__ == .__main__.:',
+
+    # Don't complain for the type checking code:
+    'if TYPE_CHECKING:'
 ]
 
 # don't fail on the code that can be found
 ignore_errors = true
 
 skip_empty = true
```

### Comparing `datumaro-1.6.0rc0/requirements-core.txt` & `datumaro-1.6.0rc1/requirements-core.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # Image generator
 requests
 
 # Sampler
 pandas>=1.1.5
 
 # OpenVINO
-openvino==2023.1.0
+openvino>=2023.2.0
 tokenizers
 
 # Encryption
 cryptography>= 38.03
 
 # Shift analyzer
 pyemd
```

### Comparing `datumaro-1.6.0rc0/rust/src/lib.rs` & `datumaro-1.6.0rc1/rust/src/utils.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,77 @@
 //  Copyright (C) 2023 Intel Corporation
 //
 //  SPDX-License-Identifier: MIT
 
-mod coco_page_mapper;
-mod page_maps;
-mod utils;
-
-use std::{fs::File, io::BufReader, path::Path};
-
-use crate::coco_page_mapper::CocoPageMapper as CocoPageMapperImpl;
+use std::io::{self};
 use pyo3::{
     exceptions::PyValueError,
     prelude::*,
     types::{PyBool, PyDict, PyFloat, PyList, PyUnicode},
 };
-use serde_json;
 
-#[pyclass]
-struct CocoPageMapper {
-    reader: BufReader<File>,
-    mapper: CocoPageMapperImpl,
+pub fn read_skipping_ws(mut reader: impl io::Read) -> io::Result<u8> {
+    loop {
+        let mut byte = 0u8;
+        reader.read_exact(std::slice::from_mut(&mut byte))?;
+        if !byte.is_ascii_whitespace() {
+            return Ok(byte);
+        }
+    }
+}
+
+pub fn invalid_data(msg: &str) -> io::Error {
+    io::Error::new(io::ErrorKind::InvalidData, msg)
+}
+
+pub fn stream_error(error: &str, offset: u64) -> io::Error {
+    let msg = format!("[Parse error, offset={}] {}", offset, error);
+    invalid_data(msg.as_str())
+}
+
+pub fn parse_serde_json_value_from_page<R>(
+    reader: &mut R,
+    offset: u64,
+    size: u64,
+) -> Result<serde_json::Value, io::Error>
+where
+    R: io::Read + io::Seek,
+{
+    reader.seek(io::SeekFrom::Start(offset))?;
+
+    let mut buf = vec![0u8; size as usize];
+    let _ = reader.read(buf.as_mut_slice())?;
+
+    let img_dict_str = String::from_utf8(buf).ok().ok_or(invalid_data(
+        format!("Cannot read offset: {} and size: {}", offset, size).as_str(),
+    ))?;
+
+    serde_json::from_str(img_dict_str.as_str())
+        .ok()
+        .ok_or(invalid_data(
+            format!("Cannot parse to dict offset: {} and size: {}", offset, size).as_str(),
+        ))
+}
+
+pub fn parse_serde_json_value(
+    reader: impl io::Read + io::Seek,
+) -> Result<serde_json::Value, io::Error> {
+    let de = serde_json::Deserializer::from_reader(reader);
+    let mut stream = de.into_iter::<serde_json::Value>();
+    match stream.next().unwrap() {
+        Ok(x) => Ok(x),
+        Err(e) => {
+            let cur_pos = stream.byte_offset();
+            let msg = format!("Parse error: {} at pos: {}", e, cur_pos);
+            Err(invalid_data(msg.as_str()))
+        }
+    }
 }
 
-fn convert_to_py_object(value: &serde_json::Value, py: Python<'_>) -> PyResult<PyObject> {
+pub fn convert_to_py_object(value: &serde_json::Value, py: Python<'_>) -> PyResult<PyObject> {
     if value.is_array() {
         let list = PyList::empty(py);
 
         for child in value.as_array().unwrap() {
             list.append(convert_to_py_object(child, py)?)?;
         }
 
@@ -47,69 +92,12 @@
     } else if value.is_i64() {
         return Ok(value.as_i64().unwrap().to_object(py));
     } else if value.is_u64() {
         return Ok(value.as_u64().unwrap().to_object(py));
     } else if value.is_string() {
         return Ok(PyUnicode::new(py, value.as_str().unwrap()).into());
     } else if value.is_null() {
-        return Ok(PyUnicode::new(py, "null").into());
+        return Ok(py.None());
     } else {
         return Err(PyValueError::new_err("Unknown value type"));
     }
 }
-
-#[pymethods]
-impl CocoPageMapper {
-    #[new]
-    fn py_new(path: String) -> PyResult<Self> {
-        let file = File::open(Path::new(&path))?;
-        let mut reader = BufReader::new(file);
-        let mapper = CocoPageMapperImpl::new(&mut reader)?;
-
-        Ok(CocoPageMapper { reader, mapper })
-    }
-
-    fn licenses(self_: PyRef<Self>) -> PyResult<PyObject> {
-        convert_to_py_object(self_.mapper.licenses(), self_.py())
-    }
-
-    fn info(self_: PyRef<Self>) -> PyResult<PyObject> {
-        convert_to_py_object(self_.mapper.info(), self_.py())
-    }
-
-    fn categories(self_: PyRef<Self>) -> PyResult<PyObject> {
-        convert_to_py_object(self_.mapper.categories(), self_.py())
-    }
-
-    fn get_item_dict(&mut self, py: Python<'_>, img_id: i64) -> PyResult<PyObject> {
-        let item_dict = self.mapper.get_item_dict(img_id, &mut self.reader)?;
-        Ok(convert_to_py_object(&item_dict, py)?)
-    }
-
-    fn get_anns_dict(&mut self, py: Python<'_>, img_id: i64) -> PyResult<PyObject> {
-        let anns_list = PyList::new(
-            py,
-            self.mapper
-                .get_anns_dict(img_id, &mut self.reader)?
-                .iter()
-                .map(|child| convert_to_py_object(child, py).unwrap()),
-        );
-        Ok(anns_list.into())
-    }
-
-    fn get_img_ids(&self) -> Vec<i64> {
-        self.mapper.get_img_ids().to_owned()
-    }
-
-    fn __len__(&self) -> PyResult<usize> {
-        Ok(self.mapper.get_img_ids().len())
-    }
-}
-
-/// Datumaro Rust API
-#[pymodule]
-#[pyo3(name = "rust_api")]
-fn rust_api(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
-    m.add_class::<CocoPageMapper>()?;
-
-    Ok(())
-}
```

### Comparing `datumaro-1.6.0rc0/rust/src/page_maps.rs` & `datumaro-1.6.0rc1/rust/src/page_maps.rs`

 * *Files 13% similar despite different names*

```diff
@@ -30,39 +30,74 @@
 
 #[derive(Debug)]
 pub struct ImgPage {
     pub offset: u64,
     pub size: u32,
 }
 
+pub trait ItemPageMapKeyTrait:
+    std::cmp::Eq + std::hash::Hash + std::clone::Clone + std::fmt::Display
+{
+    fn get_id(parsed_map: HashMap<String, JsonDict>, offset: u64) -> Result<Self, io::Error>
+    where
+        Self: Sized;
+}
+
+impl ItemPageMapKeyTrait for i64 {
+    fn get_id(parsed_map: HashMap<String, JsonDict>, offset: u64) -> Result<Self, io::Error> {
+        parsed_map
+            .get("id")
+            .ok_or(stream_error("Cannot find an image id", offset))?
+            .as_i64()
+            .ok_or(stream_error("The image id is not an integer.", offset))
+    }
+}
+
+impl ItemPageMapKeyTrait for String {
+    fn get_id(parsed_map: HashMap<String, JsonDict>, offset: u64) -> Result<Self, io::Error> {
+        Ok(parsed_map
+            .get("id")
+            .ok_or(stream_error("Cannot find an image id", offset))?
+            .as_str()
+            .ok_or(stream_error("The image id is not an integer.", offset))?
+            .to_string())
+    }
+}
+
 #[derive(Debug)]
-pub struct ImgPageMap {
-    ids: Vec<i64>,
-    pages: HashMap<i64, ImgPage>,
+pub struct ImgPageMap<T>
+where
+    T: ItemPageMapKeyTrait,
+{
+    ids: Vec<T>,
+    pages: HashMap<T, ImgPage>,
 }
 
-impl ImgPageMap {
-    pub fn get_dict<R>(&self, reader: &mut R, img_id: i64) -> Result<JsonDict, io::Error>
+impl<T> ImgPageMap<T>
+where
+    T: ItemPageMapKeyTrait,
+{
+    pub fn get_dict<R>(&self, reader: &mut R, img_id: &T) -> Result<JsonDict, io::Error>
     where
         R: io::Read + io::Seek,
     {
-        match self.pages.get(&img_id) {
+        match self.pages.get(img_id) {
             Some(page) => parse_serde_json_value_from_page(reader, page.offset, page.size as u64),
             None => Err(invalid_data(
                 format!("Image id: {} is not on the page map", img_id).as_str(),
             )),
         }
     }
 
-    pub fn push(&mut self, img_id: i64, page: ImgPage) {
-        self.ids.push(img_id);
-        self.pages.insert(img_id, page);
+    pub fn push(&mut self, img_id: T, page: ImgPage) {
+        self.ids.push(img_id.clone());
+        self.pages.insert(img_id.clone(), page);
     }
 
-    pub fn from_reader(mut reader: impl io::Read + io::Seek) -> Result<ImgPageMap, io::Error> {
+    pub fn from_reader(mut reader: impl io::Read + io::Seek) -> Result<ImgPageMap<T>, io::Error> {
         let mut page_map = ImgPageMap::default();
 
         let (empty, rewind_pos) = is_empty_list(&mut reader)?;
 
         if empty {
             return Ok(page_map);
         } else {
@@ -75,19 +110,15 @@
                     let curr_pos = reader.stream_position()?;
                     let de = serde_json::Deserializer::from_reader(&mut reader);
                     let mut stream = de.into_iter::<HashMap<String, serde_json::Value>>();
                     let offset = curr_pos + stream.byte_offset() as u64;
 
                     match stream.next().unwrap() {
                         Ok(parsed_map) => {
-                            let id = parsed_map
-                                .get("id")
-                                .ok_or(stream_error("Cannot find an image id", offset))?
-                                .as_i64()
-                                .ok_or(stream_error("The image id is not an integer.", offset))?;
+                            let id = ItemPageMapKeyTrait::get_id(parsed_map, offset)?;
 
                             let size = (curr_pos + stream.byte_offset() as u64 - offset) as u32;
                             page_map.push(id, ImgPage { offset, size });
                         }
                         Err(e) => {
                             return Err(stream_error(e.to_string().as_str(), offset));
                         }
@@ -96,30 +127,36 @@
                 b']' => break,
                 _ => {}
             }
         }
         Ok(page_map)
     }
 
-    pub fn ids(&self) -> &Vec<i64> {
+    pub fn ids(&self) -> &Vec<T> {
         return &self.ids;
     }
 }
 
-impl IntoIterator for ImgPageMap {
-    type Item = (i64, ImgPage);
+impl<T> IntoIterator for ImgPageMap<T>
+where
+    T: ItemPageMapKeyTrait,
+{
+    type Item = (T, ImgPage);
 
-    type IntoIter = <HashMap<i64, ImgPage> as IntoIterator>::IntoIter;
+    type IntoIter = <HashMap<T, ImgPage> as IntoIterator>::IntoIter;
 
     fn into_iter(self) -> Self::IntoIter {
         self.pages.into_iter()
     }
 }
 
-impl Default for ImgPageMap {
+impl<T> Default for ImgPageMap<T>
+where
+    T: ItemPageMapKeyTrait,
+{
     fn default() -> Self {
         Self {
             ids: Vec::with_capacity(0),
             pages: HashMap::with_capacity(0),
         }
     }
 }
```

### Comparing `datumaro-1.6.0rc0/setup.py` & `datumaro-1.6.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8",
     install_requires=CORE_REQUIREMENTS,
     extras_require={
         "tf": ["tensorflow"],
-        "tfds": ["tensorflow-datasets"],
+        "tfds": ["tensorflow-datasets<4.9.3"],
         "tf-gpu": ["tensorflow-gpu"],
         "torch": ["torch", "torchvision"],
         "default": DEFAULT_REQUIREMENTS,
     },
     ext_modules=ext_modules,
     entry_points={
         "console_scripts": [
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/capi/pybind.cpp` & `datumaro-1.6.0rc1/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/__main__.py` & `datumaro-1.6.0rc1/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/compare.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/convert.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/download.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/explain.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/explore.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/filter.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/generate.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import argparse
 import logging as log
 import os
 import os.path as osp
 from shutil import rmtree
 
 from datumaro.cli.util.errors import CliException
-from datumaro.plugins.synthetic_data import FractalImageGenerator
 from datumaro.util.definitions import get_datumaro_cache_dir
 
 from ..util import MultilineFormatter
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
@@ -72,14 +71,16 @@
 
 
 def get_sensitive_args():
     return {generate_command: ["output_dir", "model_dir"]}
 
 
 def generate_command(args):
+    from datumaro.plugins.synthetic_data import FractalImageGenerator
+
     log.info("Generating dataset...")
     output_dir = args.output_dir
 
     if osp.isdir(output_dir) and os.listdir(output_dir):
         if args.overwrite:
             rmtree(output_dir)
             os.mkdir(output_dir)
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/info.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/merge.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/patch.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/prune.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/stats.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/transform.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/commands/validate.py` & `datumaro-1.6.0rc1/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/contexts/model.py` & `datumaro-1.6.0rc1/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/contexts/source.py` & `datumaro-1.6.0rc1/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/contexts/util.py` & `datumaro-1.6.0rc1/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/util/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/util/compare.py` & `datumaro-1.6.0rc1/src/datumaro/cli/util/compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 
 import logging as log
 import os
 import os.path as osp
 import warnings
 from collections import Counter
 from enum import Enum, auto
-from itertools import zip_longest
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 import cv2
 import numpy as np
 
-from datumaro.components.media import Image
-
-with warnings.catch_warnings():
-    warnings.simplefilter("ignore")
-    import tensorboardX as tb
-
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset import IDataset
+from datumaro.components.media import Image
 from datumaro.util import parse_str_enum_value
 from datumaro.util.image import save_image
+from datumaro.util.import_util import lazy_import
+
+if TYPE_CHECKING:
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        import tensorboardX as tb
+else:
+    tb = lazy_import("tensorboardX")
 
 
 class DistanceCompareVisualizer:
     class OutputFormat(Enum):
         simple = auto()
         tensorboard = auto()
 
@@ -73,30 +75,26 @@
                 self._label_diff_writer.flush()
                 self._label_diff_writer.close()
 
     def save(self, a: IDataset, b: IDataset):
         if len(a) != len(b):
             print("Datasets have different lengths: %s vs %s" % (len(a), len(b)))
 
-        a_classes = a.categories().get(AnnotationType.label, LabelCategories())
-        b_classes = b.categories().get(AnnotationType.label, LabelCategories())
-        class_mismatch = [
-            (idx, a_cls, b_cls)
-            for idx, (a_cls, b_cls) in enumerate(zip_longest(a_classes, b_classes))
-            if getattr(a_cls, "name", None) != getattr(b_cls, "name", None)
-        ]
-        if class_mismatch:
+        a_classes = set(a.get_label_cat_names())
+        b_classes = set(b.get_label_cat_names())
+
+        if a_classes ^ b_classes:
             print("Datasets have mismatching labels:")
-            for idx, a_class, b_class in class_mismatch:
-                if a_class and b_class:
-                    print("  #%s: %s != %s" % (idx, a_class.name, b_class.name))
-                elif a_class:
-                    print("  #%s:  > %s" % (idx, a_class.name))
-                else:
-                    print("  #%s:  < %s" % (idx, b_class.name))
+
+        for idx, diff in enumerate(a_classes - b_classes):
+            print(" #%s: > %s" % (idx, diff))
+
+        for idx, diff in enumerate(b_classes - a_classes, start=len((a_classes - b_classes))):
+            print(" #%s: < %s" % (idx, diff))
+
         self._a_classes = a.categories().get(AnnotationType.label)
         self._b_classes = b.categories().get(AnnotationType.label)
 
         ids_a = set((item.id, item.subset) for item in a)
         ids_b = set((item.id, item.subset) for item in b)
         ids = ids_a & ids_b
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/cli/util/project.py` & `datumaro-1.6.0rc1/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/abstracts/merger.py` & `datumaro-1.6.0rc1/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.6.0rc1/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from typing import Sequence
+from typing import TYPE_CHECKING, Sequence
 
 from datumaro.components.dataset import Dataset
-from datumaro.plugins.explorer import ExplorerLauncher
+
+if TYPE_CHECKING:
+    import datumaro.plugins.explorer as explorer
+else:
+    from datumaro.util.import_util import lazy_import
+
+    explorer = lazy_import("datumaro.plugins.explorer")
 
 
 class HashInference:
     def __init__(self, *datasets: Sequence[Dataset]) -> None:
         pass
 
     @property
     def model(self):
         if self._model is None:
-            self._model = ExplorerLauncher(model_name="clip_visual_ViT-B_32")
+            self._model = explorer.ExplorerLauncher(model_name="clip_visual_ViT-B_32")
         return self._model
 
     @property
     def text_model(self):
         if self._text_model is None:
-            self._text_model = ExplorerLauncher(model_name="clip_text_ViT-B_32")
+            self._text_model = explorer.ExplorerLauncher(model_name="clip_text_ViT-B_32")
         return self._text_model
 
     def _compute_hash_key(self, datasets, datasets_to_infer):
         for dataset_to_infer in datasets_to_infer:
             if dataset_to_infer:
                 dataset_to_infer.run_model(self.model, append_annotation=True)
         for dataset, dataset_to_infer in zip(datasets, datasets_to_infer):
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import math
 import random
 from abc import ABC, abstractmethod
-from typing import Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
 
 import numpy as np
-from sklearn.cluster import KMeans
 
-import datumaro.plugins.ndr as ndr
 from datumaro.components.algorithms.hash_key_inference.base import HashInference
 from datumaro.components.algorithms.hash_key_inference.hashkey_util import (
     calculate_hamming,
     format_templates,
     select_uninferenced_dataset,
     templates,
 )
 from datumaro.components.annotation import HashKey, Label, LabelCategories
 from datumaro.components.dataset import Dataset
 from datumaro.components.dataset_base import DatasetItem
 
+if TYPE_CHECKING:
+    import datumaro.plugins.ndr as ndr
+else:
+    from datumaro.util.import_util import lazy_import
+
+    ndr = lazy_import("datumaro.plugins.ndr")
+
 
 def match_num_item_for_cluster(ratio, dataset_len, cluster_num_item_list):
     total_num_selected_item = math.ceil(dataset_len * ratio)
 
     cluster_weights = np.array(cluster_num_item_list) / sum(cluster_num_item_list)
     norm_cluster_num_item_list = (cluster_weights * total_num_selected_item).astype(int)
     remaining_items = total_num_selected_item - sum(norm_cluster_num_item_list)
@@ -90,14 +95,16 @@
 
 class Centroid(PruneBase):
     """
     Select items through clustering with centers targeting the desired number.
     """
 
     def base(self, ratio, num_centers, labels, database_keys, item_list, source):
+        from sklearn.cluster import KMeans
+
         num_selected_centers = math.ceil(len(item_list) * ratio)
         kmeans = KMeans(n_clusters=num_selected_centers, random_state=0)
         clusters = kmeans.fit_predict(database_keys)
         cluster_centers = kmeans.cluster_centers_
         cluster_ids = np.unique(clusters)
 
         selected_items = []
@@ -120,14 +127,16 @@
 
 class ClusteredRandom(PruneBase):
     """
     Select items through clustering and choose randomly within each cluster.
     """
 
     def base(self, ratio, num_centers, labels, database_keys, item_list, source):
+        from sklearn.cluster import KMeans
+
         kmeans = KMeans(n_clusters=num_centers, random_state=0)
         clusters = kmeans.fit_predict(database_keys)
         cluster_ids, cluster_num_item_list = np.unique(clusters, return_counts=True)
 
         norm_cluster_num_item_list = match_num_item_for_cluster(
             ratio, len(database_keys), cluster_num_item_list
         )
@@ -144,14 +153,16 @@
 
 class QueryClust(PruneBase):
     """
     Select items through clustering with inits that imply each label.
     """
 
     def base(self, ratio, num_centers, labels, database_keys, item_list, source):
+        from sklearn.cluster import KMeans
+
         center_dict = {i: None for i in range(1, num_centers)}
         for item in item_list:
             for anno in item.annotations:
                 if isinstance(anno, Label):
                     label_ = anno.label
                     if center_dict.get(label_) is None:
                         center_dict[label_] = item
@@ -195,14 +206,16 @@
 
 class Entropy(PruneBase):
     """
     Select items through clustering and choose them based on label entropy in each cluster.
     """
 
     def base(self, ratio, num_centers, labels, database_keys, item_list, source):
+        from sklearn.cluster import KMeans
+
         kmeans = KMeans(n_clusters=num_centers, random_state=0)
         clusters = kmeans.fit_predict(database_keys)
 
         cluster_ids, cluster_num_item_list = np.unique(clusters, return_counts=True)
         norm_cluster_num_item_list = match_num_item_for_cluster(
             ratio, len(database_keys), cluster_num_item_list
         )
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
 
 from collections import defaultdict
 from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Sequence, Tuple
-
-import matplotlib.pyplot as plt
-import pandas as pd
-from matplotlib.figure import Figure
+from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Tuple
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset_base import IDataset
 from datumaro.errors import DatasetError
 
+if TYPE_CHECKING:
+    from matplotlib.figure import Figure
+    from pandas import DataFrame, Series
+
+
 __all__ = ["LossDynamicsAnalyzer", "NoisyLabelCandidate"]
 
 
 @dataclass(order=True, frozen=True)
 class NoisyLabelCandidate:
     id: str = field(compare=False)
     subset: str = field(compare=False)
@@ -88,38 +90,40 @@
     def alpha(self) -> float:
         """A parameter to obtain EMA loss dynamics statistics.
 
         ema_loss_dyns(t) := (1 - alpha) * ema_loss_dyns(t - 1) + alpha * loss_dyns(t)"""
         return self._alpha
 
     @property
-    def mean_loss_dyns(self) -> pd.Series:
+    def mean_loss_dyns(self) -> Series:
         """Pandas Series object obtained by averaging all EMA loss dynamics statistics"""
         return self._mean_loss_dyns
 
     @property
-    def mean_loss_dyns_per_label(self) -> Dict[LabelCategories.Category, pd.Series]:
+    def mean_loss_dyns_per_label(self) -> Dict[LabelCategories.Category, Series]:
         """A dictionary of Pandas Series object obtained
         by averaging EMA loss dynamics statistics according to the label category"""
         label_categories = self._dataset.categories()[AnnotationType.label]
         return {label_categories[k]: v for k, v in self._mean_loss_dyns_per_label.items()}
 
     @property
-    def ema_dataframe(self) -> pd.DataFrame:
+    def ema_dataframe(self) -> DataFrame:
         """Pandas DataFrame including full EMA loss dynamics statistics."""
         return self._df
 
     @staticmethod
     def _parse_to_dataframe(
         dataset: IDataset, ema_alpha: float = 0.001, tracking_loss_type: Optional[str] = None
-    ) -> pd.DataFrame:
+    ) -> DataFrame:
         """Parse loss dynamics statistics from Datumaro dataset to Pandas DataFrame."""
         key = (
             "loss_dynamics" if tracking_loss_type is None else f"loss_dynamics_{tracking_loss_type}"
         )
+        import pandas as pd
+
         ema_loss_dyns_list = []
         for item in dataset:
             for ann in item.annotations:
                 # The first value should be start from zero
                 loss_dyns = pd.Series(
                     [0.0] + ann.attributes.get(key),
                     index=[-1] + ann.attributes.get("iters"),
@@ -163,14 +167,16 @@
         candidates: Sequence[NoisyLabelCandidate],
         mode: str = "mean",
         mean_plot_style: str = "--",
         mean_plot_color: str = "k",
         figsize: Tuple[int, int] = (4, 3),
         **kwargs,
     ) -> Figure:
+        import matplotlib.pyplot as plt
+
         if mode == "mean":
             cands_by_label_id = {None: candidates}
         elif mode == "label_mean":
             cands_by_label_id = defaultdict(list)
             for cand in candidates:
                 cands_by_label_id[cand.label_id].append(cand)
         else:
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/algorithms/rise.py` & `datumaro-1.6.0rc1/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/annotation.py` & `datumaro-1.6.0rc1/src/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/annotations/matcher.py` & `datumaro-1.6.0rc1/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/annotations/merger.py` & `datumaro-1.6.0rc1/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/cli_plugin.py` & `datumaro-1.6.0rc1/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/comparator.py` & `datumaro-1.6.0rc1/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/config.py` & `datumaro-1.6.0rc1/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/config_model.py` & `datumaro-1.6.0rc1/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/contexts/importer.py` & `datumaro-1.6.0rc1/src/datumaro/components/contexts/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/crypter.py` & `datumaro-1.6.0rc1/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/dataset.py` & `datumaro-1.6.0rc1/src/datumaro/components/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,30 @@
 
 import inspect
 import logging as log
 import os
 import os.path as osp
 import warnings
 from contextlib import contextmanager
-from copy import copy
-from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple, Type, Union
+from copy import copy, deepcopy
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    overload,
+)
 
-from datumaro.components.annotation import AnnotationType, LabelCategories
+from datumaro.components.annotation import Annotation, AnnotationType, LabelCategories
 from datumaro.components.config_model import Source
 from datumaro.components.dataset_base import (
     DEFAULT_SUBSET_NAME,
     CategoriesInfo,
     DatasetBase,
     DatasetInfo,
     DatasetItem,
@@ -29,15 +41,20 @@
 from datumaro.components.errors import (
     DatasetImportError,
     MultipleFormatsMatchError,
     NoMatchingFormatsError,
     UnknownFormatError,
 )
 from datumaro.components.exporter import ExportContext, Exporter, ExportErrorPolicy, _ExportFail
-from datumaro.components.filter import XPathAnnotationsFilter, XPathDatasetFilter
+from datumaro.components.filter import (
+    UserFunctionAnnotationsFilter,
+    UserFunctionDatasetFilter,
+    XPathAnnotationsFilter,
+    XPathDatasetFilter,
+)
 from datumaro.components.importer import ImportContext, ImportErrorPolicy, _ImportFail
 from datumaro.components.launcher import Launcher
 from datumaro.components.media import Image, MediaElement
 from datumaro.components.merge import DEFAULT_MERGE_POLICY
 from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
 from datumaro.components.transformer import ItemTransform, ModelTransform, Transform
 from datumaro.util.log_utils import logging_disabled
@@ -311,14 +328,20 @@
         return self._data.get_annotations()
 
     def get_datasetitem_by_path(self, path):
         if self._source_path not in path:
             path = osp.join(self._source_path, path)
         return self._data.get_datasetitem_by_path(path)
 
+    def get_label_cat_names(self):
+        return [
+            label.name
+            for label in self._data.categories().get(AnnotationType.label, LabelCategories())
+        ]
+
     def get_subset_info(self) -> str:
         return (
             f"{subset_name}: # of items={len(self.get_subset(subset_name))}, "
             f"# of annotated items={self.get_subset(subset_name).get_annotated_items()}, "
             f"# of annotations={self.get_subset(subset_name).get_annotations()}, "
             f"annotation types={self.get_subset(subset_name).get_annotated_type()}\n"
             for subset_name in sorted(self.subsets().keys())
@@ -360,16 +383,21 @@
             item = item.wrap(**overrides)
 
         self._data.put(item)
 
     def remove(self, id: str, subset: Optional[str] = None) -> None:
         self._data.remove(id, subset)
 
+    @overload
     def filter(
-        self, expr: str, filter_annotations: bool = False, remove_empty: bool = False
+        self,
+        expr: str,
+        *,
+        filter_annotations: bool = False,
+        remove_empty: bool = False,
     ) -> Dataset:
         """
         Filters out some dataset items or annotations, using a custom filter
         expression.
 
         Results are stored in-place. Modifications are applied lazily.
 
@@ -380,19 +408,109 @@
             filter_annotations: Indicates if the filter should be
                 applied to items or annotations
             remove_empty: When filtering annotations, allows to
                 exclude empty items from the resulting dataset
 
         Returns: self
         """
+        ...
 
-        if filter_annotations:
-            return self.transform(XPathAnnotationsFilter, xpath=expr, remove_empty=remove_empty)
-        else:
-            return self.transform(XPathDatasetFilter, xpath=expr)
+    @overload
+    def filter(
+        self,
+        filter_func: Union[
+            Callable[[DatasetItem], bool], Callable[[DatasetItem, Annotation], bool]
+        ],
+        *,
+        filter_annotations: bool = False,
+        remove_empty: bool = False,
+    ) -> Dataset:
+        """
+        Filters out some dataset items or annotations, using a user-provided filter
+        Python function.
+
+        Results are stored in-place. Modifications are applied lazily.
+
+        Args:
+            filter_func: User-provided Python function for filtering
+            filter_annotations: Indicates if the filter should be
+                applied to items or annotations
+            remove_empty: When filtering annotations, allows to
+                exclude empty items from the resulting dataset
+
+        Returns: self
+
+        Example:
+            - (`filter_annotations=True`) This is an example of filtering
+                dataset items with images larger than 1024 pixels::
+
+                from datumaro.components.media import Image
+
+                def filter_func(item: DatasetItem) -> bool:
+                    h, w = item.media_as(Image).size
+                    return h > 1024 or w > 1024
+
+                filtered = UserFunctionDatasetFilter(
+                    extractor=dataset, filter_func=filter_func)
+                # No items with an image height or width greater than 1024
+                filtered_items = [item for item in filtered]
+
+            - (`filter_annotations=True`) This is an example of removing bounding boxes
+                sized greater than 50% of the image size::
+
+                from datumaro.components.media import Image
+                from datumaro.components.annotation import Annotation, Bbox
+
+                def filter_func(item: DatasetItem, ann: Annotation) -> bool:
+                    # If the annotation is not a Bbox, do not filter
+                    if not isinstance(ann, Bbox):
+                        return False
+
+                    h, w = item.media_as(Image).size
+                    image_size = h * w
+                    bbox_size = ann.h * ann.w
+
+                    # Accept Bboxes smaller than 50% of the image size
+                    return bbox_size < 0.5 * image_size
+
+                filtered = UserFunctionAnnotationsFilter(
+                    extractor=dataset, filter_func=filter_func)
+                # No bounding boxes with a size greater than 50% of their image
+                filtered_items = [item for item in filtered]
+        """
+        ...
+
+    def filter(
+        self,
+        expr_or_filter_func: Union[
+            str, Callable[[DatasetItem], bool], Callable[[DatasetItem, Annotation], bool]
+        ],
+        *,
+        filter_annotations: bool = False,
+        remove_empty: bool = False,
+    ) -> Dataset:
+        if isinstance(expr_or_filter_func, str):
+            expr = expr_or_filter_func
+            return (
+                self.transform(XPathAnnotationsFilter, xpath=expr, remove_empty=remove_empty)
+                if filter_annotations
+                else self.transform(XPathDatasetFilter, xpath=expr)
+            )
+        elif callable(expr_or_filter_func):
+            filter_func = expr_or_filter_func
+            return (
+                self.transform(
+                    UserFunctionAnnotationsFilter,
+                    filter_func=filter_func,
+                    remove_empty=remove_empty,
+                )
+                if filter_annotations
+                else self.transform(UserFunctionDatasetFilter, filter_func=filter_func)
+            )
+        raise TypeError(expr_or_filter_func)
 
     def update(self, source: Union[DatasetPatch, IDataset, Iterable[DatasetItem]]) -> Dataset:
         """
         Updates items of the current dataset from another dataset or an
         iterable (the source). Items from the source overwrite matching
         items in the current dataset. Unmatched items are just appended.
 
@@ -802,14 +920,22 @@
         else:
             return matches[0]
 
     @property
     def is_stream(self) -> bool:
         return self._data.is_stream
 
+    def clone(self) -> "Dataset":
+        """Create a deep copy of this dataset.
+
+        Returns:
+            A cloned instance of the `Dataset`.
+        """
+        return deepcopy(self)
+
 
 class StreamDataset(Dataset):
     _stream = True
 
     def __init__(
         self,
         source: Optional[IDataset] = None,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/dataset_base.py` & `datumaro-1.6.0rc1/src/datumaro/components/dataset_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,21 +174,21 @@
                 return self.categories()
 
             def media_type(_):
                 return self.media_type()
 
         return _DatasetFilter()
 
-    def infos(self):
+    def infos(self) -> DatasetInfo:
         return {}
 
-    def categories(self):
+    def categories(self) -> CategoriesInfo:
         return {}
 
-    def get(self, id, subset=None):
+    def get(self, id, subset=None) -> Optional[DatasetItem]:
         subset = subset or DEFAULT_SUBSET_NAME
         for item in self:
             if item.id == id and item.subset == subset:
                 return item
         return None
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.6.0rc1/src/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/dataset_storage.py` & `datumaro-1.6.0rc1/src/datumaro/components/dataset_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/environment.py` & `datumaro-1.6.0rc1/src/datumaro/components/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 import glob
 import importlib
 import logging as log
 import os.path as osp
 from functools import partial
-from inspect import isclass
+from inspect import getmodule, isclass
 from typing import (
     Callable,
     Dict,
     Generator,
     Generic,
     Iterable,
     Iterator,
@@ -198,15 +198,26 @@
             exports = module.exports
         else:
             for symbol in dir(module):
                 if symbol.startswith("_"):
                     continue
                 exports.append(getattr(module, symbol))
 
-        exports = [s for s in exports if isclass(s) and issubclass(s, types) and s not in types]
+        exports = [
+            s
+            for s in exports
+            if isclass(s)
+            and issubclass(s, types)
+            and s not in types
+            and (
+                getmodule(s)
+                is None  # Custom plugin (in the Datumaro project) can be a single file and have no module
+                or not getmodule(s).__package__.startswith("datumaro.components")
+            )
+        ]
 
         return exports
 
     @classmethod
     def _load_plugins(cls, module_names, *, importer, types=None):
         types = tuple(types or plugin_types())
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/errors.py` & `datumaro-1.6.0rc1/src/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/extractor_tfds.py` & `datumaro-1.6.0rc1/src/datumaro/components/extractor_tfds.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,54 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import itertools
 import logging as log
 import os.path as osp
+from importlib.util import find_spec
 from types import SimpleNamespace as namespace
-from typing import Any, Callable, Dict, Iterator, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+)
 
 import attrs
 import numpy as np
 from attrs import field, frozen
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories
 from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, DatasetItem, IDataset
 from datumaro.components.media import Image, MediaElement
 from datumaro.util.tf_util import import_tf
 
-try:
-    tf = import_tf()
-    import tensorflow_datasets as tfds
-except ImportError:
-    log.debug(
-        "Unable to import TensorFlow or TensorFlow Datasets. "
-        "Dataset downloading via TFDS is disabled."
-    )
-    TFDS_EXTRACTOR_AVAILABLE = False
+TFDS_EXTRACTOR_AVAILABLE = True if find_spec("tensorflow_datasets") is not None else False
+
+if TYPE_CHECKING:
+    try:
+        tf = import_tf()
+        import tensorflow_datasets as tfds
+    except ImportError:
+        log.debug(
+            "Unable to import TensorFlow or TensorFlow Datasets. "
+            "Dataset downloading via TFDS is disabled."
+        )
 else:
-    TFDS_EXTRACTOR_AVAILABLE = True
+    from datumaro.util.import_util import lazy_import
+
+    tfds = lazy_import("tensorflow_datasets")
 
 
 @frozen(kw_only=True)
 class TfdsDatasetMetadata:
     # If you add attributes to this class, make sure to update the reporting logic
     # in the `describe-downloads` command to include them.
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/format_detection.py` & `datumaro-1.6.0rc1/src/datumaro/components/format_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
         if none_found:
             self.fail(requirement_desc)
 
     @contextlib.contextmanager
     def probe_text_file(
         self, path: str, requirement_desc: str, is_binary_file: bool = False
-    ) -> Union[BufferedReader, TextIO]:
+    ) -> Iterator[Union[BufferedReader, TextIO]]:
         """
         Returns a context manager that can be used to place a requirement on
         the contents of the file referred to by `path`. To do so, you must
         enter and exit this context manager (typically, by using the `with`
         statement). On entering, the file is opened for reading in text mode and
         the resulting file object is returned. On exiting, the file object is
         closed.
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/generator.py` & `datumaro-1.6.0rc1/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/components/hl_ops/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
 
 import inspect
 import os
 import os.path as osp
 import shutil
-from typing import Dict, Iterable, Optional, Type, Union
+from typing import TYPE_CHECKING, Callable, Dict, Iterable, Optional, Type, Union, overload
 
 from datumaro.cli.util.compare import DistanceCompareVisualizer
-from datumaro.cli.util.project import generate_next_file_name
 from datumaro.components.comparator import DistanceComparator, EqualityComparator, TableComparator
-from datumaro.components.dataset import Dataset, DatasetItemStorageDatasetView, IDataset
+from datumaro.components.dataset import Dataset, IDataset
 from datumaro.components.environment import Environment
 from datumaro.components.errors import DatasetError
 from datumaro.components.exporter import Exporter
-from datumaro.components.filter import XPathAnnotationsFilter, XPathDatasetFilter
+from datumaro.components.filter import (
+    UserFunctionAnnotationsFilter,
+    UserFunctionDatasetFilter,
+    XPathAnnotationsFilter,
+    XPathDatasetFilter,
+)
 from datumaro.components.launcher import Launcher
 from datumaro.components.merge import DEFAULT_MERGE_POLICY, get_merger
 from datumaro.components.transformer import ModelTransform, Transform
 from datumaro.components.validator import TaskType, Validator
-from datumaro.util import dump_json_file, parse_str_enum_value
+from datumaro.util import parse_str_enum_value
 from datumaro.util.scope import on_error_do, scoped
 
+if TYPE_CHECKING:
+    from datumaro.components.annotation import Annotation
+    from datumaro.components.dataset_base import DatasetItem
+
 __all__ = ["HLOps"]
 
 
 class HLOps:
     """High-level dataset operations for Python API."""
 
     @staticmethod
@@ -122,14 +131,15 @@
         if not (inspect.isclass(method) and issubclass(method, Transform)):
             raise TypeError(f"Unexpected 'method' argument type: {type(method)}")
 
         produced = method(dataset, **kwargs)
 
         return Dataset(source=produced, env=env)
 
+    @overload
     @staticmethod
     def filter(
         dataset: IDataset,
         expr: str,
         *,  # pylint: disable=redefined-builtin
         filter_annotations: bool = False,
         remove_empty: bool = False,
@@ -146,23 +156,113 @@
                 applied to items or annotations
             remove_empty: When filtering annotations, allows to
                 exclude empty items from the resulting dataset
 
         Returns: a wrapper around the input dataset, which is computed lazily
             during iteration
         """
+        ...
+
+    @overload
+    @staticmethod
+    def filter(
+        dataset: IDataset,
+        filter_func: Union[
+            Callable[[DatasetItem], bool], Callable[[DatasetItem, Annotation], bool]
+        ],
+        *,  # pylint: disable=redefined-builtin
+        filter_annotations: bool = False,
+        remove_empty: bool = False,
+    ) -> IDataset:
+        """
+        Filters out some dataset items or annotations, using a user-provided filter
+        Python function.
+
+        Results are stored in-place. Modifications are applied lazily.
+
+        Args:
+            filter_func: User-provided Python function for filtering
+            filter_annotations: Indicates if the filter should be
+                applied to items or annotations
+            remove_empty: When filtering annotations, allows to
+                exclude empty items from the resulting dataset
 
-        if filter_annotations:
-            return HLOps.transform(
-                dataset, XPathAnnotationsFilter, xpath=expr, remove_empty=remove_empty
+        Returns: a wrapper around the input dataset, which is computed lazily
+            during iteration
+
+        Example:
+            - (`filter_annotations=True`) This is an example of filtering
+                dataset items with images larger than 1024 pixels::
+
+                from datumaro.components.media import Image
+
+                def filter_func(item: DatasetItem) -> bool:
+                    h, w = item.media_as(Image).size
+                    return h > 1024 or w > 1024
+
+                filtered = UserFunctionDatasetFilter(
+                    extractor=dataset, filter_func=filter_func)
+                # No items with an image height or width greater than 1024
+                filtered_items = [item for item in filtered]
+
+            - (`filter_annotations=True`) This is an example of removing bounding boxes
+                sized greater than 50% of the image size::
+
+                from datumaro.components.media import Image
+                from datumaro.components.annotation import Annotation, Bbox
+
+                def filter_func(item: DatasetItem, ann: Annotation) -> bool:
+                    # If the annotation is not a Bbox, do not filter
+                    if not isinstance(ann, Bbox):
+                        return False
+
+                    h, w = item.media_as(Image).size
+                    image_size = h * w
+                    bbox_size = ann.h * ann.w
+
+                    # Accept Bboxes smaller than 50% of the image size
+                    return bbox_size < 0.5 * image_size
+
+                filtered = UserFunctionAnnotationsFilter(
+                    extractor=dataset, filter_func=filter_func)
+                # No bounding boxes with a size greater than 50% of their image
+                filtered_items = [item for item in filtered]
+        """
+
+    def filter(
+        dataset: IDataset,
+        expr_or_filter_func: Union[
+            str, Callable[[DatasetItem], bool], Callable[[DatasetItem, Annotation], bool]
+        ],
+        *,  # pylint: disable=redefined-builtin
+        filter_annotations: bool = False,
+        remove_empty: bool = False,
+    ):
+        if isinstance(expr_or_filter_func, str):
+            expr = expr_or_filter_func
+            return (
+                HLOps.transform(
+                    dataset, XPathAnnotationsFilter, xpath=expr, remove_empty=remove_empty
+                )
+                if filter_annotations
+                else HLOps.transform(dataset, XPathDatasetFilter, xpath=expr)
+            )
+        elif callable(expr_or_filter_func):
+            filter_func = expr_or_filter_func
+            return (
+                HLOps.transform(
+                    dataset,
+                    UserFunctionAnnotationsFilter,
+                    filter_func=filter_func,
+                    remove_empty=remove_empty,
+                )
+                if filter_annotations
+                else HLOps.transform(dataset, UserFunctionDatasetFilter, filter_func=filter_func)
             )
-        else:
-            if not expr:
-                return dataset
-            return HLOps.transform(dataset, XPathDatasetFilter, xpath=expr)
+        raise TypeError(expr_or_filter_func)
 
     @staticmethod
     def merge(
         *datasets: Dataset,
         merge_policy: str = DEFAULT_MERGE_POLICY,
         report_path: Optional[str] = None,
         **kwargs,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/importer.py` & `datumaro-1.6.0rc1/src/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/launcher.py` & `datumaro-1.6.0rc1/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/lazy_plugin.py` & `datumaro-1.6.0rc1/src/datumaro/components/lazy_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import logging as log
 from abc import ABC, abstractclassmethod
 from importlib import import_module
+from importlib.util import find_spec
 from typing import List, Optional, Sequence, Type, Union
 
 from datumaro.components.dataset_base import DatasetBase
 from datumaro.components.errors import DatumaroError
 from datumaro.components.exporter import Exporter
 from datumaro.components.generator import DatasetGenerator
 from datumaro.components.importer import Importer
@@ -52,19 +54,19 @@
 
 def get_lazy_plugin(
     import_path: str,
     plugin_name: str,
     plugin_type: str,
     extra_deps: List[str] = [],
 ) -> Optional[LazyPlugin]:
-    try:
-        for extra_dep in extra_deps:
-            import_module(extra_dep)
-    except ImportError:
-        return None
+    for extra_dep in extra_deps:
+        spec = find_spec(extra_dep)
+        if spec is None:
+            log.debug(f"Cannot import extra dep={extra_dep} for plugin_name={plugin_name}.")
+            return None
 
     plugin_type_cls = STR_TO_PLUGIN_TYPES[plugin_type]
 
     class LazyPluginImpl(LazyPlugin, plugin_type_cls):
         NAME = plugin_name
 
         @classmethod
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/media.py` & `datumaro-1.6.0rc1/src/datumaro/components/media.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import os
 import os.path as osp
 import shutil
 import weakref
 from copy import deepcopy
 from enum import IntEnum
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     Iterator,
     List,
@@ -25,27 +26,34 @@
     Type,
     TypeVar,
     Union,
 )
 
 import cv2
 import numpy as np
-import pandas as pd
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.errors import DatumaroError, MediaShapeError
 from datumaro.util.definitions import BboxIntCoords
 from datumaro.util.image import (
     _image_loading_errors,
     copyto_image,
     decode_image,
     lazy_image,
     save_image,
 )
 
+if TYPE_CHECKING:
+    import pandas as pd
+else:
+    from datumaro.util.import_util import lazy_import
+
+    pd = lazy_import("pandas")
+
+
 AnyData = TypeVar("AnyData", bytes, np.ndarray)
 
 
 class MediaType(IntEnum):
     NONE = 0
     MEDIA_ELEMENT = 1
     IMAGE = 2
@@ -305,15 +313,15 @@
         self.__data = lazy_image(self.path, crypter=self._crypter)
 
         # extension from file name and real extension can be differ
         self._ext = self._ext if self._ext else osp.splitext(osp.basename(path))[1]
 
     @property
     def data(self) -> Optional[np.ndarray]:
-        """Image data in BGRA HWC [0; 255] (float) format"""
+        """Image data in BGRA HWC [0; 255] (uint8) format"""
 
         if not self.has_data:
             return None
 
         data = self.__data()
 
         if self._size is None and data is not None:
@@ -371,20 +379,20 @@
         *args,
         **kwargs,
     ):
         super().__init__(data=data, *args, **kwargs)
 
     @property
     def data(self) -> Optional[np.ndarray]:
-        """Image data in BGRA HWC [0; 255] (float) format"""
+        """Image data in BGRA HWC [0; 255] (uint8) format"""
 
         data = super().data
 
-        if isinstance(data, np.ndarray):
-            data = data.astype(np.float32)
+        if isinstance(data, np.ndarray) and data.dtype != np.uint8:
+            data = np.clip(data, 0.0, 255.0).astype(np.uint8)
         if self._size is None and data is not None:
             if not 2 <= data.ndim <= 3:
                 raise MediaShapeError("An image should have 2 (gray) or 3 (bgra) dims.")
             self._size = tuple(map(int, data.shape[:2]))
         return data
 
     @property
@@ -416,22 +424,20 @@
         return next(
             (ext for magic, ext in cls._FORMAT_MAGICS if data.startswith(magic)),
             None,
         )
 
     @property
     def data(self) -> Optional[np.ndarray]:
-        """Image data in BGRA HWC [0; 255] (float) format"""
+        """Image data in BGRA HWC [0; 255] (uint8) format"""
 
         data = super().data
 
         if isinstance(data, bytes):
-            data = decode_image(data)
-        if isinstance(data, np.ndarray):
-            data = data.astype(np.float32)
+            data = decode_image(data, dtype=np.uint8)
         if self._size is None and data is not None:
             if not 2 <= data.ndim <= 3:
                 raise MediaShapeError("An image should have 2 (gray) or 3 (bgra) dims.")
             self._size = tuple(map(int, data.shape[:2]))
         return data
 
 
@@ -1082,15 +1088,15 @@
         raise DatumaroError(f"Please use a factory function '{cls.__name__}.from_image_roi_pairs'.")
 
     @classmethod
     def from_bytes(cls, *args, **kwargs):
         raise DatumaroError(f"Please use a factory function '{cls.__name__}.from_image_roi_pairs'.")
 
 
-class MosiacImageFromData(FromDataMixin, MosaicImage):
+class MosaicImageFromData(FromDataMixin, MosaicImage):
     def save(
         self,
         fp: Union[str, io.IOBase],
         ext: Optional[str] = None,
         crypter: Crypter = NULL_CRYPTER,
     ):
         if not crypter.is_null_crypter:
@@ -1102,15 +1108,15 @@
             raise ValueError(f"{self.__class__.__name__} is empty.")
         new_ext = self._get_ext_to_save(fp, ext)
         if isinstance(fp, str):
             os.makedirs(osp.dirname(fp), exist_ok=True)
         save_image(fp, data, ext=new_ext, crypter=crypter)
 
 
-class MosaicImageFromImageRoIPairs(MosiacImageFromData):
+class MosaicImageFromImageRoIPairs(MosaicImageFromData):
     def __init__(self, data: List[ImageWithRoI], size: Tuple[int, int]) -> None:
         def _get_mosaic_img() -> np.ndarray:
             h, w = self.size
             mosaic_img = np.zeros(shape=(h, w, 3), dtype=np.float32)
             for img, roi in data:
                 assert isinstance(img, Image), "MosaicImage can only take a list of Images."
                 x, y, w, h = roi
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/media_manager.py` & `datumaro-1.6.0rc1/src/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/merge/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/merge/base.py` & `datumaro-1.6.0rc1/src/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.6.0rc1/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/merge/extractor_merger.py` & `datumaro-1.6.0rc1/src/datumaro/components/merge/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.6.0rc1/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/merge/union_merge.py` & `datumaro-1.6.0rc1/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/operations.py` & `datumaro-1.6.0rc1/src/datumaro/components/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import hashlib
 import logging as log
 import warnings
+from collections import defaultdict
 from copy import deepcopy
 from typing import Callable, Dict, Optional, Set, Tuple
 
 import cv2
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
@@ -221,18 +222,28 @@
         }
     )
 
     return stats
 
 
 def compute_ann_statistics(dataset: IDataset):
-    labels = dataset.categories().get(AnnotationType.label, LabelCategories())
+    warnings.warn(
+        "We are planning to change the type of stats['annotations']['labels']['distribution'] "
+        "and stats['annotations']['segments']['pixel distribution'] from `list` to `(named) tuple`. "
+        "If you are checking the types in your code, please revisit it after upgrading datumaro>=2.0.0.",
+        FutureWarning,
+    )
+    labels: LabelCategories = dataset.categories().get(AnnotationType.label, LabelCategories())
 
     def get_label(ann):
-        return labels.items[ann.label].name if ann.label is not None else None
+        try:
+            return labels.items[ann.label].name if ann.label is not None else None
+        except IndexError:
+            log.warning(f"annotation({ann}) has undefined label({ann.label})")
+            return ann.label
 
     stats = {
         "images count": 0,
         "annotations count": 0,
         "unannotated images count": 0,
         "unannotated images": [],
         "annotations by type": {
@@ -249,29 +260,34 @@
         "count": 0,
         "values count": 0,
         "values present": set(),
         "distribution": {},  # value -> (count, total%)
     }
     label_stat = {
         "count": 0,
-        "distribution": {l.name: [0, 0] for l in labels.items},  # label -> (count, total%)
+        "distribution": defaultdict(lambda: [0, 0]),  # label -> (count, total%)
         "attributes": {},
     }
+
     stats["annotations"]["labels"] = label_stat
     segm_stat = {
         "avg. area": 0,
         "area distribution": [],  # a histogram with 10 bins
         # (min, min+10%), ..., (min+90%, max) -> (count, total%)
-        "pixel distribution": {l.name: [0, 0] for l in labels.items},  # label -> (count, total%)
+        "pixel distribution": defaultdict(lambda: [0, 0]),  # label -> (count, total%)
     }
     stats["annotations"]["segments"] = segm_stat
     segm_areas = []
     pixel_dist = segm_stat["pixel distribution"]
     total_pixels = 0
 
+    for l in labels.items:
+        label_stat["distribution"][l.name] = [0, 0]
+        pixel_dist[l.name] = [0, 0]
+
     for item in dataset:
         if len(item.annotations) == 0:
             stats["unannotated images"].append(item.id)
             continue
 
         for ann in item.annotations:
             by_type[ann.type.name]["count"] += 1
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/progress_reporting.py` & `datumaro-1.6.0rc1/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/project.py` & `datumaro-1.6.0rc1/src/datumaro/components/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,28 @@
 import re
 import shutil
 import tempfile
 import unittest.mock
 from contextlib import ExitStack, suppress
 from enum import Enum, auto
 from typing import (
+    TYPE_CHECKING,
     Any,
     Dict,
     Generic,
     Iterable,
     Iterator,
     List,
     NewType,
     Optional,
     Tuple,
     TypeVar,
     Union,
 )
 
-import networkx as nx
-import ruamel.yaml as yaml
-
 from datumaro.components.config import Config
 from datumaro.components.config_model import (
     BuildStage,
     BuildTarget,
     Model,
     PipelineConfig,
     ProjectConfig,
@@ -83,14 +81,22 @@
     is_subpath,
     make_file_name,
     rmfile,
     rmtree,
 )
 from datumaro.util.scope import on_error_do, scope_add, scoped
 
+if TYPE_CHECKING:
+    import networkx as nx
+
+else:
+    from datumaro.util.import_util import lazy_import
+
+    nx = lazy_import("networkx")
+
 
 class ProjectSourceDataset(IDataset):
     def __init__(self, path: str, tree: Tree, source: str, readonly: bool = False):
         config = tree.sources[source]
 
         rpath = path
         if config.path:
@@ -887,15 +893,15 @@
             name=name,
         )
 
     def add_filter_stage(
         self, target: str, expr: str, params: Optional[Dict] = None, name: Optional[str] = None
     ):
         params = params or {}
-        params["expr"] = expr
+        params["expr_or_filter_func"] = expr
         return self.add_stage(
             target,
             {
                 "type": BuildStageType.filter.name,
                 "params": params,
             },
             name=name,
@@ -1411,14 +1417,16 @@
         assert is_subpath(dvcignore, base=repo_root), dvcignore
 
         _update_ignore_file(paths, repo_root=repo_root, mode=mode, filepath=dvcignore)
 
     # This ruamel parser is needed to preserve comments,
     # order and form (if multiple forms allowed by the standard)
     # of the entries in the file. It can be reused.
+    import ruamel.yaml as yaml
+
     yaml_parser = yaml.YAML(typ="rt")
 
     @classmethod
     def get_hash_from_dvcfile(cls, path) -> str:
         with open(path) as f:
             contents = cls.yaml_parser.load(f)
         return contents["outs"][0]["md5"]
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/shift_analyzer.py` & `datumaro-1.6.0rc1/src/datumaro/components/shift_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,36 @@
 #
 # SPDX-License-Identifier: MIT
 
 # ruff: noqa: E501
 
 import itertools
 from collections import defaultdict
-from typing import Dict, List, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import numpy as np
-import pyemd
-from scipy import linalg
-from scipy.stats import anderson_ksamp
 
 from datumaro.components.annotation import FeatureVector
 from datumaro.components.dataset import IDataset
 from datumaro.components.launcher import LauncherWithModelInterpreter
-from datumaro.plugins.openvino_plugin.shift_launcher import ShiftLauncher
 from datumaro.util import take_by
 
+if TYPE_CHECKING:
+    import pyemd
+    from scipy import linalg, stats
+
+    from datumaro.plugins.openvino_plugin import shift_launcher
+else:
+    from datumaro.util.import_util import lazy_import
+
+    pyemd = lazy_import("pyemd")
+    linalg = lazy_import("scipy.linalg")
+    stats = lazy_import("scipy.stats")
+    shift_launcher = lazy_import("datumaro.plugins.openvino_plugin.shift_launcher")
+
 
 class RunningStats1D:
     def __init__(self):
         self.running_mean = None
         self.running_sq_mean = None
         self.num: int = 0
 
@@ -106,15 +115,15 @@
         Parameters
         ----------
         dataset:
             Datumaro dataset to search similar dataitem.
         topk:
             Number of images.
         """
-        self._model = ShiftLauncher(
+        self._model = shift_launcher.ShiftLauncher(
             model_name="googlenet-v4-tf",
             output_layers="InceptionV4/Logits/PreLogitsFlatten/flatten_1/Reshape:0",
         )
 
     def compute_covariate_shift(self, sources: List[IDataset], method: Optional[str] = "fid"):
         assert (
             len(sources) == 2
@@ -154,15 +163,15 @@
 
         labels = defaultdict(list)
         for idx, source in enumerate(sources):
             for item in source:
                 for ann in item.annotations:
                     labels[idx].append(ann.label)
 
-        _, _, pv = anderson_ksamp([labels[0], labels[1]])
+        _, _, pv = stats.anderson_ksamp([labels[0], labels[1]])
 
         return 1 - pv
 
     def _frechet_distance(
         self,
         mu1: np.ndarray,
         sigma1: np.ndarray,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/transformer.py` & `datumaro-1.6.0rc1/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/validator.py` & `datumaro-1.6.0rc1/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/components/visualizer.py` & `datumaro-1.6.0rc1/src/datumaro/components/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
+
+import logging as log
 import math
 import random
 import warnings
 from collections import defaultdict
-from typing import Iterable, List, Optional, Tuple, Union, overload
+from typing import TYPE_CHECKING, Iterable, List, Optional, Tuple, Union, overload
 
 import cv2
-import matplotlib.patches as patches
-import matplotlib.pyplot as plt
 import numpy as np
-from matplotlib.axes import Axes
-from matplotlib.figure import Figure
-from matplotlib.text import Text
-from mpl_toolkits.axes_grid1 import make_axes_locatable
 from PIL import ImageColor
 
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
     Bbox,
     Caption,
@@ -32,14 +29,19 @@
     Polygon,
     PolyLine,
     SuperResolutionAnnotation,
 )
 from datumaro.components.dataset_base import DatasetItem, IDataset
 from datumaro.components.media import Image
 
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from matplotlib.figure import Figure
+    from matplotlib.text import Text
+
 CAPTION_BBOX_PAD = 0.2
 DEFAULT_COLOR_CYCLES: List[str] = [
     "#1f77b4",
     "#ff7f0e",
     "#2ca02c",
     "#d62728",
     "#9467bd",
@@ -83,14 +85,15 @@
         dataset: IDataset,
         ignored_types: Optional[Iterable[AnnotationType]] = None,
         figsize: Tuple[float, float] = (8, 6),
         color_cycles: Optional[List[str]] = None,
         bbox_linewidth: float = 1.0,
         text_y_offset: float = 1.5,
         alpha: float = 1.0,
+        show_plot_title: bool = True,
     ) -> None:
         """
         Visualizer for Datumaro annotations
 
         Parameters
         ----------
         dataset:
@@ -108,24 +111,28 @@
             Line width for Bbox, Polygon and PolyLine annotation
         text_y_offset:
             Offset of y axis for texts.
             The higher value puts the text in the upper place of the annotation.
         alpha:
             Transparency value when drawing annotations. It should be in [0, 1].
             If alpha=0, we do not draw any annotations.
+        show_plot_title:
+            If True, show the plot title formatted as "ID: {item_id}, Subset: {subset}".
+            Otherwise, hide the plot title.
         """
         self.dataset = dataset
         self.figsize = figsize
         self.ignored_types = set(ignored_types) if ignored_types is not None else set()
         self.color_cycles = color_cycles if color_cycles is not None else DEFAULT_COLOR_CYCLES
         self.bbox_linewidth = bbox_linewidth
         self.text_y_offset = text_y_offset
 
         assert 0.0 <= alpha <= 1.0, "alpha should be in [0, 1]."
         self.alpha = alpha
+        self.show_plot_title = show_plot_title
 
         self._items = [item for item in self.dataset]
 
     @property
     def draw_only_image(self):
         """
         If self.alpha = 0, we do not overdraw any annotation over the image.
@@ -178,15 +185,16 @@
         if ann.type == AnnotationType.super_resolution_annotation:
             return self._draw_super_resolution_annotation(ann, label_categories, fig, ax, context)
         if ann.type == AnnotationType.depth_annotation:
             return self._draw_depth_annotation(ann, label_categories, fig, ax, context)
         if ann.type == AnnotationType.ellipse:
             return self._draw_ellipse(ann, label_categories, fig, ax, context)
 
-        raise ValueError(f"Unknown ann.type={ann.type}")
+        # warning instead of raising an error for unsupported annotation types.
+        log.warning(f"Ignore unknown ann.type={ann.type}")
 
     def _get_color(self, ann: Annotation) -> str:
         color = self.color_cycles[ann.label % len(self.color_cycles)]
         return color
 
     def _sort_by_z_order(self, annotations: List[Annotation]) -> List[Annotation]:
         def _sort_key(ann: Annotation):
@@ -288,14 +296,16 @@
 
     def vis_gallery(
         self,
         *inputs,
         grid_size: Tuple[Optional[int], Optional[int]] = (None, None),
     ) -> Figure:
         """Visualize several :class:`DatasetItem` as a gallery"""
+        import matplotlib.pyplot as plt
+
         if len(inputs) == 1:
             (items,) = inputs
             ids = [item.id for item in items]
             subsets = [item.subset for item in items]
             ann_ids = [None for _ in items]
         elif len(inputs) == 2:
             ids, subsets = inputs
@@ -379,14 +389,16 @@
     def vis_one_sample(
         self,
         *inputs,
         ann_id: Optional[int] = None,
         ax: Optional[Axes] = None,
     ) -> Figure:
         """Visualize one dataset item"""
+        import matplotlib.pyplot as plt
+
         if len(inputs) == 1:
             item_id, subset = None, None
             (item,) = inputs
 
         elif len(inputs) == 2:
             item_id, subset = inputs
             item = None
@@ -419,25 +431,16 @@
             item is not Image
         ), f"Media type should be Image, Current media type={type(item.media)}"
 
         img = item.media.data.astype(np.uint8)
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         ax.imshow(img)
 
-        width = ax.transAxes.transform_point((1, 0))[0] - ax.transAxes.transform_point((0, 0))[0]
-        text = ax.set_title(f"ID: {item_id}, Subset: {subset}", loc="center", wrap=True)
-        text.__get_wrapped_text = text._get_wrapped_text
-
-        def _get_wrapped_text():
-            wrapped_text = text.__get_wrapped_text()
-            text._text = wrapped_text
-            return wrapped_text
-
-        text._get_wrapped_text = _get_wrapped_text
-        text._get_wrap_line_width = lambda: width
+        if self.show_plot_title:
+            self._plot_title(ax, item_id, subset)
 
         ax.set_axis_off()
 
         if self.draw_only_image:
             return fig
 
         annotations = self._sort_by_z_order(item.annotations)
@@ -457,14 +460,27 @@
                 continue
 
             if ann_id is None or ann_id == ann.id:
                 self._draw(ann, label_categories, fig, ax, context[ann.type])
 
         return fig
 
+    def _plot_title(self, ax: Axes, item_id: str, subset: str) -> None:
+        width = ax.transAxes.transform_point((1, 0))[0] - ax.transAxes.transform_point((0, 0))[0]
+        text = ax.set_title(f"ID: {item_id}, Subset: {subset}", loc="center", wrap=True)
+        text.__get_wrapped_text = text._get_wrapped_text
+
+        def _get_wrapped_text():
+            wrapped_text = text.__get_wrapped_text()
+            text._text = wrapped_text
+            return wrapped_text
+
+        text._get_wrapped_text = _get_wrapped_text
+        text._get_wrap_line_width = lambda: width
+
     def _draw_label(
         self,
         ann: Label,
         label_categories: Optional[LabelCategories],
         fig: Figure,
         ax: Axes,
         context: List,
@@ -538,14 +554,16 @@
         self,
         ann: Union[Polygon, PolyLine],
         label_categories: Optional[LabelCategories],
         fig: Figure,
         ax: Axes,
         context: List,
     ) -> None:
+        import matplotlib.patches as patches
+
         label_text = label_categories[ann.label].name if label_categories is not None else ann.label
         color = self._get_color(ann)
         points = np.array(ann.points)
         n_points = len(points) // 2
         points = points.reshape(n_points, 2)
 
         polyline = patches.Polygon(
@@ -572,14 +590,16 @@
         self,
         ann: Bbox,
         label_categories: Optional[LabelCategories],
         fig: Figure,
         ax: Axes,
         context: List,
     ) -> None:
+        import matplotlib.patches as patches
+
         label_text = label_categories[ann.label].name if label_categories is not None else ann.label
         color = self._get_color(ann)
         rect = patches.Rectangle(
             (ann.x, ann.y),
             ann.w,
             ann.h,
             linewidth=self.bbox_linewidth,
@@ -664,14 +684,16 @@
         self,
         ann: DepthAnnotation,
         label_categories: Optional[LabelCategories],
         fig: Figure,
         ax: Axes,
         context: List,
     ) -> None:
+        from mpl_toolkits.axes_grid1 import make_axes_locatable
+
         assert len(context) == 0, "It cannot visualize more than one DepthAnnotation per item."
 
         depth = ann.image.data
 
         im = ax.imshow(depth, alpha=self.alpha)
         divider = make_axes_locatable(ax)
         cax = divider.append_axes("right", size="5%", pad=0.05)
@@ -683,14 +705,16 @@
         self,
         ann: Ellipse,
         label_categories: Optional[LabelCategories],
         fig: Figure,
         ax: Axes,
         context: List,
     ) -> None:
+        import matplotlib.patches as patches
+
         label_text = label_categories[ann.label].name if label_categories is not None else ann.label
         color = self._get_color(ann)
         ellipse = patches.Ellipse(
             xy=(ann.c_x, ann.c_y),
             width=ann.w,
             height=ann.h,
             linewidth=self.bbox_linewidth,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # Copyright (C) 2020-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from datumaro.util.tf_util import import_tf
-
-import_tf()  # prevent TF loading and potential interpreter crash
-
 from itertools import groupby
 
 from openvino.tools.accuracy_checker.adapters import create_adapter
 from openvino.tools.accuracy_checker.data_readers import DataRepresentation
 from openvino.tools.accuracy_checker.launcher import InputFeeder, create_launcher
 from openvino.tools.accuracy_checker.postprocessor import PostprocessingExecutor
 from openvino.tools.accuracy_checker.preprocessor import PreprocessingExecutor
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/configurable_validator.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/configurable_validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Mask,
     Polygon,
 )
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
+from datumaro.rust_api import JsonSectionPageMapper
 from datumaro.util import parse_json
 from datumaro.util.image import IMAGE_EXTENSIONS, find_images, lazy_image, load_image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class Ade20k2020Path:
     MASK_PATTERN = re.compile(
@@ -219,19 +220,20 @@
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         annot_path = context.require_file("*/**/*.json")
 
         with context.probe_text_file(
             annot_path,
             'must be a JSON object with an "annotation" key',
-        ) as f:
-            contents = parse_json(f.read())
-            if not isinstance(contents, dict):
-                raise Exception
-            if "annotation" not in contents:
+        ):
+            fpath = osp.join(context.root_path, annot_path)
+            page_mapper = JsonSectionPageMapper(fpath)
+            sections = page_mapper.sections()
+
+            if "annotation" not in sections.keys():
                 raise Exception
 
     @classmethod
     def find_sources(cls, path):
         for i in range(5):
             for i in glob.iglob(osp.join(path, *("*" * i))):
                 if osp.splitext(i)[1].lower() in IMAGE_EXTENSIONS:
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,423 +1,386 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import datetime
+import csv
+import errno
 import os
-import platform
-import re
-import struct
-import tempfile
-from copy import deepcopy
-from functools import partial
-from multiprocessing.pool import ApplyResult, Pool
-from shutil import move, rmtree
-from typing import Any, Callable, Dict, Optional, Union
-
-import pyarrow as pa
-import pytz
-
-from datumaro.components.crypter import NULL_CRYPTER
-from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetItem, IDataset
-from datumaro.components.errors import DatumaroError
-from datumaro.components.exporter import ExportContext, ExportContextComponent, Exporter
-from datumaro.plugins.data_formats.datumaro.exporter import _SubsetWriter as __SubsetWriter
-from datumaro.plugins.data_formats.datumaro_binary.mapper.common import DictMapper
-from datumaro.util.file_utils import to_bytes
-
-from .format import DatumaroArrow
-from .mapper.dataset_item import DatasetItemMapper
-from .mapper.media import ImageMapper
-
-
-class PathNormalizer:
-    NORMALIZER = {r":[^/\\]": r"꞉"}
-    UNNORMALIZER = {r"꞉": r":"}
+import os.path as osp
+from typing import Optional
 
-    @classmethod
-    def normalize(cls, path: str):
-        for s, t in cls.NORMALIZER.items():
-            path = re.sub(s, t, path)
-        return path
-
-    @classmethod
-    def unnormalize(cls, path: str):
-        for s, t in cls.UNNORMALIZER.items():
-            path = re.sub(s, t, path)
-        return path
-
-
-class _SubsetWriter(__SubsetWriter):
-    def __init__(
-        self,
-        context: Exporter,
-        export_context: ExportContextComponent,
-        subset: str,
-        ctx: ExportContext,
-        max_chunk_size: int = 1000,
-        num_shards: int = 1,
-        max_shard_size: Optional[int] = None,
-    ):
-        super().__init__(
-            context=context,
-            subset=subset,
-            ann_file="",
-            export_context=export_context,
-        )
-        self._schema = deepcopy(DatumaroArrow.SCHEMA)
-        self._writers = []
-        self._fnames = []
-        self._max_chunk_size = max_chunk_size
-        self._num_shards = num_shards
-        self._max_shard_size = max_shard_size
-        self._ctx = ctx
-
-        self._data = {
-            "items": [],
-            "infos": {},
-            "categories": {},
-            "media_type": None,
-            "built_time": str(datetime.datetime.now(pytz.utc)),
-            "source_path": self.export_context.source_path,
-            "encoding_scheme": self.export_context._image_ext,
-            "version": str(DatumaroArrow.VERSION),
-            "signature": DatumaroArrow.SIGNATURE,
-        }
-
-    def add_infos(self, infos):
-        if self._writers:
-            raise ValueError("Writer has been initialized.")
-        super().add_infos(infos)
-        self._data["infos"] = DictMapper.forward(self.infos)
-
-    def add_categories(self, categories):
-        if self._writers:
-            raise ValueError("Writer has been initialized.")
-        super().add_categories(categories)
-        self._data["categories"] = DictMapper.forward(self.categories)
-
-    def add_media_type(self, media_type):
-        if self._writers:
-            raise ValueError("Writer has been initialized.")
-        self._data["media_type"] = struct.pack("<I", int(media_type))
-
-    def init_schema(self):
-        self._schema = self._schema.with_metadata(
-            {k: v for k, v in self._data.items() if k != "items"}
-        )
-
-    def _init_writer(self, idx: int):
-        # TODO:
-        # `arrow_writer.close()` does not take any effect. It seems a bug in pyarrow
-        # In linux-like system it is fine to rename a file opend but
-        # it is not in windows.
-        # As a workaround, we do not use a template in windows
-        if platform.system() != "Windows":
-            f_name = os.path.join(
-                self.export_context.save_dir,
-                self._subset + "-{idx" + str(idx) + ":0{width}d}-of-{total:0{width}d}.arrow",
-            )
-            f_name = PathNormalizer.normalize(f_name)
+from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Points
+from datumaro.components.dataset_base import DatasetBase, DatasetItem
+from datumaro.components.errors import (
+    AnnotationExportError,
+    DatasetImportError,
+    InvalidAnnotationError,
+    MediaTypeError,
+)
+from datumaro.components.exporter import Exporter
+from datumaro.components.format_detection import FormatDetectionContext
+from datumaro.components.importer import ImportContext, Importer
+from datumaro.components.media import Image
+from datumaro.util.image import find_images
+from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
+
+
+class VggFace2Path:
+    ANNOTATION_DIR = "bb_landmark"
+    IMAGE_EXT = ".jpg"
+    BBOXES_FILE = "loose_bb_"
+    LANDMARKS_FILE = "loose_landmark_"
+    LABELS_FILE = "labels.txt"
+    IMAGES_DIR_NO_LABEL = "no_label"
+
+
+class VggFace2Base(DatasetBase):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
+        subset = None
+        if osp.isdir(path):
+            self._path = path
+        elif osp.isfile(path):
+            subset = osp.splitext(osp.basename(path).split("_")[2])[0]
+            self._path = osp.dirname(path)
         else:
-            f_name = os.path.join(
-                self.export_context.save_dir, self._subset + f"-{idx:03d}-of-{0:03d}.arrow"
-            )
-        return pa.RecordBatchStreamWriter(f_name, self._schema), f_name
+            raise DatasetImportError("Can't read annotations from '%s'" % path)
 
-    def add_item(self, item: DatasetItem, pool: Optional[Pool] = None):
-        if pool is not None:
-            self.items.append(
-                pool.apply_async(
-                    self.add_item_impl,
-                    (
-                        item,
-                        self.export_context,
-                    ),
-                )
+        annotation_files = [
+            p
+            for p in os.listdir(self._path)
+            if (
+                osp.basename(p).startswith(VggFace2Path.BBOXES_FILE)
+                or osp.basename(p).startswith(VggFace2Path.LANDMARKS_FILE)
             )
-        else:
-            self.items.append(partial(self.add_item_impl, item, self.export_context))
-
-    @staticmethod
-    def add_item_impl(
-        item: DatasetItem,
-        context: ExportContextComponent,
-    ) -> Dict[str, Any]:
-        item = DatasetItemMapper.forward(item, media={"encoder": context._image_ext})
-
-        if item["media"].get("bytes", None) is not None:
-            # truncate source path since the media is embeded in arrow
-            path = item["media"].get("path")
-            if path is not None:
-                item["media"]["path"] = path.replace(context.source_path, "")
-        return item
-
-    def _write(self, batch, max_chunk_size):
-        if max_chunk_size == 0:
-            max_chunk_size = self._max_chunk_size
-        pa_table = pa.Table.from_arrays(batch, schema=self._schema)
-        idx = getattr(self, "__writer_idx", 0)
-
-        if self._max_shard_size is not None:
-            nbytes = pa_table.nbytes
-            cur_nbytes = getattr(self, "__writer_nbytes", 0)
-            free_nbytes = self._max_shard_size - cur_nbytes
-            if free_nbytes < nbytes:
-                if cur_nbytes == 0:
-                    raise DatumaroError(
-                        "'max_chunk_size' exceeded 'max_shard_size'. "
-                        "Please consider increasing 'max_shard_size' or deceasing 'max_chunk_size'."
-                    )
-                self._writers[idx].close()
-                idx += 1
-                setattr(self, "__writer_idx", idx)
-                setattr(self, "__writer_nbytes", nbytes)
-            else:
-                setattr(self, "__writer_nbytes", cur_nbytes + nbytes)
-        else:
-            setattr(self, "__writer_idx", (idx + 1) % self._num_shards)
+            and p.endswith(".csv")
+        ]
 
-        if len(self._writers) <= idx:
-            writer, fname = self._init_writer(idx)
-            self._writers.append(writer)
-            self._fnames.append(fname)
-        self._writers[idx].write_table(pa_table, max_chunk_size)
-
-    def write(self, max_chunk_size: Optional[int] = None, pool: Optional[Pool] = None):
-        if max_chunk_size is None:
-            max_chunk_size = self._max_chunk_size
-
-        if len(self.items) < max_chunk_size:
-            return
-
-        batch = [[] for _ in self._schema.names]
-        for item in self._ctx.progress_reporter.iter(
-            self.items, desc=f"Building arrow for {self._subset}"
-        ):
-            if isinstance(item, ApplyResult):
-                item = item.get(timeout=DatumaroArrow.MP_TIMEOUT)
-            if isinstance(item, partial):
-                item = item()
-            for j, name in enumerate(self._schema.names):
-                batch[j].append(item[name])
-
-            if len(batch[0]) >= max_chunk_size:
-                self._write(batch, max_chunk_size)
-                batch = [[] for _ in self._schema.names]
-        if len(batch[0]) > 0:
-            self._write(batch, max_chunk_size)
-
-        self._data["items"] = []
-
-    def done(self):
-        total = len(self._fnames)
-        width = len(str(total))
-        for idx, (fname, writer) in enumerate(zip(self._fnames, self._writers)):
-            writer.close()
-            if platform.system() != "Windows":
-                template = PathNormalizer.unnormalize(fname)
-                placeholders = {"width": width, "total": total, f"idx{idx}": idx}
-                new_fname = template.format(**placeholders)
-                if os.path.exists(new_fname):
-                    os.remove(new_fname)
-                os.rename(fname, new_fname)
-
-
-class ArrowExporter(Exporter):
-    AVAILABLE_IMAGE_EXTS = ImageMapper.AVAILABLE_SCHEMES
-    DEFAULT_IMAGE_EXT = ImageMapper.AVAILABLE_SCHEMES[0]
+        if len(annotation_files) < 1:
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations in the directory", path)
 
-    @classmethod
-    def build_cmdline_parser(cls, **kwargs):
-        parser = super().build_cmdline_parser(**kwargs)
+        super().__init__(ctx=ctx)
 
-        # '--image-ext' would be used in a different way for arrow foramt
-        _actions = []
-        for action in parser._actions:
-            if action.dest != "image_ext":
-                _actions.append(action)
-        parser._actions = _actions
-        parser._option_string_actions.pop("--image-ext")
-
-        parser.add_argument(
-            "--image-ext",
-            default=None,
-            help=f"Image encoding scheme. (default: {cls.DEFAULT_IMAGE_EXT})",
-            choices=cls.AVAILABLE_IMAGE_EXTS,
+        self._dataset_dir = osp.dirname(self._path)
+        self._subsets = (
+            {subset} if subset else set(osp.splitext(f.split("_")[2])[0] for f in annotation_files)
         )
 
-        parser.add_argument(
-            "--max-chunk-size",
-            type=int,
-            default=1000,
-            help="The maximum chunk size. (default: %(default)s)",
-        )
+        self._categories = {}
+        self._items = []
 
-        parser.add_argument(
-            "--num-shards",
-            type=int,
-            default=1,
-            help="The number of shards to export. "
-            "'--num-shards' and '--max-shard-size' are  mutually exclusive. "
-            "(default: %(default)s)",
-        )
+        self._load_categories()
+        for subset in self._subsets:
+            self._items.extend(list(self._load_items(subset).values()))
+
+    def __iter__(self):
+        return iter(self._items)
+
+    def categories(self):
+        return self._categories
+
+    def _load_categories(self):
+        label_cat = LabelCategories()
+        path = osp.join(self._dataset_dir, VggFace2Path.LABELS_FILE)
+        if has_meta_file(self._dataset_dir):
+            labels = parse_meta_file(self._dataset_dir).keys()
+            for label in labels:
+                label_cat.add(label)
+        elif osp.isfile(path):
+            with open(path, encoding="utf-8") as labels_file:
+                lines = [s.strip() for s in labels_file]
+            for line in lines:
+                objects = line.split()
+                label = objects[0]
+                class_name = None
+                if 1 < len(objects):
+                    class_name = objects[1]
+                label_cat.add(label, parent=class_name)
+        else:
+            for subset in self._subsets:
+                subset_path = osp.join(self._dataset_dir, subset)
+                if osp.isdir(subset_path):
+                    for images_dir in sorted(os.listdir(subset_path)):
+                        if (
+                            osp.isdir(osp.join(subset_path, images_dir))
+                            and images_dir != VggFace2Path.IMAGES_DIR_NO_LABEL
+                        ):
+                            label_cat.add(images_dir)
+        self._categories[AnnotationType.label] = label_cat
+
+    def _load_items(self, subset):
+        def _get_label(path):
+            label_name = path.split("/")[0]
+            label = None
+            if label_name != VggFace2Path.IMAGES_DIR_NO_LABEL:
+                label = self._categories[AnnotationType.label].find(label_name)[0]
+            return label
+
+        items = {}
+
+        image_dir = osp.join(self._dataset_dir, subset)
+        if osp.isdir(image_dir):
+            images = {
+                osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
+                for p in find_images(image_dir, recursive=True)
+            }
+        else:
+            images = {}
 
-        parser.add_argument(
-            "--max-shard-size",
-            type=str,
-            default=None,
-            help="The maximum size of each shard. "
-            "(e.g. 7KB = 7 * 2^10, 3MB = 3 * 2^20, and 2GB = 2 * 2^30). "
-            "'--num-shards' and '--max-shard-size' are  mutually exclusive. "
-            "(default: %(default)s)",
+        landmarks_path = osp.join(
+            self._dataset_dir,
+            VggFace2Path.ANNOTATION_DIR,
+            VggFace2Path.LANDMARKS_FILE + subset + ".csv",
         )
+        if osp.isfile(landmarks_path):
+            with open(landmarks_path, encoding="utf-8") as content:
+                landmarks_table = list(csv.DictReader(content))
+            for row in landmarks_table:
+                item_id = row["NAME_ID"]
+                label = None
+                if "/" in item_id:
+                    label = _get_label(item_id)
+
+                if item_id not in items:
+                    image = images.get(row["NAME_ID"])
+                    if image:
+                        image = Image.from_file(path=image)
+                    items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
+
+                annotations = items[item_id].annotations
+                if [a for a in annotations if a.type == AnnotationType.points]:
+                    raise InvalidAnnotationError(
+                        "Item %s: an image can have only one " "set of landmarks" % item_id
+                    )
 
-        parser.add_argument(
-            "--num-workers",
-            type=int,
-            default=0,
-            help="The number of multi-processing workers for export. "
-            "If num_workers = 0, do not use multiprocessing. (default: %(default)s)",
+                if len([p for p in row if row[p] == ""]) == 0 and len(row) == 11:
+                    annotations.append(
+                        Points([float(row[p]) for p in row if p != "NAME_ID"], label=label)
+                    )
+                elif label is not None:
+                    annotations.append(Label(label=label))
+
+        bboxes_path = osp.join(
+            self._dataset_dir,
+            VggFace2Path.ANNOTATION_DIR,
+            VggFace2Path.BBOXES_FILE + subset + ".csv",
         )
+        if osp.isfile(bboxes_path):
+            with open(bboxes_path, encoding="utf-8") as content:
+                bboxes_table = list(csv.DictReader(content))
+            for row in bboxes_table:
+                item_id = row["NAME_ID"]
+                label = None
+                if "/" in item_id:
+                    label = _get_label(item_id)
+
+                if item_id not in items:
+                    image = images.get(row["NAME_ID"])
+                    if image:
+                        image = Image.from_file(path=image)
+                    items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
+
+                annotations = items[item_id].annotations
+                if [a for a in annotations if a.type == AnnotationType.bbox]:
+                    raise InvalidAnnotationError(
+                        "Item %s: an image can have only one " "bbox" % item_id
+                    )
 
-        return parser
+                if len([p for p in row if row[p] == ""]) == 0 and len(row) == 5:
+                    annotations.append(
+                        Bbox(
+                            float(row["X"]),
+                            float(row["Y"]),
+                            float(row["W"]),
+                            float(row["H"]),
+                            label=label,
+                        )
+                    )
+        return items
 
-    def create_writer(self, subset: str, ctx: ExportContext) -> _SubsetWriter:
-        export_context = ExportContextComponent(
-            save_dir=self._save_dir,
-            save_media=self._save_media,
-            images_dir="",
-            pcd_dir="",
-            video_dir="",
-            crypter=NULL_CRYPTER,
-            image_ext=self._image_ext,
-            default_image_ext=self._default_image_ext,
-            source_path=os.path.abspath(self._extractor._source_path)
-            if getattr(self._extractor, "_source_path")
-            else None,
-        )
 
-        return _SubsetWriter(
-            context=self,
-            subset=subset,
-            export_context=export_context,
-            num_shards=self._num_shards,
-            max_shard_size=self._max_shard_size,
-            max_chunk_size=self._max_chunk_size,
-            ctx=ctx,
-        )
+class VggFace2Importer(Importer):
+    @classmethod
+    def detect(cls, context: FormatDetectionContext) -> None:
+        with context.require_any():
+            for prefix in (VggFace2Path.BBOXES_FILE, VggFace2Path.LANDMARKS_FILE):
+                with context.alternative():
+                    context.require_file(f"{VggFace2Path.ANNOTATION_DIR}/{prefix}*.csv")
 
-    def _apply_impl(self, *args, **kwargs):
-        if self._num_workers == 0:
-            return self._apply()
-
-        with Pool(processes=self._num_workers) as pool:
-            return self._apply(pool)
-
-    def _apply(self, pool: Optional[Pool] = None):
-        os.makedirs(self._save_dir, exist_ok=True)
-
-        if self._split_by_subsets:
-            writers = {
-                subset_name: self.create_writer(subset_name, self._ctx)
-                for subset_name, subset in self._extractor.subsets().items()
-                if len(subset)
-            }
+    @classmethod
+    def find_sources(cls, path):
+        if osp.isdir(path):
+            annotation_dir = osp.join(path, VggFace2Path.ANNOTATION_DIR)
+            if osp.isdir(annotation_dir):
+                return [
+                    {
+                        "url": annotation_dir,
+                        "format": VggFace2Base.NAME,
+                    }
+                ]
+        elif osp.isfile(path):
+            if (
+                osp.basename(path).startswith(VggFace2Path.LANDMARKS_FILE)
+                or osp.basename(path).startswith(VggFace2Path.BBOXES_FILE)
+            ) and path.endswith(".csv"):
+                return [
+                    {
+                        "url": path,
+                        "format": VggFace2Base.NAME,
+                    }
+                ]
+        return []
+
+
+class VggFace2Exporter(Exporter):
+    DEFAULT_IMAGE_EXT = VggFace2Path.IMAGE_EXT
+
+    def _apply_impl(self):
+        def _get_name_id(item_parts, label_name):
+            if 1 < len(item_parts) and item_parts[0] == label_name:
+                return "/".join([label_name, *item_parts[1:]])
+            else:
+                return "/".join([label_name, *item_parts])
+
+        if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
+            raise MediaTypeError("Media type is not an image")
+
+        save_dir = self._save_dir
+        os.makedirs(save_dir, exist_ok=True)
+
+        if self._save_dataset_meta:
+            self._save_meta_file(save_dir)
         else:
-            writers = {DEFAULT_SUBSET_NAME: self.create_writer(DEFAULT_SUBSET_NAME, self._ctx)}
+            labels_path = osp.join(save_dir, VggFace2Path.LABELS_FILE)
+            labels_file = ""
+            for label in self._extractor.categories()[AnnotationType.label]:
+                labels_file += "%s" % label.name
+                if label.parent:
+                    labels_file += " %s" % label.parent
+                labels_file += "\n"
+            with open(labels_path, "w", encoding="utf-8") as f:
+                f.write(labels_file)
 
-        for writer in writers.values():
-            writer.add_infos(self._extractor.infos())
-            writer.add_categories(self._extractor.categories())
-            writer.add_media_type(self._extractor.media_type()._type)
-            writer.init_schema()
+        label_categories = self._extractor.categories()[AnnotationType.label]
 
         for subset_name, subset in self._extractor.subsets().items():
-            writer = (
-                writers[subset_name] if self._split_by_subsets else writers[DEFAULT_SUBSET_NAME]
-            )
+            bboxes_table = []
+            landmarks_table = []
             for item in subset:
-                writer.add_item(item, pool=pool)
-
-        for writer in writers.values():
-            writer.write(0, pool=pool)
-            writer.done()
-
-    @classmethod
-    def patch(cls, dataset, patch, save_dir, **kwargs):
-        # no patch supported
-        with tempfile.TemporaryDirectory() as temp_dir:
-            cls.convert(dataset, save_dir=temp_dir, **kwargs)
-            if os.path.exists(save_dir):
-                for file in os.listdir(save_dir):
-                    file = os.path.join(save_dir, file)
-                    if os.path.isdir(file):
-                        rmtree(file)
+                item_parts = item.id.split("/")
+                if item.media and self._save_media:
+                    labels = set(
+                        p.label for p in item.annotations if (getattr(p, "label", None) is not None)
+                    )
+                    if labels:
+                        for label in labels:
+                            image_dir = label_categories[label].name
+                            if 1 < len(item_parts) and image_dir == item_parts[0]:
+                                image_dir = ""
+                            self._save_image(item, subdir=osp.join(subset_name, image_dir))
                     else:
-                        os.remove(file)
-            for file in os.listdir(temp_dir):
-                file_from = os.path.join(temp_dir, file)
-                file_to = os.path.join(save_dir, file)
-                move(file_from, file_to)
-
-    def __init__(
-        self,
-        extractor: IDataset,
-        save_dir: str,
-        *,
-        save_media: Optional[bool] = None,
-        image_ext: Optional[Union[str, Callable[[str], bytes]]] = None,
-        default_image_ext: Optional[str] = None,
-        save_dataset_meta: bool = False,
-        ctx: Optional[ExportContext] = None,
-        num_workers: int = 0,
-        num_shards: int = 1,
-        max_shard_size: Optional[int] = None,
-        max_chunk_size: int = 1000,
-        **kwargs,
-    ):
-        super().__init__(
-            extractor=extractor,
-            save_dir=save_dir,
-            save_media=save_media,
-            image_ext=image_ext,
-            default_image_ext=default_image_ext,
-            save_dataset_meta=save_dataset_meta,
-            ctx=ctx,
-        )
-
-        # TODO: Support a whole single file of arrow
-        self._split_by_subsets = True
-
-        if num_workers < 0:
-            raise DatumaroError(
-                f"num_workers should be non-negative but num_workers={num_workers}."
-            )
-        self._num_workers = num_workers
+                        image_dir = VggFace2Path.IMAGES_DIR_NO_LABEL
+                        if 1 < len(item_parts) and image_dir == item_parts[0]:
+                            image_dir = ""
+                        self._save_image(item, subdir=osp.join(subset_name, image_dir))
+
+                landmarks = [a for a in item.annotations if a.type == AnnotationType.points]
+                if 1 < len(landmarks):
+                    raise AnnotationExportError(
+                        "Item (%s, %s): an image can have only one "
+                        "set of landmarks" % (item.id, item.subset)
+                    )
+                if landmarks:
+                    if landmarks[0].label is not None and label_categories[landmarks[0].label].name:
+                        name_id = _get_name_id(
+                            item_parts, label_categories[landmarks[0].label].name
+                        )
+                    else:
+                        name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
+                    points = landmarks[0].points
+                    if len(points) != 10:
+                        landmarks_table.append({"NAME_ID": name_id})
+                    else:
+                        landmarks_table.append(
+                            {
+                                "NAME_ID": name_id,
+                                "P1X": points[0],
+                                "P1Y": points[1],
+                                "P2X": points[2],
+                                "P2Y": points[3],
+                                "P3X": points[4],
+                                "P3Y": points[5],
+                                "P4X": points[6],
+                                "P4Y": points[7],
+                                "P5X": points[8],
+                                "P5Y": points[9],
+                            }
+                        )
+
+                bboxes = [a for a in item.annotations if a.type == AnnotationType.bbox]
+                if 1 < len(bboxes):
+                    raise AnnotationExportError(
+                        "Item (%s, %s): an image can have only one " "bbox" % (item.id, item.subset)
+                    )
+                if bboxes:
+                    if bboxes[0].label is not None and label_categories[bboxes[0].label].name:
+                        name_id = _get_name_id(item_parts, label_categories[bboxes[0].label].name)
+                    else:
+                        name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
+                    bboxes_table.append(
+                        {
+                            "NAME_ID": name_id,
+                            "X": bboxes[0].x,
+                            "Y": bboxes[0].y,
+                            "W": bboxes[0].w,
+                            "H": bboxes[0].h,
+                        }
+                    )
 
-        if num_shards != 1 and max_shard_size is not None:
-            raise DatumaroError(
-                "Either one of 'num_shards' or 'max_shard_size' should be provided, not both."
-            )
+                labels = [a for a in item.annotations if a.type == AnnotationType.label]
+                for label in labels:
+                    if label.label is not None and label_categories[label.label].name:
+                        name_id = _get_name_id(item_parts, label_categories[labels[0].label].name)
+                    else:
+                        name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
+                    landmarks_table.append({"NAME_ID": name_id})
 
-        if num_shards < 0:
-            raise DatumaroError(f"num_shards should be non-negative but num_shards={num_shards}.")
-        self._num_shards = num_shards
-        self._max_shard_size = to_bytes(max_shard_size) if max_shard_size else max_shard_size
-
-        if max_chunk_size < 0:
-            raise DatumaroError(
-                f"max_chunk_size should be non-negative but max_chunk_size={max_chunk_size}."
-            )
-        self._max_chunk_size = max_chunk_size
+                if not landmarks and not bboxes and not labels:
+                    landmarks_table.append(
+                        {"NAME_ID": _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)}
+                    )
 
-        if self._save_media:
-            self._image_ext = (
-                self._image_ext if self._image_ext is not None else self._default_image_ext
+            landmarks_path = osp.join(
+                save_dir,
+                VggFace2Path.ANNOTATION_DIR,
+                VggFace2Path.LANDMARKS_FILE + subset_name + ".csv",
             )
-        else:
-            self._image_ext = "NONE"
-
-        assert (
-            self._image_ext in self.AVAILABLE_IMAGE_EXTS
-        ), f"{self._image_ext} is unkonwn ext. Available exts are {self.AVAILABLE_IMAGE_EXTS}"
+            os.makedirs(osp.dirname(landmarks_path), exist_ok=True)
+            with open(landmarks_path, "w", encoding="utf-8", newline="") as file:
+                columns = [
+                    "NAME_ID",
+                    "P1X",
+                    "P1Y",
+                    "P2X",
+                    "P2Y",
+                    "P3X",
+                    "P3Y",
+                    "P4X",
+                    "P4Y",
+                    "P5X",
+                    "P5Y",
+                ]
+                writer = csv.DictWriter(file, fieldnames=columns)
+                writer.writeheader()
+                writer.writerows(landmarks_table)
+
+            if bboxes_table:
+                bboxes_path = osp.join(
+                    save_dir,
+                    VggFace2Path.ANNOTATION_DIR,
+                    VggFace2Path.BBOXES_FILE + subset_name + ".csv",
+                )
+                os.makedirs(osp.dirname(bboxes_path), exist_ok=True)
+                with open(bboxes_path, "w", encoding="utf-8", newline="") as file:
+                    columns = ["NAME_ID", "X", "Y", "W", "H"]
+                    writer = csv.DictWriter(file, fieldnames=columns)
+                    writer.writeheader()
+                    writer.writerows(bboxes_table)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,33 @@
         return path
 
     @staticmethod
     def find_images_dir(rootpath: str, subset: str) -> str:
         return osp.join(rootpath, subset)
 
 
+class MmdetDirPathExtracter(DirPathExtracter):
+    @staticmethod
+    def find_rootpath(path: str) -> str:
+        """Find root path from annotation json file path."""
+        path = osp.abspath(path)
+        if osp.dirname(path).endswith(CocoPath.ANNOTATIONS_DIR):
+            return path.rsplit(CocoPath.ANNOTATIONS_DIR, maxsplit=1)[0]
+        raise DatasetImportError(
+            f"Annotation path ({path}) should be under the directory which is named {CocoPath.ANNOTATIONS_DIR}. "
+            "If not, Datumaro fails to find the root path for this dataset. "
+            "Please follow this instruction, https://github.com/cocodataset/cocoapi/blob/master/README.txt"
+        )
+
+    @staticmethod
+    def find_images_dir(rootpath: str, subset: str) -> str:
+        """Find images directory from the root path."""
+        return osp.join(rootpath, subset)
+
+
 class _CocoBase(SubsetBase):
     """
     Parses COCO annotations written in the following format:
     https://cocodataset.org/#format-data
     """
 
     def __init__(
@@ -117,14 +136,17 @@
 
         if coco_importer_type == CocoImporterType.default:
             self._rootpath = DirPathExtracter.find_rootpath(path)
             self._images_dir = DirPathExtracter.find_images_dir(self._rootpath, subset)
         elif coco_importer_type == CocoImporterType.roboflow:
             self._rootpath = RoboflowDirPathExtracter.find_rootpath(path)
             self._images_dir = RoboflowDirPathExtracter.find_images_dir(self._rootpath, subset)
+        elif coco_importer_type == CocoImporterType.mmdet:
+            self._rootpath = MmdetDirPathExtracter.find_rootpath(path)
+            self._images_dir = MmdetDirPathExtracter.find_images_dir(self._rootpath, subset)
         else:
             raise DatasetImportError(f"Not supported type: {coco_importer_type}")
 
         self._task = task
 
         self._merge_instance_polygons = merge_instance_polygons
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/extractor_merger.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     panoptic = auto()
     stuff = auto()
 
 
 class CocoImporterType(Enum):
     default = auto()
     roboflow = auto()
+    mmdet = auto()
 
 
 class CocoPath:
     IMAGES_DIR = "images"
     ANNOTATIONS_DIR = "annotations"
 
     IMAGE_EXT = ".jpg"
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/coco/page_mapper.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import re
 from typing import Dict, List, Optional, Type
 
-import json_stream
-from json_stream.base import StreamingJSONObject
-
 from datumaro.components.annotation import (
     NO_OBJECT_ID,
     AnnotationType,
     Bbox,
     Caption,
     Cuboid3d,
     Ellipse,
@@ -26,15 +23,16 @@
     PolyLine,
     RleMask,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError, MediaTypeError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, MediaElement, MediaType, PointCloud, Video, VideoFrame
-from datumaro.util import parse_json_file, to_dict_from_streaming_json
+from datumaro.plugins.data_formats.datumaro.page_mapper import DatumPageMapper
+from datumaro.util import parse_json_file
 from datumaro.version import __version__
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 __all__ = ["DatumaroBase"]
 
 
@@ -368,75 +366,43 @@
         video_dir: str,
         ctx: ImportContext,
     ) -> None:
         super().__init__(path, subset, rootpath, images_dir, pcd_dir, video_dir, ctx)
         self._length = None
 
     def __len__(self):
-        if self._length is None:
-            self._length = sum(1 for _ in self)
-        return self._length
+        return len(self._reader)
 
     def __iter__(self):
         pbar = self._ctx.progress_reporter
-        with open(self._reader, "rb") as fp:
-            data = json_stream.load(fp)
-            items = data.get("items", None)
-            if items is None:
-                raise DatasetImportError('Annotation JSON file should have "items" entity.')
-
-            length = 0
-            for item in pbar.iter(items):
-                item_desc = to_dict_from_streaming_json(item)
-                length += 1
-                yield self._parse_item(item_desc)
-
-            if self._length != length:
-                self._length = length
+        for item_desc in pbar.iter(
+            self._reader,
+            desc=f"Importing '{self._subset}'",
+        ):
+            yield self._parse_item(item_desc)
 
-    def _init_reader(self, path: str):
-        return path
+    def _init_reader(self, path: str) -> DatumPageMapper:
+        return DatumPageMapper(path)
 
     @staticmethod
-    def _load_media_type(path) -> Type[MediaElement]:
-        # We can assume that the media_type information will be within the first 1 KB of the file.
-        # This is because we are the producer of Datumaro format.
-        search_size = 1024  # 1 KB
-
-        pattern = '"media_type"\s*:\s*(\d+)'
-
-        with open(path, "r", encoding="utf-8") as fp:
-            out = fp.read(search_size)
-            found = re.search(pattern, out)
-
-            if found:
-                int_type = int(found.group(1))
-                return MediaType(int_type).IMAGE.media
-
-        return MediaType.IMAGE.media
+    def _load_media_type(page_mapper: DatumPageMapper) -> Type[MediaElement]:
+        media_type = page_mapper.media_type
 
-    @staticmethod
-    def _load_infos(path) -> Dict:
-        with open(path, "r", encoding="utf-8") as fp:
-            data = json_stream.load(fp)
-            infos = data.get("infos", {})
-            if isinstance(infos, StreamingJSONObject):
-                infos = to_dict_from_streaming_json(infos)
+        if media_type is None:
+            return MediaType.IMAGE.media
 
-            return infos
+        return media_type.media
 
     @staticmethod
-    def _load_categories(path) -> Dict:
-        with open(path, "r", encoding="utf-8") as fp:
-            data = json_stream.load(fp)
-            categories = data.get("categories", {})
-            if isinstance(categories, StreamingJSONObject):
-                categories = to_dict_from_streaming_json(categories)
+    def _load_infos(page_mapper: DatumPageMapper) -> Dict:
+        return page_mapper.infos
 
-            return JsonReader._load_categories({"categories": categories})
+    @staticmethod
+    def _load_categories(page_mapper: DatumPageMapper) -> Dict:
+        return JsonReader._load_categories({"categories": page_mapper.categories})
 
     def _load_items(self, parsed) -> List:
         return []
 
 
 class DatumaroBase(SubsetBase):
     LEGACY_VERSION = "legacy"
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,96 @@
 from datumaro.components.exporter import ExportContextComponent, Exporter
 from datumaro.components.media import Image, MediaElement, PointCloud, Video, VideoFrame
 from datumaro.util import cast, dump_json_file
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 
+class JsonWriter:
+    @classmethod
+    def _convert_attribute_categories(cls, attributes):
+        return sorted(attributes)
+
+    @classmethod
+    def _convert_labels_label_groups(cls, labels):
+        return sorted(labels)
+
+    @classmethod
+    def _convert_label_categories(cls, obj):
+        converted = {
+            "labels": [],
+            "label_groups": [],
+            "attributes": cls._convert_attribute_categories(obj.attributes),
+        }
+        for label in obj.items:
+            converted["labels"].append(
+                {
+                    "name": cast(label.name, str),
+                    "parent": cast(label.parent, str),
+                    "attributes": cls._convert_attribute_categories(label.attributes),
+                }
+            )
+        for label_group in obj.label_groups:
+            converted["label_groups"].append(
+                {
+                    "name": cast(label_group.name, str),
+                    "group_type": label_group.group_type.to_str(),
+                    "labels": cls._convert_labels_label_groups(label_group.labels),
+                }
+            )
+        return converted
+
+    @classmethod
+    def _convert_mask_categories(cls, obj):
+        converted = {
+            "colormap": [],
+        }
+        for label_id, color in obj.colormap.items():
+            converted["colormap"].append(
+                {
+                    "label_id": int(label_id),
+                    "r": int(color[0]),
+                    "g": int(color[1]),
+                    "b": int(color[2]),
+                }
+            )
+        return converted
+
+    @classmethod
+    def _convert_points_categories(cls, obj):
+        converted = {
+            "items": [],
+        }
+        for label_id, item in obj.items.items():
+            converted["items"].append(
+                {
+                    "label_id": int(label_id),
+                    "labels": [cast(label, str) for label in item.labels],
+                    "joints": [list(map(int, j)) for j in item.joints],
+                }
+            )
+        return converted
+
+    @classmethod
+    def write_categories(cls, categories) -> Dict[str, Dict]:
+        dict_cat = {}
+        for ann_type, desc in categories.items():
+            if isinstance(desc, LabelCategories):
+                converted_desc = cls._convert_label_categories(desc)
+            elif isinstance(desc, MaskCategories):
+                converted_desc = cls._convert_mask_categories(desc)
+            elif isinstance(desc, PointsCategories):
+                converted_desc = cls._convert_points_categories(desc)
+            else:
+                raise NotImplementedError()
+            dict_cat[ann_type.name] = converted_desc
+
+        return dict_cat
+
+
 class _SubsetWriter:
     def __init__(
         self,
         context: Exporter,
         subset: str,
         ann_file: str,
         export_context: ExportContextComponent,
@@ -212,24 +294,15 @@
 
         return item_desc
 
     def add_infos(self, infos):
         self._data["infos"].update(infos)
 
     def add_categories(self, categories):
-        for ann_type, desc in categories.items():
-            if isinstance(desc, LabelCategories):
-                converted_desc = self._convert_label_categories(desc)
-            elif isinstance(desc, MaskCategories):
-                converted_desc = self._convert_mask_categories(desc)
-            elif isinstance(desc, PointsCategories):
-                converted_desc = self._convert_points_categories(desc)
-            else:
-                raise NotImplementedError()
-            self.categories[ann_type.name] = converted_desc
+        self._data["categories"] = JsonWriter.write_categories(categories)
 
     def write(self, *args, **kwargs):
         dump_json_file(self.ann_file, self._data)
 
     def _convert_annotation(self, obj):
         assert isinstance(obj, Annotation)
 
@@ -335,73 +408,14 @@
             }
         )
         return converted
 
     def _convert_ellipse_object(self, obj: Ellipse):
         return self._convert_shape_object(obj)
 
-    def _convert_attribute_categories(self, attributes):
-        return sorted(attributes)
-
-    def _convert_labels_label_groups(self, labels):
-        return sorted(labels)
-
-    def _convert_label_categories(self, obj):
-        converted = {
-            "labels": [],
-            "label_groups": [],
-            "attributes": self._convert_attribute_categories(obj.attributes),
-        }
-        for label in obj.items:
-            converted["labels"].append(
-                {
-                    "name": cast(label.name, str),
-                    "parent": cast(label.parent, str),
-                    "attributes": self._convert_attribute_categories(label.attributes),
-                }
-            )
-        for label_group in obj.label_groups:
-            converted["label_groups"].append(
-                {
-                    "name": cast(label_group.name, str),
-                    "group_type": label_group.group_type.to_str(),
-                    "labels": self._convert_labels_label_groups(label_group.labels),
-                }
-            )
-        return converted
-
-    def _convert_mask_categories(self, obj):
-        converted = {
-            "colormap": [],
-        }
-        for label_id, color in obj.colormap.items():
-            converted["colormap"].append(
-                {
-                    "label_id": int(label_id),
-                    "r": int(color[0]),
-                    "g": int(color[1]),
-                    "b": int(color[2]),
-                }
-            )
-        return converted
-
-    def _convert_points_categories(self, obj):
-        converted = {
-            "items": [],
-        }
-        for label_id, item in obj.items.items():
-            converted["items"].append(
-                {
-                    "label_id": int(label_id),
-                    "labels": [cast(label, str) for label in item.labels],
-                    "joints": [list(map(int, j)) for j in item.joints],
-                }
-            )
-        return converted
-
 
 class _StreamSubsetWriter(_SubsetWriter):
     def __init__(
         self,
         context: Exporter,
         subset: str,
         ann_file: str,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os.path as osp
 from typing import Dict, List, Optional, Type
 
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 from datumaro.components.merge.extractor_merger import ExtractorMerger
-from datumaro.util import parse_json
+from datumaro.rust_api import JsonSectionPageMapper
 
 from .format import DatumaroPath
 
 
 class DatumaroImporter(Importer):
     PATH_CLS = DatumaroPath
 
@@ -24,17 +24,19 @@
         annot_file = context.require_file(
             osp.join(cls.PATH_CLS.ANNOTATIONS_DIR, "*" + cls.PATH_CLS.ANNOTATION_EXT)
         )
 
         with context.probe_text_file(
             annot_file,
             'must be a JSON object with "categories" ' 'and "items" keys',
-        ) as f:
-            contents = parse_json(f.read())
-            if not {"categories", "items"} <= contents.keys():
+        ):
+            fpath = osp.join(context.root_path, annot_file)
+            page_mapper = JsonSectionPageMapper(fpath)
+            sections = page_mapper.sections()
+            if not {"categories", "items"} <= sections.keys():
                 raise Exception
 
     @classmethod
     def find_sources(cls, path) -> List[Dict]:
         return cls._find_sources_recursive(
             path,
             cls.PATH_CLS.ANNOTATION_EXT,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import logging as log
 import os
 import os.path as osp
+import warnings
 from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
@@ -40,15 +41,19 @@
         self._categories = self._load_categories(path)
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self, path):
         label_cat = LabelCategories()
         for dirname in sorted(os.listdir(path)):
             if not os.path.isdir(os.path.join(path, dirname)):
-                raise NotADirectoryError(errno.ENOTDIR, os.strerror(errno.ENOTDIR), path)
+                warnings.warn(
+                    f"{dirname} is not a directory in the folder {path}, so this will"
+                    "be skipped when declaring the cateogries of `imagenet` dataset."
+                )
+                continue
             if dirname != ImagenetPath.IMAGE_DIR_NO_LABEL:
                 label_cat.add(dirname)
         return {AnnotationType.label: label_cat}
 
     def _load_items(self, path):
         items = {}
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Video
 from datumaro.plugins.data_formats.video import VIDEO_EXTENSIONS
+from datumaro.rust_api import JsonSectionPageMapper
 from datumaro.util import parse_json, parse_json_file
 from datumaro.util.os_util import find_files
 
 
 class KineticsBase(DatasetBase):
     def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         if not osp.isdir(path):
@@ -61,19 +62,21 @@
         return self._subsets[subset]
 
     def _media_files(self, subset):
         if subset in self._subset_media_files:
             return self._subset_media_files[subset]
 
         subset_path = self._subset_path(subset)
-        self._subset_media_files[subset] = {
-            osp.splitext(osp.basename(f))[0]: osp.join(subset_path, f)
-            for f in os.listdir(subset_path)
-            if osp.splitext(osp.basename(f))[1] in VIDEO_EXTENSIONS
-        }
+
+        self._subset_media_files[subset] = {}
+        for root, _, files in os.walk(subset_path):
+            for f in files:
+                key, file_extension = osp.splitext(f)
+                if file_extension.lstrip(".") in VIDEO_EXTENSIONS:
+                    self._subset_media_files[subset][key] = osp.join(root, f)
 
         return self._subset_media_files[subset]
 
     def _search_media_by_id(self, media_files, item_id):
         if item_id in media_files:
             return media_files[item_id]
 
@@ -137,18 +140,26 @@
             with context.alternative():
                 ann_file = context.require_file("*.json")
 
                 with context.probe_text_file(
                     ann_file,
                     "JSON file must contain an youtube 'url' key",
                 ) as f:
-                    contents = parse_json(f.read())
+                    fpath = osp.join(context.root_path, ann_file)
+                    page_mapper = JsonSectionPageMapper(fpath)
+                    sections = page_mapper.sections()
+
+                    page_map = next(iter(sections.values()))
+                    offset, size = page_map["offset"], page_map["size"]
+
+                    f.seek(offset, 0)
+                    contents = parse_json(f.read(size))
                     if not isinstance(contents, dict):
                         raise Exception
-                    if "youtube" not in next(iter(contents.values())).get("url", ""):
+                    if "youtube" not in contents.get("url", ""):
                         raise Exception
 
             with context.alternative():
                 ann_file = context.require_file("*.csv")
 
                 with context.probe_text_file(
                     ann_file,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,18 @@
         if osp.isfile(metafile):
             with open(metafile, "r", encoding="utf-8") as f:
                 meta = f.readlines()
 
         for i, data in enumerate(annotation_table):
             data = data.split(",")
             item_anno = []
-            label = int(data[0])
+            try:
+                label = int(data[0])
+            except ValueError:
+                continue
             if label != MnistCsvPath.NONE_LABEL:
                 item_anno.append(Label(label))
 
             if 0 < len(meta):
                 meta[i] = meta[i].strip().split(",")
 
             # support for single-channel image only
@@ -113,15 +116,15 @@
 
 class MnistCsvImporter(Importer):
     DETECT_CONFIDENCE = FormatDetectionConfidence.MEDIUM
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(
-            path, ".csv", "mnist_csv", file_filter=lambda p: osp.basename(p).startswith("mnist_")
+            path, ".csv", "mnist_csv", file_filter=lambda p: osp.basename(p).find("mnist_") != -1
         )
 
 
 class MnistCsvExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
     def _apply_impl(self):
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,73 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 from typing import Dict, List, Optional
 
+import pyarrow as pa
+
+from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
-from datumaro.errors import DatasetImportError
-from datumaro.util import parse_json
 
+from .format import DatumaroArrow
+
+__all__ = ["ArrowImporter"]
 
-class SegmentAnythingImporter(Importer):
-    _N_JSON_TO_TEST = 10
 
+class ArrowImporter(Importer):
     @classmethod
     def detect(
         cls,
         context: FormatDetectionContext,
     ) -> Optional[FormatDetectionConfidence]:
-        # test maximum 10 annotation files only
-        ctr = 0
-        for file in context.require_files_iter("*.json"):
-            ctr += 1
-            with context.probe_text_file(
-                file, "Annotation format is not Segmentat-Anything format", is_binary_file=True
-            ) as f:
-                anno = parse_json(f.read())
-                if (
-                    set(anno.keys()) != {"annotations", "image"}
-                    or (
-                        set(anno["image"].keys())
-                        != {
-                            "image_id",
-                            "width",
-                            "height",
-                            "file_name",
-                        }
-                    )
-                    or (
-                        anno["annotations"]
-                        and not {"id", "segmentation", "bbox"}.issubset(set(anno["annotations"][0]))
-                    )
-                ):
-                    raise DatasetImportError
-            if ctr > cls._N_JSON_TO_TEST:
-                break
+        if context.root_path.endswith(".arrow"):
+            cls._verify_datumaro_arrow_format(context.root_path)
+        else:
+            for arrow_file in context.require_files("*.arrow"):
+                with context.probe_text_file(
+                    arrow_file,
+                    f"{arrow_file} is not Datumaro arrow format.",
+                    is_binary_file=True,
+                ) as f:
+                    f.close()
+                    cls._verify_datumaro_arrow_format(os.path.join(context.root_path, arrow_file))
+
+    @classmethod
+    def find_sources(cls, path: str) -> List[Dict]:
+        def _filter(path: str) -> bool:
+            try:
+                cls._verify_datumaro_arrow_format(path)
+                return True
+            except DatasetImportError:
+                return False
+
+        return cls._find_sources_recursive(
+            path=path,
+            ext=".arrow",
+            extractor_name=cls.NAME,
+            file_filter=_filter,
+            max_depth=0,
+        )
 
     @classmethod
-    def find_sources(cls, path) -> List[Dict]:
-        if not os.path.isdir(path):
-            return []
-        return [{"url": path, "format": cls.NAME}]
+    def find_sources_with_params(cls, path: str, **extra_params) -> List[Dict]:
+        sources = cls.find_sources(path)
+        # Merge sources into one config but multiple file_paths
+        return [
+            {
+                "url": path,
+                "format": cls.NAME,
+                "options": {"file_paths": [source["url"] for source in sources]},
+            }
+        ]
+
+    @staticmethod
+    def _verify_datumaro_arrow_format(file: str) -> None:
+        with pa.memory_map(file, "r") as mm_file:
+            with pa.ipc.open_file(mm_file) as reader:
+                schema = reader.schema
+        DatumaroArrow.check_signature(schema.metadata.get(b"signature", b"").decode())
+        DatumaroArrow.check_version(schema.metadata.get(b"version", b"").decode())
+        DatumaroArrow.check_schema(schema)
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tabular.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tabular.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,386 +1,427 @@
-# Copyright (C) 2020-2023 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import csv
-import errno
 import os
 import os.path as osp
-from typing import Optional
+import warnings
+from typing import Dict, Optional, Type, TypeVar, Union
 
-from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Points
-from datumaro.components.dataset_base import DatasetBase, DatasetItem
-from datumaro.components.errors import (
-    AnnotationExportError,
-    DatasetImportError,
-    InvalidAnnotationError,
-    MediaTypeError,
+import numpy as np
+import pandas as pd
+from defusedxml import ElementTree
+
+from datumaro.components.annotation import (
+    AnnotationType,
+    Bbox,
+    Label,
+    LabelCategories,
+    Mask,
+    MaskCategories,
 )
-from datumaro.components.exporter import Exporter
-from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import ImportContext, Importer
-from datumaro.components.media import Image
-from datumaro.util.image import find_images
-from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
-
-
-class VggFace2Path:
-    ANNOTATION_DIR = "bb_landmark"
-    IMAGE_EXT = ".jpg"
-    BBOXES_FILE = "loose_bb_"
-    LANDMARKS_FILE = "loose_landmark_"
-    LABELS_FILE = "labels.txt"
-    IMAGES_DIR_NO_LABEL = "no_label"
-
-
-class VggFace2Base(DatasetBase):
-    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
-        subset = None
-        if osp.isdir(path):
-            self._path = path
-        elif osp.isfile(path):
-            subset = osp.splitext(osp.basename(path).split("_")[2])[0]
-            self._path = osp.dirname(path)
-        else:
-            raise DatasetImportError("Can't read annotations from '%s'" % path)
+from datumaro.components.dataset import DatasetItem
+from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetBase, SubsetBase
+from datumaro.components.errors import InvalidAnnotationError, InvalidFieldError, MissingFieldError
+from datumaro.components.importer import ImportContext
+from datumaro.components.media import Image, ImageFromFile
+from datumaro.util.image import IMAGE_EXTENSIONS, load_image
+
+T = TypeVar("T")
+
+
+class KaggleImageCsvBase(DatasetBase):
+    def __init__(
+        self,
+        path: str,
+        ann_file: str,
+        columns: Dict[str, str],
+        *,
+        subset: Optional[str] = DEFAULT_SUBSET_NAME,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(ctx=ctx)
 
-        annotation_files = [
-            p
-            for p in os.listdir(self._path)
-            if (
-                osp.basename(p).startswith(VggFace2Path.BBOXES_FILE)
-                or osp.basename(p).startswith(VggFace2Path.LANDMARKS_FILE)
-            )
-            and p.endswith(".csv")
-        ]
+        self._subset = subset
 
-        if len(annotation_files) < 1:
-            raise FileNotFoundError(errno.ENOENT, "Can't find annotations in the directory", path)
+        self._path = path
+        self._columns = columns
 
-        super().__init__(ctx=ctx)
+        self._items, label_cat = self._load_items(ann_file, columns)
+        self._categories = {AnnotationType.label: label_cat}
 
-        self._dataset_dir = osp.dirname(self._path)
-        self._subsets = (
-            {subset} if subset else set(osp.splitext(f.split("_")[2])[0] for f in annotation_files)
-        )
+    def _load_items(self, ann_file: str, columns: Dict[str, Union[str, list]]):
+        df = pd.read_csv(ann_file, header=None, on_bad_lines="skip")
+
+        indices = {}
+        for key, field in columns.items():
+            if key == "bbox":
+                indices[key] = []
+                for v in field:
+                    indices[key].append(list(df.iloc[0]).index(v))
+            else:
+                indices[key] = list(df.iloc[0]).index(field)
 
-        self._categories = {}
-        self._items = []
+        label_cat = LabelCategories()
+        items = []
+        for ind, row in df.iterrows():
+            if ind == 0:
+                continue
+            data_info = list(row)
+
+            media_name = data_info[indices["media"]]
+            id = osp.splitext(media_name)[0]
+
+            if not media_name.lower().endswith(tuple(IMAGE_EXTENSIONS)):
+                for ext in IMAGE_EXTENSIONS:
+                    media_path = osp.join(self._path, media_name + ext)
+                    if osp.exists(media_path):
+                        break
+            else:
+                media_path = osp.join(self._path, media_name)
+
+            if not osp.exists(media_path):
+                warnings.warn(
+                    f"'{media_path}' is not existed in the directory, "
+                    f"so we skip to create an dataset item according to {row}."
+                )
+                continue
 
-        self._load_categories()
-        for subset in self._subsets:
-            self._items.extend(list(self._load_items(subset).values()))
+            annotations = []
+            if "label" in indices:
+                label_name = str(data_info[indices["label"]])
+                label, cat = label_cat.find(label_name)
+
+                if not cat:
+                    label_cat.add(label_name)
+                    label, _ = label_cat.find(label_name)
+
+                annotations.append(Label(label=label))
+
+            items.append(
+                DatasetItem(
+                    id=id,
+                    subset=self._subset,
+                    media=Image.from_file(path=media_path),
+                    annotations=annotations,
+                )
+            )
 
-    def __iter__(self):
-        return iter(self._items)
+        return items, label_cat
 
     def categories(self):
         return self._categories
 
-    def _load_categories(self):
+    def __iter__(self):
+        yield from self._items
+
+
+class KaggleImageTxtBase(DatasetBase):
+    def __init__(
+        self,
+        path: str,
+        ann_file: str,
+        columns: Dict[str, int],
+        *,
+        subset: Optional[str] = DEFAULT_SUBSET_NAME,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(ctx=ctx)
+
+        self._subset = subset
+
+        self._path = path
+        self._columns = columns
+
+        self._items, label_cat = self._load_items(ann_file, columns)
+        self._categories = {AnnotationType.label: label_cat}
+
+    def _load_items(self, ann_file: str, columns: Dict[str, Union[int, list]]):
         label_cat = LabelCategories()
-        path = osp.join(self._dataset_dir, VggFace2Path.LABELS_FILE)
-        if has_meta_file(self._dataset_dir):
-            labels = parse_meta_file(self._dataset_dir).keys()
-            for label in labels:
-                label_cat.add(label)
-        elif osp.isfile(path):
-            with open(path, encoding="utf-8") as labels_file:
-                lines = [s.strip() for s in labels_file]
-            for line in lines:
-                objects = line.split()
-                label = objects[0]
-                class_name = None
-                if 1 < len(objects):
-                    class_name = objects[1]
-                label_cat.add(label, parent=class_name)
-        else:
-            for subset in self._subsets:
-                subset_path = osp.join(self._dataset_dir, subset)
-                if osp.isdir(subset_path):
-                    for images_dir in sorted(os.listdir(subset_path)):
-                        if (
-                            osp.isdir(osp.join(subset_path, images_dir))
-                            and images_dir != VggFace2Path.IMAGES_DIR_NO_LABEL
-                        ):
-                            label_cat.add(images_dir)
-        self._categories[AnnotationType.label] = label_cat
-
-    def _load_items(self, subset):
-        def _get_label(path):
-            label_name = path.split("/")[0]
-            label = None
-            if label_name != VggFace2Path.IMAGES_DIR_NO_LABEL:
-                label = self._categories[AnnotationType.label].find(label_name)[0]
-            return label
-
-        items = {}
-
-        image_dir = osp.join(self._dataset_dir, subset)
-        if osp.isdir(image_dir):
-            images = {
-                osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
-                for p in find_images(image_dir, recursive=True)
-            }
-        else:
-            images = {}
 
-        landmarks_path = osp.join(
-            self._dataset_dir,
-            VggFace2Path.ANNOTATION_DIR,
-            VggFace2Path.LANDMARKS_FILE + subset + ".csv",
-        )
-        if osp.isfile(landmarks_path):
-            with open(landmarks_path, encoding="utf-8") as content:
-                landmarks_table = list(csv.DictReader(content))
-            for row in landmarks_table:
-                item_id = row["NAME_ID"]
-                label = None
-                if "/" in item_id:
-                    label = _get_label(item_id)
-
-                if item_id not in items:
-                    image = images.get(row["NAME_ID"])
-                    if image:
-                        image = Image.from_file(path=image)
-                    items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
-
-                annotations = items[item_id].annotations
-                if [a for a in annotations if a.type == AnnotationType.points]:
-                    raise InvalidAnnotationError(
-                        "Item %s: an image can have only one " "set of landmarks" % item_id
+        item_ids = []
+        items = []
+        with open(ann_file, "r", encoding="utf-8") as f:
+            for line in f:
+                line = line.split()
+                media_name = line[columns["media"]]
+                item_id = osp.splitext(media_name)[0]
+
+                if item_id in item_ids:
+                    warnings.warn(
+                        f"There is duplicated '{id}' in {ann_file}, "
+                        f"so we skip to create an dataset item according to {line}."
                     )
+                    continue
 
-                if len([p for p in row if row[p] == ""]) == 0 and len(row) == 11:
-                    annotations.append(
-                        Points([float(row[p]) for p in row if p != "NAME_ID"], label=label)
+                if not media_name.lower().endswith(tuple(IMAGE_EXTENSIONS)):
+                    for ext in IMAGE_EXTENSIONS:
+                        media_path = osp.join(self._path, media_name + ext)
+                        if osp.exists(media_path):
+                            break
+                else:
+                    media_path = osp.join(self._path, media_name)
+
+                if not osp.exists(media_path):
+                    warnings.warn(
+                        f"'{media_path}' is not existed in the directory, "
+                        f"so we skip to create an dataset item according to {line}."
                     )
-                elif label is not None:
+                    continue
+
+                annotations = []
+                if "label" in columns:
+                    label_name = str(line[columns["label"]])
+                    label, cat = label_cat.find(label_name)
+
+                    if not cat:
+                        label_cat.add(label_name)
+                        label, _ = label_cat.find(label_name)
+
                     annotations.append(Label(label=label))
 
-        bboxes_path = osp.join(
-            self._dataset_dir,
-            VggFace2Path.ANNOTATION_DIR,
-            VggFace2Path.BBOXES_FILE + subset + ".csv",
-        )
-        if osp.isfile(bboxes_path):
-            with open(bboxes_path, encoding="utf-8") as content:
-                bboxes_table = list(csv.DictReader(content))
-            for row in bboxes_table:
-                item_id = row["NAME_ID"]
-                label = None
-                if "/" in item_id:
-                    label = _get_label(item_id)
-
-                if item_id not in items:
-                    image = images.get(row["NAME_ID"])
-                    if image:
-                        image = Image.from_file(path=image)
-                    items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
-
-                annotations = items[item_id].annotations
-                if [a for a in annotations if a.type == AnnotationType.bbox]:
-                    raise InvalidAnnotationError(
-                        "Item %s: an image can have only one " "bbox" % item_id
+                item_ids.append(item_id)
+                items.append(
+                    DatasetItem(
+                        id=item_id,
+                        subset=self._subset,
+                        media=Image.from_file(path=media_path),
+                        annotations=annotations,
                     )
+                )
 
-                if len([p for p in row if row[p] == ""]) == 0 and len(row) == 5:
-                    annotations.append(
-                        Bbox(
-                            float(row["X"]),
-                            float(row["Y"]),
-                            float(row["W"]),
-                            float(row["H"]),
-                            label=label,
-                        )
-                    )
-        return items
+        return items, label_cat
 
+    def categories(self):
+        return self._categories
 
-class VggFace2Importer(Importer):
-    @classmethod
-    def detect(cls, context: FormatDetectionContext) -> None:
-        with context.require_any():
-            for prefix in (VggFace2Path.BBOXES_FILE, VggFace2Path.LANDMARKS_FILE):
-                with context.alternative():
-                    context.require_file(f"{VggFace2Path.ANNOTATION_DIR}/{prefix}*.csv")
-
-    @classmethod
-    def find_sources(cls, path):
-        if osp.isdir(path):
-            annotation_dir = osp.join(path, VggFace2Path.ANNOTATION_DIR)
-            if osp.isdir(annotation_dir):
-                return [
-                    {
-                        "url": annotation_dir,
-                        "format": VggFace2Base.NAME,
-                    }
-                ]
-        elif osp.isfile(path):
-            if (
-                osp.basename(path).startswith(VggFace2Path.LANDMARKS_FILE)
-                or osp.basename(path).startswith(VggFace2Path.BBOXES_FILE)
-            ) and path.endswith(".csv"):
-                return [
-                    {
-                        "url": path,
-                        "format": VggFace2Base.NAME,
-                    }
-                ]
-        return []
-
-
-class VggFace2Exporter(Exporter):
-    DEFAULT_IMAGE_EXT = VggFace2Path.IMAGE_EXT
-
-    def _apply_impl(self):
-        def _get_name_id(item_parts, label_name):
-            if 1 < len(item_parts) and item_parts[0] == label_name:
-                return "/".join([label_name, *item_parts[1:]])
-            else:
-                return "/".join([label_name, *item_parts])
+    def __iter__(self):
+        yield from self._items
+
+
+class KaggleImageMaskBase(DatasetBase):
+    def __init__(
+        self,
+        path: str,
+        mask_path: str,
+        labelmap_file: Optional[str] = None,
+        *,
+        subset: Optional[str] = DEFAULT_SUBSET_NAME,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(ctx=ctx)
 
-        if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
-            raise MediaTypeError("Media type is not an image")
+        self._subset = subset
 
-        save_dir = self._save_dir
-        os.makedirs(save_dir, exist_ok=True)
+        self._path = path
+        self._mask_path = mask_path
 
-        if self._save_dataset_meta:
-            self._save_meta_file(save_dir)
+        self._categories = self._load_categories(labelmap_file)
+        self._items = self._load_items()
+
+    def _load_categories(self, label_map_file: Optional[str]):
+        label_map = dict()
+        if not label_map_file:
+            label_map["background"] = (0, 0, 0)
+            label_map["object"] = (255, 255, 255)
         else:
-            labels_path = osp.join(save_dir, VggFace2Path.LABELS_FILE)
-            labels_file = ""
-            for label in self._extractor.categories()[AnnotationType.label]:
-                labels_file += "%s" % label.name
-                if label.parent:
-                    labels_file += " %s" % label.parent
-                labels_file += "\n"
-            with open(labels_path, "w", encoding="utf-8") as f:
-                f.write(labels_file)
-
-        label_categories = self._extractor.categories()[AnnotationType.label]
-
-        for subset_name, subset in self._extractor.subsets().items():
-            bboxes_table = []
-            landmarks_table = []
-            for item in subset:
-                item_parts = item.id.split("/")
-                if item.media and self._save_media:
-                    labels = set(
-                        p.label for p in item.annotations if (getattr(p, "label", None) is not None)
-                    )
-                    if labels:
-                        for label in labels:
-                            image_dir = label_categories[label].name
-                            if 1 < len(item_parts) and image_dir == item_parts[0]:
-                                image_dir = ""
-                            self._save_image(item, subdir=osp.join(subset_name, image_dir))
-                    else:
-                        image_dir = VggFace2Path.IMAGES_DIR_NO_LABEL
-                        if 1 < len(item_parts) and image_dir == item_parts[0]:
-                            image_dir = ""
-                        self._save_image(item, subdir=osp.join(subset_name, image_dir))
-
-                landmarks = [a for a in item.annotations if a.type == AnnotationType.points]
-                if 1 < len(landmarks):
-                    raise AnnotationExportError(
-                        "Item (%s, %s): an image can have only one "
-                        "set of landmarks" % (item.id, item.subset)
+            df = pd.read_csv(label_map_file)
+            for _, row in df.iterrows():
+                name = row[0]
+                color = tuple([int(c) for c in row[1:]])
+                label_map[name] = color
+
+        label_categories = LabelCategories()
+        for label in label_map:
+            label_categories.add(label)
+
+        categories = {}
+        categories[AnnotationType.label] = label_categories
+
+        colormap = {}
+        for label_name, label_color in label_map.items():
+            label_id = label_categories.find(label_name)[0]
+            colormap[label_id] = label_color
+
+        categories[AnnotationType.mask] = MaskCategories(colormap)
+
+        return categories
+
+    def _load_items(self):
+        def _lazy_extract_mask(mask, c):
+            return lambda: mask == c
+
+        items = []
+        for media_name in os.listdir(self._path):
+            id = osp.splitext(media_name)[0]
+
+            anns = []
+            for mask_name in os.listdir(self._mask_path):
+                if id in mask_name:
+                    instances_mask = load_image(
+                        osp.join(self._mask_path, mask_name), dtype=np.int32
                     )
-                if landmarks:
-                    if landmarks[0].label is not None and label_categories[landmarks[0].label].name:
-                        name_id = _get_name_id(
-                            item_parts, label_categories[landmarks[0].label].name
-                        )
-                    else:
-                        name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
-                    points = landmarks[0].points
-                    if len(points) != 10:
-                        landmarks_table.append({"NAME_ID": name_id})
-                    else:
-                        landmarks_table.append(
-                            {
-                                "NAME_ID": name_id,
-                                "P1X": points[0],
-                                "P1Y": points[1],
-                                "P2X": points[2],
-                                "P2Y": points[3],
-                                "P3X": points[4],
-                                "P3Y": points[5],
-                                "P4X": points[6],
-                                "P4Y": points[7],
-                                "P5X": points[8],
-                                "P5Y": points[9],
-                            }
+                    label_ids = np.unique(instances_mask)
+                    for label_id in label_ids:
+                        anns.append(
+                            Mask(
+                                image=_lazy_extract_mask(instances_mask, label_id),
+                                label=label_id,
+                            )
                         )
 
-                bboxes = [a for a in item.annotations if a.type == AnnotationType.bbox]
-                if 1 < len(bboxes):
-                    raise AnnotationExportError(
-                        "Item (%s, %s): an image can have only one " "bbox" % (item.id, item.subset)
-                    )
-                if bboxes:
-                    if bboxes[0].label is not None and label_categories[bboxes[0].label].name:
-                        name_id = _get_name_id(item_parts, label_categories[bboxes[0].label].name)
-                    else:
-                        name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
-                    bboxes_table.append(
-                        {
-                            "NAME_ID": name_id,
-                            "X": bboxes[0].x,
-                            "Y": bboxes[0].y,
-                            "W": bboxes[0].w,
-                            "H": bboxes[0].h,
-                        }
-                    )
+            items.append(
+                DatasetItem(
+                    id=id,
+                    subset=self._subset,
+                    media=Image.from_file(path=osp.join(self._path, media_name)),
+                    annotations=anns,
+                )
+            )
 
-                labels = [a for a in item.annotations if a.type == AnnotationType.label]
-                for label in labels:
-                    if label.label is not None and label_categories[label.label].name:
-                        name_id = _get_name_id(item_parts, label_categories[labels[0].label].name)
-                    else:
-                        name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
-                    landmarks_table.append({"NAME_ID": name_id})
-
-                if not landmarks and not bboxes and not labels:
-                    landmarks_table.append(
-                        {"NAME_ID": _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)}
-                    )
+        return items
 
-            landmarks_path = osp.join(
-                save_dir,
-                VggFace2Path.ANNOTATION_DIR,
-                VggFace2Path.LANDMARKS_FILE + subset_name + ".csv",
+    def categories(self):
+        return self._categories
+
+    def __iter__(self):
+        yield from self._items
+
+
+class KaggleVocBase(SubsetBase):
+    ann_extensions = ".xml"
+
+    def __init__(
+        self,
+        path: str,
+        ann_path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(subset=subset, ctx=ctx)
+
+        self._label_cat = LabelCategories()
+        self._items = []
+        self._size = None
+
+        for img_filename in os.listdir(path):
+            if not img_filename.lower().endswith(tuple(IMAGE_EXTENSIONS)):
+                continue
+            item_id = os.path.splitext(img_filename)[0]
+
+            img_file = os.path.join(path, img_filename)
+            ann_file = os.path.join(ann_path, item_id + self.ann_extensions)
+
+            annotations = (
+                self._parse_annotations(img_file, ann_file) if os.path.isfile(ann_file) else []
             )
-            os.makedirs(osp.dirname(landmarks_path), exist_ok=True)
-            with open(landmarks_path, "w", encoding="utf-8", newline="") as file:
-                columns = [
-                    "NAME_ID",
-                    "P1X",
-                    "P1Y",
-                    "P2X",
-                    "P2Y",
-                    "P3X",
-                    "P3Y",
-                    "P4X",
-                    "P4Y",
-                    "P5X",
-                    "P5Y",
-                ]
-                writer = csv.DictWriter(file, fieldnames=columns)
-                writer.writeheader()
-                writer.writerows(landmarks_table)
-
-            if bboxes_table:
-                bboxes_path = osp.join(
-                    save_dir,
-                    VggFace2Path.ANNOTATION_DIR,
-                    VggFace2Path.BBOXES_FILE + subset_name + ".csv",
+
+            media = Image.from_file(path=img_file, size=self._size)
+
+            self._items.append(
+                DatasetItem(
+                    id=item_id,
+                    subset=self._subset,
+                    media=media,
+                    annotations=annotations,
                 )
-                os.makedirs(osp.dirname(bboxes_path), exist_ok=True)
-                with open(bboxes_path, "w", encoding="utf-8", newline="") as file:
-                    columns = ["NAME_ID", "X", "Y", "W", "H"]
-                    writer = csv.DictWriter(file, fieldnames=columns)
-                    writer.writeheader()
-                    writer.writerows(bboxes_table)
+            )
+        self._categories = {AnnotationType.label: self._label_cat}
+
+    def _parse_annotations(self, img_file: str, ann_file: str):
+        root_elem = ElementTree.parse(ann_file).getroot()
+        if root_elem.tag != "annotation":
+            raise MissingFieldError("annotation")
+
+        height = self._parse_field(root_elem, "size/height", int, required=False)
+        width = self._parse_field(root_elem, "size/width", int, required=False)
+        if height and width:
+            self._size = (height, width)
+
+        annotations = []
+        for obj_id, object_elem in enumerate(root_elem.iterfind("object")):
+            label_name = self._parse_field(object_elem, "name", str, required=True)
+
+            bbox_elem = object_elem.find("bndbox")
+            if not bbox_elem:
+                raise MissingFieldError("bndbox")
+
+            xmin = self._parse_field(bbox_elem, "xmin", float)
+            xmax = self._parse_field(bbox_elem, "xmax", float)
+            ymin = self._parse_field(bbox_elem, "ymin", float)
+            ymax = self._parse_field(bbox_elem, "ymax", float)
+
+            self._label_cat.add(label_name)
+            label_id, _ = self._label_cat.find(label_name)
+            annotations.append(
+                Bbox(id=obj_id, label=label_id, x=xmin, y=ymin, w=xmax - xmin, h=ymax - ymin)
+            )
+
+        return annotations
+
+    @staticmethod
+    def _parse_field(root, xpath: str, cls: Type[T] = str, required: bool = True) -> Optional[T]:
+        elem = root.find(xpath)
+        if elem is None:
+            if required:
+                raise MissingFieldError(xpath)
+            else:
+                return None
+
+        if cls is str:
+            return elem.text
+
+        try:
+            return cls(elem.text)
+        except Exception as e:
+            raise InvalidFieldError(xpath) from e
+
+
+class KaggleYoloBase(KaggleVocBase, SubsetBase):
+    ann_extensions = ".txt"
+
+    def __init__(
+        self,
+        path: str,
+        ann_path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(path=path, ann_path=ann_path, subset=subset, ctx=ctx)
+
+    def _parse_annotations(self, img_file: str, ann_file: str):
+        image = ImageFromFile(path=img_file)
+        image_height, image_width = image.size
+
+        lines = []
+        with open(ann_file, "r", encoding="utf-8") as f:
+            for line in f:
+                line = line.strip()
+                if line:
+                    lines.append(line)
+
+        annotations = []
+        for obj_id, line in enumerate(lines):
+            parts = line.split()
+            if len(parts) != 5:
+                raise InvalidAnnotationError(
+                    f"Unexpected field count {len(parts)} in the bbox description. "
+                    "Expected 5 fields (label, xc, yc, w, h)."
+                )
+            label_name, xc, yc, w, h = parts
+            xc = float(xc)
+            yc = float(yc)
+            w = float(w)
+            h = float(h)
+            x = (xc - w * 0.5) * image_width
+            y = (yc - h * 0.5) * image_height
+            w *= image_width
+            h *= image_height
+
+            self._label_cat.add(label_name)
+            label_id, _ = self._label_cat.find(label_name)
+
+            annotations.append(Bbox(id=obj_id, label=label_id, x=x, y=y, w=w, h=h))
+
+        return annotations
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/explorer.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/framework_converter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/framework_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,17 +108,14 @@
 
             self.transform = transform
             self.target_transform = target_transform
 
         def __getitem__(self, idx):
             image, label = self._gen_item(idx)
 
-            if image.dtype == np.uint8 or image.max() > 1:
-                image = image.astype(np.float32) / 255
-
             if len(image.shape) == 2:
                 image = np.expand_dims(image, axis=-1)
 
             if self.transform:
                 image = self.transform(image)
 
             if self.target_transform:
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/ndr.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Copyright (C) 2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import math
 import re
-
-import pandas as pd
+from typing import TYPE_CHECKING
 
 from .algorithm import InferenceResultAnalyzer
 
+if TYPE_CHECKING:
+    import pandas as pd
+else:
+    from datumaro.util.import_util import lazy_import
+
+    pd = lazy_import("pandas")
+
 
 class SampleEntropy(InferenceResultAnalyzer):
     """
     Entropy is a class that inherits an Sampler,
     calculates an uncertainty score based on an entropy,
     and get samples based on that score.
     """
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._seed = seed
         self._count = count
         self._indices = None
         self._subset = subset
 
     def __iter__(self):
         if self._indices is None:
-            rng = Random(self._seed)
+            rng = Random(self._seed)  # nosec B311
 
             if self._subset:
                 n = len(self._extractor.get_subset(self._subset))
             else:
                 n = len(self._extractor)
             self._indices = rng.sample(range(n), min(self._count, n))
             self._indices.sort()
@@ -210,15 +210,15 @@
 
         def _make_bucket():
             # label -> bucket
             return {label: [] for label in self._label_counts}
 
         buckets = defaultdict(_make_bucket)  # subset -> subset_buckets
 
-        rng = Random(self._seed)
+        rng = Random(self._seed)  # nosec B311
 
         for i, item in enumerate(self._extractor):
             labels = set(getattr(ann, "label", None) for ann in item.annotations)
             labels.discard(None)
             for label in labels:
                 if len(buckets[item.subset][label]) < self._label_counts[label]:
                     buckets[item.subset][label].append(item)
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # Copyright (C) 2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from collections import defaultdict
-from typing import Optional, Union
-
-import pandas as pd
+from typing import TYPE_CHECKING, Optional, Union
 
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import IDataset
 from datumaro.components.transformer import Transform
 from datumaro.util import parse_str_enum_value
 
 from .algorithm.algorithm import Algorithm, SamplingMethod
 
+if TYPE_CHECKING:
+    import pandas as pd
+else:
+    from datumaro.util.import_util import lazy_import
+
+    pd = lazy_import("pandas")
+
 
 class RelevancySampler(Transform, CliPlugin):
     r"""
     Sampler that analyzes model inference results on the dataset |n
     and picks the best sample for training.|n
     |n
     Creates a dataset from the `-k/--count` hardest items for a model.
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/specs.json` & `datumaro-1.6.0rc1/src/datumaro/plugins/specs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9601449275362319%*

 * *Differences: {'delete': '[2, 1, 0]',*

 * * 'insert': "[(89, OrderedDict([('import_path', "*

 * *           "'datumaro.plugins.data_formats.kaggle.base.KaggleImageCsvBase'), ('plugin_name', "*

 * *           "'kaggle_image_csv'), ('plugin_type', 'DatasetBase'), ('extra_deps', [])])), (90, "*

 * *           "OrderedDict([('import_path', "*

 * *           "'datumaro.plugins.data_formats.kaggle.base.KaggleImageMaskBase'), ('plugin_name', "*

 * *           "'kaggle_image_mask'), ('plugin_type', 'DatasetBase'), ('extra_deps', [])])), (91, "*

 * *           "Or […]*

```diff
@@ -1,27 +1,9 @@
 [
     {
-        "extra_deps": [],
-        "import_path": "datumaro.components.launcher.LauncherWithModelInterpreter",
-        "plugin_name": "launcher_with_model_interpreter",
-        "plugin_type": "Launcher"
-    },
-    {
-        "extra_deps": [],
-        "import_path": "datumaro.components.merge.extractor_merger.ExtractorMerger",
-        "plugin_name": "extractor_merger",
-        "plugin_type": "DatasetBase"
-    },
-    {
-        "extra_deps": [],
-        "import_path": "datumaro.components.transformer.ModelTransform",
-        "plugin_name": "model",
-        "plugin_type": "Transform"
-    },
-    {
         "extra_deps": [
             "openvino.tools",
             "tensorflow"
         ],
         "import_path": "datumaro.plugins.accuracy_checker_plugin.ac_launcher.AcLauncher",
         "plugin_name": "ac",
         "plugin_type": "Launcher"
@@ -552,14 +534,44 @@
         "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.imagenet_txt.ImagenetTxtImporter",
         "plugin_name": "imagenet_txt",
         "plugin_type": "Importer"
     },
     {
         "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.kaggle.base.KaggleImageCsvBase",
+        "plugin_name": "kaggle_image_csv",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.kaggle.base.KaggleImageMaskBase",
+        "plugin_name": "kaggle_image_mask",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.kaggle.base.KaggleImageTxtBase",
+        "plugin_name": "kaggle_image_txt",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.kaggle.base.KaggleVocBase",
+        "plugin_name": "kaggle_voc",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.kaggle.base.KaggleYoloBase",
+        "plugin_name": "kaggle_yolo",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.kinetics.KineticsBase",
         "plugin_name": "kinetics",
         "plugin_type": "DatasetBase"
     },
     {
         "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.kinetics.KineticsImporter",
@@ -726,14 +738,26 @@
         "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.mars.MarsImporter",
         "plugin_name": "mars",
         "plugin_type": "Importer"
     },
     {
         "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.mmdet.MmdetCocoBase",
+        "plugin_name": "mmdet_coco",
+        "plugin_type": "DatasetBase"
+    },
+    {
+        "extra_deps": [],
+        "import_path": "datumaro.plugins.data_formats.mmdet.MmdetCocoImporter",
+        "plugin_name": "mmdet_coco",
+        "plugin_type": "Importer"
+    },
+    {
+        "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.mnist.MnistBase",
         "plugin_name": "mnist",
         "plugin_type": "DatasetBase"
     },
     {
         "extra_deps": [],
         "import_path": "datumaro.plugins.data_formats.mnist.MnistExporter",
@@ -1414,14 +1438,20 @@
         "extra_deps": [],
         "import_path": "datumaro.plugins.openvino_plugin.shift_launcher.ShiftLauncher",
         "plugin_name": "shift",
         "plugin_type": "Launcher"
     },
     {
         "extra_deps": [],
+        "import_path": "datumaro.plugins.sam_transforms.automatic_mask_gen.SAMAutomaticMaskGeneration",
+        "plugin_name": "samautomatic_mask_generation",
+        "plugin_type": "Transform"
+    },
+    {
+        "extra_deps": [],
         "import_path": "datumaro.plugins.sam_transforms.bbox_to_inst_mask.SAMBboxToInstanceMask",
         "plugin_name": "sambbox_to_instance_mask",
         "plugin_type": "Transform"
     },
     {
         "extra_deps": [],
         "import_path": "datumaro.plugins.sampler.random_sampler.LabelRandomSampler",
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/specs.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/splitter.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
         self._download_colorization_model(self._model_dir)
 
         mp_ctx = get_context("spawn")  # On Mac 10.15 and Python 3.7 fork leads to hangs
         with mp_ctx.Pool(processes=self._cpu_count) as pool:
             try:
                 params = pool.map(
-                    self._generate_category, [Random(i) for i in range(self._categories)]
+                    self._generate_category,
+                    [Random(i) for i in range(self._categories)],  # nosec B311
                 )
             finally:
                 pool.close()
                 pool.join()
 
         instances_weights = np.repeat(self._weights, self._instances, axis=0)
         weight_per_img = np.tile(instances_weights, (self._categories, 1))
@@ -121,24 +122,24 @@
 
         net = cv.dnn.readNetFromCaffe(proto, model)
         net.getLayer(net.getLayerId("class8_ab")).blobs = [pts_in_hull]
         net.getLayer(net.getLayerId("conv8_313_rh")).blobs = [np.full([1, 313], 2.606, np.float32)]
 
         for i, param, w in zip(indices, params, weights):
             image = self._generate_image(
-                Random(i),
+                Random(i),  # nosec B311
                 param,
                 self._iterations,
                 self._height,
                 self._width,
                 draw_point=False,
                 weight=w,
             )
             color_image = colorize(image, net)
-            aug_image = augment(Random(i), color_image, background_colors)
+            aug_image = augment(Random(i), color_image, background_colors)  # nosec B311
             save_image(
                 osp.join(self._output_dir, "{:06d}.png".format(i)), aug_image, create_dir=True
             )
 
     def _generate_image(
         self,
         rng: Random,
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import platform
 import warnings
 from contextlib import contextmanager
 from random import Random
 from typing import ContextManager
 
 import cv2 as cv
 import numpy as np
@@ -113,18 +112,14 @@
 
     frame = frame.astype(np.float32) / 255
     img_l = rgb2lab(frame)  # get L from Lab image
     img_rs = cv.resize(img_l, (224, 224))  # resize image to network input size
     img_l_rs = img_rs - 50  # subtract 50 for mean-centering
 
     net.setInput(cv.dnn.blobFromImage(img_l_rs))
-    if platform.system() == "Darwin" and hasattr(net, "enableWinograd"):
-        # TODO: We temporarily disable Winograd for MacOS because there is an OpenCV assertion error only for MacOS
-        # https://github.com/openvinotoolkit/datumaro/actions/runs/3851853611/jobs/6563454834#step:5:1199
-        net.enableWinograd(False)
     ab_dec = net.forward()[0, :, :, :].transpose((1, 2, 0))
 
     ab_dec_us = cv.resize(ab_dec, (W_orig, H_orig))
     img_lab_out = np.concatenate(
         (img_l[..., np.newaxis], ab_dec_us), axis=2
     )  # concatenate with original image L
     img_bgr_out = np.clip(cv.cvtColor(img_lab_out, cv.COLOR_Lab2BGR), 0, 1)
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/tiling/util.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/transforms.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/plugins/validators.py` & `datumaro-1.6.0rc1/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/__init__.py` & `datumaro-1.6.0rc1/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/annotation_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/attrs_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/definitions.py` & `datumaro-1.6.0rc1/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/file_utils.py` & `datumaro-1.6.0rc1/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/image.py` & `datumaro-1.6.0rc1/src/datumaro/util/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+from __future__ import annotations
 
 import importlib
 import os
 import os.path as osp
 import shlex
 import weakref
 from contextlib import contextmanager
+from contextvars import ContextVar
 from enum import Enum, auto
 from io import BytesIO, IOBase
-from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 
 import numpy as np
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.errors import DatumaroError
 
 try:
@@ -25,61 +27,104 @@
 
 
 class _IMAGE_BACKENDS(Enum):
     cv2 = auto()
     PIL = auto()
 
 
-_IMAGE_BACKEND = None
+_IMAGE_BACKEND: ContextVar[_IMAGE_BACKENDS] = ContextVar("_IMAGE_BACKENDS")
 _image_loading_errors = (FileNotFoundError,)
 try:
     importlib.import_module("cv2")
-    _IMAGE_BACKEND = _IMAGE_BACKENDS.cv2
+    _IMAGE_BACKEND.set(_IMAGE_BACKENDS.cv2)
 except ModuleNotFoundError:
     import PIL
 
-    _IMAGE_BACKEND = _IMAGE_BACKENDS.PIL
+    _IMAGE_BACKEND.set(_IMAGE_BACKENDS.PIL)
     _image_loading_errors = (*_image_loading_errors, PIL.UnidentifiedImageError)
 
 from datumaro.util.image_cache import ImageCache
 from datumaro.util.os_util import find_files
 
+if TYPE_CHECKING:
+    from PIL.Image import Image as PILImage
+
+
+class ImageColorScale(Enum):
+    """Image color scale
+
+    - UNCHANGED: Use the original image's scale (default)
+    - COLOR: Use 3 channels (it can ignore the alpha channel or convert the gray scale image to BGR)
+    """
+
+    UNCHANGED = 0
+    COLOR = 1
+
+    def convert_cv2(self, img: np.ndarray) -> np.ndarray:
+        import cv2
+
+        if self == ImageColorScale.COLOR:
+            return cv2.imdecode(img, cv2.IMREAD_COLOR)
+
+        return cv2.imdecode(img, cv2.IMREAD_UNCHANGED)
+
+    def convert_pil(self, img: PILImage) -> PILImage:
+        if self == ImageColorScale.COLOR:
+            return img.convert("RGB")
+
+        return img
+
+
+IMAGE_COLOR_SCALE: ContextVar[ImageColorScale] = ContextVar(
+    "IMAGE_COLOR_SCALE", default=ImageColorScale.UNCHANGED
+)
+
+
+@contextmanager
+def decode_image_context(color_scale: ImageColorScale):
+    """Change Datumaro image decoding color scale.
+
+    For model training, it is recommended to use this context manager
+    to load images in the BGR 3-channel format. For example,
+
+    .. code-block:: python
+
+        import datumaro as dm
+        with decode_image_context(ImageColorScale.COLOR):
+            item: dm.DatasetItem
+            img_data = item.media_as(dm.Image).data
+            assert img_data.shape[-1] == 3  # It should be a 3-channel image
+    """
+    curr_ctx = IMAGE_COLOR_SCALE.get()
+    IMAGE_COLOR_SCALE.set(color_scale)
+    yield
+    IMAGE_COLOR_SCALE.set(curr_ctx)
+
 
 def load_image(path: str, dtype: DTypeLike = np.uint8, crypter: Crypter = NULL_CRYPTER):
     """
     Reads an image in the HWC Grayscale/BGR(A) [0; 255] format (default dtype is uint8).
     """
 
-    if _IMAGE_BACKEND == _IMAGE_BACKENDS.cv2:
+    if _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.cv2:
         # cv2.imread does not support paths that are not representable
         # in the locale encoding on Windows, so we read the image bytes
         # ourselves.
 
         with open(path, "rb") as f:
             image_bytes = crypter.decrypt(f.read())
 
         return decode_image(image_bytes, dtype=dtype)
-    elif _IMAGE_BACKEND == _IMAGE_BACKENDS.PIL:
-        from PIL import Image
-
-        if not crypter.is_null_crypter:
-            raise DatumaroError("PIL backend should have crypter=NullCrypter.")
+    elif _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.PIL:
+        with open(path, "rb") as f:
+            image_bytes = crypter.decrypt(f.read())
 
-        image = Image.open(path)
-        image = np.asarray(image, dtype=dtype)
-        if len(image.shape) == 3 and image.shape[2] in {3, 4}:
-            image = np.array(image)  # Release read-only
-            image[:, :, :3] = image[:, :, 2::-1]  # RGB to BGR
-    else:
-        raise NotImplementedError()
+        return decode_image(image_bytes, dtype=dtype)
 
-    assert len(image.shape) in {2, 3}
-    if len(image.shape) == 3:
-        assert image.shape[2] in {3, 4}
-    return image
+    raise NotImplementedError(_IMAGE_BACKEND)
 
 
 def copyto_image(
     src: Union[str, IOBase], dst: Union[str, IOBase], src_crypter: Crypter, dst_crypter: Crypter
 ) -> None:
     if src_crypter == dst_crypter and src == dst:
         return
@@ -126,15 +171,15 @@
 
     if not kwargs:
         kwargs = {}
 
     # NOTE: OpenCV documentation says "If the image format is not supported,
     # the image will be converted to 8-bit unsigned and saved that way".
     # Conversion from np.int32 to np.uint8 is not working properly
-    backend = _IMAGE_BACKEND
+    backend = _IMAGE_BACKEND.get()
     if dtype == np.int32:
         backend = _IMAGE_BACKENDS.PIL
     if backend == _IMAGE_BACKENDS.cv2:
         # cv2.imwrite does not support paths that are not representable
         # in the locale encoding on Windows, so we write the image bytes
         # ourselves.
 
@@ -168,15 +213,15 @@
         raise NotImplementedError()
 
 
 def encode_image(image: np.ndarray, ext: str, dtype: DTypeLike = np.uint8, **kwargs) -> bytes:
     if not kwargs:
         kwargs = {}
 
-    if _IMAGE_BACKEND == _IMAGE_BACKENDS.cv2:
+    if _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.cv2:
         import cv2
 
         params = []
 
         if not ext.startswith("."):
             ext = "." + ext
 
@@ -184,15 +229,15 @@
             params = [int(cv2.IMWRITE_JPEG_QUALITY), kwargs.get("jpeg_quality", 75)]
 
         image = image.astype(dtype)
         success, result = cv2.imencode(ext, image, params=params)
         if not success:
             raise Exception("Failed to encode image to '%s' format" % (ext))
         return result.tobytes()
-    elif _IMAGE_BACKEND == _IMAGE_BACKENDS.PIL:
+    elif _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.PIL:
         from PIL import Image
 
         if ext.startswith("."):
             ext = ext[1:]
 
         params = {}
         params["quality"] = kwargs.get("jpeg_quality")
@@ -207,24 +252,25 @@
             image.save(buffer, format=ext, **params)
             return buffer.getvalue()
     else:
         raise NotImplementedError()
 
 
 def decode_image(image_bytes: bytes, dtype: DTypeLike = np.uint8) -> np.ndarray:
-    if _IMAGE_BACKEND == _IMAGE_BACKENDS.cv2:
-        import cv2
+    ctx_color_scale = IMAGE_COLOR_SCALE.get()
 
+    if _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.cv2:
         image = np.frombuffer(image_bytes, dtype=np.uint8)
-        image = cv2.imdecode(image, cv2.IMREAD_UNCHANGED)
+        image = ctx_color_scale.convert_cv2(image)
         image = image.astype(dtype)
-    elif _IMAGE_BACKEND == _IMAGE_BACKENDS.PIL:
+    elif _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.PIL:
         from PIL import Image
 
         image = Image.open(BytesIO(image_bytes))
+        image = ctx_color_scale.convert_pil(image)
         image = np.asarray(image, dtype=dtype)
         if len(image.shape) == 3 and image.shape[2] in {3, 4}:
             image = np.array(image)  # Release read-only
             image[:, :, :3] = image[:, :, 2::-1]  # RGB to BGR
     else:
         raise NotImplementedError()
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/image_cache.py` & `datumaro-1.6.0rc1/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/log_utils.py` & `datumaro-1.6.0rc1/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/mask_tools.py` & `datumaro-1.6.0rc1/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/meta_file_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/multi_procs_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/multi_procs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/os_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/os_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 try:
     # Declare functions to remove files and directories.
     #
     # Use rmtree from GitPython to avoid the problem with removal of
     # readonly files on Windows, which Git uses extensively
     # It double checks if a file cannot be removed because of readonly flag
     from git.util import rmfile, rmtree  # noqa: F401
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     from os import remove as rmfile  # noqa: F401
     from shutil import rmtree as rmtree  # noqa: F401
 
 from . import cast
 from .definitions import DEFAULT_SUBSET_NAME
 
 DEFAULT_MAX_DEPTH = 10
```

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/pickle_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/scope.py` & `datumaro-1.6.0rc1/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/telemetry_stub.py` & `datumaro-1.6.0rc1/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/telemetry_utils.py` & `datumaro-1.6.0rc1/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro/util/tf_util.py` & `datumaro-1.6.0rc1/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc0/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.6.0rc1/src/datumaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.0rc0
+Version: 1.6.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,41 +29,41 @@
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
 Requires-Dist: pandas>=1.1.5
-Requires-Dist: openvino==2023.1.0
+Requires-Dist: openvino>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
 Requires-Dist: protobuf<4
 Requires-Dist: tabulate
 Requires-Dist: ovmsclient
 Requires-Dist: tritonclient[all]
 Requires-Dist: scikit-learn
 Requires-Dist: json-stream
 Requires-Dist: opencv-python
 Provides-Extra: tf
 Requires-Dist: tensorflow; extra == "tf"
 Provides-Extra: tfds
-Requires-Dist: tensorflow-datasets; extra == "tfds"
+Requires-Dist: tensorflow-datasets<4.9.3; extra == "tfds"
 Provides-Extra: tf-gpu
 Requires-Dist: tensorflow-gpu; extra == "tf-gpu"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: torchvision; extra == "torch"
 Provides-Extra: default
-Requires-Dist: dvc>=3.0.0; extra == "default"
+Requires-Dist: dvc==3.30.1; extra == "default"
 Requires-Dist: fsspec<=2022.11.0; python_version < "3.8" and extra == "default"
 Requires-Dist: GitPython!=3.1.25,>=3.1.18; extra == "default"
 Requires-Dist: openvino-telemetry>=2022.1.0; extra == "default"
-Requires-Dist: openvino-dev==2023.1.0; extra == "default"
+Requires-Dist: openvino-dev>=2023.2.0; extra == "default"
 
 # Dataset Management Framework (Datumaro)
 
 [![Build status](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml/badge.svg)](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml)
 [![codecov](https://codecov.io/gh/openvinotoolkit/datumaro/branch/develop/graph/badge.svg?token=FG25VU096Q)](https://codecov.io/gh/openvinotoolkit/datumaro)
 
 A framework and CLI tool to build, transform, and analyze datasets.
@@ -105,15 +105,15 @@
   - [Open Images](https://storage.googleapis.com/openimages/web/download.html)
   - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/index.html)
     (`classification`, `detection`, `segmentation`, `action_classification`, `person_layout`)
   - [TF Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/using_your_own_dataset.md)
     (`bboxes`, `masks`)
   - [YOLO](https://github.com/AlexeyAB/darknet#how-to-train-pascal-voc-data) (`bboxes`)
 
-  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/supported_formats).
+  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/formats).
 - Dataset building
   - Merging multiple datasets into one
   - Dataset filtering by a custom criteria:
     - remove polygons of a certain class
     - remove images without annotations of a specific class
     - remove `occluded` annotations from images
     - keep only vertically-oriented images
```

### Comparing `datumaro-1.6.0rc0/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.6.0rc1/src/datumaro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 README.md
 pyproject.toml
 requirements-core.txt
 requirements-default.txt
 setup.py
 rust/Cargo.toml
 rust/src/coco_page_mapper.rs
+rust/src/datum_page_mapper.rs
+rust/src/json_section_page_mapper.rs
 rust/src/lib.rs
+rust/src/page_mapper.rs
 rust/src/page_maps.rs
 rust/src/utils.rs
 src/datumaro/__init__.py
 src/datumaro/__main__.py
 src/datumaro/errors.py
 src/datumaro/ops.py
 src/datumaro/project.py
@@ -151,36 +154,35 @@
 src/datumaro/plugins/data_formats/imagenet.py
 src/datumaro/plugins/data_formats/imagenet_txt.py
 src/datumaro/plugins/data_formats/kinetics.py
 src/datumaro/plugins/data_formats/labelme.py
 src/datumaro/plugins/data_formats/lfw.py
 src/datumaro/plugins/data_formats/market1501.py
 src/datumaro/plugins/data_formats/mars.py
+src/datumaro/plugins/data_formats/mmdet.py
 src/datumaro/plugins/data_formats/mnist.py
 src/datumaro/plugins/data_formats/mnist_csv.py
 src/datumaro/plugins/data_formats/mot.py
 src/datumaro/plugins/data_formats/mots.py
 src/datumaro/plugins/data_formats/nyu_depth_v2.py
 src/datumaro/plugins/data_formats/open_images.py
 src/datumaro/plugins/data_formats/tabular.py
 src/datumaro/plugins/data_formats/vgg_face2.py
 src/datumaro/plugins/data_formats/video.py
 src/datumaro/plugins/data_formats/vott_csv.py
 src/datumaro/plugins/data_formats/vott_json.py
 src/datumaro/plugins/data_formats/widerface.py
 src/datumaro/plugins/data_formats/arrow/__init__.py
-src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
 src/datumaro/plugins/data_formats/arrow/base.py
 src/datumaro/plugins/data_formats/arrow/exporter.py
 src/datumaro/plugins/data_formats/arrow/format.py
 src/datumaro/plugins/data_formats/arrow/importer.py
 src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
 src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
 src/datumaro/plugins/data_formats/arrow/mapper/media.py
-src/datumaro/plugins/data_formats/arrow/mapper/utils.py
 src/datumaro/plugins/data_formats/ava/__init__.py
 src/datumaro/plugins/data_formats/ava/ava.py
 src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
 src/datumaro/plugins/data_formats/celeba/__init__.py
 src/datumaro/plugins/data_formats/celeba/align_celeba.py
 src/datumaro/plugins/data_formats/celeba/celeba.py
 src/datumaro/plugins/data_formats/coco/__init__.py
@@ -195,28 +197,31 @@
 src/datumaro/plugins/data_formats/cvat/exporter.py
 src/datumaro/plugins/data_formats/cvat/format.py
 src/datumaro/plugins/data_formats/datumaro/__init__.py
 src/datumaro/plugins/data_formats/datumaro/base.py
 src/datumaro/plugins/data_formats/datumaro/exporter.py
 src/datumaro/plugins/data_formats/datumaro/format.py
 src/datumaro/plugins/data_formats/datumaro/importer.py
+src/datumaro/plugins/data_formats/datumaro/page_mapper.py
 src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
 src/datumaro/plugins/data_formats/datumaro_binary/base.py
 src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
 src/datumaro/plugins/data_formats/datumaro_binary/format.py
 src/datumaro/plugins/data_formats/datumaro_binary/importer.py
 src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
 src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
 src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
 src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
 src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
 src/datumaro/plugins/data_formats/icdar/__init__.py
 src/datumaro/plugins/data_formats/icdar/base.py
 src/datumaro/plugins/data_formats/icdar/exporter.py
 src/datumaro/plugins/data_formats/icdar/format.py
+src/datumaro/plugins/data_formats/kaggle/__init__.py
+src/datumaro/plugins/data_formats/kaggle/base.py
 src/datumaro/plugins/data_formats/kitti/__init__.py
 src/datumaro/plugins/data_formats/kitti/base.py
 src/datumaro/plugins/data_formats/kitti/exporter.py
 src/datumaro/plugins/data_formats/kitti/format.py
 src/datumaro/plugins/data_formats/kitti/importer.py
 src/datumaro/plugins/data_formats/kitti_raw/__init__.py
 src/datumaro/plugins/data_formats/kitti_raw/base.py
@@ -281,16 +286,18 @@
 src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
 src/datumaro/plugins/openvino_plugin/samples/imagenet.class
 src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
 src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
 src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
 src/datumaro/plugins/openvino_plugin/samples/utils.py
 src/datumaro/plugins/sam_transforms/__init__.py
+src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
 src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
 src/datumaro/plugins/sam_transforms/interpreters/__init__.py
+src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
 src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
 src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
 src/datumaro/plugins/sampler/__init__.py
 src/datumaro/plugins/sampler/random_sampler.py
 src/datumaro/plugins/sampler/relevancy_sampler.py
 src/datumaro/plugins/sampler/algorithm/__init__.py
 src/datumaro/plugins/sampler/algorithm/algorithm.py
@@ -306,14 +313,15 @@
 src/datumaro/util/__init__.py
 src/datumaro/util/annotation_util.py
 src/datumaro/util/attrs_util.py
 src/datumaro/util/definitions.py
 src/datumaro/util/file_utils.py
 src/datumaro/util/image.py
 src/datumaro/util/image_cache.py
+src/datumaro/util/import_util.py
 src/datumaro/util/log_utils.py
 src/datumaro/util/mask_tools.py
 src/datumaro/util/meta_file_util.py
 src/datumaro/util/multi_procs_util.py
 src/datumaro/util/os_util.py
 src/datumaro/util/pickle_util.py
 src/datumaro/util/samples.py
```

### Comparing `datumaro-1.6.0rc0/src/datumaro.egg-info/requires.txt` & `datumaro-1.6.0rc1/src/datumaro.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 typing_extensions>=3.7.4.3
 tqdm
 PyYAML>=5.3.1
 tensorboardX!=2.3,>=1.8
 scipy
 requests
 pandas>=1.1.5
-openvino==2023.1.0
+openvino>=2023.2.0
 tokenizers
 cryptography>=38.03
 pyemd
 pyarrow
 protobuf<4
 tabulate
 ovmsclient
@@ -33,27 +33,27 @@
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
 
 [default]
-dvc>=3.0.0
+dvc==3.30.1
 GitPython!=3.1.25,>=3.1.18
 openvino-telemetry>=2022.1.0
-openvino-dev==2023.1.0
+openvino-dev>=2023.2.0
 
 [default:python_version < "3.8"]
 fsspec<=2022.11.0
 
 [tf]
 tensorflow
 
 [tf-gpu]
 tensorflow-gpu
 
 [tfds]
-tensorflow-datasets
+tensorflow-datasets<4.9.3
 
 [torch]
 torch
 torchvision
```

