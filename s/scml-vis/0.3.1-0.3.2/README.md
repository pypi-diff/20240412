# Comparing `tmp/scml-vis-0.3.1.tar.gz` & `tmp/scml-vis-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scml-vis-0.3.1.tar", last modified: Thu Mar 21 07:06:20 2024, max compression
+gzip compressed data, was "scml-vis-0.3.2.tar", last modified: Fri Apr 12 04:45:25 2024, max compression
```

## Comparing `scml-vis-0.3.1.tar` & `scml-vis-0.3.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.141453 scml-vis-0.3.1/
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.107889 scml-vis-0.3.1/.github/
--rw-r--r--   0 yasser     (501) staff       (20)     6148 2023-12-03 18:24:49.000000 scml-vis-0.3.1/.github/.DS_Store
--rw-r--r--   0 yasser     (501) staff       (20)      148 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.github/FUNDING.yml
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.108833 scml-vis-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 yasser     (501) staff       (20)      688 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 yasser     (501) staff       (20)      600 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.109195 scml-vis-0.3.1/.github/workflows/
--rw-r--r--   0 yasser     (501) staff       (20)     1736 2023-03-17 04:06:53.000000 scml-vis-0.3.1/.github/workflows/main.yml
--rw-r--r--   0 yasser     (501) staff       (20)      149 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.gitignore
--rw-r--r--   0 yasser     (501) staff       (20)     3959 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.vimspector.json
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.110225 scml-vis-0.3.1/.vscode/
--rw-r--r--   0 yasser     (501) staff       (20)      695 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.vscode/launch.json
--rw-r--r--   0 yasser     (501) staff       (20)      115 2022-04-11 08:17:37.000000 scml-vis-0.3.1/.vscode/settings.json
--rw-r--r--   0 yasser     (501) staff       (20)        1 2022-05-18 03:00:49.000000 scml-vis-0.3.1/CHANGELOG.md
--rw-r--r--   0 yasser     (501) staff       (20)     3230 2022-04-11 08:17:37.000000 scml-vis-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 yasser     (501) staff       (20)     3456 2022-04-11 08:17:37.000000 scml-vis-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 yasser     (501) staff       (20)    10255 2022-04-11 08:17:37.000000 scml-vis-0.3.1/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)      757 2022-04-11 08:17:37.000000 scml-vis-0.3.1/Makefile
--rw-r--r--   0 yasser     (501) staff       (20)     5696 2024-03-21 07:06:20.141607 scml-vis-0.3.1/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)     4927 2022-05-18 03:03:33.000000 scml-vis-0.3.1/README.md
--rw-r--r--   0 yasser     (501) staff       (20)     5331 2023-03-17 04:06:53.000000 scml-vis-0.3.1/README.rst
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.111668 scml-vis-0.3.1/config/
--rw-r--r--   0 yasser     (501) staff       (20)      340 2022-04-11 08:17:37.000000 scml-vis-0.3.1/config/coverage.ini
--rw-r--r--   0 yasser     (501) staff       (20)     2554 2022-04-11 08:17:37.000000 scml-vis-0.3.1/config/flake8.ini
--rw-r--r--   0 yasser     (501) staff       (20)       63 2022-04-11 08:17:37.000000 scml-vis-0.3.1/config/mypy.ini
--rw-r--r--   0 yasser     (501) staff       (20)      184 2022-04-11 08:17:37.000000 scml-vis-0.3.1/config/pytest.ini
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.128108 scml-vis-0.3.1/docs/
--rw-r--r--   0 yasser     (501) staff       (20)     6148 2023-12-03 18:24:49.000000 scml-vis-0.3.1/docs/.DS_Store
--rw-r--r--   0 yasser     (501) staff       (20)   353348 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/aftercompile.png
--rw-r--r--   0 yasser     (501) staff       (20)       21 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/changelog.md
--rw-r--r--   0 yasser     (501) staff       (20)       27 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/code_of_conduct.md
--rw-r--r--   0 yasser     (501) staff       (20)    86443 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/compile.png
--rw-r--r--   0 yasser     (501) staff       (20)       24 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/contributing.md
--rw-r--r--   0 yasser     (501) staff       (20)       16 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/credits.md
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.129399 scml-vis-0.3.1/docs/css/
--rw-r--r--   0 yasser     (501) staff       (20)      688 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/css/mkdocstrings.css
--rw-r--r--   0 yasser     (501) staff       (20)    89541 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/datasette.png
--rw-r--r--   0 yasser     (501) staff       (20)   293912 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/datasettelarge.png
--rw-r--r--   0 yasser     (501) staff       (20)       18 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/index.md
--rw-r--r--   0 yasser     (501) staff       (20)       24 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/license.md
--rw-r--r--   0 yasser     (501) staff       (20)     2673 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/macros.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.129960 scml-vis-0.3.1/docs/reference/
--rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/reference/cli.md
--rw-r--r--   0 yasser     (501) staff       (20)  1316811 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/shot1.png
--rw-r--r--   0 yasser     (501) staff       (20)  1125356 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/shot2.png
--rw-r--r--   0 yasser     (501) staff       (20)   190689 2022-04-11 08:17:37.000000 scml-vis-0.3.1/docs/show.png
--rw-r--r--   0 yasser     (501) staff       (20)     9474 2022-04-11 08:17:37.000000 scml-vis-0.3.1/duties.py
--rw-r--r--   0 yasser     (501) staff       (20)     1035 2022-04-11 08:17:37.000000 scml-vis-0.3.1/mkdocs.yml
--rw-r--r--   0 yasser     (501) staff       (20)      100 2022-05-17 23:37:59.000000 scml-vis-0.3.1/pyproject.toml
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.133818 scml-vis-0.3.1/scripts/
--rwxr-xr-x   0 yasser     (501) staff       (20)      735 2022-04-11 08:17:37.000000 scml-vis-0.3.1/scripts/multirun.sh
--rwxr-xr-x   0 yasser     (501) staff       (20)      871 2022-04-11 08:17:37.000000 scml-vis-0.3.1/scripts/setup.sh
--rw-r--r--   0 yasser     (501) staff       (20)     2128 2024-03-21 07:06:20.145172 scml-vis-0.3.1/setup.cfg
--rwxr-xr-x   0 yasser     (501) staff       (20)       69 2022-05-17 23:37:39.000000 scml-vis-0.3.1/setup.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.100118 scml-vis-0.3.1/src/
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.136545 scml-vis-0.3.1/src/scml_vis/
--rw-r--r--   0 yasser     (501) staff       (20)      199 2024-03-21 07:06:01.000000 scml-vis-0.3.1/src/scml_vis/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      342 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/__main__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     3252 2023-12-27 05:20:41.000000 scml-vis-0.3.1/src/scml_vis/cli.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    36766 2024-03-21 06:54:59.000000 scml-vis-0.3.1/src/scml_vis/compiler.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    52140 2024-03-21 06:54:26.000000 scml-vis-0.3.1/src/scml_vis/presenter.py
--rw-r--r--   0 yasser     (501) staff       (20)    24790 2024-03-21 06:44:16.000000 scml-vis-0.3.1/src/scml_vis/utils.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.138319 scml-vis-0.3.1/src/scml_vis/vendor/
--rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/vendor/__init__.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.140200 scml-vis-0.3.1/src/scml_vis/vendor/quick/
--rw-r--r--   0 yasser     (501) staff       (20)    35147 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/vendor/quick/LICENSE
--rw-r--r--   0 yasser     (501) staff       (20)     2465 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/vendor/quick/README.md
--rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/vendor/quick/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    29282 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/vendor/quick/quick.py
--rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:17:37.000000 scml-vis-0.3.1/src/scml_vis/vendor/quick/requirements.txt
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.138008 scml-vis-0.3.1/src/scml_vis.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)     5696 2024-03-21 07:06:19.000000 scml-vis-0.3.1/src/scml_vis.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)     1409 2024-03-21 07:06:19.000000 scml-vis-0.3.1/src/scml_vis.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2024-03-21 07:06:19.000000 scml-vis-0.3.1/src/scml_vis.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)      101 2024-03-21 07:06:19.000000 scml-vis-0.3.1/src/scml_vis.egg-info/entry_points.txt
--rw-r--r--   0 yasser     (501) staff       (20)      226 2024-03-21 07:06:19.000000 scml-vis-0.3.1/src/scml_vis.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)        9 2024-03-21 07:06:19.000000 scml-vis-0.3.1/src/scml_vis.egg-info/top_level.txt
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-03-21 07:06:20.141208 scml-vis-0.3.1/tests/
--rw-r--r--   0 yasser     (501) staff       (20)      161 2022-04-11 08:17:37.000000 scml-vis-0.3.1/tests/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)       47 2022-04-11 08:17:37.000000 scml-vis-0.3.1/tests/conftest.py
--rw-r--r--   0 yasser     (501) staff       (20)      410 2022-04-11 08:17:37.000000 scml-vis-0.3.1/tests/test_cli.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.870389 scml-vis-0.3.2/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.754058 scml-vis-0.3.2/.github/
+-rw-r--r--   0 yasser     (501) staff       (20)     6148 2024-04-12 04:15:15.000000 scml-vis-0.3.2/.github/.DS_Store
+-rw-r--r--   0 yasser     (501) staff       (20)      148 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.github/FUNDING.yml
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.760882 scml-vis-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 yasser     (501) staff       (20)      688 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 yasser     (501) staff       (20)      600 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.763676 scml-vis-0.3.2/.github/workflows/
+-rw-r--r--   0 yasser     (501) staff       (20)     1736 2023-03-17 04:06:53.000000 scml-vis-0.3.2/.github/workflows/main.yml
+-rw-r--r--   0 yasser     (501) staff       (20)      149 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.gitignore
+-rw-r--r--   0 yasser     (501) staff       (20)     3959 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.vimspector.json
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.769745 scml-vis-0.3.2/.vscode/
+-rw-r--r--   0 yasser     (501) staff       (20)      695 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.vscode/launch.json
+-rw-r--r--   0 yasser     (501) staff       (20)      115 2022-04-11 08:17:37.000000 scml-vis-0.3.2/.vscode/settings.json
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2022-05-18 03:00:49.000000 scml-vis-0.3.2/CHANGELOG.md
+-rw-r--r--   0 yasser     (501) staff       (20)     3230 2022-04-11 08:17:37.000000 scml-vis-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 yasser     (501) staff       (20)     3456 2022-04-11 08:17:37.000000 scml-vis-0.3.2/CONTRIBUTING.md
+-rw-r--r--   0 yasser     (501) staff       (20)    10255 2022-04-11 08:17:37.000000 scml-vis-0.3.2/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)      757 2022-04-11 08:17:37.000000 scml-vis-0.3.2/Makefile
+-rw-r--r--   0 yasser     (501) staff       (20)     6381 2024-04-12 04:45:25.870181 scml-vis-0.3.2/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     4927 2022-05-18 03:03:33.000000 scml-vis-0.3.2/README.md
+-rw-r--r--   0 yasser     (501) staff       (20)     5331 2023-03-17 04:06:53.000000 scml-vis-0.3.2/README.rst
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.783459 scml-vis-0.3.2/config/
+-rw-r--r--   0 yasser     (501) staff       (20)      340 2022-04-11 08:17:37.000000 scml-vis-0.3.2/config/coverage.ini
+-rw-r--r--   0 yasser     (501) staff       (20)     2554 2022-04-11 08:17:37.000000 scml-vis-0.3.2/config/flake8.ini
+-rw-r--r--   0 yasser     (501) staff       (20)       63 2022-04-11 08:17:37.000000 scml-vis-0.3.2/config/mypy.ini
+-rw-r--r--   0 yasser     (501) staff       (20)      184 2022-04-11 08:17:37.000000 scml-vis-0.3.2/config/pytest.ini
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.842961 scml-vis-0.3.2/docs/
+-rw-r--r--   0 yasser     (501) staff       (20)     6148 2024-04-12 04:15:16.000000 scml-vis-0.3.2/docs/.DS_Store
+-rw-r--r--   0 yasser     (501) staff       (20)   353348 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/aftercompile.png
+-rw-r--r--   0 yasser     (501) staff       (20)       21 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/changelog.md
+-rw-r--r--   0 yasser     (501) staff       (20)       27 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/code_of_conduct.md
+-rw-r--r--   0 yasser     (501) staff       (20)    86443 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/compile.png
+-rw-r--r--   0 yasser     (501) staff       (20)       24 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/contributing.md
+-rw-r--r--   0 yasser     (501) staff       (20)       16 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/credits.md
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.849759 scml-vis-0.3.2/docs/css/
+-rw-r--r--   0 yasser     (501) staff       (20)      688 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/css/mkdocstrings.css
+-rw-r--r--   0 yasser     (501) staff       (20)    89541 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/datasette.png
+-rw-r--r--   0 yasser     (501) staff       (20)   293912 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/datasettelarge.png
+-rw-r--r--   0 yasser     (501) staff       (20)       18 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/index.md
+-rw-r--r--   0 yasser     (501) staff       (20)       24 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/license.md
+-rw-r--r--   0 yasser     (501) staff       (20)     2673 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/macros.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.852115 scml-vis-0.3.2/docs/reference/
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/reference/cli.md
+-rw-r--r--   0 yasser     (501) staff       (20)  1316811 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/shot1.png
+-rw-r--r--   0 yasser     (501) staff       (20)  1125356 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/shot2.png
+-rw-r--r--   0 yasser     (501) staff       (20)   190689 2022-04-11 08:17:37.000000 scml-vis-0.3.2/docs/show.png
+-rw-r--r--   0 yasser     (501) staff       (20)     9474 2022-04-11 08:17:37.000000 scml-vis-0.3.2/duties.py
+-rw-r--r--   0 yasser     (501) staff       (20)     1035 2022-04-11 08:17:37.000000 scml-vis-0.3.2/mkdocs.yml
+-rw-r--r--   0 yasser     (501) staff       (20)      100 2022-05-17 23:37:59.000000 scml-vis-0.3.2/pyproject.toml
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.856345 scml-vis-0.3.2/scripts/
+-rwxr-xr-x   0 yasser     (501) staff       (20)      735 2022-04-11 08:17:37.000000 scml-vis-0.3.2/scripts/multirun.sh
+-rwxr-xr-x   0 yasser     (501) staff       (20)      871 2022-04-11 08:17:37.000000 scml-vis-0.3.2/scripts/setup.sh
+-rw-r--r--   0 yasser     (501) staff       (20)     2138 2024-04-12 04:45:25.871313 scml-vis-0.3.2/setup.cfg
+-rwxr-xr-x   0 yasser     (501) staff       (20)       69 2022-05-17 23:37:39.000000 scml-vis-0.3.2/setup.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.708993 scml-vis-0.3.2/src/
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.858078 scml-vis-0.3.2/src/scml_vis/
+-rw-r--r--   0 yasser     (501) staff       (20)      161 2024-04-12 04:17:22.000000 scml-vis-0.3.2/src/scml_vis/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)      342 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/__main__.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)     6666 2024-04-12 04:13:05.000000 scml-vis-0.3.2/src/scml_vis/cli.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    36887 2024-04-11 07:59:47.000000 scml-vis-0.3.2/src/scml_vis/compiler.py
+-rwxr-xr-x   0 yasser     (501) staff       (20)    52140 2024-03-21 06:54:26.000000 scml-vis-0.3.2/src/scml_vis/presenter.py
+-rw-r--r--   0 yasser     (501) staff       (20)    24790 2024-03-21 06:44:16.000000 scml-vis-0.3.2/src/scml_vis/utils.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.859810 scml-vis-0.3.2/src/scml_vis/vendor/
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/vendor/__init__.py
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.860996 scml-vis-0.3.2/src/scml_vis/vendor/quick/
+-rw-r--r--   0 yasser     (501) staff       (20)    35147 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/vendor/quick/LICENSE
+-rw-r--r--   0 yasser     (501) staff       (20)     2465 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/vendor/quick/README.md
+-rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/vendor/quick/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)    29282 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/vendor/quick/quick.py
+-rw-r--r--   0 yasser     (501) staff       (20)       17 2022-04-11 08:17:37.000000 scml-vis-0.3.2/src/scml_vis/vendor/quick/requirements.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.869362 scml-vis-0.3.2/src/scml_vis.egg-info/
+-rw-r--r--   0 yasser     (501) staff       (20)     6381 2024-04-12 04:45:25.000000 scml-vis-0.3.2/src/scml_vis.egg-info/PKG-INFO
+-rw-r--r--   0 yasser     (501) staff       (20)     1409 2024-04-12 04:45:25.000000 scml-vis-0.3.2/src/scml_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        1 2024-04-12 04:45:25.000000 scml-vis-0.3.2/src/scml_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 yasser     (501) staff       (20)      101 2024-04-12 04:45:25.000000 scml-vis-0.3.2/src/scml_vis.egg-info/entry_points.txt
+-rw-r--r--   0 yasser     (501) staff       (20)      233 2024-04-12 04:45:25.000000 scml-vis-0.3.2/src/scml_vis.egg-info/requires.txt
+-rw-r--r--   0 yasser     (501) staff       (20)        9 2024-04-12 04:45:25.000000 scml-vis-0.3.2/src/scml_vis.egg-info/top_level.txt
+drwxr-xr-x   0 yasser     (501) staff       (20)        0 2024-04-12 04:45:25.868726 scml-vis-0.3.2/tests/
+-rw-r--r--   0 yasser     (501) staff       (20)      161 2022-04-11 08:17:37.000000 scml-vis-0.3.2/tests/__init__.py
+-rw-r--r--   0 yasser     (501) staff       (20)       47 2022-04-11 08:17:37.000000 scml-vis-0.3.2/tests/conftest.py
+-rw-r--r--   0 yasser     (501) staff       (20)      410 2022-04-11 08:17:37.000000 scml-vis-0.3.2/tests/test_cli.py
```

### Comparing `scml-vis-0.3.1/.github/.DS_Store` & `scml-vis-0.3.2/.github/.DS_Store`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `scml-vis-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `scml-vis-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/.github/workflows/main.yml` & `scml-vis-0.3.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/.vimspector.json` & `scml-vis-0.3.2/.vimspector.json`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/.vscode/launch.json` & `scml-vis-0.3.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/CODE_OF_CONDUCT.md` & `scml-vis-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/CONTRIBUTING.md` & `scml-vis-0.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/LICENSE` & `scml-vis-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/Makefile` & `scml-vis-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/PKG-INFO` & `scml-vis-0.3.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 Metadata-Version: 2.1
 Name: scml-vis
