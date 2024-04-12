# Comparing `tmp/geohey-0.0.4.tar.gz` & `tmp/geohey-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geohey-0.0.4.tar", last modified: Mon Mar 25 18:41:50 2024, max compression
+gzip compressed data, was "geohey-0.0.5.tar", last modified: Fri Apr 12 19:06:29 2024, max compression
```

## Comparing `geohey-0.0.4.tar` & `geohey-0.0.5.tar`

### file list

```diff
@@ -1,88 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.183828 geohey-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-25 18:41:38.000000 geohey-0.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.159829 geohey-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.163828 geohey-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.167828 geohey-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-25 18:41:38.000000 geohey-0.0.4/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-25 18:41:38.000000 geohey-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-25 18:41:38.000000 geohey-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:41:38.000000 geohey-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-25 18:41:38.000000 geohey-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-25 18:41:50.183828 geohey-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-25 18:41:38.000000 geohey-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.167828 geohey-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.167828 geohey-0.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/examples/csv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/examples/random.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/examples/vector.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/geohey.md
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.167828 geohey-0.0.4/docs/labs/
--rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/labs/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/labs/lab5.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.167828 geohey-0.0.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.171829 geohey-0.0.4/docs/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/01_getting_started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22686 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/02_variables_data_types.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20592 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/03_introducing_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26960 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/04_working_with_lists.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30225 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/05_if_statements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28469 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/06_dictionaries.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23915 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/07_user_input_while_loops.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    41581 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/08_functions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    26777 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/09_classes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    46711 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/10_files_and_exceptions.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.179829 geohey-0.0.4/docs/python/data/
--rw-r--r--   0 runner    (1001) docker     (127)   804335 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/A-Tale-of-Two-Cities.txt
--rw-r--r--   0 runner    (1001) docker     (127)   169855 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/alice.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1053436 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/little_women.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1276220 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/moby_dick.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/numbers.json
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/pi_digits.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1030000 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/pi_million_digits.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/programming.txt
--rw-r--r--   0 runner    (1001) docker     (127)   241175 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/siddhartha.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1063095 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/tn_place_names.csv
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/data/username.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/python/jupytext.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 18:41:38.000000 geohey-0.0.4/docs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.179829 geohey-0.0.4/geohey/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-25 18:41:38.000000 geohey-0.0.4/geohey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-25 18:41:38.000000 geohey-0.0.4/geohey/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-25 18:41:38.000000 geohey-0.0.4/geohey/geohey.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-25 18:41:38.000000 geohey-0.0.4/geohey/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.183828 geohey-0.0.4/geohey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-25 18:41:50.000000 geohey-0.0.4/geohey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-25 18:41:50.000000 geohey-0.0.4/geohey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:41:50.000000 geohey-0.0.4/geohey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 18:41:50.000000 geohey-0.0.4/geohey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-25 18:41:50.000000 geohey-0.0.4/geohey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 18:41:50.000000 geohey-0.0.4/geohey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-25 18:41:38.000000 geohey-0.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-25 18:41:38.000000 geohey-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 18:41:38.000000 geohey-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-25 18:41:38.000000 geohey-0.0.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 18:41:50.183828 geohey-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:41:50.183828 geohey-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 18:41:38.000000 geohey-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-25 18:41:38.000000 geohey-0.0.4/tests/test_geohey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.289199 geohey-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-12 19:06:18.000000 geohey-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.265199 geohey-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.269199 geohey-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.269199 geohey-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-12 19:06:18.000000 geohey-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 19:06:18.000000 geohey-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-12 19:06:18.000000 geohey-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:06:18.000000 geohey-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 19:06:18.000000 geohey-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-12 19:06:29.285199 geohey-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-12 19:06:18.000000 geohey-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.269199 geohey-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.273199 geohey-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16333 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/ipywidgets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/random.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/toolbar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/geohey.md
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.273199 geohey-0.0.5/docs/labs/
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/labs/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/labs/lab5.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.273199 geohey-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.277199 geohey-0.0.5/docs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/01_getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22686 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/02_variables_data_types.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20592 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/03_introducing_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26960 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/04_working_with_lists.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30225 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/05_if_statements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28469 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/06_dictionaries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23915 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/07_user_input_while_loops.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    41581 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/08_functions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    26777 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/09_classes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    46711 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/10_files_and_exceptions.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.285199 geohey-0.0.5/docs/python/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   804335 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/A-Tale-of-Two-Cities.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   169855 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/alice.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1053436 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/little_women.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1276220 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/moby_dick.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/numbers.json
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/pi_digits.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1030000 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/pi_million_digits.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/programming.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   241175 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/siddhartha.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1063095 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/tn_place_names.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/data/username.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/python/jupytext.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 19:06:18.000000 geohey-0.0.5/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.285199 geohey-0.0.5/geohey/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 19:06:18.000000 geohey-0.0.5/geohey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 19:06:18.000000 geohey-0.0.5/geohey/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-12 19:06:18.000000 geohey-0.0.5/geohey/geohey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-12 19:06:18.000000 geohey-0.0.5/geohey/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.285199 geohey-0.0.5/geohey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-12 19:06:29.000000 geohey-0.0.5/geohey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-12 19:06:29.000000 geohey-0.0.5/geohey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:06:29.000000 geohey-0.0.5/geohey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 19:06:29.000000 geohey-0.0.5/geohey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 19:06:29.000000 geohey-0.0.5/geohey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 19:06:29.000000 geohey-0.0.5/geohey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-12 19:06:18.000000 geohey-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-12 19:06:18.000000 geohey-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 19:06:18.000000 geohey-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-12 19:06:18.000000 geohey-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:06:29.289199 geohey-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:06:29.285199 geohey-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 19:06:18.000000 geohey-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-12 19:06:18.000000 geohey-0.0.5/tests/test_geohey.py
```

### Comparing `geohey-0.0.4/.github/workflows/docs-build.yml` & `geohey-0.0.5/.github/workflows/docs-build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                   gdalinfo --version
             - name: Install dependencies
               run: |
                   pip install --no-cache-dir Cython
                   pip install -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
