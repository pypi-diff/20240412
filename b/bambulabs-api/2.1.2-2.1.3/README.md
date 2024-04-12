# Comparing `tmp/bambulabs_api-2.1.2.tar.gz` & `tmp/bambulabs_api-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambulabs_api-2.1.2.tar", last modified: Fri Apr 12 17:58:38 2024, max compression
+gzip compressed data, was "bambulabs_api-2.1.3.tar", last modified: Fri Apr 12 18:16:23 2024, max compression
```

## Comparing `bambulabs_api-2.1.2.tar` & `bambulabs_api-2.1.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.237133 bambulabs_api-2.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.241133 bambulabs_api-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/.github/workflows/pytest-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.241133 bambulabs_api-2.1.2/bambulabs_api/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/camera_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/filament_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/ftp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/bambulabs_api/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/bambulabs_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-12 17:58:38.000000 bambulabs_api-2.1.2/bambulabs_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 17:58:38.000000 bambulabs_api-2.1.2/bambulabs_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:58:38.000000 bambulabs_api-2.1.2/bambulabs_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 17:58:38.000000 bambulabs_api-2.1.2/bambulabs_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 17:58:38.000000 bambulabs_api-2.1.2/bambulabs_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.245133 bambulabs_api-2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.245133 bambulabs_api-2.1.2/docs/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   220931 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/.doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.245133 bambulabs_api-2.1.2/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.249133 bambulabs_api-2.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.249133 bambulabs_api-2.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.253134 bambulabs_api-2.1.2/docs/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/docs/doc_conf/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/doc_conf/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/doc_conf/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    74797 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/docs/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.241133 bambulabs_api-2.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/examples/Basic/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/examples/Basic/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:58:38.257134 bambulabs_api-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 17:58:33.000000 bambulabs_api-2.1.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.462942 bambulabs_api-2.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.466942 bambulabs_api-2.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/.github/workflows/pytest-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.470942 bambulabs_api-2.1.3/bambulabs_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/filament_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/ftp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/bambulabs_api/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/bambulabs_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 18:16:23.000000 bambulabs_api-2.1.3/bambulabs_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 18:16:23.000000 bambulabs_api-2.1.3/bambulabs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:16:23.000000 bambulabs_api-2.1.3/bambulabs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 18:16:23.000000 bambulabs_api-2.1.3/bambulabs_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 18:16:23.000000 bambulabs_api-2.1.3/bambulabs_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.470942 bambulabs_api-2.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.470942 bambulabs_api-2.1.3/docs/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   220931 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/.doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.470942 bambulabs_api-2.1.3/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.474942 bambulabs_api-2.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.474942 bambulabs_api-2.1.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/docs/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/docs/doc_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/doc_conf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/doc_conf/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    74797 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/docs/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.466942 bambulabs_api-2.1.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/examples/Basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/examples/Basic/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:16:23.482942 bambulabs_api-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 18:16:16.000000 bambulabs_api-2.1.3/tests/test_client.py
```

### Comparing `bambulabs_api-2.1.2/.github/workflows/flake8.yml` & `bambulabs_api-2.1.3/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/.github/workflows/publish.yml` & `bambulabs_api-2.1.3/.github/workflows/publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -64,18 +64,23 @@
         with:
           name: python-package-distributions
           path: dist/
       - name: Sign the dists with Sigstore
         uses: sigstore/gh-action-sigstore-python@v1.2.3
         with:
           inputs: ./dist/*.tar.gz ./dist/*.whl
-      - name: Get version from PyToml file
+      - name: Install dependencies
+        run: python3 -m pip install toml
+      - name: Get version from pyproject.toml file
         id: get_version
-        run: echo ::set-output name=version::$(python3 -c "import toml; print(toml.load('pyproject.toml')['project']['version'])")
+        run: |
+          version=$(python3 -c "import toml; print(toml.load('pyproject.toml')['project']['version'])")
+          echo "VERSION=${version}" >> $GITHUB_ENV
       - name: Create GitHub Release
         env:
-          GITHUB_TOKEN: ${{ github.token }}
-        run: gh release create "${{ steps.get_version.outputs.version }}" --repo "${{ github.repository }}" --notes ""
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        run: gh release create "${{ env.VERSION }}" --repo "${{ github.repository }}" --notes ""
       - name: Upload artifact signatures to GitHub Release
         env:
-          GITHUB_TOKEN: ${{ github.token }}
-        run: gh release upload "${{ steps.get_version.outputs.version }}" dist/** --repo "${{ github.repository }}"
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        run: gh release upload "${{ env.VERSION }}" dist/** --repo "${{ github.repository }}"
+
```

### Comparing `bambulabs_api-2.1.2/.github/workflows/pytest-unit-tests.yml` & `bambulabs_api-2.1.3/.github/workflows/pytest-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/.github/workflows/static.yml` & `bambulabs_api-2.1.3/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/.gitignore` & `bambulabs_api-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/LICENSE` & `bambulabs_api-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/PKG-INFO` & `bambulabs_api-2.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.1.2
+Version: 2.1.3
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
@@ -14,38 +14,67 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: paho-mqtt>=2.0.0
 
 # Bambulabs API
 
-This package provides a Python API for the Bambulabs 3D Printers via MQTT.
+This package provides a Python API for the Bambulabs 3D Printers.
 
 ## Status
 
 [![flake8](https://github.com/acse-ci223/bambulabs_api/actions/workflows/flake8.yml/badge.svg)](https://github.com/acse-ci223/bambulabs_api/actions/workflows/flake8.yml)
 
 [![pytest-unit-tests](https://github.com/acse-ci223/bambulabs_api/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/acse-ci223/bambulabs_api/actions/workflows/pytest-unit-tests.yml)
 
 [![GitHub Pages](https://github.com/acse-ci223/bambulabs_api/actions/workflows/static.yml/badge.svg)](https://github.com/acse-ci223/bambulabs_api/actions/workflows/static.yml)
 
 
-
 ## Documentation
 
 The documentation for this package can be found [here](https://acse-ci223.github.io/bambulabs_api/).
 
 ## Usage
 
 To use the package, run the following command in the terminal:
 
 ```bash
 pip install bambulabs_api
 ```
 
+## Examples
+
+```python
+import bambulabs_api as bl
+
+IP = '192.168.1.200'
+SERIAL = 'AC12309BH109'
+ACCESS_CODE = '12347890'
+
+if __name__ == '__main__':
+    print('Starting bambulabs_api example')
+    print('Connecting to Bambulabs 3D printer')
+    print(f'IP: {IP}')
+    print(f'Serial: {SERIAL}')
+    print(f'Access Code: {ACCESS_CODE}')
+
+    # Create a new instance of the API
+    printer = bl.Printer(IP, SERIAL, ACCESS_CODE)
+
+    # Connect to the Bambulabs 3D printer
+    printer.connect()
+
+    # Get the printer status
+    status = printer.get_state()
+    print(f'Printer status: {status}')
+
+    # Disconnect from the Bambulabs 3D printer
+    printer.disconnect()
+```
+
 ## Development
 
 To install the package, make sure conda is installed and then run the following commands in the terminal:
 
 ```bash
 # Clone the repository
 git clone https://github.com/acse-ci223/bambulabs_api.git
@@ -58,10 +87,7 @@
 
 # Activate the environment
 conda activate blapi
 
 # Install the package
 pip install -e .
 ```
-
-## Examples
-
```

### Comparing `bambulabs_api-2.1.2/bambulabs_api/camera_client.py` & `bambulabs_api-2.1.3/bambulabs_api/camera_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/bambulabs_api/client.py` & `bambulabs_api-2.1.3/bambulabs_api/client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/bambulabs_api/filament_info.py` & `bambulabs_api-2.1.3/bambulabs_api/filament_info.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/bambulabs_api/ftp_client.py` & `bambulabs_api-2.1.3/bambulabs_api/ftp_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/bambulabs_api/mqtt_client.py` & `bambulabs_api-2.1.3/bambulabs_api/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/bambulabs_api/states_info.py` & `bambulabs_api-2.1.3/bambulabs_api/states_info.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/bambulabs_api.egg-info/PKG-INFO` & `bambulabs_api-2.1.3/bambulabs_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.1.2
+Version: 2.1.3
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
@@ -14,38 +14,67 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: paho-mqtt>=2.0.0
 
 # Bambulabs API
 
-This package provides a Python API for the Bambulabs 3D Printers via MQTT.
+This package provides a Python API for the Bambulabs 3D Printers.
 
 ## Status
 
 [![flake8](https://github.com/acse-ci223/bambulabs_api/actions/workflows/flake8.yml/badge.svg)](https://github.com/acse-ci223/bambulabs_api/actions/workflows/flake8.yml)
 
 [![pytest-unit-tests](https://github.com/acse-ci223/bambulabs_api/actions/workflows/pytest-unit-tests.yml/badge.svg)](https://github.com/acse-ci223/bambulabs_api/actions/workflows/pytest-unit-tests.yml)
 
 [![GitHub Pages](https://github.com/acse-ci223/bambulabs_api/actions/workflows/static.yml/badge.svg)](https://github.com/acse-ci223/bambulabs_api/actions/workflows/static.yml)
 
 
-
 ## Documentation
 
 The documentation for this package can be found [here](https://acse-ci223.github.io/bambulabs_api/).
 
 ## Usage
 
 To use the package, run the following command in the terminal:
 
 ```bash
 pip install bambulabs_api
 ```
 
+## Examples
+
+```python
+import bambulabs_api as bl
+
+IP = '192.168.1.200'
+SERIAL = 'AC12309BH109'
+ACCESS_CODE = '12347890'
+
+if __name__ == '__main__':
+    print('Starting bambulabs_api example')
+    print('Connecting to Bambulabs 3D printer')
+    print(f'IP: {IP}')
+    print(f'Serial: {SERIAL}')
+    print(f'Access Code: {ACCESS_CODE}')
+
+    # Create a new instance of the API
+    printer = bl.Printer(IP, SERIAL, ACCESS_CODE)
+
+    # Connect to the Bambulabs 3D printer
+    printer.connect()
+
+    # Get the printer status
+    status = printer.get_state()
+    print(f'Printer status: {status}')
+
+    # Disconnect from the Bambulabs 3D printer
+    printer.disconnect()
+```
+
 ## Development
 
 To install the package, make sure conda is installed and then run the following commands in the terminal:
 
 ```bash
 # Clone the repository
 git clone https://github.com/acse-ci223/bambulabs_api.git
@@ -58,10 +87,7 @@
 
 # Activate the environment
 conda activate blapi
 
 # Install the package
 pip install -e .
 ```
-
-## Examples
-
```

### Comparing `bambulabs_api-2.1.2/bambulabs_api.egg-info/SOURCES.txt` & `bambulabs_api-2.1.3/bambulabs_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/.doctrees/environment.pickle` & `bambulabs_api-2.1.3/docs/.doctrees/environment.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -566,26 +566,26 @@
 00002350: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
 00002360: 6c65 7394 5d94 8c03 656e 7694 6803 8c1d  les.]...env.h...
 00002370: 7472 696d 5f66 6f6f 746e 6f74 655f 7265  trim_footnote_re
 00002380: 6665 7265 6e63 655f 7370 6163 6594 898c  ference_space...
 00002390: 0d6c 616e 6775 6167 655f 636f 6465 9468  .language_code.h
 000023a0: 508c 0c73 6d61 7274 5f71 756f 7465 7394  P..smart_quotes.
 000023b0: 8875 8c08 616c 6c5f 646f 6373 947d 946a  .u..all_docs.}.j
-000023c0: b302 0000 4741 d986 5b40 403c 0473 8c0c  ....GA..[@@<.s..
+000023c0: b302 0000 4741 d986 5e03 164d 1973 8c0c  ....GA..^..M.s..
 000023d0: 6465 7065 6e64 656e 6369 6573 948c 0b63  dependencies...c
 000023e0: 6f6c 6c65 6374 696f 6e73 948c 0b64 6566  ollections...def
 000023f0: 6175 6c74 6469 6374 9493 948c 0862 7569  aultdict.....bui
 00002400: 6c74 696e 7394 8c03 7365 7494 9394 8594  ltins...set.....
-00002410: 5294 6ab3 0200 008f 9428 8c22 2e2e 2f2e  R.j......(."../.
+00002410: 5294 6ab3 0200 008f 9428 8c1d 2e2e 2f2e  R.j......(..../.
 00002420: 2e2f 6261 6d62 756c 6162 735f 6170 692f  ./bambulabs_api/
-00002430: 7374 6174 6573 5f69 6e66 6f2e 7079 948c  states_info.py..
-00002440: 1d2e 2e2f 2e2e 2f62 616d 6275 6c61 6273  .../../bambulabs
-00002450: 5f61 7069 2f63 6c69 656e 742e 7079 948c  _api/client.py..
-00002460: 242e 2e2f 2e2e 2f62 616d 6275 6c61 6273  $../../bambulabs
-00002470: 5f61 7069 2f66 696c 616d 656e 745f 696e  _api/filament_in
+00002430: 636c 6965 6e74 2e70 7994 8c24 2e2e 2f2e  client.py..$../.
+00002440: 2e2f 6261 6d62 756c 6162 735f 6170 692f  ./bambulabs_api/
+00002450: 6669 6c61 6d65 6e74 5f69 6e66 6f2e 7079  filament_info.py
+00002460: 948c 222e 2e2f 2e2e 2f62 616d 6275 6c61  .."../../bambula
+00002470: 6273 5f61 7069 2f73 7461 7465 735f 696e  bs_api/states_in
 00002480: 666f 2e70 7994 9073 8c08 696e 636c 7564  fo.py..s..includ
 00002490: 6564 946a e402 0000 6ae7 0200 0085 9452  ed.j....j......R
 000024a0: 948c 0d72 6572 6561 645f 616c 7761 7973  ...reread_always
 000024b0: 948f 948c 086d 6574 6164 6174 6194 6ae4  .....metadata.j.
 000024c0: 0200 006a e502 0000 8c04 6469 6374 9493  ...j......dict..
 000024d0: 9485 9452 948c 0674 6974 6c65 7394 7d94  ...R...titles.}.
 000024e0: 6ab3 0200 008c 0e64 6f63 7574 696c 732e  j......docutils.
```

### Comparing `bambulabs_api-2.1.2/docs/.doctrees/index.doctree` & `bambulabs_api-2.1.3/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_sources/index.rst.txt` & `bambulabs_api-2.1.3/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/_sphinx_javascript_frameworks_compat.js` & `bambulabs_api-2.1.3/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/basic.css` & `bambulabs_api-2.1.3/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/badge_only.css` & `bambulabs_api-2.1.3/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.eot` & `bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.svg` & `bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.ttf` & `bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/fontawesome-webfont.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold-italic.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold-italic.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-bold.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal-italic.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal-italic.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal.woff` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/fonts/lato-normal.woff2` & `bambulabs_api-2.1.3/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/css/theme.css` & `bambulabs_api-2.1.3/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/doctools.js` & `bambulabs_api-2.1.3/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/jquery-3.6.0.js` & `bambulabs_api-2.1.3/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/jquery.js` & `bambulabs_api-2.1.3/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/js/badge_only.js` & `bambulabs_api-2.1.3/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/js/html5shiv-printshiv.min.js` & `bambulabs_api-2.1.3/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/js/html5shiv.min.js` & `bambulabs_api-2.1.3/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/js/theme.js` & `bambulabs_api-2.1.3/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/language_data.js` & `bambulabs_api-2.1.3/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/pygments.css` & `bambulabs_api-2.1.3/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/searchtools.js` & `bambulabs_api-2.1.3/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/underscore-1.13.1.js` & `bambulabs_api-2.1.3/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/_static/underscore.js` & `bambulabs_api-2.1.3/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/doc_conf/index.rst` & `bambulabs_api-2.1.3/docs/doc_conf/index.rst`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/genindex.html` & `bambulabs_api-2.1.3/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/index.html` & `bambulabs_api-2.1.3/docs/index.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/objects.inv` & `bambulabs_api-2.1.3/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/py-modindex.html` & `bambulabs_api-2.1.3/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/search.html` & `bambulabs_api-2.1.3/docs/search.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/docs/searchindex.js` & `bambulabs_api-2.1.3/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/examples/Basic/basic.py` & `bambulabs_api-2.1.3/examples/Basic/basic.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.2/pyproject.toml` & `bambulabs_api-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bambulabs_api"
-version = "2.1.2"
+version = "2.1.3"
 authors = [
   { name="Chris Ioannidis", email="chris.ioannidis23@imperial.ac.uk" },
 ]
 description = "API for BambuLabs 3D Printers over MQTT"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `bambulabs_api-2.1.2/setup.py` & `bambulabs_api-2.1.3/setup.py`

 * *Files identical despite different names*