-Version: 0.3.1
+Version: 0.3.2
 Summary: "A simple visualiser for SCML worlds and tournaments"
 Home-page: https://github.com/yasserfarouk/negmas
 Author-email: yasserfarouk@gmail.com
 License: Apache License 2.0
 Keywords: negotiation,mas,multi-agent,simulation,AI,negmas,scml,scml-agents
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Click>=6.0
+Requires-Dist: numpy
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: seaborn
+Requires-Dist: streamlit>=1.12.0
+Requires-Dist: plotly
+Requires-Dist: click
+Requires-Dist: click-config-file
+Requires-Dist: watchdog
+Requires-Dist: datasette-vega
+Requires-Dist: csvs-to-sqlite
+Requires-Dist: scml>=0.7.3
+Provides-Extra: dev
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: pytest-sugar; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # scml-vis
 
 [![ci](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml/badge.svg)](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://scml-vis.github.io/scml-vis/)
 [![pypi version](https://img.shields.io/pypi/v/scml-vis.svg)](https://pypi.org/project/scml-vis/)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/scml-vis/community)
```

### Comparing `scml-vis-0.3.1/README.md` & `scml-vis-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/README.rst` & `scml-vis-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/config/flake8.ini` & `scml-vis-0.3.2/config/flake8.ini`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/.DS_Store` & `scml-vis-0.3.2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/aftercompile.png` & `scml-vis-0.3.2/docs/aftercompile.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/compile.png` & `scml-vis-0.3.2/docs/compile.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/css/mkdocstrings.css` & `scml-vis-0.3.2/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/datasette.png` & `scml-vis-0.3.2/docs/datasette.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/datasettelarge.png` & `scml-vis-0.3.2/docs/datasettelarge.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/macros.py` & `scml-vis-0.3.2/docs/macros.py`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/shot1.png` & `scml-vis-0.3.2/docs/shot1.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/shot2.png` & `scml-vis-0.3.2/docs/shot2.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/docs/show.png` & `scml-vis-0.3.2/docs/show.png`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/duties.py` & `scml-vis-0.3.2/duties.py`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/mkdocs.yml` & `scml-vis-0.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/scripts/multirun.sh` & `scml-vis-0.3.2/scripts/multirun.sh`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/scripts/setup.sh` & `scml-vis-0.3.2/scripts/setup.sh`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/setup.cfg` & `scml-vis-0.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [bumpversion]
-current_version = 0.3.1
+current_version = 0.3.2
 delete_bookmark = True
 commit = False
 tag = False
 
 [metadata]
 name = scml-vis
-version = 0.3.1
+version = 0.3.2
 description = "A simple visualiser for SCML worlds and tournaments"
 authors = ["Yasser Mohammad <yasserfarouk@gmail.com>"]
 license = Apache License 2.0
 readme = "README.md"
 repository = "https://github.com/scml-vis/scml-vis"
 homepage = "https://github.com/scml-vis/scml-vis"
 author_email = yasserfarouk@gmail.com
@@ -37,15 +37,15 @@
 [options]
 package_dir = 
 	=src
 packages = scml_vis
 install_requires = 
 	Click (>=6.0)
 	numpy
-	pandas
+	pandas (>=2.0.2)
 	seaborn
 	streamlit (>=1.12.0)
 	plotly
 	click
 	click-config-file
 	watchdog
 	datasette-vega
```

### Comparing `scml-vis-0.3.1/src/scml_vis/compiler.py` & `scml-vis-0.3.2/src/scml_vis/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 import itertools
+import math
 import json
 import re
 import sys
 from pathlib import Path
 from typing import Dict, Iterable, Optional
 
 import numpy as np
@@ -361,14 +362,15 @@
             "tournament",
             "round",
         ],
     )
     for cname in CONTRACTS_FILE:
         if nonzero(path / cname):
             contracts = pd.read_csv(path / cname, index_col=0)
+            break
     if nonzero(path / NEGOTIATIONS_FILE):
         negotiations = pd.read_csv(path / NEGOTIATIONS_FILE, index_col=0)
         negotiations = negotiations.loc[
             :,
             [
                 "id",
                 "agreement",
@@ -442,14 +444,16 @@
         )
         # atmap = dict(zip(all_agents["name"].to_list(), all_agents["type"].to_list()))
         # negotiations.agreement[negotiations.agreement.isna(), "agreement"] = None
         for c in ["quantity", "delivery_step", "unit_price"]:
             negotiations[c] = None
 
         def lst(x):
+            if isinstance(x, float) and math.isnan(x):
+                return [-1, -1, -1]
             return (
                 [-1, -1, -1]
                 if not x or (isinstance(x, str) and x.lower() == "none")
                 else list(eval(x))
                 if isinstance(x, str)
                 else list(x)
             )
```

### Comparing `scml-vis-0.3.1/src/scml_vis/presenter.py` & `scml-vis-0.3.2/src/scml_vis/presenter.py`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/src/scml_vis/utils.py` & `scml-vis-0.3.2/src/scml_vis/utils.py`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/src/scml_vis/vendor/quick/LICENSE` & `scml-vis-0.3.2/src/scml_vis/vendor/quick/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/src/scml_vis/vendor/quick/README.md` & `scml-vis-0.3.2/src/scml_vis/vendor/quick/README.md`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/src/scml_vis/vendor/quick/quick.py` & `scml-vis-0.3.2/src/scml_vis/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `scml-vis-0.3.1/src/scml_vis.egg-info/PKG-INFO` & `scml-vis-0.3.2/src/scml_vis.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 Metadata-Version: 2.1
 Name: scml-vis
-Version: 0.3.1
+Version: 0.3.2
 Summary: "A simple visualiser for SCML worlds and tournaments"
 Home-page: https://github.com/yasserfarouk/negmas
 Author-email: yasserfarouk@gmail.com
 License: Apache License 2.0
 Keywords: negotiation,mas,multi-agent,simulation,AI,negmas,scml,scml-agents
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Click>=6.0
+Requires-Dist: numpy
+Requires-Dist: pandas>=2.0.2
+Requires-Dist: seaborn
+Requires-Dist: streamlit>=1.12.0
+Requires-Dist: plotly
+Requires-Dist: click
+Requires-Dist: click-config-file
+Requires-Dist: watchdog
+Requires-Dist: datasette-vega
+Requires-Dist: csvs-to-sqlite
+Requires-Dist: scml>=0.7.3
+Provides-Extra: dev
+Requires-Dist: autoflake; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: pytest-sugar; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # scml-vis
 
 [![ci](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml/badge.svg)](https://github.com/yasserfarouk/scml-vis/actions/workflows/main.yml)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://scml-vis.github.io/scml-vis/)
 [![pypi version](https://img.shields.io/pypi/v/scml-vis.svg)](https://pypi.org/project/scml-vis/)
 [![gitter](https://badges.gitter.im/join%20chat.svg)](https://gitter.im/scml-vis/community)
```

### Comparing `scml-vis-0.3.1/src/scml_vis.egg-info/SOURCES.txt` & `scml-vis-0.3.2/src/scml_vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