-              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git,*.txt" --ignore-words-list="aci,acount,hist"
+              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git,*.txt,*data_types.ipynb" --ignore-words-list="aci,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - name: Build docs
               run: |
                   mkdocs build
             # - name: Deploy to Netlify
```

### Comparing `geohey-0.0.4/.github/workflows/docs.yml` & `geohey-0.0.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.github/workflows/installation.yml` & `geohey-0.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.github/workflows/macos.yml` & `geohey-0.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.github/workflows/pypi.yml` & `geohey-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.github/workflows/ubuntu.yml` & `geohey-0.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.github/workflows/windows.yml` & `geohey-0.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.gitignore` & `geohey-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/.pre-commit-config.yaml` & `geohey-0.0.5/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
-      rev: v4.5.0
+      rev: v4.6.0
       hooks:
           - id: check-toml
           - id: check-yaml
           - id: end-of-file-fixer
             types: [python]
           - id: trailing-whitespace
           - id: requirements-txt-fixer
           - id: check-added-large-files
             args: ["--maxkb=500"]
 
     - repo: https://github.com/psf/black
-      rev: 24.2.0
+      rev: 24.3.0
       hooks:
           - id: black-jupyter
             language_version: python3.11
 
     # - repo: https://github.com/codespell-project/codespell
     #   rev: v2.2.6
     #   hooks:
```

### Comparing `geohey-0.0.4/PKG-INFO` & `geohey-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohey
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package demo for geospatial analysis
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/giswqs/geohey
 Keywords: geohey
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,8 +35,9 @@
 -   Free software: MIT License
 -   Documentation: https://geohey.gishub.org
 
 ## Features
 
 -   Visualizing raster and vector data
 -   Analyzing raster and vector data
