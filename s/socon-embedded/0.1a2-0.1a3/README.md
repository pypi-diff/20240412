# Comparing `tmp/socon-embedded-0.1a2.tar.gz` & `tmp/socon-embedded-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socon-embedded-0.1a2.tar", last modified: Thu Jan 25 15:52:13 2024, max compression
+gzip compressed data, was "socon-embedded-0.1a3.tar", last modified: Fri Apr 12 09:06:54 2024, max compression
```

## Comparing `socon-embedded-0.1a2.tar` & `socon-embedded-0.1a3.tar`

### file list

```diff
@@ -1,72 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.954434 socon-embedded-0.1a2/
--rw-rw-rw-   0        0        0      986 2023-07-27 15:39:35.000000 socon-embedded-0.1a2/.gitignore
--rw-rw-rw-   0        0        0      127 2023-07-14 08:31:36.000000 socon-embedded-0.1a2/AUTHORS
--rw-rw-rw-   0        0        0     5352 2023-07-14 08:31:36.000000 socon-embedded-0.1a2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     1556 2023-07-14 08:31:36.000000 socon-embedded-0.1a2/LICENSE
--rw-rw-rw-   0        0        0     1767 2024-01-25 15:52:13.952432 socon-embedded-0.1a2/PKG-INFO
--rw-rw-rw-   0        0        0      670 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/README.rst
--rw-rw-rw-   0        0        0        0 2023-07-13 15:45:21.000000 socon-embedded-0.1a2/__init__.py
--rw-rw-rw-   0        0        0      128 2023-07-14 08:31:36.000000 socon-embedded-0.1a2/plugins.py
--rw-rw-rw-   0        0        0     1286 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/pyproject.toml
--rw-rw-rw-   0        0        0       98 2024-01-25 15:49:53.000000 socon-embedded-0.1a2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-01-25 15:52:13.954434 socon-embedded-0.1a2/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-07-14 08:31:36.000000 socon-embedded-0.1a2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.641641 socon-embedded-0.1a2/socon_embedded/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a2/socon_embedded/__init__.py
--rw-rw-rw-   0        0        0      424 2024-01-25 15:52:13.000000 socon-embedded-0.1a2/socon_embedded/_version.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.688582 socon-embedded-0.1a2/socon_embedded/apps/
--rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/socon_embedded/apps/__init__.py
--rw-rw-rw-   0        0        0     8519 2023-11-24 09:01:36.000000 socon-embedded-0.1a2/socon_embedded/apps/executor.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.721938 socon-embedded-0.1a2/socon_embedded/builder/
--rw-rw-rw-   0        0        0    10397 2023-11-24 08:04:25.000000 socon-embedded-0.1a2/socon_embedded/builder/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-08-09 17:55:43.000000 socon-embedded-0.1a2/socon_embedded/builder/parser.py
--rw-rw-rw-   0        0        0     1203 2023-08-10 13:33:57.000000 socon-embedded-0.1a2/socon_embedded/builder/result.py
--rw-rw-rw-   0        0        0      564 2023-08-08 10:14:56.000000 socon-embedded-0.1a2/socon_embedded/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.724904 socon-embedded-0.1a2/socon_embedded/management/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a2/socon_embedded/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.736106 socon-embedded-0.1a2/socon_embedded/management/commands/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:12.000000 socon-embedded-0.1a2/socon_embedded/management/commands/__init__.py
--rw-rw-rw-   0        0        0     7895 2023-11-24 09:39:41.000000 socon-embedded-0.1a2/socon_embedded/management/commands/build.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.749068 socon-embedded-0.1a2/socon_embedded/management/commands/subcommands/
--rw-rw-rw-   0        0        0        0 2023-08-08 10:14:56.000000 socon-embedded-0.1a2/socon_embedded/management/commands/subcommands/__init__.py
--rw-rw-rw-   0        0        0     1946 2023-11-24 09:01:51.000000 socon-embedded-0.1a2/socon_embedded/management/commands/subcommands/from_file.py
--rw-rw-rw-   0        0        0     1683 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/socon_embedded/managers.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.778365 socon-embedded-0.1a2/socon_embedded/schema/
--rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon-embedded-0.1a2/socon_embedded/schema/__init__.py
--rw-rw-rw-   0        0        0     8881 2023-11-24 08:54:01.000000 socon-embedded-0.1a2/socon_embedded/schema/apps.py
--rw-rw-rw-   0        0        0      736 2023-08-08 10:14:56.000000 socon-embedded-0.1a2/socon_embedded/schema/base.py
--rw-rw-rw-   0        0        0        0 2023-08-09 07:09:48.000000 socon-embedded-0.1a2/socon_embedded/schema/build.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.805659 socon-embedded-0.1a2/socon_embedded/schema/tasks/
--rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon-embedded-0.1a2/socon_embedded/schema/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.822805 socon-embedded-0.1a2/socon_embedded/schema/tasks/action/
--rw-rw-rw-   0        0        0      153 2023-08-10 14:36:42.000000 socon-embedded-0.1a2/socon_embedded/schema/tasks/action/__init__.py
--rw-rw-rw-   0        0        0      111 2023-08-10 15:30:39.000000 socon-embedded-0.1a2/socon_embedded/schema/tasks/action/copy.py
--rw-rw-rw-   0        0        0      826 2023-08-10 14:24:58.000000 socon-embedded-0.1a2/socon_embedded/schema/tasks/executor.py
--rw-rw-rw-   0        0        0     3157 2023-08-09 09:23:30.000000 socon-embedded-0.1a2/socon_embedded/schema/tasks/task.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.867159 socon-embedded-0.1a2/socon_embedded/utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a2/socon_embedded/utils/__init__.py
--rw-rw-rw-   0        0        0     1452 2023-07-27 15:38:12.000000 socon-embedded-0.1a2/socon_embedded/utils/converter.py
--rw-rw-rw-   0        0        0      493 2023-07-27 15:38:12.000000 socon-embedded-0.1a2/socon_embedded/utils/jinja.py
--rw-rw-rw-   0        0        0     1773 2023-08-08 10:14:56.000000 socon-embedded-0.1a2/socon_embedded/utils/loader.py
--rw-rw-rw-   0        0        0     2192 2023-07-27 15:38:12.000000 socon-embedded-0.1a2/socon_embedded/utils/parser.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.951430 socon-embedded-0.1a2/socon_embedded.egg-info/
--rw-rw-rw-   0        0        0     1767 2024-01-25 15:52:13.000000 socon-embedded-0.1a2/socon_embedded.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1565 2024-01-25 15:52:13.000000 socon-embedded-0.1a2/socon_embedded.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 15:52:13.000000 socon-embedded-0.1a2/socon_embedded.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2024-01-25 15:52:13.000000 socon-embedded-0.1a2/socon_embedded.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-01-25 15:52:13.000000 socon-embedded-0.1a2/socon_embedded.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.912865 socon-embedded-0.1a2/tests/
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.921903 socon-embedded-0.1a2/tests/app_configs/
--rw-rw-rw-   0        0        0      383 2023-08-08 14:29:59.000000 socon-embedded-0.1a2/tests/app_configs/simple_app_config.yml
--rw-rw-rw-   0        0        0      287 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/tests/builder.py
--rw-rw-rw-   0        0        0      362 2023-07-27 15:39:35.000000 socon-embedded-0.1a2/tests/conftest.py
--rw-rw-rw-   0        0        0       77 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/tests/pytest.ini
--rw-rw-rw-   0        0        0       62 2023-07-14 08:31:36.000000 socon-embedded-0.1a2/tests/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.933002 socon-embedded-0.1a2/tests/schema/
--rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/tests/schema/__init__.py
--rw-rw-rw-   0        0        0     2050 2023-11-20 08:57:35.000000 socon-embedded-0.1a2/tests/schema/tests.py
--rw-rw-rw-   0        0        0      739 2023-08-10 12:58:45.000000 socon-embedded-0.1a2/tests/test_build.py
-drwxrwxrwx   0        0        0        0 2024-01-25 15:52:13.947469 socon-embedded-0.1a2/tests/utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 15:39:35.000000 socon-embedded-0.1a2/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     2275 2023-07-27 15:39:35.000000 socon-embedded-0.1a2/tests/utils/test_splitter.py
--rw-rw-rw-   0        0        0     1361 2023-07-27 15:39:35.000000 socon-embedded-0.1a2/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.563077 socon-embedded-0.1a3/
+-rw-rw-rw-   0        0        0      986 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/.gitignore
+-rw-rw-rw-   0        0        0      127 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/AUTHORS
+-rw-rw-rw-   0        0        0     5352 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0     1556 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/LICENSE
+-rw-rw-rw-   0        0        0     1767 2024-04-12 09:06:54.560061 socon-embedded-0.1a3/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/README.rst
+-rw-rw-rw-   0        0        0        0 2023-07-13 15:45:21.000000 socon-embedded-0.1a3/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/plugins.py
+-rw-rw-rw-   0        0        0     1286 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/pyproject.toml
+-rw-rw-rw-   0        0        0       98 2024-01-25 15:49:53.000000 socon-embedded-0.1a3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 09:06:54.564079 socon-embedded-0.1a3/setup.cfg
+-rw-rw-rw-   0        0        0       73 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.060394 socon-embedded-0.1a3/socon_embedded/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a3/socon_embedded/__init__.py
+-rw-rw-rw-   0        0        0      424 2024-04-12 09:06:52.000000 socon-embedded-0.1a3/socon_embedded/_version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.177153 socon-embedded-0.1a3/socon_embedded/action/
+-rw-rw-rw-   0        0        0      771 2024-04-11 12:13:38.000000 socon-embedded-0.1a3/socon_embedded/action/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-04-11 09:42:54.000000 socon-embedded-0.1a3/socon_embedded/action/call.py
+-rw-rw-rw-   0        0        0     2917 2024-04-11 09:41:05.000000 socon-embedded-0.1a3/socon_embedded/action/copy.py
+-rw-rw-rw-   0        0        0      256 2024-04-11 09:44:01.000000 socon-embedded-0.1a3/socon_embedded/action/move.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.192909 socon-embedded-0.1a3/socon_embedded/builder/
+-rw-rw-rw-   0        0        0    10354 2024-04-11 13:05:46.000000 socon-embedded-0.1a3/socon_embedded/builder/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-08-09 17:55:43.000000 socon-embedded-0.1a3/socon_embedded/builder/parser.py
+-rw-rw-rw-   0        0        0     1203 2023-08-10 13:33:57.000000 socon-embedded-0.1a3/socon_embedded/builder/result.py
+-rw-rw-rw-   0        0        0      564 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.214996 socon-embedded-0.1a3/socon_embedded/executor/
+-rw-rw-rw-   0        0        0        0 2024-04-11 11:55:38.000000 socon-embedded-0.1a3/socon_embedded/executor/__init__.py
+-rw-rw-rw-   0        0        0    10090 2024-04-11 13:37:06.000000 socon-embedded-0.1a3/socon_embedded/executor/app_executor.py
+-rw-rw-rw-   0        0        0     4370 2024-04-11 13:38:20.000000 socon-embedded-0.1a3/socon_embedded/executor/task_executor.py
+-rw-rw-rw-   0        0        0      818 2024-04-11 12:15:08.000000 socon-embedded-0.1a3/socon_embedded/executor/task_result.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.219715 socon-embedded-0.1a3/socon_embedded/management/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a3/socon_embedded/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.230012 socon-embedded-0.1a3/socon_embedded/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:12.000000 socon-embedded-0.1a3/socon_embedded/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     7842 2024-04-11 13:07:03.000000 socon-embedded-0.1a3/socon_embedded/management/commands/build.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.241254 socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/
+-rw-rw-rw-   0        0        0        0 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/__init__.py
+-rw-rw-rw-   0        0        0     1956 2024-04-11 12:47:56.000000 socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/from_file.py
+-rw-rw-rw-   0        0        0     2950 2024-04-12 07:54:43.000000 socon-embedded-0.1a3/socon_embedded/managers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.260404 socon-embedded-0.1a3/socon_embedded/schema/
+-rw-rw-rw-   0        0        0        0 2023-08-07 08:27:21.000000 socon-embedded-0.1a3/socon_embedded/schema/__init__.py
+-rw-rw-rw-   0        0        0     8498 2024-04-11 12:13:57.000000 socon-embedded-0.1a3/socon_embedded/schema/apps.py
+-rw-rw-rw-   0        0        0      736 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/schema/base.py
+-rw-rw-rw-   0        0        0     3734 2024-04-12 09:00:31.000000 socon-embedded-0.1a3/socon_embedded/schema/task.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.287245 socon-embedded-0.1a3/socon_embedded/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:38:11.000000 socon-embedded-0.1a3/socon_embedded/utils/__init__.py
+-rw-rw-rw-   0        0        0     2523 2024-04-04 12:31:10.000000 socon-embedded-0.1a3/socon_embedded/utils/converter.py
+-rw-rw-rw-   0        0        0      493 2023-07-27 15:38:12.000000 socon-embedded-0.1a3/socon_embedded/utils/jinja.py
+-rw-rw-rw-   0        0        0     1773 2023-08-08 10:14:56.000000 socon-embedded-0.1a3/socon_embedded/utils/loader.py
+-rw-rw-rw-   0        0        0     2192 2023-07-27 15:38:12.000000 socon-embedded-0.1a3/socon_embedded/utils/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.553450 socon-embedded-0.1a3/socon_embedded.egg-info/
+-rw-rw-rw-   0        0        0     1767 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2529 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 09:06:53.000000 socon-embedded-0.1a3/socon_embedded.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.307933 socon-embedded-0.1a3/tests/
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.345221 socon-embedded-0.1a3/tests/action/
+-rw-rw-rw-   0        0        0      267 2024-04-11 12:46:08.000000 socon-embedded-0.1a3/tests/action/__init__.py
+-rw-rw-rw-   0        0        0      720 2024-04-11 12:45:24.000000 socon-embedded-0.1a3/tests/action/test_call_command.py
+-rw-rw-rw-   0        0        0     1755 2024-04-11 12:44:43.000000 socon-embedded-0.1a3/tests/action/test_copy.py
+-rw-rw-rw-   0        0        0      626 2024-04-12 08:59:07.000000 socon-embedded-0.1a3/tests/action/test_discover.py
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:45:29.000000 socon-embedded-0.1a3/tests/action/test_move.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.365882 socon-embedded-0.1a3/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:32:35.000000 socon-embedded-0.1a3/tests/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.380365 socon-embedded-0.1a3/tests/commands/datafixtures/
+-rw-rw-rw-   0        0        0      397 2024-04-11 13:02:05.000000 socon-embedded-0.1a3/tests/commands/datafixtures/simple_app_config.yml
+-rw-rw-rw-   0        0        0      493 2024-04-11 13:02:22.000000 socon-embedded-0.1a3/tests/commands/datafixtures/simple_app_with_task.yml
+-rw-rw-rw-   0        0        0      370 2024-04-11 12:36:04.000000 socon-embedded-0.1a3/tests/commands/test_build_command.py
+-rw-rw-rw-   0        0        0      439 2024-04-12 08:53:56.000000 socon-embedded-0.1a3/tests/commands/test_from_file.py
+-rw-rw-rw-   0        0        0      330 2024-04-12 08:52:00.000000 socon-embedded-0.1a3/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.404499 socon-embedded-0.1a3/tests/executor/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:18:37.000000 socon-embedded-0.1a3/tests/executor/__init__.py
+-rw-rw-rw-   0        0        0       72 2024-04-11 12:28:37.000000 socon-embedded-0.1a3/tests/executor/test_task_executor.py
+-rw-rw-rw-   0        0        0      580 2024-04-11 12:23:44.000000 socon-embedded-0.1a3/tests/executor/test_task_result.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.416931 socon-embedded-0.1a3/tests/management/
+-rw-rw-rw-   0        0        0        0 2024-04-11 12:58:57.000000 socon-embedded-0.1a3/tests/management/__init__.py
+-rw-rw-rw-   0        0        0       33 2024-04-11 12:59:16.000000 socon-embedded-0.1a3/tests/management/config.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.426288 socon-embedded-0.1a3/tests/projects/
+-rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon-embedded-0.1a3/tests/projects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.457763 socon-embedded-0.1a3/tests/projects/test_project/
+-rw-rw-rw-   0        0        0        0 2024-04-12 08:47:26.000000 socon-embedded-0.1a3/tests/projects/test_project/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-04-12 08:56:26.000000 socon-embedded-0.1a3/tests/projects/test_project/action.py
+-rw-rw-rw-   0        0        0      287 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/projects/test_project/builder.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.464141 socon-embedded-0.1a3/tests/projects/test_project/management/
+-rw-rw-rw-   0        0        0       33 2024-04-12 08:51:00.000000 socon-embedded-0.1a3/tests/projects/test_project/management/config.py
+-rw-rw-rw-   0        0        0      171 2024-04-12 08:51:38.000000 socon-embedded-0.1a3/tests/projects/test_project/projects.py
+-rw-rw-rw-   0        0        0       77 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/pytest.ini
+-rw-rw-rw-   0        0        0       62 2023-07-14 08:31:36.000000 socon-embedded-0.1a3/tests/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.486348 socon-embedded-0.1a3/tests/schema/
+-rw-rw-rw-   0        0        0        0 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/schema/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.533233 socon-embedded-0.1a3/tests/schema/datafixtures/
+-rw-rw-rw-   0        0        0       80 2024-04-04 13:07:32.000000 socon-embedded-0.1a3/tests/schema/datafixtures/action_extra_args.yml
+-rw-rw-rw-   0        0        0       47 2024-04-02 13:14:24.000000 socon-embedded-0.1a3/tests/schema/datafixtures/bad_action.yml
+-rw-rw-rw-   0        0        0       59 2024-04-02 13:13:17.000000 socon-embedded-0.1a3/tests/schema/datafixtures/copy_schema.yml
+-rw-rw-rw-   0        0        0       91 2024-04-02 15:27:00.000000 socon-embedded-0.1a3/tests/schema/datafixtures/multiple_valid_action.yml
+-rw-rw-rw-   0        0        0       19 2024-04-02 15:22:54.000000 socon-embedded-0.1a3/tests/schema/datafixtures/no_action.yml
+-rw-rw-rw-   0        0        0       77 2024-04-02 13:15:18.000000 socon-embedded-0.1a3/tests/schema/datafixtures/set_action.yml
+-rw-rw-rw-   0        0        0     2050 2023-11-20 08:57:35.000000 socon-embedded-0.1a3/tests/schema/test_app_registry.py
+-rw-rw-rw-   0        0        0     2652 2024-04-11 12:14:54.000000 socon-embedded-0.1a3/tests/schema/test_tasks.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:06:54.545081 socon-embedded-0.1a3/tests/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     2275 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/tests/utils/test_splitter.py
+-rw-rw-rw-   0        0        0     1361 2023-07-27 15:39:35.000000 socon-embedded-0.1a3/tox.ini
```

### Comparing `socon-embedded-0.1a2/.gitignore` & `socon-embedded-0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/CODE_OF_CONDUCT.md` & `socon-embedded-0.1a3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/LICENSE` & `socon-embedded-0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/PKG-INFO` & `socon-embedded-0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socon-embedded
-Version: 0.1a2
+Version: 0.1a3
 Summary: Build/Flash tool plugin for socon
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/socon-dev/socon-embedded
 Keywords: build,flasH,embedded,socon
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `socon-embedded-0.1a2/README.rst` & `socon-embedded-0.1a3/README.rst`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/pyproject.toml` & `socon-embedded-0.1a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded/apps/executor.py` & `socon-embedded-0.1a3/socon_embedded/executor/app_executor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,33 @@
 import os
 from pathlib import Path
 import shutil
 
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, Union
 
 from socon_embedded.builder.result import BuildResult, Result, Status
 from socon_embedded.managers import BuilderManager
