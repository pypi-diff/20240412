# Comparing `tmp/gen3_tracker-0.0.3rc1.tar.gz` & `tmp/gen3_tracker-0.0.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.3rc1.tar", last modified: Fri Apr 12 00:05:16 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.3rc2.tar", last modified: Fri Apr 12 00:16:43 2024, max compression
```

## Comparing `gen3_tracker-0.0.3rc1.tar` & `gen3_tracker-0.0.3rc2.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.785117 gen3_tracker-0.0.3rc1/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.3rc1/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-12 00:05:16.784659 gen3_tracker-0.0.3rc1/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1338 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.784138 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-12 00:05:16.000000 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     2827 2024-04-12 00:05:16.000000 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-04-12 00:05:16.000000 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       47 2024-04-12 00:05:16.000000 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      186 2024-04-12 00:05:16.000000 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2024-04-12 00:05:16.000000 gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/top_level.txt
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.743307 gen3_tracker-0.0.3rc1/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2885 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.749019 gen3_tracker-0.0.3rc1/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3307 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4706 2024-04-12 00:03:34.000000 gen3_tracker-0.0.3rc1/gen3_util/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.752995 gen3_tracker-0.0.3rc1/gen3_util/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.3rc1/gen3_util/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.3rc1/gen3_util/access/policies/add-project-default.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       77 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/access/policies/add-user-delete.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.3rc1/gen3_util/access/policies/add-user-read.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142      199 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/access/policies/add-user-write.yaml
--rw-r--r--   0 walsbr   (320923486) 1971611142     6813 2024-04-11 23:53:48.000000 gen3_tracker-0.0.3rc1/gen3_util/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1052 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/access/submitter.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.753875 gen3_tracker-0.0.3rc1/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.754127 gen3_tracker-0.0.3rc1/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142    13758 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.754607 gen3_tracker-0.0.3rc1/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142    10225 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      876 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/config.yaml
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.756548 gen3_tracker-0.0.3rc1/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1457 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    10733 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3751 2024-03-01 20:19:22.000000 gen3_tracker-0.0.3rc1/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12564 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/files/manifest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1503 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/files/middleware.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      634 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5194 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.757317 gen3_tracker-0.0.3rc1/gen3_util/jobs/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc1/gen3_util/jobs/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2618 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/jobs/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/jobs/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.760770 gen3_tracker-0.0.3rc1/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4438 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1415 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/bundler.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8981 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      687 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/delta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2894 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/differ.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      326 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1655 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2932 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/publisher.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    15141 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/skeleton.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.761085 gen3_tracker-0.0.3rc1/gen3_util/meta/tabular/
--rw-r--r--   0 walsbr   (320923486) 1971611142    11706 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4660 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4477 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.762363 gen3_tracker-0.0.3rc1/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2778 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3696 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2341 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1496 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.765220 gen3_tracker-0.0.3rc1/gen3_util/repo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4557 2024-04-11 18:50:38.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    17370 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3726 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/cloner.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     9643 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/committer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/history.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1512 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/initializer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1699 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/puller.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4405 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/pusher.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2959 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/gen3_util/repo/status.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.765761 gen3_tracker-0.0.3rc1/gen3_util/users/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.3rc1/gen3_util/users/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1694 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/gen3_util/users/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-04-12 00:05:16.785197 gen3_tracker-0.0.3rc1/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5581 2024-04-12 00:04:49.000000 gen3_tracker-0.0.3rc1/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.714826 gen3_tracker-0.0.3rc1/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.768651 gen3_tracker-0.0.3rc1/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc1/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1091 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1066 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      454 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    12460 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/integration/test_commit.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      257 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/integration/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2182 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/integration/test_init.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     9506 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/integration/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     8848 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/integration/test_meta_skeleton.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1321 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.780216 gen3_tracker-0.0.3rc1/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc1/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      464 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/conftest.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.780750 gen3_tracker-0.0.3rc1/tests/unit/plugins/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc1/tests/unit/plugins/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.781436 gen3_tracker-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:05:16.783860 gen3_tracker-0.0.3rc1/tests/unit/tabular/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    16696 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1172 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     7826 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/test_default_columns.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1035 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/test_dir_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/test_from_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3779 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/test_to_tabular.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      737 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/tabular/test_validate.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3429 2024-04-11 17:33:16.000000 gen3_tracker-0.0.3rc1/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4881 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/unit/test_coding.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc1/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      532 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1417 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      445 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc1/tests/unit/test_job_dependencies.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      734 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/test_manifest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/test_validate_directory.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      625 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc1/tests/unit/test_version.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.571513 gen3_tracker-0.0.3rc2/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.3rc2/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-12 00:16:43.570992 gen3_tracker-0.0.3rc2/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1338 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.570265 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2415 2024-04-12 00:16:43.000000 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2827 2024-04-12 00:16:43.000000 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-04-12 00:16:43.000000 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       47 2024-04-12 00:16:43.000000 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      186 2024-04-12 00:16:43.000000 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2024-04-12 00:16:43.000000 gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.530737 gen3_tracker-0.0.3rc2/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2885 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.536564 gen3_tracker-0.0.3rc2/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3307 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4706 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.545998 gen3_tracker-0.0.3rc2/gen3_util/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.3rc2/gen3_util/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.3rc2/gen3_util/access/policies/add-project-default.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       77 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/access/policies/add-user-delete.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.3rc2/gen3_util/access/policies/add-user-read.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142      199 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/access/policies/add-user-write.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6813 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/access/requestor.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1052 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/access/submitter.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.552258 gen3_tracker-0.0.3rc2/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.552618 gen3_tracker-0.0.3rc2/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13758 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.553195 gen3_tracker-0.0.3rc2/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10225 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      876 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/config.yaml
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.555417 gen3_tracker-0.0.3rc2/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1457 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10733 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3751 2024-03-01 20:19:22.000000 gen3_tracker-0.0.3rc2/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12564 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/files/manifest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1503 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/files/middleware.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      634 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5194 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.556120 gen3_tracker-0.0.3rc2/gen3_util/jobs/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc2/gen3_util/jobs/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2618 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/jobs/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/jobs/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.558796 gen3_tracker-0.0.3rc2/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4438 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1415 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/bundler.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8981 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      687 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/delta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2894 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/differ.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      326 2023-10-19 18:01:08.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2204 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1655 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2932 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/publisher.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    15141 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/skeleton.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.559010 gen3_tracker-0.0.3rc2/gen3_util/meta/tabular/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11706 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/tabular/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4660 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4477 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.559855 gen3_tracker-0.0.3rc2/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2778 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3696 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2341 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1496 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.561947 gen3_tracker-0.0.3rc2/gen3_util/repo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4557 2024-04-11 18:50:38.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    17370 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3726 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/cloner.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9643 2024-04-11 23:52:05.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/committer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/history.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1512 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/initializer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1699 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/puller.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4405 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/pusher.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2959 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/gen3_util/repo/status.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.562336 gen3_tracker-0.0.3rc2/gen3_util/users/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.3rc2/gen3_util/users/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1829 2024-04-12 00:15:21.000000 gen3_tracker-0.0.3rc2/gen3_util/users/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-04-12 00:16:43.571630 gen3_tracker-0.0.3rc2/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5581 2024-04-12 00:16:16.000000 gen3_tracker-0.0.3rc2/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.480321 gen3_tracker-0.0.3rc2/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.564508 gen3_tracker-0.0.3rc2/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc2/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1091 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1066 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      454 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    12460 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/tests/integration/test_commit.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      257 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/integration/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2182 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/tests/integration/test_init.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     9506 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/integration/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     8848 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/integration/test_meta_skeleton.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1321 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.566952 gen3_tracker-0.0.3rc2/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc2/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      464 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/conftest.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.567199 gen3_tracker-0.0.3rc2/tests/unit/plugins/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc2/tests/unit/plugins/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.567433 gen3_tracker-0.0.3rc2/tests/unit/plugins/gen3_util_plugin_foo/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1450 2023-07-07 00:45:48.000000 gen3_tracker-0.0.3rc2/tests/unit/plugins/gen3_util_plugin_foo/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-04-12 00:16:43.569892 gen3_tracker-0.0.3rc2/tests/unit/tabular/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    16696 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1172 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7826 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/test_default_columns.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1035 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/test_dir_to_tabular.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1888 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/test_from_tabular.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3779 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/test_to_tabular.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      737 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/tabular/test_validate.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3429 2024-04-12 00:15:07.000000 gen3_tracker-0.0.3rc2/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4881 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/tests/unit/test_coding.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_tracker-0.0.3rc2/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      532 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1417 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      445 2024-04-11 23:52:06.000000 gen3_tracker-0.0.3rc2/tests/unit/test_job_dependencies.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      734 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/test_manifest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/test_validate_directory.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      625 2024-02-26 20:51:35.000000 gen3_tracker-0.0.3rc2/tests/unit/test_version.py
```

### Comparing `gen3_tracker-0.0.3rc1/LICENSE` & `gen3_tracker-0.0.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/PKG-INFO` & `gen3_tracker-0.0.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.3rc1
+Version: 0.0.3rc2
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gen3_tracker-0.0.3rc1/README.md` & `gen3_tracker-0.0.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/PKG-INFO` & `gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-tracker
-Version: 0.0.3rc1
+Version: 0.0.3rc2
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gen3_tracker-0.0.3rc1/gen3_tracker.egg-info/SOURCES.txt` & `gen3_tracker-0.0.3rc2/gen3_tracker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/access/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/access/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/access/requestor.py` & `gen3_tracker-0.0.3rc2/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/access/submitter.py` & `gen3_tracker-0.0.3rc2/gen3_util/access/submitter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/buckets/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/buckets/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/buckets/lister.py` & `gen3_tracker-0.0.3rc2/gen3_util/buckets/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/common/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/config/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/config/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/config/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/lister.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/manifest.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/manifest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/middleware.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/middleware.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/remover.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/files/uploader.py` & `gen3_tracker-0.0.3rc2/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/jobs/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/jobs/lister.py` & `gen3_tracker-0.0.3rc2/gen3_util/jobs/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/bundler.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/bundler.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/delta.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/delta.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/differ.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/differ.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/importer.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/lister.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/publisher.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/publisher.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/skeleton.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/skeleton.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/tabular/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/uploader.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/meta/validator.py` & `gen3_tracker-0.0.3rc2/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/projects/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/projects/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/projects/lister.py` & `gen3_tracker-0.0.3rc2/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/projects/remover.py` & `gen3_tracker-0.0.3rc2/gen3_util/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/__init__.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/cloner.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/cloner.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/committer.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/committer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/initializer.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/initializer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/puller.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/puller.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/pusher.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/pusher.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/repo/status.py` & `gen3_tracker-0.0.3rc2/gen3_util/repo/status.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/gen3_util/users/cli.py` & `gen3_tracker-0.0.3rc2/gen3_util/users/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,21 +19,26 @@
 @click.option('--username', default=None, show_default=True,
               help="Email of user", required=True)
 @click.option('--write/--no-write', '-w', help='Give user write privileges', is_flag=True, default=False, show_default=True)
 @click.option('--delete/--no-delete', '-d', help='Give user delete privileges', is_flag=True, default=False, show_default=True)
 @click.pass_obj
 def project_add_user(config: Config, username: str, project_id: str, write: bool, delete: bool):
     """Add user to project."""