--   Print out useful message
+-   Visualizing raster data
+-   Analyzing raster data
```

### Comparing `geohey-0.0.4/docs/contributing.md` & `geohey-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/examples/csv.ipynb` & `geohey-0.0.5/docs/examples/csv.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/examples/demo.ipynb` & `geohey-0.0.5/docs/examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/examples/ipyleaflet.ipynb` & `geohey-0.0.5/docs/examples/ipyleaflet.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/examples/vector.ipynb` & `geohey-0.0.5/docs/examples/vector.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/installation.md` & `geohey-0.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/labs/lab4.ipynb` & `geohey-0.0.5/docs/labs/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/labs/lab5.ipynb` & `geohey-0.0.5/docs/labs/lab5.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/01_getting_started.ipynb` & `geohey-0.0.5/docs/python/01_getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/02_variables_data_types.ipynb` & `geohey-0.0.5/docs/python/02_variables_data_types.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/03_introducing_lists.ipynb` & `geohey-0.0.5/docs/python/03_introducing_lists.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/04_working_with_lists.ipynb` & `geohey-0.0.5/docs/python/04_working_with_lists.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/05_if_statements.ipynb` & `geohey-0.0.5/docs/python/05_if_statements.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/06_dictionaries.ipynb` & `geohey-0.0.5/docs/python/06_dictionaries.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/07_user_input_while_loops.ipynb` & `geohey-0.0.5/docs/python/07_user_input_while_loops.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/08_functions.ipynb` & `geohey-0.0.5/docs/python/08_functions.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/09_classes.ipynb` & `geohey-0.0.5/docs/python/09_classes.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/10_files_and_exceptions.ipynb` & `geohey-0.0.5/docs/python/10_files_and_exceptions.ipynb`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/A-Tale-of-Two-Cities.txt` & `geohey-0.0.5/docs/python/data/A-Tale-of-Two-Cities.txt`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/alice.txt` & `geohey-0.0.5/docs/python/data/alice.txt`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/little_women.txt` & `geohey-0.0.5/docs/python/data/little_women.txt`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/moby_dick.txt` & `geohey-0.0.5/docs/python/data/moby_dick.txt`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/pi_million_digits.txt` & `geohey-0.0.5/docs/python/data/pi_million_digits.txt`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/siddhartha.txt` & `geohey-0.0.5/docs/python/data/siddhartha.txt`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/data/tn_place_names.csv` & `geohey-0.0.5/docs/python/data/tn_place_names.csv`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/docs/python/jupytext.toml` & `geohey-0.0.5/docs/python/jupytext.toml`

 * *Files identical despite different names*

### Comparing `geohey-0.0.4/geohey.egg-info/PKG-INFO` & `geohey-0.0.5/geohey.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohey
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package demo for geospatial analysis
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/giswqs/geohey
 Keywords: geohey
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -35,8 +35,9 @@
 -   Free software: MIT License
 -   Documentation: https://geohey.gishub.org
 
 ## Features
 
 -   Visualizing raster and vector data
 -   Analyzing raster and vector data
--   Print out useful message
+-   Visualizing raster data
+-   Analyzing raster data
```

### Comparing `geohey-0.0.4/geohey.egg-info/SOURCES.txt` & `geohey-0.0.5/geohey.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 docs/installation.md
 docs/usage.md
 docs/utils.md
 docs/examples/csv.ipynb
 docs/examples/demo.ipynb
 docs/examples/intro.ipynb
 docs/examples/ipyleaflet.ipynb
+docs/examples/ipywidgets.ipynb
 docs/examples/random.ipynb
+docs/examples/raster.ipynb
+docs/examples/toolbar.ipynb
 docs/examples/vector.ipynb
 docs/labs/lab4.ipynb
 docs/labs/lab5.ipynb
 docs/overrides/main.html
 docs/python/01_getting_started.ipynb
 docs/python/02_variables_data_types.ipynb
 docs/python/03_introducing_lists.ipynb
```

### Comparing `geohey-0.0.4/mkdocs.yml` & `geohey-0.0.5/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,21 @@
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
           execute: True
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["labs/lab5.ipynb", "labs/lab4.ipynb", "vector.ipynb"]
+          execute_ignore:
+              [
+                  "labs/lab5.ipynb",
+                  "labs/lab4.ipynb",
+                  "vector.ipynb",
+                  "raster.ipynb",
+              ]
 
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -84,14 +90,17 @@
           - common module: common.md
           - utils module: utils.md
     - Examples:
           - examples/intro.ipynb
           - examples/random.ipynb
           - examples/demo.ipynb
           - examples/csv.ipynb
+          - examples/ipywidgets.ipynb
+          - examples/raster.ipynb
+          - examples/toolbar.ipynb
     - Python Basics:
           - python/01_getting_started.ipynb
           - python/02_variables_data_types.ipynb
           - python/03_introducing_lists.ipynb
           - python/04_working_with_lists.ipynb
           - python/05_if_statements.ipynb
           - python/06_dictionaries.ipynb
```

### Comparing `geohey-0.0.4/pyproject.toml` & `geohey-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geohey"
-version = "0.0.4"
+version = "0.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package demo for geospatial analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.4"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