-from socon_embedded.schema.apps import AppRegistry
+from socon_embedded.schema.apps import AppRegistry, BuildConfig, AppConfig
 from socon_embedded.builder import BuildInfo, Builder
-from socon_embedded.schema.tasks.executor import Executor, TaskExecutor
-from socon_embedded.schema.tasks.task import Task
+from socon_embedded.executor.task_executor import TaskPlayer
 
 from socon.core.registry import projects
 from socon.core.registry.config import ProjectConfig
 from socon.utils.terminal import terminal
 
 from junitparser import JUnitXml, TestCase, TestSuite, Failure, Skipped
 
 
-def execute_tasks(tasks: List[Task]) -> None:
-    """
-    Execute a task. Exit on any exception and clean the task.
-    """
-    for task in tasks:
-        tsx = TaskExecutor(task)
-        tsx.run()
-
-
-class AppRegistryExecutor(Executor):
+class AppRegistryExecutor:
 
     def __init__(
         self,
         app_registry: AppRegistry,
         builder_manager: BuilderManager,
-        project_config: ProjectConfig = None
+        project_config: ProjectConfig = None,
     ) -> None:
         self._app_registry = app_registry
         self._builder_manager = builder_manager
         self._project_config = project_config
 
         # Load the project config if none are given
         if self._project_config is None:
@@ -66,15 +56,15 @@
         self,
         filters: Dict[str, Any] = {},
         excludes: Dict[str, Any] = {},
         variant_args_filters: Dict[str, Any] = {},
         output_dir: Union[str, os.PathLike] = None,
         exit_on_error: bool = False,
         warning_as_error: bool = False,
-    ):
+    ) -> AppRegistry:
         """Build the application in each registries based on the given filters"""
         self._clear_cache()
 
         # Re-define output_dir if not given
         output_dir = self._get_output_dir(output_dir)
 
         # Create a build section
@@ -89,27 +79,41 @@
         # Raise a LookupError if we don't find any build configuration
         if not reg.apps:
             raise LookupError(
                 "Nothing to build. You should check if you have registered your\n"
                 "applications or if your filters are correct."
             )
 
+        self.pre_build(reg)
+
         # Stop building in case exit_on_error is True and an issue was found.
         # This flag allow to still create a report with the rest of the application
         # set as skipped
         stop_building = False
 
+        # Run the general tasks in priority
+        task_player = TaskPlayer()
+        task_player.run(reg.tasks)
+
         # Build each build configuration
         for app_config in reg.apps:
 
+            # Run the Application config tasks
+            task_player.run(app_config.tasks)
+
+            self.post_process_app_config(app_config)
+
             # Get all build configuration for each application
             build_configs = app_config.get_build_configs(variant_args_filters)
 
             for build_config in build_configs:
 
