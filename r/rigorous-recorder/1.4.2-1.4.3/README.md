# Comparing `tmp/rigorous_recorder-1.4.2.tar.gz` & `tmp/rigorous_recorder-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigorous_recorder-1.4.2.tar", last modified: Sun May 28 15:55:05 2023, max compression
+gzip compressed data, was "rigorous_recorder-1.4.3.tar", last modified: Fri Apr 12 14:41:15 2024, max compression
```

## Comparing `rigorous_recorder-1.4.2.tar` & `rigorous_recorder-1.4.3.tar`

### file list

```diff
@@ -1,11 +1,555 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:55:05.492176 rigorous_recorder-1.4.2/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-28 15:55:05.492026 rigorous_recorder-1.4.2/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:55:05.490858 rigorous_recorder-1.4.2/rigorous_recorder/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    35674 2023-05-25 20:48:40.000000 rigorous_recorder-1.4.2/rigorous_recorder/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:55:05.491852 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     7504 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      202 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2023-05-28 15:55:05.000000 rigorous_recorder-1.4.2/rigorous_recorder.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-05-28 15:55:05.492220 rigorous_recorder-1.4.2/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1104 2023-04-24 13:58:53.000000 rigorous_recorder-1.4.2/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.237050 rigorous_recorder-1.4.3/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-03-19 13:33:17.000000 rigorous_recorder-1.4.3/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7720 2024-04-12 14:41:15.236899 rigorous_recorder-1.4.3/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-03-19 13:33:17.000000 rigorous_recorder-1.4.3/license.txt
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.181596 rigorous_recorder-1.4.3/rigorous_recorder/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.182184 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6126 2023-04-24 13:57:23.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.182320 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4315 2023-04-24 14:15:25.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.182431 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-04-24 13:57:23.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.182964 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.183391 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.183901 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.171923 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.184166 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.186023 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.186321 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.186802 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.186956 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.187421 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.187573 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.187690 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.188015 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.188359 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.188583 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.190813 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.192037 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.174327 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.192177 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.172863 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.173105 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.192803 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.193454 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.194414 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.194769 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.195113 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.173895 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.195259 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.195501 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196021 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196142 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196348 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196471 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196556 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196637 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196733 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.196835 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.198553 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.199240 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.199353 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.199666 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.199996 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.200627 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.200854 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.201140 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.201268 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-05-25 20:52:14.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.201879 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      420 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1327 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.202302 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.202851 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.175049 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.203098 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.204120 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.204570 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/main/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3216 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.204671 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/main/super_hash/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12071 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/main/super_hash/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27813 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      486 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.204783 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.204896 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.205198 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.205583 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.205865 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.209901 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.211487 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.177388 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.211607 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.175878 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.176041 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.213769 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.214439 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.215078 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.215394 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.215608 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.177130 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.215711 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.215877 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216072 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216176 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216340 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216478 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216561 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216641 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216719 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.216798 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.218189 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.218858 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.219184 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.219514 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.219941 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.220158 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.220374 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.220579 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/tests/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      321 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/tests/output.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      644 2023-05-28 15:54:26.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_hash/tests/test.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.221113 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      419 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      733 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.221591 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.222204 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      143 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.177995 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.222498 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.223479 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.223888 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1141 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.224091 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/super_map/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    14527 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/super_map/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    16088 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/main/super_map/neo_map.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27953 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      489 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.224199 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.224307 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.224598 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.224938 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.225161 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.227951 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13245 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.229174 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.180477 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.229284 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.179165 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.179356 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.229817 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.230447 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.231138 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.231460 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.231676 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.180194 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.231781 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.231951 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232143 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232250 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232411 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232526 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232607 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232695 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232776 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.232866 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.234243 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.234888 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    27936 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.235210 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.235564 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.236182 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.236465 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.236709 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-05-25 20:53:11.000000 rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/super_map/settings/requirements/system_tools.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    35694 2024-04-12 14:35:40.000000 rigorous_recorder-1.4.3/rigorous_recorder/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      335 2023-04-24 13:58:33.000000 rigorous_recorder-1.4.3/rigorous_recorder/settings.json
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2024-04-12 14:41:15.182082 rigorous_recorder-1.4.3/rigorous_recorder.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     7720 2024-04-12 14:41:14.000000 rigorous_recorder-1.4.3/rigorous_recorder.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    44313 2024-04-12 14:41:15.000000 rigorous_recorder-1.4.3/rigorous_recorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2024-04-12 14:41:14.000000 rigorous_recorder-1.4.3/rigorous_recorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       18 2024-04-12 14:41:14.000000 rigorous_recorder-1.4.3/rigorous_recorder.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2024-04-12 14:41:15.237092 rigorous_recorder-1.4.3/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1478 2024-04-12 14:33:34.000000 rigorous_recorder-1.4.3/setup.py
```

### Comparing `rigorous_recorder-1.4.2/PKG-INFO` & `rigorous_recorder-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous_recorder
-Version: 1.4.2
+Version: 1.4.3
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -102,21 +102,31 @@
 recorder.save_to("where/ever/you_want.pickle")
 ```
 
 # How do I use this?
 
 `pip install rigorous-recorder`
 
+Super simple usage:
+
+```python
+from rigorous_recorder import RecordKeeper
+record_keeper = RecordKeeper().live_write_to("where/ever/you_want.yaml", as_yaml=True)
+record_keeper.push(x=1, y=1)
+```
+
+Project/Experiment collection usage:
+
 ```python
 from rigorous_recorder import RecordKeeper, ExperimentCollection
 
 from statistics import mean as average
 from random import random, sample, choices
 