+    if not project_id:
+        project_id = config.gen3.project_id
+
     with CLIOutput(config=config) as output:
         output.update(add_user(config, project_id, username, write, delete))
 
 
 @users_group.command(name="rm")
 @click.option('--project_id', default=None, show_default=True,
               help="Gen3 program-project", envvar=f"{ENV_VARIABLE_PREFIX}PROJECT_ID")
 @click.option('--username', default=None, show_default=True,
               help="Email of user", required=True)
 @click.pass_obj
 def project_rm_user(config: Config, username: str, project_id: str):
     """Remove user from project."""
+    if not project_id:
+        project_id = config.gen3.project_id
     with CLIOutput(config=config) as output:
         output.update(rm_user(config, project_id, username))
```

### Comparing `gen3_tracker-0.0.3rc1/setup.py` & `gen3_tracker-0.0.3rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_tracker',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.3rc1',  # Required
+    version='0.0.3rc2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/conftest.py` & `gen3_tracker-0.0.3rc2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/test_access.py` & `gen3_tracker-0.0.3rc2/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/test_commit.py` & `gen3_tracker-0.0.3rc2/tests/integration/test_commit.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/test_init.py` & `gen3_tracker-0.0.3rc2/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/test_meta.py` & `gen3_tracker-0.0.3rc2/tests/integration/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/test_meta_skeleton.py` & `gen3_tracker-0.0.3rc2/tests/integration/test_meta_skeleton.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/integration/test_project.py` & `gen3_tracker-0.0.3rc2/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/plugins/gen3_util_plugin_foo/__init__.py` & `gen3_tracker-0.0.3rc2/tests/unit/plugins/gen3_util_plugin_foo/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/conftest.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/conftest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/test_config.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/test_default_columns.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/test_default_columns.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/test_dir_to_tabular.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/test_dir_to_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/test_from_tabular.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/test_from_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/test_to_tabular.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/test_to_tabular.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/tabular/test_validate.py` & `gen3_tracker-0.0.3rc2/tests/unit/tabular/test_validate.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_cli.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_coding.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_coding.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_coding_conventions.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_config.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_files.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_manifest.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_validate_directory.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.3rc1/tests/unit/test_version.py` & `gen3_tracker-0.0.3rc2/tests/unit/test_version.py`

 * *Files identical despite different names*