+                # Run the build config tasks
+                task_player.run(build_config.tasks)
+
                 # Create a build info object
                 build_info = build_config.create_buildinfo()
 
                 # If stop building is True, we still create result with skipped
                 # status and the build info
                 if stop_building is True:
                     result = BuildResult(
@@ -118,69 +122,106 @@
                     result.build_info = build_info
                     self._build_results.append(result)
                     continue
 
                 # Create the artifact directory
                 artifact_path = self._create_artifact_directory(build_info, output_dir)
 
+                self.pre_build_config(build_config)
+
                 # Build the application
                 builder = self._get_builder(build_config.builder.name)
                 result = builder.build(
                     **build_config.get_buildinfo(),
                     output_file=Path(artifact_path, f"{build_info.app}.log"),
                     warning_as_error=warning_as_error,
-                    vars=self._app_registry.vars
+                    variables=self._app_registry.vars,
                 )
 
+                self.post_build_config(build_config, result)
+
                 # Save the fail result of the current apps
                 self._build_results.append(result)
 
                 # In case we need to exit on error. We need to stop the build
                 # of all application but still put the next application that
                 # were not build as skipped for the junit report.
                 if result.is_fail and exit_on_error is True:
                     stop_building = True
 
+                # Run the post build configs only if we decided not to stop
+                # building.
+                task_player.run(build_config.post_tasks)
+
+            # Run the post application config tasks
+            task_player.run(app_config.post_tasks)
+
+        task_player.run(reg.post_tasks)
+
+        # Call the post_build method for the user
+        self.post_build(reg, output_dir)
+
+        # Clean all the tasks at the end
+        task_player.cleanup()
+
+        return reg
+
+    def pre_build(self, registry: AppRegistry):
+        """Pre build method with the filtered application registry"""
+
+    def post_build(self, registry: AppRegistry, output_dir: str):
+        """Post build method with the filtered application registry"""
+
+    def pre_build_config(self, build_config: BuildConfig):
+        """Pre build config method with the configuration of the build"""
+
+    def post_build_config(self, build_config: BuildConfig, result: Result):
+        """Post build config method started after the build"""
+
+    def post_process_app_config(self, app_config: AppConfig):
+        """Post processing the application config"""
+
     def _get_output_dir(self, output_dir: str = None) -> str:
         output_dir = output_dir if output_dir else os.getcwd()
         return Path(output_dir, self._app_registry.name)
 
     def _create_artifact_directory(
-        self,
-        build_info: BuildInfo,
-        output_dir: str,
-        clean: bool = False
+        self, build_info: BuildInfo, output_dir: str, clean: bool = False
     ):
         """
         Save the output in an artifact directory at the current location or
         inside the specified output directory.
         If clean = True, the directory will be cleaned
         """
-        artifact_path = list(filter(None, [
-            output_dir, build_info.builder, build_info.app,
-            "_".join(sorted(build_info.variant_args.values()))
-        ]))
+        artifact_path = list(
+            filter(
+                None,
+                [
+                    output_dir,
+                    build_info.builder,
+                    build_info.app,
+                    "_".join(sorted(build_info.variant_args.values())),
+                ],
+            )
+        )
         artifact_path = Path().joinpath(*artifact_path)
 
         # In case the result folder does not exist, we create it. In case the
         # clean options is set, we remove and recreate the folder.
         if artifact_path.is_dir():
             if clean:
                 shutil.rmtree(artifact_path)
                 os.mkdir(artifact_path)
         else:
             os.makedirs(artifact_path, exist_ok=True)
 
         return artifact_path
 
     def create_report(
-        self,
-        output_file: str,
-        output_dir: str = None,
-        add_skipped_apps: bool = True
+        self, output_file: str, output_dir: str = None, add_skipped_apps: bool = True
     ) -> None:
         """Create junit report from buidled and skipped apps"""
         output_dir = self._get_output_dir(output_dir)
         junit_file = Path(output_dir) / output_file
 
         # Create the Junit object
         junit = JUnitXml()
@@ -218,12 +259,14 @@
         return junit
 
     def _get_builder(self, name: str) -> Builder:
         """Get the builder in cache or via the manager"""
         if name in self._cached_builders:
             builder = self._cached_builders.get(name)
         else:
-            builder_klass = self._builder_manager.search_hook_impl(name, self._project_config)
+            builder_klass = self._builder_manager.search_hook_impl(
+                name, self._project_config
+            )
             builder = builder_klass()
             self._cached_builders[name] = builder
 
         return builder
```

### Comparing `socon-embedded-0.1a2/socon_embedded/builder/__init__.py` & `socon-embedded-0.1a3/socon_embedded/builder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,39 +36,36 @@
             self._cmd, self._cause, self._cmdline
         )
 
 
 @dataclass
 class BuildInfo:
     """Store building information"""