-collection = ExperimentCollection("data/my_study") # <- this string is a filepath 
+collection = ExperimentCollection("data/my_study") # <- filepath 
 number_of_new_experiments = 1
 
 for _ in range(number_of_new_experiments):
     
     # at the end (even when an error is thrown), all data is saved to disk automatically
     # experiment number increments based on the last saved-to-disk experiment number
     # running again (after error) won't double-increment the experiment number (same number until non-error run is achieved)
```

### Comparing `rigorous_recorder-1.4.2/rigorous_recorder/__init__.py` & `rigorous_recorder-1.4.3/rigorous_recorder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -766,14 +766,15 @@
         
         # clear existing data, make sure folder exists
         FS.write(data="", to=path)
         local_and_parent_data = AncestorDict(ancestors=self.local_data_lineage).__json__()
         self._live_files.append(open(path, 'a'))
         self._live_files[-1].write(f'''parent_data_snapshot: {json.dumps(local_and_parent_data, indent=4)}\n''')
         self._live_files[-1].write(f'''records:\n''')
+        return self
     
     def __del__(self):
         for each in self._live_files:
             each.close()
 
 class Experiment(object):
     def __init__(self, internal_experiment_info, save_experiment):
```

### Comparing `rigorous_recorder-1.4.2/rigorous_recorder.egg-info/PKG-INFO` & `rigorous_recorder-1.4.3/rigorous_recorder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rigorous-recorder
-Version: 1.4.2
+Version: 1.4.3
 Summary: Save everything in a filterable way
 Home-page: https://github.com/jeff-hykin/rigorous_recorder.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -102,21 +102,31 @@
 recorder.save_to("where/ever/you_want.pickle")
 ```
 
 # How do I use this?
 
 `pip install rigorous-recorder`
 
+Super simple usage:
+
+```python
+from rigorous_recorder import RecordKeeper
+record_keeper = RecordKeeper().live_write_to("where/ever/you_want.yaml", as_yaml=True)
+record_keeper.push(x=1, y=1)
+```
+
+Project/Experiment collection usage:
+
 ```python
 from rigorous_recorder import RecordKeeper, ExperimentCollection
 
 from statistics import mean as average
 from random import random, sample, choices
 
-collection = ExperimentCollection("data/my_study") # <- this string is a filepath 
+collection = ExperimentCollection("data/my_study") # <- filepath 
 number_of_new_experiments = 1
 
 for _ in range(number_of_new_experiments):
     
     # at the end (even when an error is thrown), all data is saved to disk automatically
     # experiment number increments based on the last saved-to-disk experiment number
     # running again (after error) won't double-increment the experiment number (same number until non-error run is achieved)
```

### Comparing `rigorous_recorder-1.4.2/setup.py` & `rigorous_recorder-1.4.3/rigorous_recorder/__dependencies__/__sources__/file_system_py/main/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,20 +22,23 @@
     description=package_info["description"],
     url=package_info["url"],
     author=package_info["author"],
     author_email=package_info["author_email"],
     license=package_info["license"],
     packages=[package_info["name"]],
     install_requires=[
+        # examples:
+        # 'python-socketio >= 5.3.0',
+        # 'requests == 2.26.0',
     ],
     classifiers=[
         # examples:
         # 'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python',
-        "Programming Language :: Python :: 3",
-        "Operating System :: OS Independent",
+        # 'Intended Audience :: Developers',
+        # 'Programming Language :: Python',
+        # "Programming Language :: Python :: 3",
+        # "Operating System :: OS Independent",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
 )
```