+
     app: str
     builder: str
     project_file: str
     variant_args: dict = field(default_factory=dict)
     cmdline: list = field(default_factory=list)
 
     def __str__(self) -> str:
         output = [
             f"Application: {self.app}",
             f"Input file: {self.project_file}",
-            f"Builder: {self.builder}"
+            f"Builder: {self.builder}",
         ]
         variant_args = self.variant_args
         if variant_args:
             for key, value in variant_args.items():
                 output.append(f"{key.title()}: {value}")
         return "\n".join(output)
 
     def get_case_name(self) -> str:
         """Get the testcase name that will be used in the junit report"""
-        return " - ".join([
-            self.app,
-            self.builder,
-            *self.variant_args.values()
-        ])
+        return " - ".join([self.app, self.builder, *self.variant_args.values()])
 
 
 class Builder(Hook, abstract=True):
     """Base class for toolchain or compiler"""
 
     manager = "builder"
 
@@ -77,15 +74,15 @@
 
     # If True, a shell will be used when executing git commands.
     use_shell = False
 
     def __init__(
         self,
         name: Optional[str] = None,
-        executable: Optional[Union[str, os.PathLike]] = None
+        executable: Optional[Union[str, os.PathLike]] = None,
     ) -> None:
         self.name = name or getattr(self, "name", self.__class__.__name__)
         self.executable = executable or self.get_executable()
         if not self.executable:
             raise AttributeError(
                 "'executable' attribute is required by '{}'".format(self.name)
             )
@@ -103,15 +100,15 @@
         app: str,
         project_file: Union[str, os.PathLike],
         variant_args: dict = {},
         raw_args: list[str] = [],
         warning_as_error: bool = False,
         output_file: Union[str, os.PathLike] = None,
         clean: bool = False,
-        vars: dict = {},
+        variables: dict = {},
         **kwargs: Any,
     ) -> BuildResult:
         """
         Compile an application using the input path, the specified mode and arguments
         """
         main_args = self.get_main_args(project_file, **variant_args)
         if isinstance(main_args, str):
@@ -145,32 +142,30 @@
 
         # Create the build info object
         buildinfo = BuildInfo(
             app=app,
             builder=self.name,
             project_file=project_file,
             cmdline=cmdline,
-            variant_args=variant_args
+            variant_args=variant_args,
         )
         self.display_build_info(buildinfo)
 
         # Run pre_build method if required
-        self.pre_build(buildinfo, **vars)
+        self.pre_build(buildinfo, **variables)
 
         # Get an approximation build time execution
         time_started = time.time()
 
         # Build the application. In case the command is not found, we catch
         # the exception and make a result out of it.
         try:
             status_code, output = self.execute(cmdline, **kwargs)
         except BuildCommandNotFound as e:
-            build_result = BuildResult(
-                Result(Status.FAILURE, str(e)), str(e)
-            )
+            build_result = BuildResult(Result(Status.FAILURE, str(e)), str(e))
         else:
             # Get the execution time of the build
             execution_time = time.time() - time_started
 
             # Load the parser, parse and interpret the results
             parser = self.parser(warning_as_error)
             build_result = parser.execute(status_code, output)
@@ -180,51 +175,50 @@
         build_result.build_info = buildinfo
 
         # Display the result. Let the user re-define that if wanted
         self.display_result(build_result)
 
         # Save the log into the artifact path
         if output_file:
-            with open(output_file, 'w+') as f:
+            with open(output_file, "w+") as f:
                 f.write(build_result.output)
 
         # call the post_build method
         output_dir = Path(output_file).parent
-        self.post_build(build_result, output_dir, **vars)
+        self.post_build(build_result, output_dir, **variables)
 
         return build_result
 
     @abstractmethod
     def get_main_args(
         self, project_file: Union[str, os.PathLike], **variant_args
     ) -> list[str]:
         """Return the main command line argument for the builder"""
         pass
 
     def execute(
-        self, commands: list[str],
-        **subprocess_args: Any
+        self, commands: list[str], **subprocess_args: Any
     ) -> Tuple[int, Union[str, bytes], str]:
         return self._execute(commands, **subprocess_args)
 
     def display_result(self, build_result: BuildResult) -> None:
         """Display build result"""
         status_msg = build_result.get_status_message()
         color = "green"
         if build_result.is_fail:
             color = "red"
         if build_result.result.message:
             terminal.line(build_result.result.message)
         terminal.line(f"Result: {status_msg}\n", fg=color)
 
-    def pre_build(self, build_info: BuildInfo, **vars):
+    def pre_build(self, build_info: BuildInfo, **variables):
         """Method executed just before the build execution"""
         pass
 
-    def post_build(self, result: BuildResult, **vars):
+    def post_build(self, result: BuildResult, output_dir: str, **variables):
         """Method executed after the build execution"""
         pass
 
     def display_build_info(self, buildinfo: BuildInfo) -> None:
         terminal.line(str(buildinfo))
 
     def _execute(
@@ -266,15 +260,15 @@
             process = subprocess.Popen(
                 command,
                 shell=shell is not None and shell or self.use_shell,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 universal_newlines=True,
-                **subprocess_kwargs
+                **subprocess_kwargs,
             )
 
             if silent is True:
                 print("Building...")
 
             # Display realtime output and save it
             logger.debug("Command generated following output: ")
```

### Comparing `socon-embedded-0.1a2/socon_embedded/builder/parser.py` & `socon-embedded-0.1a3/socon_embedded/builder/parser.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded/builder/result.py` & `socon-embedded-0.1a3/socon_embedded/builder/result.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded/exceptions.py` & `socon-embedded-0.1a3/socon_embedded/exceptions.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded/management/commands/build.py` & `socon-embedded-0.1a3/socon_embedded/management/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         parser.add_argument(
             "--variant-args",
             help=(
                 "Filter a build variant args configiration. "
                 "Like a mode variant configuration. "
                 'Example: --variant-args "mode=release"'
             ),
-            action="append"
+            action="append",
         )
         parser.add_argument(
             "--extras-vars",
             help=(
                 "Set variables as key=value or YAML/JSON, if filename prepend with @. "
                 'Example: --set-vars "fruit=apple", --set-vars "@file.yml"'
             ),
@@ -77,18 +77,16 @@
             help="Exit if there is an error",
             action="store_true",
         )
         parser.add_argument(
             "--wae", "--warning-as-error", help="Treat a warning as an error"
         )
         parser.add_argument(
-            "--artifact-dir", help=(
-                "Path to the artifact folder that will store "
-                "the build artifacts"
-            )
+            "--artifact-dir",
+            help=("Path to the artifact folder that will store " "the build artifacts"),
         )
         self.add_build_arguments(parser)
 
     def add_build_arguments(self, parser: ArgumentParser) -> None:
         """Add more arguments to the base build arguments"""
         pass
 
@@ -99,24 +97,22 @@
         extras_vars = self.load_template_args(config.getoption("extras_vars", []))
         variant_args = self.load_template_args(config.getoption("variant_args", []))
 
         # Merge the extras filters with the default one passed on the command line
         filters_opt = self._create_filter(
             ("name__in", config.getoption("app")),
             ("group__in", config.getoption("group")),
-            ("builders__name__in", config.getoption("builder"))
+            ("builders__name__in", config.getoption("builder")),
         )
         filters = filters | filters_opt
 
         # Create the variant config filter
         variant_args_filters = {}
         for var_config, value in variant_args.items():
-            variant_args_filters.update(
-                {f"variant_args__{var_config}": value}
-            )
+            variant_args_filters.update({f"variant_args__{var_config}": value})
 
         # Create a context based on the extras vars and the base directory. This
         # will be mainly use to resolve any further jinja template file
         base_dir = config.getoption("base_dir")
         context = extras_vars
         if base_dir is not None:
             context.update({"base_dir": base_dir})
@@ -146,41 +142,41 @@
             project_config=project_config,
             filters=filters,
             excludes=excludes,
             variant_args_filters=variant_args_filters,
             exit_on_error=eoe,
             context=context,
             warning_as_error=wae,
-            artifact_dir=artifact_dir
+            artifact_dir=artifact_dir,
         )
 
     def handle_build(
         self,
         config: Config,
         project_config: ProjectConfig,
         filters: dict = {},
         excludes: dict = {},
         variant_args_filters: dict = {},
         context: dict = {},
         exit_on_error: bool = False,
         warning_as_error: bool = False,
-        artifact_dir: str = None
+        artifact_dir: str = None,
     ) -> str:
         raise NotImplementedError(
             "Subclass of '{}' must implement handle_build(...) method".format(
                 self.__class__.__name__
             )
         )
 
     @staticmethod
-    def load_template_args(vars: list[Any] = tuple()) -> Dict[str, str]:
+    def load_template_args(variables: list[Any] = tuple()) -> Dict[str, str]:
         """Load vars passed in command line arguments"""
         loaded_vars = {}
 
-        for var_opt in vars:
+        for var_opt in variables:
             data = None
             var_opt = to_text(var_opt)
             if var_opt is None or not var_opt:
                 continue
             if var_opt.startswith("@"):
                 # Argument is a YAML file (JSON is a subset of YAML)
                 data = load_from_file(var_opt[1:])
```

### Comparing `socon-embedded-0.1a2/socon_embedded/management/commands/subcommands/from_file.py` & `socon-embedded-0.1a3/socon_embedded/management/commands/subcommands/from_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argparse import ArgumentParser
 from pathlib import Path
 
-from socon_embedded.apps.executor import AppRegistryExecutor
+from socon_embedded.executor.app_executor import AppRegistryExecutor
 from socon_embedded.management.commands.build import BuildCommandInterface
 
 from socon.core.management.base import Config
 from socon.core.registry.config import ProjectConfig
 
 from socon_embedded.managers import get_builder_manager
 
@@ -38,22 +38,22 @@
 
         # Create the RegistryExecutor that will handle the execution of
         # all registries
         regexec = AppRegistryExecutor.from_file(
             app_registry,
             context=context,
             project_config=project_config,
-            builder_manager=get_builder_manager()
+            builder_manager=get_builder_manager(),
         )
 
         # Build the application using the selected registry
         regexec.build(
             filters=filters,
             excludes=excludes,
             variant_args_filters=variant_args_filters,
             exit_on_error=exit_on_error,
             warning_as_error=warning_as_error,
-            output_dir=artifact_dir
+            output_dir=artifact_dir,
         )
 
         # Make a report at the root of the artifact directory
         regexec.create_report("results.xml", artifact_dir)
```

### Comparing `socon-embedded-0.1a2/socon_embedded/schema/apps.py` & `socon-embedded-0.1a3/socon_embedded/schema/apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 
 from typing import Dict, List, Optional, Union
 from socon_embedded.builder import BuildInfo
 
 from socon_embedded.exceptions import YamlFormatError, YamlParserError
 from socon_embedded.managers import get_builder_manager
-from socon_embedded.schema.tasks.task import Taskable
+from socon_embedded.schema.task import Taskable
 from socon_embedded.schema.base import Base, Nameable, get_field_names
 
 from pydantic import BaseModel, field_validator, model_validator
 
 from datalookup import Dataset
 
 
@@ -36,18 +36,15 @@
 
         # Re-create the AppConfig object for each filtered apps
         filtered_apps = []
         for app in apps:
             filtered_apps.append(AppConfig(**app.values()))
 
         # Return a new registry with the filtered apps
-        return AppRegistry(
-            **self.model_dump(exclude="apps"),
-            apps=filtered_apps
-        )
+        return AppRegistry(**self.model_dump(exclude="apps"), apps=filtered_apps)
 
     def _get_app(self, name: str) -> Optional[AppConfig]:
         """Get an application from the registry"""
         for app in self.apps:
             if name == app.name:
                 return app
         return None
@@ -86,16 +83,15 @@
         not_existing_builders = []
         for builder in self.builders:
             if builder.name not in builder_manager.get_hooks_name():
                 not_existing_builders.append(builder.name)
 
         if not_existing_builders:
             raise YamlParserError(
-                "Following builder(s) does not exist(s):\n"
-                f"{not_existing_builders}"
+                "Following builder(s) does not exist(s):\n" f"{not_existing_builders}"
             )
 
         return self
 
     @model_validator(mode="after")
     def validate_builder_ref(self):
         builders = [builder.name for builder in self.builders]
@@ -107,17 +103,15 @@
                         f"Reference to '{ref}' builder does not exist.\n"
                         f"Please check following variant:\n{variant}"
                     )
         return self
 
     @staticmethod
     def _get_build_configs(
-        app: str,
-        builder: AppBuilder,
-        filters: dict = {}
+        app: str, builder: AppBuilder, filters: dict = {}
     ) -> list[BuildConfig]:
         build_configs = []
 
         # If the user specified the configs entry, we need to create
         # multiple build configuration
         if builder.variant_args:
             keys, values = zip(*builder.variant_args.items())
@@ -126,48 +120,40 @@
             ]
             for variant in permutations_dicts:
                 config_builder = AppBuilder(
                     **builder.model_dump(exclude="variant_args"), variant_args=variant
                 )
                 app_dataset = Dataset(config_builder.model_dump())
                 if len(app_dataset.filter(**filters)) != 0:
-                    build_configs.append(
-                        BuildConfig(app=app, builder=config_builder)
-                    )
+                    build_configs.append(BuildConfig(app=app, builder=config_builder))
         else:
-            build_configs.append(
-                BuildConfig(app=app, builder=builder)
-            )
+            build_configs.append(BuildConfig(app=app, builder=builder))
 
         return build_configs
 
     def get_build_configs(self, filters: dict = {}) -> List[BuildConfig]:
         build_configs = []
         builders_ref: Dict[str, AppBuilder] = {}
 
         for builder in self.builders:
             # Save the builder reference for the variant
             if builder.name not in builders_ref:
                 builders_ref[builder.name] = builder
 
             # If the user specified the configs entry, we need to create
             # multiple build configuration
-            build_configs.extend(
-                self._get_build_configs(self.name, builder, filters)
-            )
+            build_configs.extend(self._get_build_configs(self.name, builder, filters))
 
         for variant in self.variants:
             app = self.name + f".{variant.name}"
             for vbuilder in variant.builders:
                 for ref in vbuilder.ref:
                     builder_ref = builders_ref[ref]
                     builder = builder_ref.merge_variant_builder(vbuilder)
-                    build_configs.extend(
-                        self._get_build_configs(app, builder, filters)
-                    )
+                    build_configs.extend(self._get_build_configs(app, builder, filters))
 
         return build_configs
 
     def _get_builder(self, name: str) -> Optional[AppBuilder]:
         for builder in self.builders:
             if name == builder.name:
                 return builder
@@ -196,28 +182,22 @@
     builder: AppBuilder
 
     def get_buildinfo(self) -> dict:
         return {
             "app": self.app,
             **self.builder.model_dump(
                 by_alias=True,
-                exclude=[
-                    *get_field_names(Taskable),
-                    *get_field_names(Nameable)
-                ]
-            )
+                exclude=[*get_field_names(Taskable), *get_field_names(Nameable)],
+            ),
         }
 
     def create_buildinfo(self) -> BuildInfo:
         build_info = self.get_buildinfo()
         build_info.pop("raw_args")
-        return BuildInfo(
-            builder=self.builder.name,
-            **build_info
-        )
+        return BuildInfo(builder=self.builder.name, **build_info)
 
 
 class Builder(Taskable):
     variant_args: Optional[Dict[str, Union[str, list]]] = {}
     raw_args: Optional[list] = []
 
 
@@ -230,18 +210,15 @@
 
         # Merge tasks from other to the current builder
         builder.merge_tasks(other, other.keep_tasks, "tasks")
         builder.merge_tasks(other, other.keep_post_tasks, "post_tasks")
 
         # Merge all remaining fields
         builder_dict = builder.model_dump() | other.model_dump(
-            exclude=[
-                *get_field_names(Taskable),
-                *get_field_names(VariantBuilderField)
-            ]
+            exclude=[*get_field_names(Taskable), *get_field_names(VariantBuilderField)]
         )
 
         return AppBuilder(**builder_dict)
 
 
 class VariantBuilderField(BaseModel):
     ref: Union[str, list]
```

### Comparing `socon-embedded-0.1a2/socon_embedded/schema/base.py` & `socon-embedded-0.1a3/socon_embedded/schema/base.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded/schema/tasks/task.py` & `socon-embedded-0.1a3/socon_embedded/schema/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,107 @@
 from __future__ import annotations
 
-from typing import List, Literal, Type
-from socon_embedded.exceptions import ParserError
+from typing import List, Literal, Optional, Type
+
+from socon.core.registry import projects
 
+from socon_embedded.exceptions import ParserError
+from socon_embedded.managers import get_action_manager
 from socon_embedded.schema.base import Base, Nameable, get_field_names
 
 from pydantic import BaseModel, Field, model_validator
 
 
 class Task(Base, Nameable):
     """Call a module (action) with specific arguments and other parameters"""
-    action: str
+
+    action: Type
     args: dict = {}
 
+    retries: Optional[int] = 0
+    timeout: Optional[int] = None
+
     @model_validator(mode="before")
+    @classmethod
     def preprocess_action(cls, values):
         action = None
         args = {}
 
-        if 'action' in values:
-            action = values['action']
-        if 'args' in values:
-            args = values['args']
+        if "action" in values:
+            action = values["action"]
+        if "args" in values:
+            args = values["args"]
 
         # filter out task attributes so we're only querying unrecognized keys as actions/modules
         non_task_values = dict(
-            (k, v) for k, v in values.items()
-            if (k not in get_field_names(Task))
+            (k, v) for k, v in values.items() if (k not in get_field_names(Task))
         )
 
         # walk the filtered input dictionary to see if we recognize a module name
+        action_manager = get_action_manager()
         for item, value in non_task_values.items():
             is_action_candidate = False
-            if item in ['copy', 'move']:
+            if item in action_manager.get_hooks_name():
                 is_action_candidate = True
 
             if is_action_candidate:
 
                 # finding more than one module name is a problem
                 if action is not None:
                     raise ParserError(
-                        "conflicting action statements: {}, {}".format(
-                            action, item
-                        )
+                        "conflicting action statements: {}, {}".format(action, item)
                     )
 
                 action = item
                 args = value
 
         # if we didn't see any module in the task at all, it's not a task really
         if action is None:
-            if non_task_values:  # there was one non-task action, but we couldn't find it
+            if (
+                non_task_values
+            ):  # there was one non-task action, but we couldn't find it
                 bad_action = list(non_task_values.keys())[0]
                 raise ParserError(
                     "couldn't resolve module/action '{0}'. This often indicates a "
                     "misspelling, missing collection, or "
-                    "incorrect module path.".format(bad_action))
-            else:
-                raise ParserError(
-                    "no module/action detected in task."
+                    "incorrect module path.".format(bad_action)
                 )
+            else:
+                raise ParserError("no module/action detected in task.")
+
+        try:
+            project_config = projects.get_project_config_by_env()
+        except LookupError:
+            project_config = None
+        action = action_manager.search_hook_impl(action, project_config)
 
         # Set the action if no previous error
-        values['action'] = action
-        values['args'] = args
+        values["action"] = action
+        values["args"] = args
         return values
 
+    @model_validator(mode="after")
+    def post_process_action(self):
+        """Validate the action schema"""
+        self.action = self.action(self)
+        return self
+
 
 class Taskable(BaseModel):
     """
     Make a schema taskable.
     Give the ability to have pre_tasks, post_tasks and tasks
     """
 
     # Tasks list attribute
     tasks: List[Task] = Field(default_factory=list)
     post_tasks: List[Task] = Field(default_factory=list)
 
     def merge_tasks(
-        self,
-        y: Type[Taskable],
-        keep: bool,
-        tasks_type: Literal["tasks", "post_tasks"]
+        self, y: Type[Taskable], keep: bool, tasks_type: Literal["tasks", "post_tasks"]
     ) -> Type[Taskable]:
         """Merge y tasks into x tasks"""
         if keep is False:
             setattr(self, tasks_type, getattr(y, tasks_type))
         else:
             for task in getattr(y, tasks_type):
                 if task not in getattr(self, tasks_type):
```

### Comparing `socon-embedded-0.1a2/socon_embedded/utils/converter.py` & `socon-embedded-0.1a3/socon_embedded/utils/converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -43,7 +43,40 @@
                 value = repr(obj)
             except UnicodeError:
                 return ""
     elif nonstring == "passthru":
         return obj
 
     return to_text(value, encoding)
+
+
+def to_bytes(obj: Union[str, bytes]):
+    """Make sure that a string is a byte string"""
+    if isinstance(obj, bytes):
+        return obj
+
+    original_errors = None
+    if isinstance(obj, str):
+        try:
+            # Try this first as it's the fastest
+            return obj.encode("utf-8")
+        except UnicodeEncodeError:
+            if original_errors in (None, "surrogate_then_replace"):
+                # We should only reach this if encoding was non-utf8 original_errors was
+                # surrogate_then_escape and errors was surrogateescape
+
+                # Slow but works
+                return_string = obj.encode("utf-8", "surrogateescape")
+                return_string = return_string.decode("utf-8", "replace")
+                return return_string.encode("utf-8", "replace")
+            raise
+
+    try:
+        value = str(obj)
+    except UnicodeError:
+        try:
+            value = repr(obj)
+        except UnicodeError:
+            # Giving up
+            return to_bytes("")
+
+    return to_bytes(value)
```

### Comparing `socon-embedded-0.1a2/socon_embedded/utils/loader.py` & `socon-embedded-0.1a3/socon_embedded/utils/loader.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded/utils/parser.py` & `socon-embedded-0.1a3/socon_embedded/utils/parser.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/socon_embedded.egg-info/PKG-INFO` & `socon-embedded-0.1a3/socon_embedded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socon-embedded
-Version: 0.1a2
+Version: 0.1a3
 Summary: Build/Flash tool plugin for socon
 Author-email: Stephane Capponi <stephane.capponi@proton.me>
 License: BSD-3-Clause
 Project-URL: repository, https://github.com/socon-dev/socon-embedded
 Keywords: build,flasH,embedded,socon
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `socon-embedded-0.1a2/tests/schema/tests.py` & `socon-embedded-0.1a3/tests/schema/test_app_registry.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/tests/utils/test_splitter.py` & `socon-embedded-0.1a3/tests/utils/test_splitter.py`

 * *Files identical despite different names*

### Comparing `socon-embedded-0.1a2/tox.ini` & `socon-embedded-0.1a3/tox.ini`

 * *Files identical despite different names*

