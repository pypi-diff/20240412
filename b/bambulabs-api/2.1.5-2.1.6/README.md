# Comparing `tmp/bambulabs_api-2.1.5.tar.gz` & `tmp/bambulabs_api-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambulabs_api-2.1.5.tar", last modified: Fri Apr 12 19:00:22 2024, max compression
+gzip compressed data, was "bambulabs_api-2.1.6.tar", last modified: Fri Apr 12 19:10:37 2024, max compression
```

## Comparing `bambulabs_api-2.1.5.tar` & `bambulabs_api-2.1.6.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.822347 bambulabs_api-2.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.826347 bambulabs_api-2.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/pytest-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.826347 bambulabs_api-2.1.5/bambulabs_api/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/camera_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/filament_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/ftp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/bambulabs_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.830347 bambulabs_api-2.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.830347 bambulabs_api-2.1.5/docs/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   220931 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/.doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.830347 bambulabs_api-2.1.5/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.834347 bambulabs_api-2.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.834347 bambulabs_api-2.1.5/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.838347 bambulabs_api-2.1.5/docs/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/docs/doc_conf/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/doc_conf/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/doc_conf/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    74797 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.826347 bambulabs_api-2.1.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/examples/Basic/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/examples/Basic/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.437961 bambulabs_api-2.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.417961 bambulabs_api-2.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.421961 bambulabs_api-2.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/.github/workflows/pytest-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 19:10:37.437961 bambulabs_api-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.421961 bambulabs_api-2.1.6/bambulabs_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/filament_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/ftp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/bambulabs_api/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.437961 bambulabs_api-2.1.6/bambulabs_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 19:10:37.000000 bambulabs_api-2.1.6/bambulabs_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 19:10:37.000000 bambulabs_api-2.1.6/bambulabs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:10:37.000000 bambulabs_api-2.1.6/bambulabs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 19:10:37.000000 bambulabs_api-2.1.6/bambulabs_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 19:10:37.000000 bambulabs_api-2.1.6/bambulabs_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.421961 bambulabs_api-2.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.421961 bambulabs_api-2.1.6/docs/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    32671 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   232408 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/.doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.425961 bambulabs_api-2.1.6/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.425961 bambulabs_api-2.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.425961 bambulabs_api-2.1.6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.433961 bambulabs_api-2.1.6/docs/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.433961 bambulabs_api-2.1.6/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.433961 bambulabs_api-2.1.6/docs/doc_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/doc_conf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/doc_conf/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21761 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    78296 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/docs/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.417961 bambulabs_api-2.1.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.433961 bambulabs_api-2.1.6/examples/Basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/examples/Basic/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:10:37.437961 bambulabs_api-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:10:37.437961 bambulabs_api-2.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 19:10:30.000000 bambulabs_api-2.1.6/tests/test_client.py
```

### Comparing `bambulabs_api-2.1.5/.github/workflows/flake8.yml` & `bambulabs_api-2.1.6/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/.github/workflows/publish.yml` & `bambulabs_api-2.1.6/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
         with:
           inputs: ./dist/*.tar.gz ./dist/*.whl
       - name: Install dependencies
         run: python3 -m pip install toml
       - name: Get version from pyproject.toml file
         id: get_version
         run: |
+          ls
           cd $GITHUB_WORKSPACE
+          ls
           version=$(python3 -c "import toml; print(toml.load('pyproject.toml')['project']['version'])")
           echo "VERSION=${version}" >> $GITHUB_ENV
       - name: Create GitHub Release
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: gh release create "${{ env.VERSION }}" --repo "${{ github.repository }}" --notes ""
       - name: Upload artifact signatures to GitHub Release
```

### Comparing `bambulabs_api-2.1.5/.github/workflows/pytest-unit-tests.yml` & `bambulabs_api-2.1.6/.github/workflows/pytest-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/.github/workflows/static.yml` & `bambulabs_api-2.1.6/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/.gitignore` & `bambulabs_api-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/LICENSE` & `bambulabs_api-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/PKG-INFO` & `bambulabs_api-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.1.5
+Version: 2.1.6
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
```

### Comparing `bambulabs_api-2.1.5/README.md` & `bambulabs_api-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api/camera_client.py` & `bambulabs_api-2.1.6/bambulabs_api/camera_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api/client.py` & `bambulabs_api-2.1.6/bambulabs_api/client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api/filament_info.py` & `bambulabs_api-2.1.6/bambulabs_api/filament_info.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api/ftp_client.py` & `bambulabs_api-2.1.6/bambulabs_api/ftp_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api/mqtt_client.py` & `bambulabs_api-2.1.6/bambulabs_api/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api/states_info.py` & `bambulabs_api-2.1.6/bambulabs_api/states_info.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/bambulabs_api.egg-info/PKG-INFO` & `bambulabs_api-2.1.6/bambulabs_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.1.5
+Version: 2.1.6
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
```

### Comparing `bambulabs_api-2.1.5/bambulabs_api.egg-info/SOURCES.txt` & `bambulabs_api-2.1.6/bambulabs_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/.doctrees/environment.pickle` & `bambulabs_api-2.1.6/docs/.doctrees/environment.pickle`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8005 95ae 7900 0000 0000 008c 1273 7068  ....y........sph
+00000000: 8005 9594 7f00 0000 0000 008c 1273 7068  .............sph
 00000010: 696e 782e 656e 7669 726f 6e6d 656e 7494  inx.environment.
 00000020: 8c10 4275 696c 6445 6e76 6972 6f6e 6d65  ..BuildEnvironme
 00000030: 6e74 9493 9429 8194 7d94 288c 0361 7070  nt...)..}.(..app
 00000040: 944e 8c0a 646f 6374 7265 6564 6972 948c  .N..doctreedir..
 00000050: 4343 3a5c 5573 6572 735c 6369 6372 695c  CC:\Users\cicri\
 00000060: 4465 736b 746f 705c 436f 6469 6e67 5c49  Desktop\Coding\I
 00000070: 6d70 6572 6961 6c5c 6261 6d62 756c 6162  mperial\bambulab
@@ -566,24 +566,24 @@
 00002350: 736d 6172 7471 756f 7465 735f 6c6f 6361  smartquotes_loca
 00002360: 6c65 7394 5d94 8c03 656e 7694 6803 8c1d  les.]...env.h...
 00002370: 7472 696d 5f66 6f6f 746e 6f74 655f 7265  trim_footnote_re
 00002380: 6665 7265 6e63 655f 7370 6163 6594 898c  ference_space...
 00002390: 0d6c 616e 6775 6167 655f 636f 6465 9468  .language_code.h
 000023a0: 508c 0c73 6d61 7274 5f71 756f 7465 7394  P..smart_quotes.
 000023b0: 8875 8c08 616c 6c5f 646f 6373 947d 946a  .u..all_docs.}.j
-000023c0: b302 0000 4741 d986 5e03 164d 1973 8c0c  ....GA..^..M.s..
+000023c0: b302 0000 4741 d986 618f 20c0 6a73 8c0c  ....GA..a. .js..
 000023d0: 6465 7065 6e64 656e 6369 6573 948c 0b63  dependencies...c
 000023e0: 6f6c 6c65 6374 696f 6e73 948c 0b64 6566  ollections...def
 000023f0: 6175 6c74 6469 6374 9493 948c 0862 7569  aultdict.....bui
 00002400: 6c74 696e 7394 8c03 7365 7494 9394 8594  ltins...set.....
-00002410: 5294 6ab3 0200 008f 9428 8c1d 2e2e 2f2e  R.j......(..../.
+00002410: 5294 6ab3 0200 008f 9428 8c24 2e2e 2f2e  R.j......(.$../.
 00002420: 2e2f 6261 6d62 756c 6162 735f 6170 692f  ./bambulabs_api/
-00002430: 636c 6965 6e74 2e70 7994 8c24 2e2e 2f2e  client.py..$../.
-00002440: 2e2f 6261 6d62 756c 6162 735f 6170 692f  ./bambulabs_api/
-00002450: 6669 6c61 6d65 6e74 5f69 6e66 6f2e 7079  filament_info.py
+00002430: 6669 6c61 6d65 6e74 5f69 6e66 6f2e 7079  filament_info.py
+00002440: 948c 1d2e 2e2f 2e2e 2f62 616d 6275 6c61  ...../../bambula
+00002450: 6273 5f61 7069 2f63 6c69 656e 742e 7079  bs_api/client.py
 00002460: 948c 222e 2e2f 2e2e 2f62 616d 6275 6c61  .."../../bambula
 00002470: 6273 5f61 7069 2f73 7461 7465 735f 696e  bs_api/states_in
 00002480: 666f 2e70 7994 9073 8c08 696e 636c 7564  fo.py..s..includ
 00002490: 6564 946a e402 0000 6ae7 0200 0085 9452  ed.j....j......R
 000024a0: 948c 0d72 6572 6561 645f 616c 7761 7973  ...reread_always
 000024b0: 948f 948c 086d 6574 6164 6174 6194 6ae4  .....metadata.j.
 000024c0: 0200 006a e502 0000 8c04 6469 6374 9493  ...j......dict..
@@ -751,1198 +751,1292 @@
 00002ee0: 005d 946a 0e03 0000 5d94 6a10 0300 005d  .].j....].j....]
 00002ef0: 946a 1203 0000 5d94 6a14 0300 005d 9475  .j....].j....].u
 00002f00: 6a16 0300 006a 2603 0000 6a09 0300 006a  j....j&...j....j
 00002f10: d903 0000 7562 616a 0a03 0000 7d94 286a  ....ubaj....}.(j
 00002f20: 0c03 0000 5d94 6a0e 0300 005d 946a 1003  ....].j....].j..
 00002f30: 0000 5d94 6a12 0300 005d 946a 1403 0000  ..].j....].j....
 00002f40: 5d94 756a 1603 0000 6a20 0300 006a 0903  ].uj....j ...j..
-00002f50: 0000 6a1d 0300 0075 6265 6a0a 0300 007d  ..j....ubej....}
-00002f60: 9428 6a0c 0300 005d 946a 0e03 0000 5d94  .(j....].j....].
-00002f70: 6a10 0300 005d 946a 1203 0000 5d94 6a14  j....].j....].j.
-00002f80: 0300 005d 9475 6a16 0300 006a 1b03 0000  ...].uj....j....
-00002f90: 7562 738c 0f74 6f63 5f6e 756d 5f65 6e74  ubs..toc_num_ent
-00002fa0: 7269 6573 947d 946a b302 0000 4b06 738c  ries.}.j....K.s.
-00002fb0: 0e74 6f63 5f73 6563 6e75 6d62 6572 7394  .toc_secnumbers.
-00002fc0: 7d94 8c0e 746f 635f 6669 676e 756d 6265  }...toc_fignumbe
-00002fd0: 7273 947d 948c 1074 6f63 7472 6565 5f69  rs.}...toctree_i
-00002fe0: 6e63 6c75 6465 7394 7d94 8c10 6669 6c65  ncludes.}...file
-00002ff0: 735f 746f 5f72 6562 7569 6c64 947d 948c  s_to_rebuild.}..
-00003000: 0d67 6c6f 625f 746f 6374 7265 6573 948f  .glob_toctrees..
-00003010: 948c 116e 756d 6265 7265 645f 746f 6374  ...numbered_toct
-00003020: 7265 6573 948f 948c 0a64 6f6d 6169 6e64  rees.....domaind
-00003030: 6174 6194 7d94 288c 0163 947d 9428 8c0b  ata.}.(..c.}.(..
-00003040: 726f 6f74 5f73 796d 626f 6c94 6ab6 0200  root_symbol.j...
-00003050: 008c 0653 796d 626f 6c94 9394 2981 947d  ...Symbol...)..}
-00003060: 9428 6a09 0300 004e 8c0c 7369 626c 696e  .(j....N..siblin
-00003070: 6741 626f 7665 944e 8c0c 7369 626c 696e  gAbove.N..siblin
-00003080: 6742 656c 6f77 944e 8c05 6964 656e 7494  gBelow.N..ident.
-00003090: 4e8c 0b64 6563 6c61 7261 7469 6f6e 944e  N..declaration.N
-000030a0: 8c07 646f 636e 616d 6594 4e8c 046c 696e  ..docname.N..lin
-000030b0: 6594 4e8c 0f69 7352 6564 6563 6c61 7261  e.N..isRedeclara
-000030c0: 7469 6f6e 9489 8c09 5f63 6869 6c64 7265  tion...._childre
-000030d0: 6e94 5d94 8c0d 5f61 6e6f 6e43 6869 6c64  n.]..._anonChild
-000030e0: 7265 6e94 5d94 7562 8c07 6f62 6a65 6374  ren.].ub..object
-000030f0: 7394 7d94 6ab4 0200 004b 0075 8c09 6368  s.}.j....K.u..ch
-00003100: 616e 6765 7365 7494 7d94 288c 0763 6861  angeset.}.(..cha
-00003110: 6e67 6573 947d 946a b402 0000 4b00 758c  nges.}.j....K.u.
-00003120: 0863 6974 6174 696f 6e94 7d94 286a b402  .citation.}.(j..
-00003130: 0000 4b00 8c09 6369 7461 7469 6f6e 7394  ..K...citations.
-00003140: 7d94 8c0d 6369 7461 7469 6f6e 5f72 6566  }...citation_ref
-00003150: 7394 7d94 758c 0363 7070 947d 9428 6a15  s.}.u..cpp.}.(j.
-00003160: 0400 006a b902 0000 6a16 0400 0093 9429  ...j....j......)
-00003170: 8194 7d94 286a 0903 0000 4e6a 1a04 0000  ..}.(j....Nj....
-00003180: 4e6a 1b04 0000 4e8c 0969 6465 6e74 4f72  Nj....N..identOr
-00003190: 4f70 944e 8c0e 7465 6d70 6c61 7465 5061  Op.N..templatePa
-000031a0: 7261 6d73 944e 8c0c 7465 6d70 6c61 7465  rams.N..template
-000031b0: 4172 6773 944e 6a1d 0400 004e 6a1e 0400  Args.Nj....Nj...
-000031c0: 004e 6a1f 0400 004e 6a20 0400 0089 6a21  .Nj....Nj ....j!
-000031d0: 0400 005d 946a 2304 0000 5d94 7562 8c05  ...].j#...].ub..
-000031e0: 6e61 6d65 7394 7d94 6ab4 0200 004b 0075  names.}.j....K.u
-000031f0: 8c05 696e 6465 7894 7d94 286a b402 0000  ..index.}.(j....
-00003200: 4b00 8c07 656e 7472 6965 7394 7d94 6ab3  K...entries.}.j.
-00003210: 0200 005d 9428 288c 0470 6169 7294 8c1d  ...].((..pair...
-00003220: 6d6f 6475 6c65 3b20 6261 6d62 756c 6162  module; bambulab
-00003230: 735f 6170 692e 5072 696e 7465 7294 8c1c  s_api.Printer...
-00003240: 6d6f 6475 6c65 2d62 616d 6275 6c61 6273  module-bambulabs
-00003250: 5f61 7069 2e50 7269 6e74 6572 9468 424e  _api.Printer.hBN
-00003260: 7494 288c 0673 696e 676c 6594 8c35 6361  t.(..single..5ca
-00003270: 6c69 6272 6174 655f 7072 696e 7465 7228  librate_printer(
-00003280: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
-00003290: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-000032a0: 6572 2994 8c27 6261 6d62 756c 6162 735f  er)..'bambulabs_
-000032b0: 6170 692e 5072 696e 7465 722e 6361 6c69  api.Printer.cali
-000032c0: 6272 6174 655f 7072 696e 7465 7294 6842  brate_printer.hB
-000032d0: 4e74 9428 6a46 0400 008c 2b63 6f6e 6e65  Nt.(jF....+conne
-000032e0: 6374 2829 2028 696e 206d 6f64 756c 6520  ct() (in module 
-000032f0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00003300: 696e 7465 7229 948c 1d62 616d 6275 6c61  inter)...bambula
-00003310: 6273 5f61 7069 2e50 7269 6e74 6572 2e63  bs_api.Printer.c
-00003320: 6f6e 6e65 6374 9468 424e 7494 286a 4604  onnect.hBNt.(jF.
-00003330: 0000 8c2f 6465 6c65 7465 5f66 696c 6528  .../delete_file(
-00003340: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
-00003350: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00003360: 6572 2994 8c21 6261 6d62 756c 6162 735f  er)..!bambulabs_
-00003370: 6170 692e 5072 696e 7465 722e 6465 6c65  api.Printer.dele
-00003380: 7465 5f66 696c 6594 6842 4e74 9428 6a46  te_file.hBNt.(jF
-00003390: 0400 008c 2e64 6973 636f 6e6e 6563 7428  .....disconnect(
-000033a0: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
-000033b0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-000033c0: 6572 2994 8c20 6261 6d62 756c 6162 735f  er).. bambulabs_
-000033d0: 6170 692e 5072 696e 7465 722e 6469 7363  api.Printer.disc
-000033e0: 6f6e 6e65 6374 9468 424e 7494 286a 4604  onnect.hBNt.(jF.
-000033f0: 0000 8c37 6765 745f 6265 645f 7465 6d70  ...7get_bed_temp
-00003400: 6572 6174 7572 6528 2920 2869 6e20 6d6f  erature() (in mo
-00003410: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
-00003420: 7069 2e50 7269 6e74 6572 2994 8c29 6261  pi.Printer)..)ba
-00003430: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00003440: 7465 722e 6765 745f 6265 645f 7465 6d70  ter.get_bed_temp
-00003450: 6572 6174 7572 6594 6842 4e74 9428 6a46  erature.hBNt.(jF
-00003460: 0400 008c 3467 6574 5f63 616d 6572 615f  ....4get_camera_
-00003470: 6672 616d 6528 2920 2869 6e20 6d6f 6475  frame() (in modu
-00003480: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00003490: 2e50 7269 6e74 6572 2994 8c26 6261 6d62  .Printer)..&bamb
-000034a0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-000034b0: 722e 6765 745f 6361 6d65 7261 5f66 7261  r.get_camera_fra
-000034c0: 6d65 9468 424e 7494 286a 4604 0000 8c31  me.hBNt.(jF....1
-000034d0: 6765 745f 6669 6c65 5f6e 616d 6528 2920  get_file_name() 
-000034e0: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
-000034f0: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
-00003500: 2994 8c23 6261 6d62 756c 6162 735f 6170  )..#bambulabs_ap
-00003510: 692e 5072 696e 7465 722e 6765 745f 6669  i.Printer.get_fi
-00003520: 6c65 5f6e 616d 6594 6842 4e74 9428 6a46  le_name.hBNt.(jF
-00003530: 0400 008c 3367 6574 5f6c 6967 6874 5f73  ....3get_light_s
-00003540: 7461 7465 2829 2028 696e 206d 6f64 756c  tate() (in modul
-00003550: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-00003560: 5072 696e 7465 7229 948c 2562 616d 6275  Printer)..%bambu
-00003570: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
-00003580: 2e67 6574 5f6c 6967 6874 5f73 7461 7465  .get_light_state
-00003590: 9468 424e 7494 286a 4604 0000 8c3a 6765  .hBNt.(jF....:ge
-000035a0: 745f 6e6f 7a7a 6c65 5f74 656d 7065 7261  t_nozzle_tempera
-000035b0: 7475 7265 2829 2028 696e 206d 6f64 756c  ture() (in modul
-000035c0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-000035d0: 5072 696e 7465 7229 948c 2c62 616d 6275  Printer)..,bambu
-000035e0: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
-000035f0: 2e67 6574 5f6e 6f7a 7a6c 655f 7465 6d70  .get_nozzle_temp
-00003600: 6572 6174 7572 6594 6842 4e74 9428 6a46  erature.hBNt.(jF
-00003610: 0400 008c 3267 6574 5f70 6572 6365 6e74  ....2get_percent
-00003620: 6167 6528 2920 2869 6e20 6d6f 6475 6c65  age() (in module
-00003630: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
-00003640: 7269 6e74 6572 2994 8c24 6261 6d62 756c  rinter)..$bambul
-00003650: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
-00003660: 6765 745f 7065 7263 656e 7461 6765 9468  get_percentage.h
-00003670: 424e 7494 286a 4604 0000 8c33 6765 745f  BNt.(jF....3get_
-00003680: 7072 696e 745f 7370 6565 6428 2920 2869  print_speed() (i
-00003690: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
-000036a0: 6273 5f61 7069 2e50 7269 6e74 6572 2994  bs_api.Printer).
-000036b0: 8c25 6261 6d62 756c 6162 735f 6170 692e  .%bambulabs_api.
-000036c0: 5072 696e 7465 722e 6765 745f 7072 696e  Printer.get_prin
-000036d0: 745f 7370 6565 6494 6842 4e74 9428 6a46  t_speed.hBNt.(jF
-000036e0: 0400 008c 2d67 6574 5f73 7461 7465 2829  ....-get_state()
-000036f0: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
-00003700: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00003710: 7229 948c 1f62 616d 6275 6c61 6273 5f61  r)...bambulabs_a
-00003720: 7069 2e50 7269 6e74 6572 2e67 6574 5f73  pi.Printer.get_s
-00003730: 7461 7465 9468 424e 7494 286a 4604 0000  tate.hBNt.(jF...
-00003740: 8c2c 6765 745f 7469 6d65 2829 2028 696e  .,get_time() (in
-00003750: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00003760: 735f 6170 692e 5072 696e 7465 7229 948c  s_api.Printer)..
-00003770: 1e62 616d 6275 6c61 6273 5f61 7069 2e50  .bambulabs_api.P
-00003780: 7269 6e74 6572 2e67 6574 5f74 696d 6594  rinter.get_time.
-00003790: 6842 4e74 9428 6a46 0400 008c 3068 6f6d  hBNt.(jF....0hom
-000037a0: 655f 7072 696e 7465 7228 2920 2869 6e20  e_printer() (in 
-000037b0: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
-000037c0: 5f61 7069 2e50 7269 6e74 6572 2994 8c22  _api.Printer).."
-000037d0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-000037e0: 696e 7465 722e 686f 6d65 5f70 7269 6e74  inter.home_print
-000037f0: 6572 9468 424e 7494 286a 4604 0000 8c37  er.hBNt.(jF....7
-00003800: 6c6f 6164 5f66 696c 616d 656e 745f 7370  load_filament_sp
-00003810: 6f6f 6c28 2920 2869 6e20 6d6f 6475 6c65  ool() (in module
-00003820: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
-00003830: 7269 6e74 6572 2994 8c29 6261 6d62 756c  rinter)..)bambul
-00003840: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
-00003850: 6c6f 6164 5f66 696c 616d 656e 745f 7370  load_filament_sp
-00003860: 6f6f 6c94 6842 4e74 9428 6a46 0400 008c  ool.hBNt.(jF....
-00003870: 2f6d 6f76 655f 7a5f 6178 6973 2829 2028  /move_z_axis() (
-00003880: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
-00003890: 6162 735f 6170 692e 5072 696e 7465 7229  abs_api.Printer)
-000038a0: 948c 2162 616d 6275 6c61 6273 5f61 7069  ..!bambulabs_api
-000038b0: 2e50 7269 6e74 6572 2e6d 6f76 655f 7a5f  .Printer.move_z_
-000038c0: 6178 6973 9468 424e 7494 286a 4604 0000  axis.hBNt.(jF...
-000038d0: 8c2f 7061 7573 655f 7072 696e 7428 2920  ./pause_print() 
-000038e0: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
-000038f0: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
-00003900: 2994 8c21 6261 6d62 756c 6162 735f 6170  )..!bambulabs_ap
-00003910: 692e 5072 696e 7465 722e 7061 7573 655f  i.Printer.pause_
-00003920: 7072 696e 7494 6842 4e74 9428 6a46 0400  print.hBNt.(jF..
-00003930: 008c 3072 6573 756d 655f 7072 696e 7428  ..0resume_print(
-00003940: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
-00003950: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00003960: 6572 2994 8c22 6261 6d62 756c 6162 735f  er).."bambulabs_
-00003970: 6170 692e 5072 696e 7465 722e 7265 7375  api.Printer.resu
-00003980: 6d65 5f70 7269 6e74 9468 424e 7494 286a  me_print.hBNt.(j
-00003990: 4604 0000 8c39 7265 7472 795f 6669 6c61  F....9retry_fila
-000039a0: 6d65 6e74 5f61 6374 696f 6e28 2920 2869  ment_action() (i
-000039b0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
-000039c0: 6273 5f61 7069 2e50 7269 6e74 6572 2994  bs_api.Printer).
-000039d0: 8c2b 6261 6d62 756c 6162 735f 6170 692e  .+bambulabs_api.
-000039e0: 5072 696e 7465 722e 7265 7472 795f 6669  Printer.retry_fi
-000039f0: 6c61 6d65 6e74 5f61 6374 696f 6e94 6842  lament_action.hB
-00003a00: 4e74 9428 6a46 0400 008c 3773 6574 5f62  Nt.(jF....7set_b
-00003a10: 6564 5f74 656d 7065 7261 7475 7265 2829  ed_temperature()
-00003a20: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
-00003a30: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00003a40: 7229 948c 2962 616d 6275 6c61 6273 5f61  r)..)bambulabs_a
-00003a50: 7069 2e50 7269 6e74 6572 2e73 6574 5f62  pi.Printer.set_b
-00003a60: 6564 5f74 656d 7065 7261 7475 7265 9468  ed_temperature.h
-00003a70: 424e 7494 286a 4604 0000 8c38 7365 745f  BNt.(jF....8set_
-00003a80: 6669 6c61 6d65 6e74 5f70 7269 6e74 6572  filament_printer
-00003a90: 2829 2028 696e 206d 6f64 756c 6520 6261  () (in module ba
-00003aa0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00003ab0: 7465 7229 948c 2a62 616d 6275 6c61 6273  ter)..*bambulabs
-00003ac0: 5f61 7069 2e50 7269 6e74 6572 2e73 6574  _api.Printer.set
-00003ad0: 5f66 696c 616d 656e 745f 7072 696e 7465  _filament_printe
-00003ae0: 7294 6842 4e74 9428 6a46 0400 008c 3a73  r.hBNt.(jF....:s
-00003af0: 6574 5f6e 6f7a 7a6c 655f 7465 6d70 6572  et_nozzle_temper
-00003b00: 6174 7572 6528 2920 2869 6e20 6d6f 6475  ature() (in modu
-00003b10: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00003b20: 2e50 7269 6e74 6572 2994 8c2c 6261 6d62  .Printer)..,bamb
-00003b30: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00003b40: 722e 7365 745f 6e6f 7a7a 6c65 5f74 656d  r.set_nozzle_tem
-00003b50: 7065 7261 7475 7265 9468 424e 7494 286a  perature.hBNt.(j
-00003b60: 4604 0000 8c33 7365 745f 7072 696e 745f  F....3set_print_
-00003b70: 7370 6565 6428 2920 2869 6e20 6d6f 6475  speed() (in modu
-00003b80: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00003b90: 2e50 7269 6e74 6572 2994 8c25 6261 6d62  .Printer)..%bamb
-00003ba0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00003bb0: 722e 7365 745f 7072 696e 745f 7370 6565  r.set_print_spee
-00003bc0: 6494 6842 4e74 9428 6a46 0400 008c 2f73  d.hBNt.(jF..../s
-00003bd0: 7461 7274 5f70 7269 6e74 2829 2028 696e  tart_print() (in
-00003be0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00003bf0: 735f 6170 692e 5072 696e 7465 7229 948c  s_api.Printer)..
-00003c00: 2162 616d 6275 6c61 6273 5f61 7069 2e50  !bambulabs_api.P
-00003c10: 7269 6e74 6572 2e73 7461 7274 5f70 7269  rinter.start_pri
-00003c20: 6e74 9468 424e 7494 286a 4604 0000 8c2e  nt.hBNt.(jF.....
-00003c30: 7374 6f70 5f70 7269 6e74 2829 2028 696e  stop_print() (in
-00003c40: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00003c50: 735f 6170 692e 5072 696e 7465 7229 948c  s_api.Printer)..
-00003c60: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
-00003c70: 7269 6e74 6572 2e73 746f 705f 7072 696e  rinter.stop_prin
-00003c80: 7494 6842 4e74 9428 6a46 0400 008c 3274  t.hBNt.(jF....2t
-00003c90: 7572 6e5f 6c69 6768 745f 6f66 6628 2920  urn_light_off() 
-00003ca0: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
-00003cb0: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
-00003cc0: 2994 8c24 6261 6d62 756c 6162 735f 6170  )..$bambulabs_ap
-00003cd0: 692e 5072 696e 7465 722e 7475 726e 5f6c  i.Printer.turn_l
-00003ce0: 6967 6874 5f6f 6666 9468 424e 7494 286a  ight_off.hBNt.(j
-00003cf0: 4604 0000 8c31 7475 726e 5f6c 6967 6874  F....1turn_light
-00003d00: 5f6f 6e28 2920 2869 6e20 6d6f 6475 6c65  _on() (in module
-00003d10: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
-00003d20: 7269 6e74 6572 2994 8c23 6261 6d62 756c  rinter)..#bambul
-00003d30: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
-00003d40: 7475 726e 5f6c 6967 6874 5f6f 6e94 6842  turn_light_on.hB
-00003d50: 4e74 9428 6a46 0400 008c 3975 6e6c 6f61  Nt.(jF....9unloa
-00003d60: 645f 6669 6c61 6d65 6e74 5f73 706f 6f6c  d_filament_spool
-00003d70: 2829 2028 696e 206d 6f64 756c 6520 6261  () (in module ba
-00003d80: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00003d90: 7465 7229 948c 2b62 616d 6275 6c61 6273  ter)..+bambulabs
-00003da0: 5f61 7069 2e50 7269 6e74 6572 2e75 6e6c  _api.Printer.unl
-00003db0: 6f61 645f 6669 6c61 6d65 6e74 5f73 706f  oad_filament_spo
-00003dc0: 6f6c 9468 424e 7494 286a 4604 0000 8c2f  ol.hBNt.(jF..../
-00003dd0: 7570 6c6f 6164 5f66 696c 6528 2920 2869  upload_file() (i
-00003de0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
-00003df0: 6273 5f61 7069 2e50 7269 6e74 6572 2994  bs_api.Printer).
-00003e00: 8c21 6261 6d62 756c 6162 735f 6170 692e  .!bambulabs_api.
-00003e10: 5072 696e 7465 722e 7570 6c6f 6164 5f66  Printer.upload_f
-00003e20: 696c 6594 6842 4e74 9428 6a42 0400 008c  ile.hBNt.(jB....
-00003e30: 1e6d 6f64 756c 653b 2062 616d 6275 6c61  .module; bambula
-00003e40: 6273 5f61 7069 2e46 696c 616d 656e 7494  bs_api.Filament.
-00003e50: 8c1d 6d6f 6475 6c65 2d62 616d 6275 6c61  ..module-bambula
-00003e60: 6273 5f61 7069 2e46 696c 616d 656e 7494  bs_api.Filament.
-00003e70: 6842 4e74 9428 6a46 0400 008c 2f50 4f4c  hBNt.(jF..../POL
-00003e80: 594c 4954 455f 504c 4120 2869 6e20 6d6f  YLITE_PLA (in mo
-00003e90: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
-00003ea0: 7069 2e46 696c 616d 656e 7429 948c 2362  pi.Filament)..#b
-00003eb0: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-00003ec0: 616d 656e 742e 504f 4c59 4c49 5445 5f50  ament.POLYLITE_P
-00003ed0: 4c41 9468 424e 7494 286a 4604 0000 8c30  LA.hBNt.(jF....0
-00003ee0: 504f 4c59 5445 5252 415f 504c 4120 2869  POLYTERRA_PLA (i
-00003ef0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
-00003f00: 6273 5f61 7069 2e46 696c 616d 656e 7429  bs_api.Filament)
-00003f10: 948c 2462 616d 6275 6c61 6273 5f61 7069  ..$bambulabs_api
-00003f20: 2e46 696c 616d 656e 742e 504f 4c59 5445  .Filament.POLYTE
-00003f30: 5252 415f 504c 4194 6842 4e74 9428 6a46  RRA_PLA.hBNt.(jF
-00003f40: 0400 008c 2c42 414d 4255 5f41 4253 2028  ....,BAMBU_ABS (
-00003f50: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
-00003f60: 6162 735f 6170 692e 4669 6c61 6d65 6e74  abs_api.Filament
-00003f70: 2994 8c20 6261 6d62 756c 6162 735f 6170  ).. bambulabs_ap
-00003f80: 692e 4669 6c61 6d65 6e74 2e42 414d 4255  i.Filament.BAMBU
-00003f90: 5f41 4253 9468 424e 7494 286a 4604 0000  _ABS.hBNt.(jF...
-00003fa0: 8c2e 4241 4d42 555f 5041 5f43 4620 2869  ..BAMBU_PA_CF (i
-00003fb0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
-00003fc0: 6273 5f61 7069 2e46 696c 616d 656e 7429  bs_api.Filament)
-00003fd0: 948c 2262 616d 6275 6c61 6273 5f61 7069  .."bambulabs_api
-00003fe0: 2e46 696c 616d 656e 742e 4241 4d42 555f  .Filament.BAMBU_
-00003ff0: 5041 5f43 4694 6842 4e74 9428 6a46 0400  PA_CF.hBNt.(jF..
-00004000: 008c 2b42 414d 4255 5f50 4320 2869 6e20  ..+BAMBU_PC (in 
-00004010: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
-00004020: 5f61 7069 2e46 696c 616d 656e 7429 948c  _api.Filament)..
-00004030: 1f62 616d 6275 6c61 6273 5f61 7069 2e46  .bambulabs_api.F
-00004040: 696c 616d 656e 742e 4241 4d42 555f 5043  ilament.BAMBU_PC
-00004050: 9468 424e 7494 286a 4604 0000 8c32 4241  .hBNt.(jF....2BA
-00004060: 4d42 555f 504c 415f 4261 7369 6320 2869  MBU_PLA_Basic (i
+00002f50: 0000 6a1d 0300 0075 626a 2103 0000 2981  ..j....ubj!...).
+00002f60: 947d 9428 6aff 0200 0068 426a 0003 0000  .}.(j....hBj....
+00002f70: 5d94 6a27 0300 0029 8194 7d94 286a ff02  ].j'...)..}.(j..
+00002f80: 0000 6842 6a00 0300 005d 946a 2c03 0000  ..hBj....].j,...
+00002f90: 2981 947d 9428 6aff 0200 0068 426a 0003  )..}.(j....hBj..
+00002fa0: 0000 5d94 6a03 0300 008c 0a47 636f 6465  ..].j......Gcode
+00002fb0: 5374 6174 6594 8594 8194 7d94 286a ff02  State.....}.(j..
+00002fc0: 0000 8c0a 4763 6f64 6553 7461 7465 946a  ....GcodeState.j
+00002fd0: 0903 0000 6a03 0400 0075 6261 6a0a 0300  ....j....ubaj...
+00002fe0: 007d 9428 6a0c 0300 005d 946a 0e03 0000  .}.(j....].j....
+00002ff0: 5d94 6a10 0300 005d 946a 1203 0000 5d94  ].j....].j....].
+00003000: 6a14 0300 005d 948c 0869 6e74 6572 6e61  j....]...interna
+00003010: 6c94 888c 0672 6566 7572 6994 6ab3 0200  l....refuri.j...
+00003020: 008c 0a61 6e63 686f 726e 616d 6594 8c0b  ...anchorname...
+00003030: 2367 636f 6465 7374 6174 6594 756a 1603  #gcodestate.uj..
+00003040: 0000 6a2b 0300 006a 0903 0000 6a00 0400  ..j+...j....j...
+00003050: 0075 6261 6a0a 0300 007d 9428 6a0c 0300  .ubaj....}.(j...
+00003060: 005d 946a 0e03 0000 5d94 6a10 0300 005d  .].j....].j....]
+00003070: 946a 1203 0000 5d94 6a14 0300 005d 9475  .j....].j....].u
+00003080: 6a16 0300 006a 2603 0000 6a09 0300 006a  j....j&...j....j
+00003090: fd03 0000 7562 616a 0a03 0000 7d94 286a  ....ubaj....}.(j
+000030a0: 0c03 0000 5d94 6a0e 0300 005d 946a 1003  ....].j....].j..
+000030b0: 0000 5d94 6a12 0300 005d 946a 1403 0000  ..].j....].j....
+000030c0: 5d94 756a 1603 0000 6a20 0300 006a 0903  ].uj....j ...j..
+000030d0: 0000 6a1d 0300 0075 6265 6a0a 0300 007d  ..j....ubej....}
+000030e0: 9428 6a0c 0300 005d 946a 0e03 0000 5d94  .(j....].j....].
+000030f0: 6a10 0300 005d 946a 1203 0000 5d94 6a14  j....].j....].j.
+00003100: 0300 005d 9475 6a16 0300 006a 1b03 0000  ...].uj....j....
+00003110: 7562 738c 0f74 6f63 5f6e 756d 5f65 6e74  ubs..toc_num_ent
+00003120: 7269 6573 947d 946a b302 0000 4b07 738c  ries.}.j....K.s.
+00003130: 0e74 6f63 5f73 6563 6e75 6d62 6572 7394  .toc_secnumbers.
+00003140: 7d94 8c0e 746f 635f 6669 676e 756d 6265  }...toc_fignumbe
+00003150: 7273 947d 948c 1074 6f63 7472 6565 5f69  rs.}...toctree_i
+00003160: 6e63 6c75 6465 7394 7d94 8c10 6669 6c65  ncludes.}...file
+00003170: 735f 746f 5f72 6562 7569 6c64 947d 948c  s_to_rebuild.}..
+00003180: 0d67 6c6f 625f 746f 6374 7265 6573 948f  .glob_toctrees..
+00003190: 948c 116e 756d 6265 7265 645f 746f 6374  ...numbered_toct
+000031a0: 7265 6573 948f 948c 0a64 6f6d 6169 6e64  rees.....domaind
+000031b0: 6174 6194 7d94 288c 0163 947d 9428 8c0b  ata.}.(..c.}.(..
+000031c0: 726f 6f74 5f73 796d 626f 6c94 6ab6 0200  root_symbol.j...
+000031d0: 008c 0653 796d 626f 6c94 9394 2981 947d  ...Symbol...)..}
+000031e0: 9428 6a09 0300 004e 8c0c 7369 626c 696e  .(j....N..siblin
+000031f0: 6741 626f 7665 944e 8c0c 7369 626c 696e  gAbove.N..siblin
+00003200: 6742 656c 6f77 944e 8c05 6964 656e 7494  gBelow.N..ident.
+00003210: 4e8c 0b64 6563 6c61 7261 7469 6f6e 944e  N..declaration.N
+00003220: 8c07 646f 636e 616d 6594 4e8c 046c 696e  ..docname.N..lin
+00003230: 6594 4e8c 0f69 7352 6564 6563 6c61 7261  e.N..isRedeclara
+00003240: 7469 6f6e 9489 8c09 5f63 6869 6c64 7265  tion...._childre
+00003250: 6e94 5d94 8c0d 5f61 6e6f 6e43 6869 6c64  n.]..._anonChild
+00003260: 7265 6e94 5d94 7562 8c07 6f62 6a65 6374  ren.].ub..object
+00003270: 7394 7d94 6ab4 0200 004b 0075 8c09 6368  s.}.j....K.u..ch
+00003280: 616e 6765 7365 7494 7d94 288c 0763 6861  angeset.}.(..cha
+00003290: 6e67 6573 947d 946a b402 0000 4b00 758c  nges.}.j....K.u.
+000032a0: 0863 6974 6174 696f 6e94 7d94 286a b402  .citation.}.(j..
+000032b0: 0000 4b00 8c09 6369 7461 7469 6f6e 7394  ..K...citations.
+000032c0: 7d94 8c0d 6369 7461 7469 6f6e 5f72 6566  }...citation_ref
+000032d0: 7394 7d94 758c 0363 7070 947d 9428 6a39  s.}.u..cpp.}.(j9
+000032e0: 0400 006a b902 0000 6a3a 0400 0093 9429  ...j....j:.....)
+000032f0: 8194 7d94 286a 0903 0000 4e6a 3e04 0000  ..}.(j....Nj>...
+00003300: 4e6a 3f04 0000 4e8c 0969 6465 6e74 4f72  Nj?...N..identOr
+00003310: 4f70 944e 8c0e 7465 6d70 6c61 7465 5061  Op.N..templatePa
+00003320: 7261 6d73 944e 8c0c 7465 6d70 6c61 7465  rams.N..template
+00003330: 4172 6773 944e 6a41 0400 004e 6a42 0400  Args.NjA...NjB..
+00003340: 004e 6a43 0400 004e 6a44 0400 0089 6a45  .NjC...NjD....jE
+00003350: 0400 005d 946a 4704 0000 5d94 7562 8c05  ...].jG...].ub..
+00003360: 6e61 6d65 7394 7d94 6ab4 0200 004b 0075  names.}.j....K.u
+00003370: 8c05 696e 6465 7894 7d94 286a b402 0000  ..index.}.(j....
+00003380: 4b00 8c07 656e 7472 6965 7394 7d94 6ab3  K...entries.}.j.
+00003390: 0200 005d 9428 288c 0470 6169 7294 8c1d  ...].((..pair...
+000033a0: 6d6f 6475 6c65 3b20 6261 6d62 756c 6162  module; bambulab
+000033b0: 735f 6170 692e 5072 696e 7465 7294 8c1c  s_api.Printer...
+000033c0: 6d6f 6475 6c65 2d62 616d 6275 6c61 6273  module-bambulabs
+000033d0: 5f61 7069 2e50 7269 6e74 6572 9468 424e  _api.Printer.hBN
+000033e0: 7494 288c 0673 696e 676c 6594 8c35 6361  t.(..single..5ca
+000033f0: 6c69 6272 6174 655f 7072 696e 7465 7228  librate_printer(
+00003400: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
+00003410: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00003420: 6572 2994 8c27 6261 6d62 756c 6162 735f  er)..'bambulabs_
+00003430: 6170 692e 5072 696e 7465 722e 6361 6c69  api.Printer.cali
+00003440: 6272 6174 655f 7072 696e 7465 7294 6842  brate_printer.hB
+00003450: 4e74 9428 6a6a 0400 008c 2b63 6f6e 6e65  Nt.(jj....+conne
+00003460: 6374 2829 2028 696e 206d 6f64 756c 6520  ct() (in module 
+00003470: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+00003480: 696e 7465 7229 948c 1d62 616d 6275 6c61  inter)...bambula
+00003490: 6273 5f61 7069 2e50 7269 6e74 6572 2e63  bs_api.Printer.c
+000034a0: 6f6e 6e65 6374 9468 424e 7494 286a 6a04  onnect.hBNt.(jj.
+000034b0: 0000 8c2f 6465 6c65 7465 5f66 696c 6528  .../delete_file(
+000034c0: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
+000034d0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+000034e0: 6572 2994 8c21 6261 6d62 756c 6162 735f  er)..!bambulabs_
+000034f0: 6170 692e 5072 696e 7465 722e 6465 6c65  api.Printer.dele
+00003500: 7465 5f66 696c 6594 6842 4e74 9428 6a6a  te_file.hBNt.(jj
+00003510: 0400 008c 2e64 6973 636f 6e6e 6563 7428  .....disconnect(
+00003520: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
+00003530: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00003540: 6572 2994 8c20 6261 6d62 756c 6162 735f  er).. bambulabs_
+00003550: 6170 692e 5072 696e 7465 722e 6469 7363  api.Printer.disc
+00003560: 6f6e 6e65 6374 9468 424e 7494 286a 6a04  onnect.hBNt.(jj.
+00003570: 0000 8c37 6765 745f 6265 645f 7465 6d70  ...7get_bed_temp
+00003580: 6572 6174 7572 6528 2920 2869 6e20 6d6f  erature() (in mo
+00003590: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+000035a0: 7069 2e50 7269 6e74 6572 2994 8c29 6261  pi.Printer)..)ba
+000035b0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+000035c0: 7465 722e 6765 745f 6265 645f 7465 6d70  ter.get_bed_temp
+000035d0: 6572 6174 7572 6594 6842 4e74 9428 6a6a  erature.hBNt.(jj
+000035e0: 0400 008c 3467 6574 5f63 616d 6572 615f  ....4get_camera_
+000035f0: 6672 616d 6528 2920 2869 6e20 6d6f 6475  frame() (in modu
+00003600: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00003610: 2e50 7269 6e74 6572 2994 8c26 6261 6d62  .Printer)..&bamb
+00003620: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+00003630: 722e 6765 745f 6361 6d65 7261 5f66 7261  r.get_camera_fra
+00003640: 6d65 9468 424e 7494 286a 6a04 0000 8c31  me.hBNt.(jj....1
+00003650: 6765 745f 6669 6c65 5f6e 616d 6528 2920  get_file_name() 
+00003660: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+00003670: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+00003680: 2994 8c23 6261 6d62 756c 6162 735f 6170  )..#bambulabs_ap
+00003690: 692e 5072 696e 7465 722e 6765 745f 6669  i.Printer.get_fi
+000036a0: 6c65 5f6e 616d 6594 6842 4e74 9428 6a6a  le_name.hBNt.(jj
+000036b0: 0400 008c 3367 6574 5f6c 6967 6874 5f73  ....3get_light_s
+000036c0: 7461 7465 2829 2028 696e 206d 6f64 756c  tate() (in modul
+000036d0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+000036e0: 5072 696e 7465 7229 948c 2562 616d 6275  Printer)..%bambu
+000036f0: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+00003700: 2e67 6574 5f6c 6967 6874 5f73 7461 7465  .get_light_state
+00003710: 9468 424e 7494 286a 6a04 0000 8c3a 6765  .hBNt.(jj....:ge
+00003720: 745f 6e6f 7a7a 6c65 5f74 656d 7065 7261  t_nozzle_tempera
+00003730: 7475 7265 2829 2028 696e 206d 6f64 756c  ture() (in modul
+00003740: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00003750: 5072 696e 7465 7229 948c 2c62 616d 6275  Printer)..,bambu
+00003760: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+00003770: 2e67 6574 5f6e 6f7a 7a6c 655f 7465 6d70  .get_nozzle_temp
+00003780: 6572 6174 7572 6594 6842 4e74 9428 6a6a  erature.hBNt.(jj
+00003790: 0400 008c 3267 6574 5f70 6572 6365 6e74  ....2get_percent
+000037a0: 6167 6528 2920 2869 6e20 6d6f 6475 6c65  age() (in module
+000037b0: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
+000037c0: 7269 6e74 6572 2994 8c24 6261 6d62 756c  rinter)..$bambul
+000037d0: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
+000037e0: 6765 745f 7065 7263 656e 7461 6765 9468  get_percentage.h
+000037f0: 424e 7494 286a 6a04 0000 8c33 6765 745f  BNt.(jj....3get_
+00003800: 7072 696e 745f 7370 6565 6428 2920 2869  print_speed() (i
+00003810: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00003820: 6273 5f61 7069 2e50 7269 6e74 6572 2994  bs_api.Printer).
+00003830: 8c25 6261 6d62 756c 6162 735f 6170 692e  .%bambulabs_api.
+00003840: 5072 696e 7465 722e 6765 745f 7072 696e  Printer.get_prin
+00003850: 745f 7370 6565 6494 6842 4e74 9428 6a6a  t_speed.hBNt.(jj
+00003860: 0400 008c 2d67 6574 5f73 7461 7465 2829  ....-get_state()
+00003870: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
+00003880: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+00003890: 7229 948c 1f62 616d 6275 6c61 6273 5f61  r)...bambulabs_a
+000038a0: 7069 2e50 7269 6e74 6572 2e67 6574 5f73  pi.Printer.get_s
+000038b0: 7461 7465 9468 424e 7494 286a 6a04 0000  tate.hBNt.(jj...
+000038c0: 8c2c 6765 745f 7469 6d65 2829 2028 696e  .,get_time() (in
+000038d0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+000038e0: 735f 6170 692e 5072 696e 7465 7229 948c  s_api.Printer)..
+000038f0: 1e62 616d 6275 6c61 6273 5f61 7069 2e50  .bambulabs_api.P
+00003900: 7269 6e74 6572 2e67 6574 5f74 696d 6594  rinter.get_time.
+00003910: 6842 4e74 9428 6a6a 0400 008c 3068 6f6d  hBNt.(jj....0hom
+00003920: 655f 7072 696e 7465 7228 2920 2869 6e20  e_printer() (in 
+00003930: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
+00003940: 5f61 7069 2e50 7269 6e74 6572 2994 8c22  _api.Printer).."
+00003950: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+00003960: 696e 7465 722e 686f 6d65 5f70 7269 6e74  inter.home_print
+00003970: 6572 9468 424e 7494 286a 6a04 0000 8c37  er.hBNt.(jj....7
+00003980: 6c6f 6164 5f66 696c 616d 656e 745f 7370  load_filament_sp
+00003990: 6f6f 6c28 2920 2869 6e20 6d6f 6475 6c65  ool() (in module
+000039a0: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
+000039b0: 7269 6e74 6572 2994 8c29 6261 6d62 756c  rinter)..)bambul
+000039c0: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
+000039d0: 6c6f 6164 5f66 696c 616d 656e 745f 7370  load_filament_sp
+000039e0: 6f6f 6c94 6842 4e74 9428 6a6a 0400 008c  ool.hBNt.(jj....
+000039f0: 2f6d 6f76 655f 7a5f 6178 6973 2829 2028  /move_z_axis() (
+00003a00: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
+00003a10: 6162 735f 6170 692e 5072 696e 7465 7229  abs_api.Printer)
+00003a20: 948c 2162 616d 6275 6c61 6273 5f61 7069  ..!bambulabs_api
+00003a30: 2e50 7269 6e74 6572 2e6d 6f76 655f 7a5f  .Printer.move_z_
+00003a40: 6178 6973 9468 424e 7494 286a 6a04 0000  axis.hBNt.(jj...
+00003a50: 8c2f 7061 7573 655f 7072 696e 7428 2920  ./pause_print() 
+00003a60: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+00003a70: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+00003a80: 2994 8c21 6261 6d62 756c 6162 735f 6170  )..!bambulabs_ap
+00003a90: 692e 5072 696e 7465 722e 7061 7573 655f  i.Printer.pause_
+00003aa0: 7072 696e 7494 6842 4e74 9428 6a6a 0400  print.hBNt.(jj..
+00003ab0: 008c 3072 6573 756d 655f 7072 696e 7428  ..0resume_print(
+00003ac0: 2920 2869 6e20 6d6f 6475 6c65 2062 616d  ) (in module bam
+00003ad0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00003ae0: 6572 2994 8c22 6261 6d62 756c 6162 735f  er).."bambulabs_
+00003af0: 6170 692e 5072 696e 7465 722e 7265 7375  api.Printer.resu
+00003b00: 6d65 5f70 7269 6e74 9468 424e 7494 286a  me_print.hBNt.(j
+00003b10: 6a04 0000 8c39 7265 7472 795f 6669 6c61  j....9retry_fila
+00003b20: 6d65 6e74 5f61 6374 696f 6e28 2920 2869  ment_action() (i
+00003b30: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00003b40: 6273 5f61 7069 2e50 7269 6e74 6572 2994  bs_api.Printer).
+00003b50: 8c2b 6261 6d62 756c 6162 735f 6170 692e  .+bambulabs_api.
+00003b60: 5072 696e 7465 722e 7265 7472 795f 6669  Printer.retry_fi
+00003b70: 6c61 6d65 6e74 5f61 6374 696f 6e94 6842  lament_action.hB
+00003b80: 4e74 9428 6a6a 0400 008c 3773 6574 5f62  Nt.(jj....7set_b
+00003b90: 6564 5f74 656d 7065 7261 7475 7265 2829  ed_temperature()
+00003ba0: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
+00003bb0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+00003bc0: 7229 948c 2962 616d 6275 6c61 6273 5f61  r)..)bambulabs_a
+00003bd0: 7069 2e50 7269 6e74 6572 2e73 6574 5f62  pi.Printer.set_b
+00003be0: 6564 5f74 656d 7065 7261 7475 7265 9468  ed_temperature.h
+00003bf0: 424e 7494 286a 6a04 0000 8c38 7365 745f  BNt.(jj....8set_
+00003c00: 6669 6c61 6d65 6e74 5f70 7269 6e74 6572  filament_printer
+00003c10: 2829 2028 696e 206d 6f64 756c 6520 6261  () (in module ba
+00003c20: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00003c30: 7465 7229 948c 2a62 616d 6275 6c61 6273  ter)..*bambulabs
+00003c40: 5f61 7069 2e50 7269 6e74 6572 2e73 6574  _api.Printer.set
+00003c50: 5f66 696c 616d 656e 745f 7072 696e 7465  _filament_printe
+00003c60: 7294 6842 4e74 9428 6a6a 0400 008c 3a73  r.hBNt.(jj....:s
+00003c70: 6574 5f6e 6f7a 7a6c 655f 7465 6d70 6572  et_nozzle_temper
+00003c80: 6174 7572 6528 2920 2869 6e20 6d6f 6475  ature() (in modu
+00003c90: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00003ca0: 2e50 7269 6e74 6572 2994 8c2c 6261 6d62  .Printer)..,bamb
+00003cb0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+00003cc0: 722e 7365 745f 6e6f 7a7a 6c65 5f74 656d  r.set_nozzle_tem
+00003cd0: 7065 7261 7475 7265 9468 424e 7494 286a  perature.hBNt.(j
+00003ce0: 6a04 0000 8c33 7365 745f 7072 696e 745f  j....3set_print_
+00003cf0: 7370 6565 6428 2920 2869 6e20 6d6f 6475  speed() (in modu
+00003d00: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00003d10: 2e50 7269 6e74 6572 2994 8c25 6261 6d62  .Printer)..%bamb
+00003d20: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+00003d30: 722e 7365 745f 7072 696e 745f 7370 6565  r.set_print_spee
+00003d40: 6494 6842 4e74 9428 6a6a 0400 008c 2f73  d.hBNt.(jj..../s
+00003d50: 7461 7274 5f70 7269 6e74 2829 2028 696e  tart_print() (in
+00003d60: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+00003d70: 735f 6170 692e 5072 696e 7465 7229 948c  s_api.Printer)..
+00003d80: 2162 616d 6275 6c61 6273 5f61 7069 2e50  !bambulabs_api.P
+00003d90: 7269 6e74 6572 2e73 7461 7274 5f70 7269  rinter.start_pri
+00003da0: 6e74 9468 424e 7494 286a 6a04 0000 8c2e  nt.hBNt.(jj.....
+00003db0: 7374 6f70 5f70 7269 6e74 2829 2028 696e  stop_print() (in
+00003dc0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+00003dd0: 735f 6170 692e 5072 696e 7465 7229 948c  s_api.Printer)..
+00003de0: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
+00003df0: 7269 6e74 6572 2e73 746f 705f 7072 696e  rinter.stop_prin
+00003e00: 7494 6842 4e74 9428 6a6a 0400 008c 3274  t.hBNt.(jj....2t
+00003e10: 7572 6e5f 6c69 6768 745f 6f66 6628 2920  urn_light_off() 
+00003e20: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+00003e30: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+00003e40: 2994 8c24 6261 6d62 756c 6162 735f 6170  )..$bambulabs_ap
+00003e50: 692e 5072 696e 7465 722e 7475 726e 5f6c  i.Printer.turn_l
+00003e60: 6967 6874 5f6f 6666 9468 424e 7494 286a  ight_off.hBNt.(j
+00003e70: 6a04 0000 8c31 7475 726e 5f6c 6967 6874  j....1turn_light
+00003e80: 5f6f 6e28 2920 2869 6e20 6d6f 6475 6c65  _on() (in module
+00003e90: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
+00003ea0: 7269 6e74 6572 2994 8c23 6261 6d62 756c  rinter)..#bambul
+00003eb0: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
+00003ec0: 7475 726e 5f6c 6967 6874 5f6f 6e94 6842  turn_light_on.hB
+00003ed0: 4e74 9428 6a6a 0400 008c 3975 6e6c 6f61  Nt.(jj....9unloa
+00003ee0: 645f 6669 6c61 6d65 6e74 5f73 706f 6f6c  d_filament_spool
+00003ef0: 2829 2028 696e 206d 6f64 756c 6520 6261  () (in module ba
+00003f00: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00003f10: 7465 7229 948c 2b62 616d 6275 6c61 6273  ter)..+bambulabs
+00003f20: 5f61 7069 2e50 7269 6e74 6572 2e75 6e6c  _api.Printer.unl
+00003f30: 6f61 645f 6669 6c61 6d65 6e74 5f73 706f  oad_filament_spo
+00003f40: 6f6c 9468 424e 7494 286a 6a04 0000 8c2f  ol.hBNt.(jj..../
+00003f50: 7570 6c6f 6164 5f66 696c 6528 2920 2869  upload_file() (i
+00003f60: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00003f70: 6273 5f61 7069 2e50 7269 6e74 6572 2994  bs_api.Printer).
+00003f80: 8c21 6261 6d62 756c 6162 735f 6170 692e  .!bambulabs_api.
+00003f90: 5072 696e 7465 722e 7570 6c6f 6164 5f66  Printer.upload_f
+00003fa0: 696c 6594 6842 4e74 9428 6a66 0400 008c  ile.hBNt.(jf....
+00003fb0: 1e6d 6f64 756c 653b 2062 616d 6275 6c61  .module; bambula
+00003fc0: 6273 5f61 7069 2e46 696c 616d 656e 7494  bs_api.Filament.
+00003fd0: 8c1d 6d6f 6475 6c65 2d62 616d 6275 6c61  ..module-bambula
+00003fe0: 6273 5f61 7069 2e46 696c 616d 656e 7494  bs_api.Filament.
+00003ff0: 6842 4e74 9428 6a6a 0400 008c 2f50 4f4c  hBNt.(jj..../POL
+00004000: 594c 4954 455f 504c 4120 2869 6e20 6d6f  YLITE_PLA (in mo
+00004010: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+00004020: 7069 2e46 696c 616d 656e 7429 948c 2362  pi.Filament)..#b
+00004030: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
+00004040: 616d 656e 742e 504f 4c59 4c49 5445 5f50  ament.POLYLITE_P
+00004050: 4c41 9468 424e 7494 286a 6a04 0000 8c30  LA.hBNt.(jj....0
+00004060: 504f 4c59 5445 5252 415f 504c 4120 2869  POLYTERRA_PLA (i
 00004070: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
 00004080: 6273 5f61 7069 2e46 696c 616d 656e 7429  bs_api.Filament)
-00004090: 948c 2662 616d 6275 6c61 6273 5f61 7069  ..&bambulabs_api
-000040a0: 2e46 696c 616d 656e 742e 4241 4d42 555f  .Filament.BAMBU_
-000040b0: 504c 415f 4261 7369 6394 6842 4e74 9428  PLA_Basic.hBNt.(
-000040c0: 6a46 0400 008c 3242 414d 4255 5f50 4c41  jF....2BAMBU_PLA
-000040d0: 5f4d 6174 7465 2028 696e 206d 6f64 756c  _Matte (in modul
-000040e0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-000040f0: 4669 6c61 6d65 6e74 2994 8c26 6261 6d62  Filament)..&bamb
-00004100: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
-00004110: 6e74 2e42 414d 4255 5f50 4c41 5f4d 6174  nt.BAMBU_PLA_Mat
-00004120: 7465 9468 424e 7494 286a 4604 0000 8c2c  te.hBNt.(jF....,
-00004130: 5355 5050 4f52 545f 4720 2869 6e20 6d6f  SUPPORT_G (in mo
-00004140: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
-00004150: 7069 2e46 696c 616d 656e 7429 948c 2062  pi.Filament).. b
-00004160: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-00004170: 616d 656e 742e 5355 5050 4f52 545f 4794  ament.SUPPORT_G.
-00004180: 6842 4e74 9428 6a46 0400 008c 2c53 5550  hBNt.(jF....,SUP
-00004190: 504f 5254 5f57 2028 696e 206d 6f64 756c  PORT_W (in modul
-000041a0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-000041b0: 4669 6c61 6d65 6e74 2994 8c20 6261 6d62  Filament).. bamb
-000041c0: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
-000041d0: 6e74 2e53 5550 504f 5254 5f57 9468 424e  nt.SUPPORT_W.hBN
-000041e0: 7494 286a 4604 0000 8c30 4241 4d42 555f  t.(jF....0BAMBU_
-000041f0: 5450 555f 3935 4120 2869 6e20 6d6f 6475  TPU_95A (in modu
-00004200: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00004210: 2e46 696c 616d 656e 7429 948c 2462 616d  .Filament)..$bam
-00004220: 6275 6c61 6273 5f61 7069 2e46 696c 616d  bulabs_api.Filam
-00004230: 656e 742e 4241 4d42 555f 5450 555f 3935  ent.BAMBU_TPU_95
-00004240: 4194 6842 4e74 9428 6a46 0400 008c 2641  A.hBNt.(jF....&A
-00004250: 4253 2028 696e 206d 6f64 756c 6520 6261  BS (in module ba
-00004260: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
-00004270: 6d65 6e74 2994 8c1a 6261 6d62 756c 6162  ment)...bambulab
-00004280: 735f 6170 692e 4669 6c61 6d65 6e74 2e41  s_api.Filament.A
-00004290: 4253 9468 424e 7494 286a 4604 0000 8c26  BS.hBNt.(jF....&
-000042a0: 4153 4120 2869 6e20 6d6f 6475 6c65 2062  ASA (in module b
-000042b0: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-000042c0: 616d 656e 7429 948c 1a62 616d 6275 6c61  ament)...bambula
-000042d0: 6273 5f61 7069 2e46 696c 616d 656e 742e  bs_api.Filament.
-000042e0: 4153 4194 6842 4e74 9428 6a46 0400 008c  ASA.hBNt.(jF....
-000042f0: 2550 4120 2869 6e20 6d6f 6475 6c65 2062  %PA (in module b
-00004300: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-00004310: 616d 656e 7429 948c 1962 616d 6275 6c61  ament)...bambula
-00004320: 6273 5f61 7069 2e46 696c 616d 656e 742e  bs_api.Filament.
-00004330: 5041 9468 424e 7494 286a 4604 0000 8c28  PA.hBNt.(jF....(
-00004340: 5041 5f43 4620 2869 6e20 6d6f 6475 6c65  PA_CF (in module
-00004350: 2062 616d 6275 6c61 6273 5f61 7069 2e46   bambulabs_api.F
-00004360: 696c 616d 656e 7429 948c 1c62 616d 6275  ilament)...bambu
-00004370: 6c61 6273 5f61 7069 2e46 696c 616d 656e  labs_api.Filamen
-00004380: 742e 5041 5f43 4694 6842 4e74 9428 6a46  t.PA_CF.hBNt.(jF
-00004390: 0400 008c 2550 4320 2869 6e20 6d6f 6475  ....%PC (in modu
-000043a0: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-000043b0: 2e46 696c 616d 656e 7429 948c 1962 616d  .Filament)...bam
-000043c0: 6275 6c61 6273 5f61 7069 2e46 696c 616d  bulabs_api.Filam
-000043d0: 656e 742e 5043 9468 424e 7494 286a 4604  ent.PC.hBNt.(jF.
-000043e0: 0000 8c27 5045 5447 2028 696e 206d 6f64  ...'PETG (in mod
-000043f0: 756c 6520 6261 6d62 756c 6162 735f 6170  ule bambulabs_ap
-00004400: 692e 4669 6c61 6d65 6e74 2994 8c1b 6261  i.Filament)...ba
-00004410: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
-00004420: 6d65 6e74 2e50 4554 4794 6842 4e74 9428  ment.PETG.hBNt.(
-00004430: 6a46 0400 008c 2650 4c41 2028 696e 206d  jF....&PLA (in m
-00004440: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
-00004450: 6170 692e 4669 6c61 6d65 6e74 2994 8c1a  api.Filament)...
-00004460: 6261 6d62 756c 6162 735f 6170 692e 4669  bambulabs_api.Fi
-00004470: 6c61 6d65 6e74 2e50 4c41 9468 424e 7494  lament.PLA.hBNt.
-00004480: 286a 4604 0000 8c29 504c 415f 4346 2028  (jF....)PLA_CF (
-00004490: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
-000044a0: 6162 735f 6170 692e 4669 6c61 6d65 6e74  abs_api.Filament
-000044b0: 2994 8c1d 6261 6d62 756c 6162 735f 6170  )...bambulabs_ap
-000044c0: 692e 4669 6c61 6d65 6e74 2e50 4c41 5f43  i.Filament.PLA_C
-000044d0: 4694 6842 4e74 9428 6a46 0400 008c 2650  F.hBNt.(jF....&P
-000044e0: 5641 2028 696e 206d 6f64 756c 6520 6261  VA (in module ba
-000044f0: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
-00004500: 6d65 6e74 2994 8c1a 6261 6d62 756c 6162  ment)...bambulab
-00004510: 735f 6170 692e 4669 6c61 6d65 6e74 2e50  s_api.Filament.P
-00004520: 5641 9468 424e 7494 286a 4604 0000 8c26  VA.hBNt.(jF....&
-00004530: 5450 5520 2869 6e20 6d6f 6475 6c65 2062  TPU (in module b
-00004540: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-00004550: 616d 656e 7429 948c 1a62 616d 6275 6c61  ament)...bambula
-00004560: 6273 5f61 7069 2e46 696c 616d 656e 742e  bs_api.Filament.
-00004570: 5450 5594 6842 4e74 9428 6a42 0400 008c  TPU.hBNt.(jB....
-00004580: 296d 6f64 756c 653b 2062 616d 6275 6c61  )module; bambula
-00004590: 6273 5f61 7069 2e41 4d53 4669 6c61 6d65  bs_api.AMSFilame
-000045a0: 6e74 5365 7474 696e 6773 948c 286d 6f64  ntSettings..(mod
-000045b0: 756c 652d 6261 6d62 756c 6162 735f 6170  ule-bambulabs_ap
-000045c0: 692e 414d 5346 696c 616d 656e 7453 6574  i.AMSFilamentSet
-000045d0: 7469 6e67 7394 6842 4e74 9428 6a46 0400  tings.hBNt.(jF..
-000045e0: 008c 3b74 7261 795f 696e 666f 5f69 6478  ..;tray_info_idx
-000045f0: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
-00004600: 756c 6162 735f 6170 692e 414d 5346 696c  ulabs_api.AMSFil
-00004610: 616d 656e 7453 6574 7469 6e67 7329 948c  amentSettings)..
-00004620: 2f62 616d 6275 6c61 6273 5f61 7069 2e41  /bambulabs_api.A
-00004630: 4d53 4669 6c61 6d65 6e74 5365 7474 696e  MSFilamentSettin
-00004640: 6773 2e74 7261 795f 696e 666f 5f69 6478  gs.tray_info_idx
-00004650: 9468 424e 7494 286a 4604 0000 8c3d 6e6f  .hBNt.(jF....=no
-00004660: 7a7a 6c65 5f74 656d 705f 6d69 6e20 2869  zzle_temp_min (i
-00004670: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
-00004680: 6273 5f61 7069 2e41 4d53 4669 6c61 6d65  bs_api.AMSFilame
-00004690: 6e74 5365 7474 696e 6773 2994 8c31 6261  ntSettings)..1ba
-000046a0: 6d62 756c 6162 735f 6170 692e 414d 5346  mbulabs_api.AMSF
-000046b0: 696c 616d 656e 7453 6574 7469 6e67 732e  ilamentSettings.
-000046c0: 6e6f 7a7a 6c65 5f74 656d 705f 6d69 6e94  nozzle_temp_min.
-000046d0: 6842 4e74 9428 6a46 0400 008c 3d6e 6f7a  hBNt.(jF....=noz
-000046e0: 7a6c 655f 7465 6d70 5f6d 6178 2028 696e  zle_temp_max (in
-000046f0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00004700: 735f 6170 692e 414d 5346 696c 616d 656e  s_api.AMSFilamen
-00004710: 7453 6574 7469 6e67 7329 948c 3162 616d  tSettings)..1bam
-00004720: 6275 6c61 6273 5f61 7069 2e41 4d53 4669  bulabs_api.AMSFi
-00004730: 6c61 6d65 6e74 5365 7474 696e 6773 2e6e  lamentSettings.n
-00004740: 6f7a 7a6c 655f 7465 6d70 5f6d 6178 9468  ozzle_temp_max.h
-00004750: 424e 7494 286a 4604 0000 8c37 7472 6179  BNt.(jF....7tray
-00004760: 5f74 7970 6520 2869 6e20 6d6f 6475 6c65  _type (in module
-00004770: 2062 616d 6275 6c61 6273 5f61 7069 2e41   bambulabs_api.A
-00004780: 4d53 4669 6c61 6d65 6e74 5365 7474 696e  MSFilamentSettin
-00004790: 6773 2994 8c2b 6261 6d62 756c 6162 735f  gs)..+bambulabs_
-000047a0: 6170 692e 414d 5346 696c 616d 656e 7453  api.AMSFilamentS
-000047b0: 6574 7469 6e67 732e 7472 6179 5f74 7970  ettings.tray_typ
-000047c0: 6594 6842 4e74 9428 6a42 0400 008c 216d  e.hBNt.(jB....!m
-000047d0: 6f64 756c 653b 2062 616d 6275 6c61 6273  odule; bambulabs
-000047e0: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
-000047f0: 948c 206d 6f64 756c 652d 6261 6d62 756c  .. module-bambul
-00004800: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-00004810: 7475 7394 6842 4e74 9428 6a46 0400 008c  tus.hBNt.(jF....
-00004820: 2e50 5249 4e54 494e 4720 2869 6e20 6d6f  .PRINTING (in mo
-00004830: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
-00004840: 7069 2e50 7269 6e74 5374 6174 7573 2994  pi.PrintStatus).
-00004850: 8c22 6261 6d62 756c 6162 735f 6170 692e  ."bambulabs_api.
-00004860: 5072 696e 7453 7461 7475 732e 5052 494e  PrintStatus.PRIN
-00004870: 5449 4e47 9468 424e 7494 286a 4604 0000  TING.hBNt.(jF...
-00004880: 8c37 4155 544f 5f42 4544 5f4c 4556 454c  .7AUTO_BED_LEVEL
-00004890: 494e 4720 2869 6e20 6d6f 6475 6c65 2062  ING (in module b
-000048a0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-000048b0: 6e74 5374 6174 7573 2994 8c2b 6261 6d62  ntStatus)..+bamb
-000048c0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-000048d0: 7461 7475 732e 4155 544f 5f42 4544 5f4c  tatus.AUTO_BED_L
-000048e0: 4556 454c 494e 4794 6842 4e74 9428 6a46  EVELING.hBNt.(jF
-000048f0: 0400 008c 3848 4541 5442 4544 5f50 5245  ....8HEATBED_PRE
-00004900: 4845 4154 494e 4720 2869 6e20 6d6f 6475  HEATING (in modu
-00004910: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00004920: 2e50 7269 6e74 5374 6174 7573 2994 8c2c  .PrintStatus)..,
-00004930: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00004940: 696e 7453 7461 7475 732e 4845 4154 4245  intStatus.HEATBE
-00004950: 445f 5052 4548 4541 5449 4e47 9468 424e  D_PREHEATING.hBN
-00004960: 7494 286a 4604 0000 8c3b 5357 4545 5049  t.(jF....;SWEEPI
-00004970: 4e47 5f58 595f 4d45 4348 5f4d 4f44 4520  NG_XY_MECH_MODE 
-00004980: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
-00004990: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-000049a0: 6174 7573 2994 8c2f 6261 6d62 756c 6162  atus)../bambulab
-000049b0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
-000049c0: 732e 5357 4545 5049 4e47 5f58 595f 4d45  s.SWEEPING_XY_ME
-000049d0: 4348 5f4d 4f44 4594 6842 4e74 9428 6a46  CH_MODE.hBNt.(jF
-000049e0: 0400 008c 3743 4841 4e47 494e 475f 4649  ....7CHANGING_FI
-000049f0: 4c41 4d45 4e54 2028 696e 206d 6f64 756c  LAMENT (in modul
-00004a00: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-00004a10: 5072 696e 7453 7461 7475 7329 948c 2b62  PrintStatus)..+b
+00004090: 948c 2462 616d 6275 6c61 6273 5f61 7069  ..$bambulabs_api
+000040a0: 2e46 696c 616d 656e 742e 504f 4c59 5445  .Filament.POLYTE
+000040b0: 5252 415f 504c 4194 6842 4e74 9428 6a6a  RRA_PLA.hBNt.(jj
+000040c0: 0400 008c 2c42 414d 4255 5f41 4253 2028  ....,BAMBU_ABS (
+000040d0: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
+000040e0: 6162 735f 6170 692e 4669 6c61 6d65 6e74  abs_api.Filament
+000040f0: 2994 8c20 6261 6d62 756c 6162 735f 6170  ).. bambulabs_ap
+00004100: 692e 4669 6c61 6d65 6e74 2e42 414d 4255  i.Filament.BAMBU
+00004110: 5f41 4253 9468 424e 7494 286a 6a04 0000  _ABS.hBNt.(jj...
+00004120: 8c2e 4241 4d42 555f 5041 5f43 4620 2869  ..BAMBU_PA_CF (i
+00004130: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00004140: 6273 5f61 7069 2e46 696c 616d 656e 7429  bs_api.Filament)
+00004150: 948c 2262 616d 6275 6c61 6273 5f61 7069  .."bambulabs_api
+00004160: 2e46 696c 616d 656e 742e 4241 4d42 555f  .Filament.BAMBU_
+00004170: 5041 5f43 4694 6842 4e74 9428 6a6a 0400  PA_CF.hBNt.(jj..
+00004180: 008c 2b42 414d 4255 5f50 4320 2869 6e20  ..+BAMBU_PC (in 
+00004190: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
+000041a0: 5f61 7069 2e46 696c 616d 656e 7429 948c  _api.Filament)..
+000041b0: 1f62 616d 6275 6c61 6273 5f61 7069 2e46  .bambulabs_api.F
+000041c0: 696c 616d 656e 742e 4241 4d42 555f 5043  ilament.BAMBU_PC
+000041d0: 9468 424e 7494 286a 6a04 0000 8c32 4241  .hBNt.(jj....2BA
+000041e0: 4d42 555f 504c 415f 4261 7369 6320 2869  MBU_PLA_Basic (i
+000041f0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00004200: 6273 5f61 7069 2e46 696c 616d 656e 7429  bs_api.Filament)
+00004210: 948c 2662 616d 6275 6c61 6273 5f61 7069  ..&bambulabs_api
+00004220: 2e46 696c 616d 656e 742e 4241 4d42 555f  .Filament.BAMBU_
+00004230: 504c 415f 4261 7369 6394 6842 4e74 9428  PLA_Basic.hBNt.(
+00004240: 6a6a 0400 008c 3242 414d 4255 5f50 4c41  jj....2BAMBU_PLA
+00004250: 5f4d 6174 7465 2028 696e 206d 6f64 756c  _Matte (in modul
+00004260: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00004270: 4669 6c61 6d65 6e74 2994 8c26 6261 6d62  Filament)..&bamb
+00004280: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
+00004290: 6e74 2e42 414d 4255 5f50 4c41 5f4d 6174  nt.BAMBU_PLA_Mat
+000042a0: 7465 9468 424e 7494 286a 6a04 0000 8c2c  te.hBNt.(jj....,
+000042b0: 5355 5050 4f52 545f 4720 2869 6e20 6d6f  SUPPORT_G (in mo
+000042c0: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+000042d0: 7069 2e46 696c 616d 656e 7429 948c 2062  pi.Filament).. b
+000042e0: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
+000042f0: 616d 656e 742e 5355 5050 4f52 545f 4794  ament.SUPPORT_G.
+00004300: 6842 4e74 9428 6a6a 0400 008c 2c53 5550  hBNt.(jj....,SUP
+00004310: 504f 5254 5f57 2028 696e 206d 6f64 756c  PORT_W (in modul
+00004320: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00004330: 4669 6c61 6d65 6e74 2994 8c20 6261 6d62  Filament).. bamb
+00004340: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
+00004350: 6e74 2e53 5550 504f 5254 5f57 9468 424e  nt.SUPPORT_W.hBN
+00004360: 7494 286a 6a04 0000 8c30 4241 4d42 555f  t.(jj....0BAMBU_
+00004370: 5450 555f 3935 4120 2869 6e20 6d6f 6475  TPU_95A (in modu
+00004380: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00004390: 2e46 696c 616d 656e 7429 948c 2462 616d  .Filament)..$bam
+000043a0: 6275 6c61 6273 5f61 7069 2e46 696c 616d  bulabs_api.Filam
+000043b0: 656e 742e 4241 4d42 555f 5450 555f 3935  ent.BAMBU_TPU_95
+000043c0: 4194 6842 4e74 9428 6a6a 0400 008c 2641  A.hBNt.(jj....&A
+000043d0: 4253 2028 696e 206d 6f64 756c 6520 6261  BS (in module ba
+000043e0: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
+000043f0: 6d65 6e74 2994 8c1a 6261 6d62 756c 6162  ment)...bambulab
+00004400: 735f 6170 692e 4669 6c61 6d65 6e74 2e41  s_api.Filament.A
+00004410: 4253 9468 424e 7494 286a 6a04 0000 8c26  BS.hBNt.(jj....&
+00004420: 4153 4120 2869 6e20 6d6f 6475 6c65 2062  ASA (in module b
+00004430: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
+00004440: 616d 656e 7429 948c 1a62 616d 6275 6c61  ament)...bambula
+00004450: 6273 5f61 7069 2e46 696c 616d 656e 742e  bs_api.Filament.
+00004460: 4153 4194 6842 4e74 9428 6a6a 0400 008c  ASA.hBNt.(jj....
+00004470: 2550 4120 2869 6e20 6d6f 6475 6c65 2062  %PA (in module b
+00004480: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
+00004490: 616d 656e 7429 948c 1962 616d 6275 6c61  ament)...bambula
+000044a0: 6273 5f61 7069 2e46 696c 616d 656e 742e  bs_api.Filament.
+000044b0: 5041 9468 424e 7494 286a 6a04 0000 8c28  PA.hBNt.(jj....(
+000044c0: 5041 5f43 4620 2869 6e20 6d6f 6475 6c65  PA_CF (in module
+000044d0: 2062 616d 6275 6c61 6273 5f61 7069 2e46   bambulabs_api.F
+000044e0: 696c 616d 656e 7429 948c 1c62 616d 6275  ilament)...bambu
+000044f0: 6c61 6273 5f61 7069 2e46 696c 616d 656e  labs_api.Filamen
+00004500: 742e 5041 5f43 4694 6842 4e74 9428 6a6a  t.PA_CF.hBNt.(jj
+00004510: 0400 008c 2550 4320 2869 6e20 6d6f 6475  ....%PC (in modu
+00004520: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00004530: 2e46 696c 616d 656e 7429 948c 1962 616d  .Filament)...bam
+00004540: 6275 6c61 6273 5f61 7069 2e46 696c 616d  bulabs_api.Filam
+00004550: 656e 742e 5043 9468 424e 7494 286a 6a04  ent.PC.hBNt.(jj.
+00004560: 0000 8c27 5045 5447 2028 696e 206d 6f64  ...'PETG (in mod
+00004570: 756c 6520 6261 6d62 756c 6162 735f 6170  ule bambulabs_ap
+00004580: 692e 4669 6c61 6d65 6e74 2994 8c1b 6261  i.Filament)...ba
+00004590: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
+000045a0: 6d65 6e74 2e50 4554 4794 6842 4e74 9428  ment.PETG.hBNt.(
+000045b0: 6a6a 0400 008c 2650 4c41 2028 696e 206d  jj....&PLA (in m
+000045c0: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
+000045d0: 6170 692e 4669 6c61 6d65 6e74 2994 8c1a  api.Filament)...
+000045e0: 6261 6d62 756c 6162 735f 6170 692e 4669  bambulabs_api.Fi
+000045f0: 6c61 6d65 6e74 2e50 4c41 9468 424e 7494  lament.PLA.hBNt.
+00004600: 286a 6a04 0000 8c29 504c 415f 4346 2028  (jj....)PLA_CF (
+00004610: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
+00004620: 6162 735f 6170 692e 4669 6c61 6d65 6e74  abs_api.Filament
+00004630: 2994 8c1d 6261 6d62 756c 6162 735f 6170  )...bambulabs_ap
+00004640: 692e 4669 6c61 6d65 6e74 2e50 4c41 5f43  i.Filament.PLA_C
+00004650: 4694 6842 4e74 9428 6a6a 0400 008c 2650  F.hBNt.(jj....&P
+00004660: 5641 2028 696e 206d 6f64 756c 6520 6261  VA (in module ba
+00004670: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
+00004680: 6d65 6e74 2994 8c1a 6261 6d62 756c 6162  ment)...bambulab
+00004690: 735f 6170 692e 4669 6c61 6d65 6e74 2e50  s_api.Filament.P
+000046a0: 5641 9468 424e 7494 286a 6a04 0000 8c26  VA.hBNt.(jj....&
+000046b0: 5450 5520 2869 6e20 6d6f 6475 6c65 2062  TPU (in module b
+000046c0: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
+000046d0: 616d 656e 7429 948c 1a62 616d 6275 6c61  ament)...bambula
+000046e0: 6273 5f61 7069 2e46 696c 616d 656e 742e  bs_api.Filament.
+000046f0: 5450 5594 6842 4e74 9428 6a66 0400 008c  TPU.hBNt.(jf....
+00004700: 296d 6f64 756c 653b 2062 616d 6275 6c61  )module; bambula
+00004710: 6273 5f61 7069 2e41 4d53 4669 6c61 6d65  bs_api.AMSFilame
+00004720: 6e74 5365 7474 696e 6773 948c 286d 6f64  ntSettings..(mod
+00004730: 756c 652d 6261 6d62 756c 6162 735f 6170  ule-bambulabs_ap
+00004740: 692e 414d 5346 696c 616d 656e 7453 6574  i.AMSFilamentSet
+00004750: 7469 6e67 7394 6842 4e74 9428 6a6a 0400  tings.hBNt.(jj..
+00004760: 008c 3b74 7261 795f 696e 666f 5f69 6478  ..;tray_info_idx
+00004770: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
+00004780: 756c 6162 735f 6170 692e 414d 5346 696c  ulabs_api.AMSFil
+00004790: 616d 656e 7453 6574 7469 6e67 7329 948c  amentSettings)..
+000047a0: 2f62 616d 6275 6c61 6273 5f61 7069 2e41  /bambulabs_api.A
+000047b0: 4d53 4669 6c61 6d65 6e74 5365 7474 696e  MSFilamentSettin
+000047c0: 6773 2e74 7261 795f 696e 666f 5f69 6478  gs.tray_info_idx
+000047d0: 9468 424e 7494 286a 6a04 0000 8c3d 6e6f  .hBNt.(jj....=no
+000047e0: 7a7a 6c65 5f74 656d 705f 6d69 6e20 2869  zzle_temp_min (i
+000047f0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00004800: 6273 5f61 7069 2e41 4d53 4669 6c61 6d65  bs_api.AMSFilame
+00004810: 6e74 5365 7474 696e 6773 2994 8c31 6261  ntSettings)..1ba
+00004820: 6d62 756c 6162 735f 6170 692e 414d 5346  mbulabs_api.AMSF
+00004830: 696c 616d 656e 7453 6574 7469 6e67 732e  ilamentSettings.
+00004840: 6e6f 7a7a 6c65 5f74 656d 705f 6d69 6e94  nozzle_temp_min.
+00004850: 6842 4e74 9428 6a6a 0400 008c 3d6e 6f7a  hBNt.(jj....=noz
+00004860: 7a6c 655f 7465 6d70 5f6d 6178 2028 696e  zle_temp_max (in
+00004870: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+00004880: 735f 6170 692e 414d 5346 696c 616d 656e  s_api.AMSFilamen
+00004890: 7453 6574 7469 6e67 7329 948c 3162 616d  tSettings)..1bam
+000048a0: 6275 6c61 6273 5f61 7069 2e41 4d53 4669  bulabs_api.AMSFi
+000048b0: 6c61 6d65 6e74 5365 7474 696e 6773 2e6e  lamentSettings.n
+000048c0: 6f7a 7a6c 655f 7465 6d70 5f6d 6178 9468  ozzle_temp_max.h
+000048d0: 424e 7494 286a 6a04 0000 8c37 7472 6179  BNt.(jj....7tray
+000048e0: 5f74 7970 6520 2869 6e20 6d6f 6475 6c65  _type (in module
+000048f0: 2062 616d 6275 6c61 6273 5f61 7069 2e41   bambulabs_api.A
+00004900: 4d53 4669 6c61 6d65 6e74 5365 7474 696e  MSFilamentSettin
+00004910: 6773 2994 8c2b 6261 6d62 756c 6162 735f  gs)..+bambulabs_
+00004920: 6170 692e 414d 5346 696c 616d 656e 7453  api.AMSFilamentS
+00004930: 6574 7469 6e67 732e 7472 6179 5f74 7970  ettings.tray_typ
+00004940: 6594 6842 4e74 9428 6a66 0400 008c 216d  e.hBNt.(jf....!m
+00004950: 6f64 756c 653b 2062 616d 6275 6c61 6273  odule; bambulabs
+00004960: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
+00004970: 948c 206d 6f64 756c 652d 6261 6d62 756c  .. module-bambul
+00004980: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00004990: 7475 7394 6842 4e74 9428 6a6a 0400 008c  tus.hBNt.(jj....
+000049a0: 2e50 5249 4e54 494e 4720 2869 6e20 6d6f  .PRINTING (in mo
+000049b0: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+000049c0: 7069 2e50 7269 6e74 5374 6174 7573 2994  pi.PrintStatus).
+000049d0: 8c22 6261 6d62 756c 6162 735f 6170 692e  ."bambulabs_api.
+000049e0: 5072 696e 7453 7461 7475 732e 5052 494e  PrintStatus.PRIN
+000049f0: 5449 4e47 9468 424e 7494 286a 6a04 0000  TING.hBNt.(jj...
+00004a00: 8c37 4155 544f 5f42 4544 5f4c 4556 454c  .7AUTO_BED_LEVEL
+00004a10: 494e 4720 2869 6e20 6d6f 6475 6c65 2062  ING (in module b
 00004a20: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00004a30: 6e74 5374 6174 7573 2e43 4841 4e47 494e  ntStatus.CHANGIN
-00004a40: 475f 4649 4c41 4d45 4e54 9468 424e 7494  G_FILAMENT.hBNt.
-00004a50: 286a 4604 0000 8c30 4d34 3030 5f50 4155  (jF....0M400_PAU
-00004a60: 5345 2028 696e 206d 6f64 756c 6520 6261  SE (in module ba
-00004a70: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00004a80: 7453 7461 7475 7329 948c 2462 616d 6275  tStatus)..$bambu
-00004a90: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00004aa0: 6174 7573 2e4d 3430 305f 5041 5553 4594  atus.M400_PAUSE.
-00004ab0: 6842 4e74 9428 6a46 0400 008c 3c50 4155  hBNt.(jF....<PAU
-00004ac0: 5345 445f 4649 4c41 4d45 4e54 5f52 554e  SED_FILAMENT_RUN
-00004ad0: 4f55 5420 2869 6e20 6d6f 6475 6c65 2062  OUT (in module b
-00004ae0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00004af0: 6e74 5374 6174 7573 2994 8c30 6261 6d62  ntStatus)..0bamb
-00004b00: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00004b10: 7461 7475 732e 5041 5553 4544 5f46 494c  tatus.PAUSED_FIL
-00004b20: 414d 454e 545f 5255 4e4f 5554 9468 424e  AMENT_RUNOUT.hBN
-00004b30: 7494 286a 4604 0000 8c34 4845 4154 494e  t.(jF....4HEATIN
-00004b40: 475f 484f 5445 4e44 2028 696e 206d 6f64  G_HOTEND (in mod
-00004b50: 756c 6520 6261 6d62 756c 6162 735f 6170  ule bambulabs_ap
-00004b60: 692e 5072 696e 7453 7461 7475 7329 948c  i.PrintStatus)..
-00004b70: 2862 616d 6275 6c61 6273 5f61 7069 2e50  (bambulabs_api.P
-00004b80: 7269 6e74 5374 6174 7573 2e48 4541 5449  rintStatus.HEATI
-00004b90: 4e47 5f48 4f54 454e 4494 6842 4e74 9428  NG_HOTEND.hBNt.(
-00004ba0: 6a46 0400 008c 3b43 414c 4942 5241 5449  jF....;CALIBRATI
-00004bb0: 4e47 5f45 5854 5255 5349 4f4e 2028 696e  NG_EXTRUSION (in
-00004bc0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00004bd0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
-00004be0: 7329 948c 2f62 616d 6275 6c61 6273 5f61  s)../bambulabs_a
-00004bf0: 7069 2e50 7269 6e74 5374 6174 7573 2e43  pi.PrintStatus.C
-00004c00: 414c 4942 5241 5449 4e47 5f45 5854 5255  ALIBRATING_EXTRU
-00004c10: 5349 4f4e 9468 424e 7494 286a 4604 0000  SION.hBNt.(jF...
-00004c20: 8c3a 5343 414e 4e49 4e47 5f42 4544 5f53  .:SCANNING_BED_S
-00004c30: 5552 4641 4345 2028 696e 206d 6f64 756c  URFACE (in modul
-00004c40: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-00004c50: 5072 696e 7453 7461 7475 7329 948c 2e62  PrintStatus)...b
+00004a30: 6e74 5374 6174 7573 2994 8c2b 6261 6d62  ntStatus)..+bamb
+00004a40: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+00004a50: 7461 7475 732e 4155 544f 5f42 4544 5f4c  tatus.AUTO_BED_L
+00004a60: 4556 454c 494e 4794 6842 4e74 9428 6a6a  EVELING.hBNt.(jj
+00004a70: 0400 008c 3848 4541 5442 4544 5f50 5245  ....8HEATBED_PRE
+00004a80: 4845 4154 494e 4720 2869 6e20 6d6f 6475  HEATING (in modu
+00004a90: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00004aa0: 2e50 7269 6e74 5374 6174 7573 2994 8c2c  .PrintStatus)..,
+00004ab0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+00004ac0: 696e 7453 7461 7475 732e 4845 4154 4245  intStatus.HEATBE
+00004ad0: 445f 5052 4548 4541 5449 4e47 9468 424e  D_PREHEATING.hBN
+00004ae0: 7494 286a 6a04 0000 8c3b 5357 4545 5049  t.(jj....;SWEEPI
+00004af0: 4e47 5f58 595f 4d45 4348 5f4d 4f44 4520  NG_XY_MECH_MODE 
+00004b00: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+00004b10: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+00004b20: 6174 7573 2994 8c2f 6261 6d62 756c 6162  atus)../bambulab
+00004b30: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00004b40: 732e 5357 4545 5049 4e47 5f58 595f 4d45  s.SWEEPING_XY_ME
+00004b50: 4348 5f4d 4f44 4594 6842 4e74 9428 6a6a  CH_MODE.hBNt.(jj
+00004b60: 0400 008c 3743 4841 4e47 494e 475f 4649  ....7CHANGING_FI
+00004b70: 4c41 4d45 4e54 2028 696e 206d 6f64 756c  LAMENT (in modul
+00004b80: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00004b90: 5072 696e 7453 7461 7475 7329 948c 2b62  PrintStatus)..+b
+00004ba0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00004bb0: 6e74 5374 6174 7573 2e43 4841 4e47 494e  ntStatus.CHANGIN
+00004bc0: 475f 4649 4c41 4d45 4e54 9468 424e 7494  G_FILAMENT.hBNt.
+00004bd0: 286a 6a04 0000 8c30 4d34 3030 5f50 4155  (jj....0M400_PAU
+00004be0: 5345 2028 696e 206d 6f64 756c 6520 6261  SE (in module ba
+00004bf0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00004c00: 7453 7461 7475 7329 948c 2462 616d 6275  tStatus)..$bambu
+00004c10: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+00004c20: 6174 7573 2e4d 3430 305f 5041 5553 4594  atus.M400_PAUSE.
+00004c30: 6842 4e74 9428 6a6a 0400 008c 3c50 4155  hBNt.(jj....<PAU
+00004c40: 5345 445f 4649 4c41 4d45 4e54 5f52 554e  SED_FILAMENT_RUN
+00004c50: 4f55 5420 2869 6e20 6d6f 6475 6c65 2062  OUT (in module b
 00004c60: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00004c70: 6e74 5374 6174 7573 2e53 4341 4e4e 494e  ntStatus.SCANNIN
-00004c80: 475f 4245 445f 5355 5246 4143 4594 6842  G_BED_SURFACE.hB
-00004c90: 4e74 9428 6a46 0400 008c 3c49 4e53 5045  Nt.(jF....<INSPE
-00004ca0: 4354 494e 475f 4649 5253 545f 4c41 5945  CTING_FIRST_LAYE
-00004cb0: 5220 2869 6e20 6d6f 6475 6c65 2062 616d  R (in module bam
-00004cc0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00004cd0: 5374 6174 7573 2994 8c30 6261 6d62 756c  Status)..0bambul
-00004ce0: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-00004cf0: 7475 732e 494e 5350 4543 5449 4e47 5f46  tus.INSPECTING_F
-00004d00: 4952 5354 5f4c 4159 4552 9468 424e 7494  IRST_LAYER.hBNt.
-00004d10: 286a 4604 0000 8c42 4944 454e 5449 4659  (jF....BIDENTIFY
-00004d20: 494e 475f 4255 494c 445f 504c 4154 455f  ING_BUILD_PLATE_
-00004d30: 5459 5045 2028 696e 206d 6f64 756c 6520  TYPE (in module 
-00004d40: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00004d50: 696e 7453 7461 7475 7329 948c 3662 616d  intStatus)..6bam
-00004d60: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00004d70: 5374 6174 7573 2e49 4445 4e54 4946 5949  Status.IDENTIFYI
-00004d80: 4e47 5f42 5549 4c44 5f50 4c41 5445 5f54  NG_BUILD_PLATE_T
-00004d90: 5950 4594 6842 4e74 9428 6a46 0400 008c  YPE.hBNt.(jF....
-00004da0: 3d43 414c 4942 5241 5449 4e47 5f4d 4943  =CALIBRATING_MIC
-00004db0: 524f 5f4c 4944 4152 2028 696e 206d 6f64  RO_LIDAR (in mod
-00004dc0: 756c 6520 6261 6d62 756c 6162 735f 6170  ule bambulabs_ap
-00004dd0: 692e 5072 696e 7453 7461 7475 7329 948c  i.PrintStatus)..
-00004de0: 3162 616d 6275 6c61 6273 5f61 7069 2e50  1bambulabs_api.P
-00004df0: 7269 6e74 5374 6174 7573 2e43 414c 4942  rintStatus.CALIB
-00004e00: 5241 5449 4e47 5f4d 4943 524f 5f4c 4944  RATING_MICRO_LID
-00004e10: 4152 9468 424e 7494 286a 4604 0000 8c35  AR.hBNt.(jF....5
-00004e20: 484f 4d49 4e47 5f54 4f4f 4c48 4541 4420  HOMING_TOOLHEAD 
-00004e30: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
-00004e40: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00004e50: 6174 7573 2994 8c29 6261 6d62 756c 6162  atus)..)bambulab
-00004e60: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
-00004e70: 732e 484f 4d49 4e47 5f54 4f4f 4c48 4541  s.HOMING_TOOLHEA
-00004e80: 4494 6842 4e74 9428 6a46 0400 008c 3943  D.hBNt.(jF....9C
-00004e90: 4c45 414e 494e 475f 4e4f 5a5a 4c45 5f54  LEANING_NOZZLE_T
-00004ea0: 4950 2028 696e 206d 6f64 756c 6520 6261  IP (in module ba
-00004eb0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00004ec0: 7453 7461 7475 7329 948c 2d62 616d 6275  tStatus)..-bambu
-00004ed0: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00004ee0: 6174 7573 2e43 4c45 414e 494e 475f 4e4f  atus.CLEANING_NO
-00004ef0: 5a5a 4c45 5f54 4950 9468 424e 7494 286a  ZZLE_TIP.hBNt.(j
-00004f00: 4604 0000 8c43 4348 4543 4b49 4e47 5f45  F....CCHECKING_E
-00004f10: 5854 5255 4445 525f 5445 4d50 4552 4154  XTRUDER_TEMPERAT
-00004f20: 5552 4520 2869 6e20 6d6f 6475 6c65 2062  URE (in module b
-00004f30: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00004f40: 6e74 5374 6174 7573 2994 8c37 6261 6d62  ntStatus)..7bamb
-00004f50: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00004f60: 7461 7475 732e 4348 4543 4b49 4e47 5f45  tatus.CHECKING_E
-00004f70: 5854 5255 4445 525f 5445 4d50 4552 4154  XTRUDER_TEMPERAT
-00004f80: 5552 4594 6842 4e74 9428 6a46 0400 008c  URE.hBNt.(jF....
-00004f90: 3150 4155 5345 445f 5553 4552 2028 696e  1PAUSED_USER (in
-00004fa0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00004fb0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
-00004fc0: 7329 948c 2562 616d 6275 6c61 6273 5f61  s)..%bambulabs_a
-00004fd0: 7069 2e50 7269 6e74 5374 6174 7573 2e50  pi.PrintStatus.P
-00004fe0: 4155 5345 445f 5553 4552 9468 424e 7494  AUSED_USER.hBNt.
-00004ff0: 286a 4604 0000 8c40 5041 5553 4544 5f46  (jF....@PAUSED_F
-00005000: 524f 4e54 5f43 4f56 4552 5f46 414c 4c49  RONT_COVER_FALLI
-00005010: 4e47 2028 696e 206d 6f64 756c 6520 6261  NG (in module ba
-00005020: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00005030: 7453 7461 7475 7329 948c 3462 616d 6275  tStatus)..4bambu
-00005040: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00005050: 6174 7573 2e50 4155 5345 445f 4652 4f4e  atus.PAUSED_FRON
-00005060: 545f 434f 5645 525f 4641 4c4c 494e 4794  T_COVER_FALLING.
-00005070: 6842 4e74 9428 6a46 0400 008c 3743 414c  hBNt.(jF....7CAL
-00005080: 4942 5241 5449 4e47 5f4c 4944 4152 2028  IBRATING_LIDAR (
-00005090: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
-000050a0: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-000050b0: 7475 7329 948c 2b62 616d 6275 6c61 6273  tus)..+bambulabs
-000050c0: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
-000050d0: 2e43 414c 4942 5241 5449 4e47 5f4c 4944  .CALIBRATING_LID
-000050e0: 4152 9468 424e 7494 286a 4604 0000 8c40  AR.hBNt.(jF....@
-000050f0: 4341 4c49 4252 4154 494e 475f 4558 5452  CALIBRATING_EXTR
-00005100: 5553 494f 4e5f 464c 4f57 2028 696e 206d  USION_FLOW (in m
-00005110: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
-00005120: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
-00005130: 948c 3462 616d 6275 6c61 6273 5f61 7069  ..4bambulabs_api
-00005140: 2e50 7269 6e74 5374 6174 7573 2e43 414c  .PrintStatus.CAL
-00005150: 4942 5241 5449 4e47 5f45 5854 5255 5349  IBRATING_EXTRUSI
-00005160: 4f4e 5f46 4c4f 5794 6842 4e74 9428 6a46  ON_FLOW.hBNt.(jF
-00005170: 0400 008c 4b50 4155 5345 445f 4e4f 5a5a  ....KPAUSED_NOZZ
-00005180: 4c45 5f54 454d 5045 5241 5455 5245 5f4d  LE_TEMPERATURE_M
-00005190: 414c 4655 4e43 5449 4f4e 2028 696e 206d  ALFUNCTION (in m
-000051a0: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
-000051b0: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
-000051c0: 948c 3f62 616d 6275 6c61 6273 5f61 7069  ..?bambulabs_api
-000051d0: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
-000051e0: 5345 445f 4e4f 5a5a 4c45 5f54 454d 5045  SED_NOZZLE_TEMPE
-000051f0: 5241 5455 5245 5f4d 414c 4655 4e43 5449  RATURE_MALFUNCTI
-00005200: 4f4e 9468 424e 7494 286a 4604 0000 8c4d  ON.hBNt.(jF....M
-00005210: 5041 5553 4544 5f48 4541 545f 4245 445f  PAUSED_HEAT_BED_
-00005220: 5445 4d50 4552 4154 5552 455f 4d41 4c46  TEMPERATURE_MALF
-00005230: 554e 4354 494f 4e20 2869 6e20 6d6f 6475  UNCTION (in modu
-00005240: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00005250: 2e50 7269 6e74 5374 6174 7573 2994 8c41  .PrintStatus)..A
-00005260: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00005270: 696e 7453 7461 7475 732e 5041 5553 4544  intStatus.PAUSED
-00005280: 5f48 4541 545f 4245 445f 5445 4d50 4552  _HEAT_BED_TEMPER
-00005290: 4154 5552 455f 4d41 4c46 554e 4354 494f  ATURE_MALFUNCTIO
-000052a0: 4e94 6842 4e74 9428 6a46 0400 008c 3846  N.hBNt.(jF....8F
-000052b0: 494c 414d 454e 545f 554e 4c4f 4144 494e  ILAMENT_UNLOADIN
-000052c0: 4720 2869 6e20 6d6f 6475 6c65 2062 616d  G (in module bam
-000052d0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-000052e0: 5374 6174 7573 2994 8c2c 6261 6d62 756c  Status)..,bambul
-000052f0: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-00005300: 7475 732e 4649 4c41 4d45 4e54 5f55 4e4c  tus.FILAMENT_UNL
-00005310: 4f41 4449 4e47 9468 424e 7494 286a 4604  OADING.hBNt.(jF.
-00005320: 0000 8c39 5041 5553 4544 5f53 4b49 5050  ...9PAUSED_SKIPP
-00005330: 4544 5f53 5445 5020 2869 6e20 6d6f 6475  ED_STEP (in modu
-00005340: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
-00005350: 2e50 7269 6e74 5374 6174 7573 2994 8c2d  .PrintStatus)..-
-00005360: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00005370: 696e 7453 7461 7475 732e 5041 5553 4544  intStatus.PAUSED
-00005380: 5f53 4b49 5050 4544 5f53 5445 5094 6842  _SKIPPED_STEP.hB
-00005390: 4e74 9428 6a46 0400 008c 3646 494c 414d  Nt.(jF....6FILAM
-000053a0: 454e 545f 4c4f 4144 494e 4720 2869 6e20  ENT_LOADING (in 
-000053b0: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
-000053c0: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
-000053d0: 2994 8c2a 6261 6d62 756c 6162 735f 6170  )..*bambulabs_ap
-000053e0: 692e 5072 696e 7453 7461 7475 732e 4649  i.PrintStatus.FI
-000053f0: 4c41 4d45 4e54 5f4c 4f41 4449 4e47 9468  LAMENT_LOADING.h
-00005400: 424e 7494 286a 4604 0000 8c3d 4341 4c49  BNt.(jF....=CALI
-00005410: 4252 4154 494e 475f 4d4f 544f 525f 4e4f  BRATING_MOTOR_NO
-00005420: 4953 4520 2869 6e20 6d6f 6475 6c65 2062  ISE (in module b
-00005430: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00005440: 6e74 5374 6174 7573 2994 8c31 6261 6d62  ntStatus)..1bamb
-00005450: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00005460: 7461 7475 732e 4341 4c49 4252 4154 494e  tatus.CALIBRATIN
-00005470: 475f 4d4f 544f 525f 4e4f 4953 4594 6842  G_MOTOR_NOISE.hB
-00005480: 4e74 9428 6a46 0400 008c 3550 4155 5345  Nt.(jF....5PAUSE
-00005490: 445f 414d 535f 4c4f 5354 2028 696e 206d  D_AMS_LOST (in m
-000054a0: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
-000054b0: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
-000054c0: 948c 2962 616d 6275 6c61 6273 5f61 7069  ..)bambulabs_api
-000054d0: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
-000054e0: 5345 445f 414d 535f 4c4f 5354 9468 424e  SED_AMS_LOST.hBN
-000054f0: 7494 286a 4604 0000 8c45 5041 5553 4544  t.(jF....EPAUSED
-00005500: 5f4c 4f57 5f46 414e 5f53 5045 4544 5f48  _LOW_FAN_SPEED_H
-00005510: 4541 545f 4252 4541 4b20 2869 6e20 6d6f  EAT_BREAK (in mo
-00005520: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
-00005530: 7069 2e50 7269 6e74 5374 6174 7573 2994  pi.PrintStatus).
-00005540: 8c39 6261 6d62 756c 6162 735f 6170 692e  .9bambulabs_api.
-00005550: 5072 696e 7453 7461 7475 732e 5041 5553  PrintStatus.PAUS
-00005560: 4544 5f4c 4f57 5f46 414e 5f53 5045 4544  ED_LOW_FAN_SPEED
-00005570: 5f48 4541 545f 4252 4541 4b94 6842 4e74  _HEAT_BREAK.hBNt
-00005580: 9428 6a46 0400 008c 4e50 4155 5345 445f  .(jF....NPAUSED_
-00005590: 4348 414d 4245 525f 5445 4d50 4552 4154  CHAMBER_TEMPERAT
-000055a0: 5552 455f 434f 4e54 524f 4c5f 4552 524f  URE_CONTROL_ERRO
-000055b0: 5220 2869 6e20 6d6f 6475 6c65 2062 616d  R (in module bam
-000055c0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-000055d0: 5374 6174 7573 2994 8c42 6261 6d62 756c  Status)..Bbambul
-000055e0: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-000055f0: 7475 732e 5041 5553 4544 5f43 4841 4d42  tus.PAUSED_CHAMB
-00005600: 4552 5f54 454d 5045 5241 5455 5245 5f43  ER_TEMPERATURE_C
-00005610: 4f4e 5452 4f4c 5f45 5252 4f52 9468 424e  ONTROL_ERROR.hBN
-00005620: 7494 286a 4604 0000 8c35 434f 4f4c 494e  t.(jF....5COOLIN
-00005630: 475f 4348 414d 4245 5220 2869 6e20 6d6f  G_CHAMBER (in mo
-00005640: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
-00005650: 7069 2e50 7269 6e74 5374 6174 7573 2994  pi.PrintStatus).
-00005660: 8c29 6261 6d62 756c 6162 735f 6170 692e  .)bambulabs_api.
-00005670: 5072 696e 7453 7461 7475 732e 434f 4f4c  PrintStatus.COOL
-00005680: 494e 475f 4348 414d 4245 5294 6842 4e74  ING_CHAMBER.hBNt
-00005690: 9428 6a46 0400 008c 3750 4155 5345 445f  .(jF....7PAUSED_
-000056a0: 5553 4552 5f47 434f 4445 2028 696e 206d  USER_GCODE (in m
-000056b0: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
-000056c0: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
-000056d0: 948c 2b62 616d 6275 6c61 6273 5f61 7069  ..+bambulabs_api
-000056e0: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
-000056f0: 5345 445f 5553 4552 5f47 434f 4445 9468  SED_USER_GCODE.h
-00005700: 424e 7494 286a 4604 0000 8c39 4d4f 544f  BNt.(jF....9MOTO
-00005710: 525f 4e4f 4953 455f 5348 4f57 4f46 4620  R_NOISE_SHOWOFF 
-00005720: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
-00005730: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00005740: 6174 7573 2994 8c2d 6261 6d62 756c 6162  atus)..-bambulab
-00005750: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
-00005760: 732e 4d4f 544f 525f 4e4f 4953 455f 5348  s.MOTOR_NOISE_SH
-00005770: 4f57 4f46 4694 6842 4e74 9428 6a46 0400  OWOFF.hBNt.(jF..
-00005780: 008c 4d50 4155 5345 445f 4e4f 5a5a 4c45  ..MPAUSED_NOZZLE
-00005790: 5f46 494c 414d 454e 545f 434f 5645 5245  _FILAMENT_COVERE
-000057a0: 445f 4445 5445 4354 4544 2028 696e 206d  D_DETECTED (in m
-000057b0: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
-000057c0: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
-000057d0: 948c 4162 616d 6275 6c61 6273 5f61 7069  ..Abambulabs_api
-000057e0: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
-000057f0: 5345 445f 4e4f 5a5a 4c45 5f46 494c 414d  SED_NOZZLE_FILAM
-00005800: 454e 545f 434f 5645 5245 445f 4445 5445  ENT_COVERED_DETE
-00005810: 4354 4544 9468 424e 7494 286a 4604 0000  CTED.hBNt.(jF...
-00005820: 8c39 5041 5553 4544 5f43 5554 5445 525f  .9PAUSED_CUTTER_
-00005830: 4552 524f 5220 2869 6e20 6d6f 6475 6c65  ERROR (in module
-00005840: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
-00005850: 7269 6e74 5374 6174 7573 2994 8c2d 6261  rintStatus)..-ba
-00005860: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00005870: 7453 7461 7475 732e 5041 5553 4544 5f43  tStatus.PAUSED_C
-00005880: 5554 5445 525f 4552 524f 5294 6842 4e74  UTTER_ERROR.hBNt
-00005890: 9428 6a46 0400 008c 3e50 4155 5345 445f  .(jF....>PAUSED_
-000058a0: 4649 5253 545f 4c41 5945 525f 4552 524f  FIRST_LAYER_ERRO
-000058b0: 5220 2869 6e20 6d6f 6475 6c65 2062 616d  R (in module bam
-000058c0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-000058d0: 5374 6174 7573 2994 8c32 6261 6d62 756c  Status)..2bambul
-000058e0: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-000058f0: 7475 732e 5041 5553 4544 5f46 4952 5354  tus.PAUSED_FIRST
-00005900: 5f4c 4159 4552 5f45 5252 4f52 9468 424e  _LAYER_ERROR.hBN
-00005910: 7494 286a 4604 0000 8c38 5041 5553 4544  t.(jF....8PAUSED
-00005920: 5f4e 4f5a 5a4c 455f 434c 4f47 2028 696e  _NOZZLE_CLOG (in
-00005930: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
-00005940: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
-00005950: 7329 948c 2c62 616d 6275 6c61 6273 5f61  s)..,bambulabs_a
-00005960: 7069 2e50 7269 6e74 5374 6174 7573 2e50  pi.PrintStatus.P
-00005970: 4155 5345 445f 4e4f 5a5a 4c45 5f43 4c4f  AUSED_NOZZLE_CLO
-00005980: 4794 6842 4e74 9428 6a46 0400 008c 2d55  G.hBNt.(jF....-U
-00005990: 4e4b 4e4f 574e 2028 696e 206d 6f64 756c  NKNOWN (in modul
-000059a0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
-000059b0: 5072 696e 7453 7461 7475 7329 948c 2162  PrintStatus)..!b
-000059c0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-000059d0: 6e74 5374 6174 7573 2e55 4e4b 4e4f 574e  ntStatus.UNKNOWN
-000059e0: 9468 424e 7494 286a 4604 0000 8c2a 4944  .hBNt.(jF....*ID
-000059f0: 4c45 2028 696e 206d 6f64 756c 6520 6261  LE (in module ba
-00005a00: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00005a10: 7453 7461 7475 7329 948c 1e62 616d 6275  tStatus)...bambu
-00005a20: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00005a30: 6174 7573 2e49 444c 4594 6842 4e74 9465  atus.IDLE.hBNt.e
-00005a40: 7375 8c02 6a73 947d 9428 6a25 0400 007d  su..js.}.(j%...}
-00005a50: 948c 076d 6f64 756c 6573 947d 946a b402  ...modules.}.j..
-00005a60: 0000 4b00 758c 046d 6174 6894 7d94 286a  ..K.u..math.}.(j
-00005a70: 2504 0000 7d94 8c0d 6861 735f 6571 7561  %...}...has_equa
-00005a80: 7469 6f6e 7394 7d94 6ab3 0200 0089 736a  tions.}.j.....sj
-00005a90: b402 0000 4b00 758c 0270 7994 7d94 286a  ....K.u..py.}.(j
-00005aa0: 2504 0000 7d94 288c 1562 616d 6275 6c61  %...}.(..bambula
-00005ab0: 6273 5f61 7069 2e50 7269 6e74 6572 948c  bs_api.Printer..
-00005ac0: 1573 7068 696e 782e 646f 6d61 696e 732e  .sphinx.domains.
-00005ad0: 7079 7468 6f6e 948c 0b4f 626a 6563 7445  python...ObjectE
-00005ae0: 6e74 7279 9493 9428 6ab3 0200 006a 4404  ntry...(j....jD.
-00005af0: 0000 8c06 6d6f 6475 6c65 9489 7494 8194  ....module..t...
-00005b00: 8c27 6261 6d62 756c 6162 735f 6170 692e  .'bambulabs_api.
-00005b10: 5072 696e 7465 722e 6361 6c69 6272 6174  Printer.calibrat
-00005b20: 655f 7072 696e 7465 7294 6a71 0500 0028  e_printer.jq...(
-00005b30: 6ab3 0200 006a 4804 0000 8c08 6675 6e63  j....jH.....func
-00005b40: 7469 6f6e 9489 7494 8194 8c1d 6261 6d62  tion..t.....bamb
-00005b50: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00005b60: 722e 636f 6e6e 6563 7494 6a71 0500 0028  r.connect.jq...(
-00005b70: 6ab3 0200 006a 4b04 0000 8c08 6675 6e63  j....jK.....func
-00005b80: 7469 6f6e 9489 7494 8194 8c21 6261 6d62  tion..t....!bamb
-00005b90: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00005ba0: 722e 6465 6c65 7465 5f66 696c 6594 6a71  r.delete_file.jq
-00005bb0: 0500 0028 6ab3 0200 006a 4e04 0000 8c08  ...(j....jN.....
-00005bc0: 6675 6e63 7469 6f6e 9489 7494 8194 8c20  function..t.... 
-00005bd0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00005be0: 696e 7465 722e 6469 7363 6f6e 6e65 6374  inter.disconnect
-00005bf0: 946a 7105 0000 286a b302 0000 6a51 0400  .jq...(j....jQ..
-00005c00: 008c 0866 756e 6374 696f 6e94 8974 9481  ...function..t..
-00005c10: 948c 2962 616d 6275 6c61 6273 5f61 7069  ..)bambulabs_api
-00005c20: 2e50 7269 6e74 6572 2e67 6574 5f62 6564  .Printer.get_bed
-00005c30: 5f74 656d 7065 7261 7475 7265 946a 7105  _temperature.jq.
-00005c40: 0000 286a b302 0000 6a54 0400 008c 0866  ..(j....jT.....f
-00005c50: 756e 6374 696f 6e94 8974 9481 948c 2662  unction..t....&b
-00005c60: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00005c70: 6e74 6572 2e67 6574 5f63 616d 6572 615f  nter.get_camera_
-00005c80: 6672 616d 6594 6a71 0500 0028 6ab3 0200  frame.jq...(j...
-00005c90: 006a 5704 0000 8c08 6675 6e63 7469 6f6e  .jW.....function
-00005ca0: 9489 7494 8194 8c23 6261 6d62 756c 6162  ..t....#bambulab
-00005cb0: 735f 6170 692e 5072 696e 7465 722e 6765  s_api.Printer.ge
-00005cc0: 745f 6669 6c65 5f6e 616d 6594 6a71 0500  t_file_name.jq..
-00005cd0: 0028 6ab3 0200 006a 5a04 0000 8c08 6675  .(j....jZ.....fu
-00005ce0: 6e63 7469 6f6e 9489 7494 8194 8c25 6261  nction..t....%ba
-00005cf0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00005d00: 7465 722e 6765 745f 6c69 6768 745f 7374  ter.get_light_st
-00005d10: 6174 6594 6a71 0500 0028 6ab3 0200 006a  ate.jq...(j....j
-00005d20: 5d04 0000 8c08 6675 6e63 7469 6f6e 9489  ].....function..
-00005d30: 7494 8194 8c2c 6261 6d62 756c 6162 735f  t....,bambulabs_
-00005d40: 6170 692e 5072 696e 7465 722e 6765 745f  api.Printer.get_
-00005d50: 6e6f 7a7a 6c65 5f74 656d 7065 7261 7475  nozzle_temperatu
-00005d60: 7265 946a 7105 0000 286a b302 0000 6a60  re.jq...(j....j`
-00005d70: 0400 008c 0866 756e 6374 696f 6e94 8974  .....function..t
-00005d80: 9481 948c 2462 616d 6275 6c61 6273 5f61  ....$bambulabs_a
-00005d90: 7069 2e50 7269 6e74 6572 2e67 6574 5f70  pi.Printer.get_p
-00005da0: 6572 6365 6e74 6167 6594 6a71 0500 0028  ercentage.jq...(
-00005db0: 6ab3 0200 006a 6304 0000 8c08 6675 6e63  j....jc.....func
-00005dc0: 7469 6f6e 9489 7494 8194 8c25 6261 6d62  tion..t....%bamb
-00005dd0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00005de0: 722e 6765 745f 7072 696e 745f 7370 6565  r.get_print_spee
-00005df0: 6494 6a71 0500 0028 6ab3 0200 006a 6604  d.jq...(j....jf.
-00005e00: 0000 8c08 6675 6e63 7469 6f6e 9489 7494  ....function..t.
-00005e10: 8194 8c1f 6261 6d62 756c 6162 735f 6170  ....bambulabs_ap
-00005e20: 692e 5072 696e 7465 722e 6765 745f 7374  i.Printer.get_st
-00005e30: 6174 6594 6a71 0500 0028 6ab3 0200 006a  ate.jq...(j....j
-00005e40: 6904 0000 8c08 6675 6e63 7469 6f6e 9489  i.....function..
-00005e50: 7494 8194 8c1e 6261 6d62 756c 6162 735f  t.....bambulabs_
-00005e60: 6170 692e 5072 696e 7465 722e 6765 745f  api.Printer.get_
-00005e70: 7469 6d65 946a 7105 0000 286a b302 0000  time.jq...(j....
-00005e80: 6a6c 0400 008c 0866 756e 6374 696f 6e94  jl.....function.
-00005e90: 8974 9481 948c 2262 616d 6275 6c61 6273  .t...."bambulabs
-00005ea0: 5f61 7069 2e50 7269 6e74 6572 2e68 6f6d  _api.Printer.hom
-00005eb0: 655f 7072 696e 7465 7294 6a71 0500 0028  e_printer.jq...(
-00005ec0: 6ab3 0200 006a 6f04 0000 8c08 6675 6e63  j....jo.....func
-00005ed0: 7469 6f6e 9489 7494 8194 8c29 6261 6d62  tion..t....)bamb
-00005ee0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00005ef0: 722e 6c6f 6164 5f66 696c 616d 656e 745f  r.load_filament_
-00005f00: 7370 6f6f 6c94 6a71 0500 0028 6ab3 0200  spool.jq...(j...
-00005f10: 006a 7204 0000 8c08 6675 6e63 7469 6f6e  .jr.....function
-00005f20: 9489 7494 8194 8c21 6261 6d62 756c 6162  ..t....!bambulab
-00005f30: 735f 6170 692e 5072 696e 7465 722e 6d6f  s_api.Printer.mo
-00005f40: 7665 5f7a 5f61 7869 7394 6a71 0500 0028  ve_z_axis.jq...(
-00005f50: 6ab3 0200 006a 7504 0000 8c08 6675 6e63  j....ju.....func
-00005f60: 7469 6f6e 9489 7494 8194 8c21 6261 6d62  tion..t....!bamb
-00005f70: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-00005f80: 722e 7061 7573 655f 7072 696e 7494 6a71  r.pause_print.jq
-00005f90: 0500 0028 6ab3 0200 006a 7804 0000 8c08  ...(j....jx.....
-00005fa0: 6675 6e63 7469 6f6e 9489 7494 8194 8c22  function..t...."
-00005fb0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00005fc0: 696e 7465 722e 7265 7375 6d65 5f70 7269  inter.resume_pri
-00005fd0: 6e74 946a 7105 0000 286a b302 0000 6a7b  nt.jq...(j....j{
-00005fe0: 0400 008c 0866 756e 6374 696f 6e94 8974  .....function..t
-00005ff0: 9481 948c 2b62 616d 6275 6c61 6273 5f61  ....+bambulabs_a
-00006000: 7069 2e50 7269 6e74 6572 2e72 6574 7279  pi.Printer.retry
-00006010: 5f66 696c 616d 656e 745f 6163 7469 6f6e  _filament_action
-00006020: 946a 7105 0000 286a b302 0000 6a7e 0400  .jq...(j....j~..
-00006030: 008c 0866 756e 6374 696f 6e94 8974 9481  ...function..t..
-00006040: 948c 2962 616d 6275 6c61 6273 5f61 7069  ..)bambulabs_api
-00006050: 2e50 7269 6e74 6572 2e73 6574 5f62 6564  .Printer.set_bed
-00006060: 5f74 656d 7065 7261 7475 7265 946a 7105  _temperature.jq.
-00006070: 0000 286a b302 0000 6a81 0400 008c 0866  ..(j....j......f
-00006080: 756e 6374 696f 6e94 8974 9481 948c 2a62  unction..t....*b
-00006090: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-000060a0: 6e74 6572 2e73 6574 5f66 696c 616d 656e  nter.set_filamen
-000060b0: 745f 7072 696e 7465 7294 6a71 0500 0028  t_printer.jq...(
-000060c0: 6ab3 0200 006a 8404 0000 8c08 6675 6e63  j....j......func
-000060d0: 7469 6f6e 9489 7494 8194 8c2c 6261 6d62  tion..t....,bamb
-000060e0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
-000060f0: 722e 7365 745f 6e6f 7a7a 6c65 5f74 656d  r.set_nozzle_tem
-00006100: 7065 7261 7475 7265 946a 7105 0000 286a  perature.jq...(j
-00006110: b302 0000 6a87 0400 008c 0866 756e 6374  ....j......funct
-00006120: 696f 6e94 8974 9481 948c 2562 616d 6275  ion..t....%bambu
-00006130: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
-00006140: 2e73 6574 5f70 7269 6e74 5f73 7065 6564  .set_print_speed
-00006150: 946a 7105 0000 286a b302 0000 6a8a 0400  .jq...(j....j...
-00006160: 008c 0866 756e 6374 696f 6e94 8974 9481  ...function..t..
-00006170: 948c 2162 616d 6275 6c61 6273 5f61 7069  ..!bambulabs_api
-00006180: 2e50 7269 6e74 6572 2e73 7461 7274 5f70  .Printer.start_p
-00006190: 7269 6e74 946a 7105 0000 286a b302 0000  rint.jq...(j....
-000061a0: 6a8d 0400 008c 0866 756e 6374 696f 6e94  j......function.
-000061b0: 8974 9481 948c 2062 616d 6275 6c61 6273  .t.... bambulabs
-000061c0: 5f61 7069 2e50 7269 6e74 6572 2e73 746f  _api.Printer.sto
-000061d0: 705f 7072 696e 7494 6a71 0500 0028 6ab3  p_print.jq...(j.
-000061e0: 0200 006a 9004 0000 8c08 6675 6e63 7469  ...j......functi
-000061f0: 6f6e 9489 7494 8194 8c24 6261 6d62 756c  on..t....$bambul
-00006200: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
-00006210: 7475 726e 5f6c 6967 6874 5f6f 6666 946a  turn_light_off.j
-00006220: 7105 0000 286a b302 0000 6a93 0400 008c  q...(j....j.....
-00006230: 0866 756e 6374 696f 6e94 8974 9481 948c  .function..t....
-00006240: 2362 616d 6275 6c61 6273 5f61 7069 2e50  #bambulabs_api.P
-00006250: 7269 6e74 6572 2e74 7572 6e5f 6c69 6768  rinter.turn_ligh
-00006260: 745f 6f6e 946a 7105 0000 286a b302 0000  t_on.jq...(j....
-00006270: 6a96 0400 008c 0866 756e 6374 696f 6e94  j......function.
-00006280: 8974 9481 948c 2b62 616d 6275 6c61 6273  .t....+bambulabs
-00006290: 5f61 7069 2e50 7269 6e74 6572 2e75 6e6c  _api.Printer.unl
-000062a0: 6f61 645f 6669 6c61 6d65 6e74 5f73 706f  oad_filament_spo
-000062b0: 6f6c 946a 7105 0000 286a b302 0000 6a99  ol.jq...(j....j.
-000062c0: 0400 008c 0866 756e 6374 696f 6e94 8974  .....function..t
-000062d0: 9481 948c 2162 616d 6275 6c61 6273 5f61  ....!bambulabs_a
-000062e0: 7069 2e50 7269 6e74 6572 2e75 706c 6f61  pi.Printer.uploa
-000062f0: 645f 6669 6c65 946a 7105 0000 286a b302  d_file.jq...(j..
-00006300: 0000 6a9c 0400 008c 0866 756e 6374 696f  ..j......functio
-00006310: 6e94 8974 9481 948c 1662 616d 6275 6c61  n..t.....bambula
-00006320: 6273 5f61 7069 2e46 696c 616d 656e 7494  bs_api.Filament.
-00006330: 6a71 0500 0028 6ab3 0200 006a 9f04 0000  jq...(j....j....
-00006340: 6a72 0500 0089 7494 8194 8c23 6261 6d62  jr....t....#bamb
-00006350: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
-00006360: 6e74 2e50 4f4c 594c 4954 455f 504c 4194  nt.POLYLITE_PLA.
-00006370: 6a71 0500 0028 6ab3 0200 006a a204 0000  jq...(j....j....
-00006380: 8c09 6174 7472 6962 7574 6594 8974 9481  ..attribute..t..
-00006390: 948c 2462 616d 6275 6c61 6273 5f61 7069  ..$bambulabs_api
-000063a0: 2e46 696c 616d 656e 742e 504f 4c59 5445  .Filament.POLYTE
-000063b0: 5252 415f 504c 4194 6a71 0500 0028 6ab3  RRA_PLA.jq...(j.
-000063c0: 0200 006a a504 0000 8c09 6174 7472 6962  ...j......attrib
-000063d0: 7574 6594 8974 9481 948c 2062 616d 6275  ute..t.... bambu
-000063e0: 6c61 6273 5f61 7069 2e46 696c 616d 656e  labs_api.Filamen
-000063f0: 742e 4241 4d42 555f 4142 5394 6a71 0500  t.BAMBU_ABS.jq..
-00006400: 0028 6ab3 0200 006a a804 0000 8c09 6174  .(j....j......at
-00006410: 7472 6962 7574 6594 8974 9481 948c 2262  tribute..t...."b
-00006420: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-00006430: 616d 656e 742e 4241 4d42 555f 5041 5f43  ament.BAMBU_PA_C
-00006440: 4694 6a71 0500 0028 6ab3 0200 006a ab04  F.jq...(j....j..
-00006450: 0000 8c09 6174 7472 6962 7574 6594 8974  ....attribute..t
-00006460: 9481 948c 1f62 616d 6275 6c61 6273 5f61  .....bambulabs_a
-00006470: 7069 2e46 696c 616d 656e 742e 4241 4d42  pi.Filament.BAMB
-00006480: 555f 5043 946a 7105 0000 286a b302 0000  U_PC.jq...(j....
-00006490: 6aae 0400 008c 0961 7474 7269 6275 7465  j......attribute
-000064a0: 9489 7494 8194 8c26 6261 6d62 756c 6162  ..t....&bambulab
-000064b0: 735f 6170 692e 4669 6c61 6d65 6e74 2e42  s_api.Filament.B
-000064c0: 414d 4255 5f50 4c41 5f42 6173 6963 946a  AMBU_PLA_Basic.j
-000064d0: 7105 0000 286a b302 0000 6ab1 0400 008c  q...(j....j.....
-000064e0: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
-000064f0: 8c26 6261 6d62 756c 6162 735f 6170 692e  .&bambulabs_api.
-00006500: 4669 6c61 6d65 6e74 2e42 414d 4255 5f50  Filament.BAMBU_P
-00006510: 4c41 5f4d 6174 7465 946a 7105 0000 286a  LA_Matte.jq...(j
-00006520: b302 0000 6ab4 0400 008c 0961 7474 7269  ....j......attri
-00006530: 6275 7465 9489 7494 8194 8c20 6261 6d62  bute..t.... bamb
-00006540: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
-00006550: 6e74 2e53 5550 504f 5254 5f47 946a 7105  nt.SUPPORT_G.jq.
-00006560: 0000 286a b302 0000 6ab7 0400 008c 0961  ..(j....j......a
-00006570: 7474 7269 6275 7465 9489 7494 8194 8c20  ttribute..t.... 
-00006580: 6261 6d62 756c 6162 735f 6170 692e 4669  bambulabs_api.Fi
-00006590: 6c61 6d65 6e74 2e53 5550 504f 5254 5f57  lament.SUPPORT_W
-000065a0: 946a 7105 0000 286a b302 0000 6aba 0400  .jq...(j....j...
-000065b0: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
-000065c0: 8194 8c24 6261 6d62 756c 6162 735f 6170  ...$bambulabs_ap
-000065d0: 692e 4669 6c61 6d65 6e74 2e42 414d 4255  i.Filament.BAMBU
-000065e0: 5f54 5055 5f39 3541 946a 7105 0000 286a  _TPU_95A.jq...(j
-000065f0: b302 0000 6abd 0400 008c 0961 7474 7269  ....j......attri
-00006600: 6275 7465 9489 7494 8194 8c1a 6261 6d62  bute..t.....bamb
-00006610: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
-00006620: 6e74 2e41 4253 946a 7105 0000 286a b302  nt.ABS.jq...(j..
-00006630: 0000 6ac0 0400 008c 0961 7474 7269 6275  ..j......attribu
-00006640: 7465 9489 7494 8194 8c1a 6261 6d62 756c  te..t.....bambul
-00006650: 6162 735f 6170 692e 4669 6c61 6d65 6e74  abs_api.Filament
-00006660: 2e41 5341 946a 7105 0000 286a b302 0000  .ASA.jq...(j....
-00006670: 6ac3 0400 008c 0961 7474 7269 6275 7465  j......attribute
-00006680: 9489 7494 8194 8c19 6261 6d62 756c 6162  ..t.....bambulab
-00006690: 735f 6170 692e 4669 6c61 6d65 6e74 2e50  s_api.Filament.P
-000066a0: 4194 6a71 0500 0028 6ab3 0200 006a c604  A.jq...(j....j..
-000066b0: 0000 8c09 6174 7472 6962 7574 6594 8974  ....attribute..t
-000066c0: 9481 948c 1c62 616d 6275 6c61 6273 5f61  .....bambulabs_a
-000066d0: 7069 2e46 696c 616d 656e 742e 5041 5f43  pi.Filament.PA_C
-000066e0: 4694 6a71 0500 0028 6ab3 0200 006a c904  F.jq...(j....j..
-000066f0: 0000 8c09 6174 7472 6962 7574 6594 8974  ....attribute..t
-00006700: 9481 948c 1962 616d 6275 6c61 6273 5f61  .....bambulabs_a
-00006710: 7069 2e46 696c 616d 656e 742e 5043 946a  pi.Filament.PC.j
-00006720: 7105 0000 286a b302 0000 6acc 0400 008c  q...(j....j.....
-00006730: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
-00006740: 8c1b 6261 6d62 756c 6162 735f 6170 692e  ..bambulabs_api.
-00006750: 4669 6c61 6d65 6e74 2e50 4554 4794 6a71  Filament.PETG.jq
-00006760: 0500 0028 6ab3 0200 006a cf04 0000 8c09  ...(j....j......
-00006770: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
-00006780: 1a62 616d 6275 6c61 6273 5f61 7069 2e46  .bambulabs_api.F
-00006790: 696c 616d 656e 742e 504c 4194 6a71 0500  ilament.PLA.jq..
-000067a0: 0028 6ab3 0200 006a d204 0000 8c09 6174  .(j....j......at
-000067b0: 7472 6962 7574 6594 8974 9481 948c 1d62  tribute..t.....b
-000067c0: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
-000067d0: 616d 656e 742e 504c 415f 4346 946a 7105  ament.PLA_CF.jq.
-000067e0: 0000 286a b302 0000 6ad5 0400 008c 0961  ..(j....j......a
-000067f0: 7474 7269 6275 7465 9489 7494 8194 8c1a  ttribute..t.....
-00006800: 6261 6d62 756c 6162 735f 6170 692e 4669  bambulabs_api.Fi
-00006810: 6c61 6d65 6e74 2e50 5641 946a 7105 0000  lament.PVA.jq...
-00006820: 286a b302 0000 6ad8 0400 008c 0961 7474  (j....j......att
-00006830: 7269 6275 7465 9489 7494 8194 8c1a 6261  ribute..t.....ba
-00006840: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
-00006850: 6d65 6e74 2e54 5055 946a 7105 0000 286a  ment.TPU.jq...(j
-00006860: b302 0000 6adb 0400 008c 0961 7474 7269  ....j......attri
-00006870: 6275 7465 9489 7494 8194 8c21 6261 6d62  bute..t....!bamb
-00006880: 756c 6162 735f 6170 692e 414d 5346 696c  ulabs_api.AMSFil
-00006890: 616d 656e 7453 6574 7469 6e67 7394 6a71  amentSettings.jq
-000068a0: 0500 0028 6ab3 0200 006a de04 0000 6a72  ...(j....j....jr
-000068b0: 0500 0089 7494 8194 8c2f 6261 6d62 756c  ....t..../bambul
-000068c0: 6162 735f 6170 692e 414d 5346 696c 616d  abs_api.AMSFilam
-000068d0: 656e 7453 6574 7469 6e67 732e 7472 6179  entSettings.tray
-000068e0: 5f69 6e66 6f5f 6964 7894 6a71 0500 0028  _info_idx.jq...(
-000068f0: 6ab3 0200 006a e104 0000 8c09 6174 7472  j....j......attr
-00006900: 6962 7574 6594 8974 9481 948c 3162 616d  ibute..t....1bam
-00006910: 6275 6c61 6273 5f61 7069 2e41 4d53 4669  bulabs_api.AMSFi
-00006920: 6c61 6d65 6e74 5365 7474 696e 6773 2e6e  lamentSettings.n
-00006930: 6f7a 7a6c 655f 7465 6d70 5f6d 696e 946a  ozzle_temp_min.j
-00006940: 7105 0000 286a b302 0000 6ae4 0400 008c  q...(j....j.....
-00006950: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
-00006960: 8c31 6261 6d62 756c 6162 735f 6170 692e  .1bambulabs_api.
-00006970: 414d 5346 696c 616d 656e 7453 6574 7469  AMSFilamentSetti
-00006980: 6e67 732e 6e6f 7a7a 6c65 5f74 656d 705f  ngs.nozzle_temp_
-00006990: 6d61 7894 6a71 0500 0028 6ab3 0200 006a  max.jq...(j....j
-000069a0: e704 0000 8c09 6174 7472 6962 7574 6594  ......attribute.
-000069b0: 8974 9481 948c 2b62 616d 6275 6c61 6273  .t....+bambulabs
-000069c0: 5f61 7069 2e41 4d53 4669 6c61 6d65 6e74  _api.AMSFilament
-000069d0: 5365 7474 696e 6773 2e74 7261 795f 7479  Settings.tray_ty
-000069e0: 7065 946a 7105 0000 286a b302 0000 6aea  pe.jq...(j....j.
-000069f0: 0400 008c 0961 7474 7269 6275 7465 9489  .....attribute..
-00006a00: 7494 8194 8c19 6261 6d62 756c 6162 735f  t.....bambulabs_
-00006a10: 6170 692e 5072 696e 7453 7461 7475 7394  api.PrintStatus.
-00006a20: 6a71 0500 0028 6ab3 0200 006a ed04 0000  jq...(j....j....
-00006a30: 6a72 0500 0089 7494 8194 8c22 6261 6d62  jr....t...."bamb
-00006a40: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00006a50: 7461 7475 732e 5052 494e 5449 4e47 946a  tatus.PRINTING.j
-00006a60: 7105 0000 286a b302 0000 6af0 0400 008c  q...(j....j.....
-00006a70: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
-00006a80: 8c2b 6261 6d62 756c 6162 735f 6170 692e  .+bambulabs_api.
-00006a90: 5072 696e 7453 7461 7475 732e 4155 544f  PrintStatus.AUTO
-00006aa0: 5f42 4544 5f4c 4556 454c 494e 4794 6a71  _BED_LEVELING.jq
-00006ab0: 0500 0028 6ab3 0200 006a f304 0000 8c09  ...(j....j......
-00006ac0: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
-00006ad0: 2c62 616d 6275 6c61 6273 5f61 7069 2e50  ,bambulabs_api.P
-00006ae0: 7269 6e74 5374 6174 7573 2e48 4541 5442  rintStatus.HEATB
-00006af0: 4544 5f50 5245 4845 4154 494e 4794 6a71  ED_PREHEATING.jq
-00006b00: 0500 0028 6ab3 0200 006a f604 0000 8c09  ...(j....j......
-00006b10: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
-00006b20: 2f62 616d 6275 6c61 6273 5f61 7069 2e50  /bambulabs_api.P
-00006b30: 7269 6e74 5374 6174 7573 2e53 5745 4550  rintStatus.SWEEP
-00006b40: 494e 475f 5859 5f4d 4543 485f 4d4f 4445  ING_XY_MECH_MODE
-00006b50: 946a 7105 0000 286a b302 0000 6af9 0400  .jq...(j....j...
-00006b60: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
-00006b70: 8194 8c2b 6261 6d62 756c 6162 735f 6170  ...+bambulabs_ap
-00006b80: 692e 5072 696e 7453 7461 7475 732e 4348  i.PrintStatus.CH
-00006b90: 414e 4749 4e47 5f46 494c 414d 454e 5494  ANGING_FILAMENT.
-00006ba0: 6a71 0500 0028 6ab3 0200 006a fc04 0000  jq...(j....j....
-00006bb0: 8c09 6174 7472 6962 7574 6594 8974 9481  ..attribute..t..
-00006bc0: 948c 2462 616d 6275 6c61 6273 5f61 7069  ..$bambulabs_api
-00006bd0: 2e50 7269 6e74 5374 6174 7573 2e4d 3430  .PrintStatus.M40
-00006be0: 305f 5041 5553 4594 6a71 0500 0028 6ab3  0_PAUSE.jq...(j.
-00006bf0: 0200 006a ff04 0000 8c09 6174 7472 6962  ...j......attrib
-00006c00: 7574 6594 8974 9481 948c 3062 616d 6275  ute..t....0bambu
-00006c10: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00006c20: 6174 7573 2e50 4155 5345 445f 4649 4c41  atus.PAUSED_FILA
-00006c30: 4d45 4e54 5f52 554e 4f55 5494 6a71 0500  MENT_RUNOUT.jq..
-00006c40: 0028 6ab3 0200 006a 0205 0000 8c09 6174  .(j....j......at
-00006c50: 7472 6962 7574 6594 8974 9481 948c 2862  tribute..t....(b
-00006c60: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
-00006c70: 6e74 5374 6174 7573 2e48 4541 5449 4e47  ntStatus.HEATING
-00006c80: 5f48 4f54 454e 4494 6a71 0500 0028 6ab3  _HOTEND.jq...(j.
-00006c90: 0200 006a 0505 0000 8c09 6174 7472 6962  ...j......attrib
-00006ca0: 7574 6594 8974 9481 948c 2f62 616d 6275  ute..t..../bambu
-00006cb0: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00006cc0: 6174 7573 2e43 414c 4942 5241 5449 4e47  atus.CALIBRATING
-00006cd0: 5f45 5854 5255 5349 4f4e 946a 7105 0000  _EXTRUSION.jq...
-00006ce0: 286a b302 0000 6a08 0500 008c 0961 7474  (j....j......att
-00006cf0: 7269 6275 7465 9489 7494 8194 8c2e 6261  ribute..t.....ba
-00006d00: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00006d10: 7453 7461 7475 732e 5343 414e 4e49 4e47  tStatus.SCANNING
-00006d20: 5f42 4544 5f53 5552 4641 4345 946a 7105  _BED_SURFACE.jq.
-00006d30: 0000 286a b302 0000 6a0b 0500 008c 0961  ..(j....j......a
-00006d40: 7474 7269 6275 7465 9489 7494 8194 8c30  ttribute..t....0
-00006d50: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00006d60: 696e 7453 7461 7475 732e 494e 5350 4543  intStatus.INSPEC
-00006d70: 5449 4e47 5f46 4952 5354 5f4c 4159 4552  TING_FIRST_LAYER
-00006d80: 946a 7105 0000 286a b302 0000 6a0e 0500  .jq...(j....j...
-00006d90: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
-00006da0: 8194 8c36 6261 6d62 756c 6162 735f 6170  ...6bambulabs_ap
-00006db0: 692e 5072 696e 7453 7461 7475 732e 4944  i.PrintStatus.ID
-00006dc0: 454e 5449 4659 494e 475f 4255 494c 445f  ENTIFYING_BUILD_
-00006dd0: 504c 4154 455f 5459 5045 946a 7105 0000  PLATE_TYPE.jq...
-00006de0: 286a b302 0000 6a11 0500 008c 0961 7474  (j....j......att
-00006df0: 7269 6275 7465 9489 7494 8194 8c31 6261  ribute..t....1ba
-00006e00: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00006e10: 7453 7461 7475 732e 4341 4c49 4252 4154  tStatus.CALIBRAT
-00006e20: 494e 475f 4d49 4352 4f5f 4c49 4441 5294  ING_MICRO_LIDAR.
-00006e30: 6a71 0500 0028 6ab3 0200 006a 1405 0000  jq...(j....j....
-00006e40: 8c09 6174 7472 6962 7574 6594 8974 9481  ..attribute..t..
-00006e50: 948c 2962 616d 6275 6c61 6273 5f61 7069  ..)bambulabs_api
-00006e60: 2e50 7269 6e74 5374 6174 7573 2e48 4f4d  .PrintStatus.HOM
-00006e70: 494e 475f 544f 4f4c 4845 4144 946a 7105  ING_TOOLHEAD.jq.
-00006e80: 0000 286a b302 0000 6a17 0500 008c 0961  ..(j....j......a
-00006e90: 7474 7269 6275 7465 9489 7494 8194 8c2d  ttribute..t....-
-00006ea0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-00006eb0: 696e 7453 7461 7475 732e 434c 4541 4e49  intStatus.CLEANI
-00006ec0: 4e47 5f4e 4f5a 5a4c 455f 5449 5094 6a71  NG_NOZZLE_TIP.jq
-00006ed0: 0500 0028 6ab3 0200 006a 1a05 0000 8c09  ...(j....j......
-00006ee0: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
-00006ef0: 3762 616d 6275 6c61 6273 5f61 7069 2e50  7bambulabs_api.P
-00006f00: 7269 6e74 5374 6174 7573 2e43 4845 434b  rintStatus.CHECK
-00006f10: 494e 475f 4558 5452 5544 4552 5f54 454d  ING_EXTRUDER_TEM
-00006f20: 5045 5241 5455 5245 946a 7105 0000 286a  PERATURE.jq...(j
-00006f30: b302 0000 6a1d 0500 008c 0961 7474 7269  ....j......attri
-00006f40: 6275 7465 9489 7494 8194 8c25 6261 6d62  bute..t....%bamb
-00006f50: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00006f60: 7461 7475 732e 5041 5553 4544 5f55 5345  tatus.PAUSED_USE
-00006f70: 5294 6a71 0500 0028 6ab3 0200 006a 2005  R.jq...(j....j .
-00006f80: 0000 8c09 6174 7472 6962 7574 6594 8974  ....attribute..t
-00006f90: 9481 948c 3462 616d 6275 6c61 6273 5f61  ....4bambulabs_a
-00006fa0: 7069 2e50 7269 6e74 5374 6174 7573 2e50  pi.PrintStatus.P
-00006fb0: 4155 5345 445f 4652 4f4e 545f 434f 5645  AUSED_FRONT_COVE
-00006fc0: 525f 4641 4c4c 494e 4794 6a71 0500 0028  R_FALLING.jq...(
-00006fd0: 6ab3 0200 006a 2305 0000 8c09 6174 7472  j....j#.....attr
-00006fe0: 6962 7574 6594 8974 9481 948c 2b62 616d  ibute..t....+bam
-00006ff0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00007000: 5374 6174 7573 2e43 414c 4942 5241 5449  Status.CALIBRATI
-00007010: 4e47 5f4c 4944 4152 946a 7105 0000 286a  NG_LIDAR.jq...(j
-00007020: b302 0000 6a26 0500 008c 0961 7474 7269  ....j&.....attri
-00007030: 6275 7465 9489 7494 8194 8c34 6261 6d62  bute..t....4bamb
-00007040: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00007050: 7461 7475 732e 4341 4c49 4252 4154 494e  tatus.CALIBRATIN
-00007060: 475f 4558 5452 5553 494f 4e5f 464c 4f57  G_EXTRUSION_FLOW
-00007070: 946a 7105 0000 286a b302 0000 6a29 0500  .jq...(j....j)..
-00007080: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
-00007090: 8194 8c3f 6261 6d62 756c 6162 735f 6170  ...?bambulabs_ap
-000070a0: 692e 5072 696e 7453 7461 7475 732e 5041  i.PrintStatus.PA
-000070b0: 5553 4544 5f4e 4f5a 5a4c 455f 5445 4d50  USED_NOZZLE_TEMP
-000070c0: 4552 4154 5552 455f 4d41 4c46 554e 4354  ERATURE_MALFUNCT
-000070d0: 494f 4e94 6a71 0500 0028 6ab3 0200 006a  ION.jq...(j....j
-000070e0: 2c05 0000 8c09 6174 7472 6962 7574 6594  ,.....attribute.
-000070f0: 8974 9481 948c 4162 616d 6275 6c61 6273  .t....Abambulabs
-00007100: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
-00007110: 2e50 4155 5345 445f 4845 4154 5f42 4544  .PAUSED_HEAT_BED
-00007120: 5f54 454d 5045 5241 5455 5245 5f4d 414c  _TEMPERATURE_MAL
-00007130: 4655 4e43 5449 4f4e 946a 7105 0000 286a  FUNCTION.jq...(j
-00007140: b302 0000 6a2f 0500 008c 0961 7474 7269  ....j/.....attri
-00007150: 6275 7465 9489 7494 8194 8c2c 6261 6d62  bute..t....,bamb
-00007160: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00007170: 7461 7475 732e 4649 4c41 4d45 4e54 5f55  tatus.FILAMENT_U
-00007180: 4e4c 4f41 4449 4e47 946a 7105 0000 286a  NLOADING.jq...(j
-00007190: b302 0000 6a32 0500 008c 0961 7474 7269  ....j2.....attri
-000071a0: 6275 7465 9489 7494 8194 8c2d 6261 6d62  bute..t....-bamb
-000071b0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-000071c0: 7461 7475 732e 5041 5553 4544 5f53 4b49  tatus.PAUSED_SKI
-000071d0: 5050 4544 5f53 5445 5094 6a71 0500 0028  PPED_STEP.jq...(
-000071e0: 6ab3 0200 006a 3505 0000 8c09 6174 7472  j....j5.....attr
-000071f0: 6962 7574 6594 8974 9481 948c 2a62 616d  ibute..t....*bam
-00007200: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00007210: 5374 6174 7573 2e46 494c 414d 454e 545f  Status.FILAMENT_
-00007220: 4c4f 4144 494e 4794 6a71 0500 0028 6ab3  LOADING.jq...(j.
-00007230: 0200 006a 3805 0000 8c09 6174 7472 6962  ...j8.....attrib
-00007240: 7574 6594 8974 9481 948c 3162 616d 6275  ute..t....1bambu
-00007250: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
-00007260: 6174 7573 2e43 414c 4942 5241 5449 4e47  atus.CALIBRATING
-00007270: 5f4d 4f54 4f52 5f4e 4f49 5345 946a 7105  _MOTOR_NOISE.jq.
-00007280: 0000 286a b302 0000 6a3b 0500 008c 0961  ..(j....j;.....a
-00007290: 7474 7269 6275 7465 9489 7494 8194 8c29  ttribute..t....)
-000072a0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-000072b0: 696e 7453 7461 7475 732e 5041 5553 4544  intStatus.PAUSED
-000072c0: 5f41 4d53 5f4c 4f53 5494 6a71 0500 0028  _AMS_LOST.jq...(
+00004c70: 6e74 5374 6174 7573 2994 8c30 6261 6d62  ntStatus)..0bamb
+00004c80: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+00004c90: 7461 7475 732e 5041 5553 4544 5f46 494c  tatus.PAUSED_FIL
+00004ca0: 414d 454e 545f 5255 4e4f 5554 9468 424e  AMENT_RUNOUT.hBN
+00004cb0: 7494 286a 6a04 0000 8c34 4845 4154 494e  t.(jj....4HEATIN
+00004cc0: 475f 484f 5445 4e44 2028 696e 206d 6f64  G_HOTEND (in mod
+00004cd0: 756c 6520 6261 6d62 756c 6162 735f 6170  ule bambulabs_ap
+00004ce0: 692e 5072 696e 7453 7461 7475 7329 948c  i.PrintStatus)..
+00004cf0: 2862 616d 6275 6c61 6273 5f61 7069 2e50  (bambulabs_api.P
+00004d00: 7269 6e74 5374 6174 7573 2e48 4541 5449  rintStatus.HEATI
+00004d10: 4e47 5f48 4f54 454e 4494 6842 4e74 9428  NG_HOTEND.hBNt.(
+00004d20: 6a6a 0400 008c 3b43 414c 4942 5241 5449  jj....;CALIBRATI
+00004d30: 4e47 5f45 5854 5255 5349 4f4e 2028 696e  NG_EXTRUSION (in
+00004d40: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+00004d50: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00004d60: 7329 948c 2f62 616d 6275 6c61 6273 5f61  s)../bambulabs_a
+00004d70: 7069 2e50 7269 6e74 5374 6174 7573 2e43  pi.PrintStatus.C
+00004d80: 414c 4942 5241 5449 4e47 5f45 5854 5255  ALIBRATING_EXTRU
+00004d90: 5349 4f4e 9468 424e 7494 286a 6a04 0000  SION.hBNt.(jj...
+00004da0: 8c3a 5343 414e 4e49 4e47 5f42 4544 5f53  .:SCANNING_BED_S
+00004db0: 5552 4641 4345 2028 696e 206d 6f64 756c  URFACE (in modul
+00004dc0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00004dd0: 5072 696e 7453 7461 7475 7329 948c 2e62  PrintStatus)...b
+00004de0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00004df0: 6e74 5374 6174 7573 2e53 4341 4e4e 494e  ntStatus.SCANNIN
+00004e00: 475f 4245 445f 5355 5246 4143 4594 6842  G_BED_SURFACE.hB
+00004e10: 4e74 9428 6a6a 0400 008c 3c49 4e53 5045  Nt.(jj....<INSPE
+00004e20: 4354 494e 475f 4649 5253 545f 4c41 5945  CTING_FIRST_LAYE
+00004e30: 5220 2869 6e20 6d6f 6475 6c65 2062 616d  R (in module bam
+00004e40: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00004e50: 5374 6174 7573 2994 8c30 6261 6d62 756c  Status)..0bambul
+00004e60: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00004e70: 7475 732e 494e 5350 4543 5449 4e47 5f46  tus.INSPECTING_F
+00004e80: 4952 5354 5f4c 4159 4552 9468 424e 7494  IRST_LAYER.hBNt.
+00004e90: 286a 6a04 0000 8c42 4944 454e 5449 4659  (jj....BIDENTIFY
+00004ea0: 494e 475f 4255 494c 445f 504c 4154 455f  ING_BUILD_PLATE_
+00004eb0: 5459 5045 2028 696e 206d 6f64 756c 6520  TYPE (in module 
+00004ec0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+00004ed0: 696e 7453 7461 7475 7329 948c 3662 616d  intStatus)..6bam
+00004ee0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00004ef0: 5374 6174 7573 2e49 4445 4e54 4946 5949  Status.IDENTIFYI
+00004f00: 4e47 5f42 5549 4c44 5f50 4c41 5445 5f54  NG_BUILD_PLATE_T
+00004f10: 5950 4594 6842 4e74 9428 6a6a 0400 008c  YPE.hBNt.(jj....
+00004f20: 3d43 414c 4942 5241 5449 4e47 5f4d 4943  =CALIBRATING_MIC
+00004f30: 524f 5f4c 4944 4152 2028 696e 206d 6f64  RO_LIDAR (in mod
+00004f40: 756c 6520 6261 6d62 756c 6162 735f 6170  ule bambulabs_ap
+00004f50: 692e 5072 696e 7453 7461 7475 7329 948c  i.PrintStatus)..
+00004f60: 3162 616d 6275 6c61 6273 5f61 7069 2e50  1bambulabs_api.P
+00004f70: 7269 6e74 5374 6174 7573 2e43 414c 4942  rintStatus.CALIB
+00004f80: 5241 5449 4e47 5f4d 4943 524f 5f4c 4944  RATING_MICRO_LID
+00004f90: 4152 9468 424e 7494 286a 6a04 0000 8c35  AR.hBNt.(jj....5
+00004fa0: 484f 4d49 4e47 5f54 4f4f 4c48 4541 4420  HOMING_TOOLHEAD 
+00004fb0: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+00004fc0: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+00004fd0: 6174 7573 2994 8c29 6261 6d62 756c 6162  atus)..)bambulab
+00004fe0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00004ff0: 732e 484f 4d49 4e47 5f54 4f4f 4c48 4541  s.HOMING_TOOLHEA
+00005000: 4494 6842 4e74 9428 6a6a 0400 008c 3943  D.hBNt.(jj....9C
+00005010: 4c45 414e 494e 475f 4e4f 5a5a 4c45 5f54  LEANING_NOZZLE_T
+00005020: 4950 2028 696e 206d 6f64 756c 6520 6261  IP (in module ba
+00005030: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00005040: 7453 7461 7475 7329 948c 2d62 616d 6275  tStatus)..-bambu
+00005050: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+00005060: 6174 7573 2e43 4c45 414e 494e 475f 4e4f  atus.CLEANING_NO
+00005070: 5a5a 4c45 5f54 4950 9468 424e 7494 286a  ZZLE_TIP.hBNt.(j
+00005080: 6a04 0000 8c43 4348 4543 4b49 4e47 5f45  j....CCHECKING_E
+00005090: 5854 5255 4445 525f 5445 4d50 4552 4154  XTRUDER_TEMPERAT
+000050a0: 5552 4520 2869 6e20 6d6f 6475 6c65 2062  URE (in module b
+000050b0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+000050c0: 6e74 5374 6174 7573 2994 8c37 6261 6d62  ntStatus)..7bamb
+000050d0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+000050e0: 7461 7475 732e 4348 4543 4b49 4e47 5f45  tatus.CHECKING_E
+000050f0: 5854 5255 4445 525f 5445 4d50 4552 4154  XTRUDER_TEMPERAT
+00005100: 5552 4594 6842 4e74 9428 6a6a 0400 008c  URE.hBNt.(jj....
+00005110: 3150 4155 5345 445f 5553 4552 2028 696e  1PAUSED_USER (in
+00005120: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+00005130: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00005140: 7329 948c 2562 616d 6275 6c61 6273 5f61  s)..%bambulabs_a
+00005150: 7069 2e50 7269 6e74 5374 6174 7573 2e50  pi.PrintStatus.P
+00005160: 4155 5345 445f 5553 4552 9468 424e 7494  AUSED_USER.hBNt.
+00005170: 286a 6a04 0000 8c40 5041 5553 4544 5f46  (jj....@PAUSED_F
+00005180: 524f 4e54 5f43 4f56 4552 5f46 414c 4c49  RONT_COVER_FALLI
+00005190: 4e47 2028 696e 206d 6f64 756c 6520 6261  NG (in module ba
+000051a0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+000051b0: 7453 7461 7475 7329 948c 3462 616d 6275  tStatus)..4bambu
+000051c0: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+000051d0: 6174 7573 2e50 4155 5345 445f 4652 4f4e  atus.PAUSED_FRON
+000051e0: 545f 434f 5645 525f 4641 4c4c 494e 4794  T_COVER_FALLING.
+000051f0: 6842 4e74 9428 6a6a 0400 008c 3743 414c  hBNt.(jj....7CAL
+00005200: 4942 5241 5449 4e47 5f4c 4944 4152 2028  IBRATING_LIDAR (
+00005210: 696e 206d 6f64 756c 6520 6261 6d62 756c  in module bambul
+00005220: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00005230: 7475 7329 948c 2b62 616d 6275 6c61 6273  tus)..+bambulabs
+00005240: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
+00005250: 2e43 414c 4942 5241 5449 4e47 5f4c 4944  .CALIBRATING_LID
+00005260: 4152 9468 424e 7494 286a 6a04 0000 8c40  AR.hBNt.(jj....@
+00005270: 4341 4c49 4252 4154 494e 475f 4558 5452  CALIBRATING_EXTR
+00005280: 5553 494f 4e5f 464c 4f57 2028 696e 206d  USION_FLOW (in m
+00005290: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
+000052a0: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
+000052b0: 948c 3462 616d 6275 6c61 6273 5f61 7069  ..4bambulabs_api
+000052c0: 2e50 7269 6e74 5374 6174 7573 2e43 414c  .PrintStatus.CAL
+000052d0: 4942 5241 5449 4e47 5f45 5854 5255 5349  IBRATING_EXTRUSI
+000052e0: 4f4e 5f46 4c4f 5794 6842 4e74 9428 6a6a  ON_FLOW.hBNt.(jj
+000052f0: 0400 008c 4b50 4155 5345 445f 4e4f 5a5a  ....KPAUSED_NOZZ
+00005300: 4c45 5f54 454d 5045 5241 5455 5245 5f4d  LE_TEMPERATURE_M
+00005310: 414c 4655 4e43 5449 4f4e 2028 696e 206d  ALFUNCTION (in m
+00005320: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
+00005330: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
+00005340: 948c 3f62 616d 6275 6c61 6273 5f61 7069  ..?bambulabs_api
+00005350: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
+00005360: 5345 445f 4e4f 5a5a 4c45 5f54 454d 5045  SED_NOZZLE_TEMPE
+00005370: 5241 5455 5245 5f4d 414c 4655 4e43 5449  RATURE_MALFUNCTI
+00005380: 4f4e 9468 424e 7494 286a 6a04 0000 8c4d  ON.hBNt.(jj....M
+00005390: 5041 5553 4544 5f48 4541 545f 4245 445f  PAUSED_HEAT_BED_
+000053a0: 5445 4d50 4552 4154 5552 455f 4d41 4c46  TEMPERATURE_MALF
+000053b0: 554e 4354 494f 4e20 2869 6e20 6d6f 6475  UNCTION (in modu
+000053c0: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+000053d0: 2e50 7269 6e74 5374 6174 7573 2994 8c41  .PrintStatus)..A
+000053e0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+000053f0: 696e 7453 7461 7475 732e 5041 5553 4544  intStatus.PAUSED
+00005400: 5f48 4541 545f 4245 445f 5445 4d50 4552  _HEAT_BED_TEMPER
+00005410: 4154 5552 455f 4d41 4c46 554e 4354 494f  ATURE_MALFUNCTIO
+00005420: 4e94 6842 4e74 9428 6a6a 0400 008c 3846  N.hBNt.(jj....8F
+00005430: 494c 414d 454e 545f 554e 4c4f 4144 494e  ILAMENT_UNLOADIN
+00005440: 4720 2869 6e20 6d6f 6475 6c65 2062 616d  G (in module bam
+00005450: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00005460: 5374 6174 7573 2994 8c2c 6261 6d62 756c  Status)..,bambul
+00005470: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00005480: 7475 732e 4649 4c41 4d45 4e54 5f55 4e4c  tus.FILAMENT_UNL
+00005490: 4f41 4449 4e47 9468 424e 7494 286a 6a04  OADING.hBNt.(jj.
+000054a0: 0000 8c39 5041 5553 4544 5f53 4b49 5050  ...9PAUSED_SKIPP
+000054b0: 4544 5f53 5445 5020 2869 6e20 6d6f 6475  ED_STEP (in modu
+000054c0: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+000054d0: 2e50 7269 6e74 5374 6174 7573 2994 8c2d  .PrintStatus)..-
+000054e0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+000054f0: 696e 7453 7461 7475 732e 5041 5553 4544  intStatus.PAUSED
+00005500: 5f53 4b49 5050 4544 5f53 5445 5094 6842  _SKIPPED_STEP.hB
+00005510: 4e74 9428 6a6a 0400 008c 3646 494c 414d  Nt.(jj....6FILAM
+00005520: 454e 545f 4c4f 4144 494e 4720 2869 6e20  ENT_LOADING (in 
+00005530: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
+00005540: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
+00005550: 2994 8c2a 6261 6d62 756c 6162 735f 6170  )..*bambulabs_ap
+00005560: 692e 5072 696e 7453 7461 7475 732e 4649  i.PrintStatus.FI
+00005570: 4c41 4d45 4e54 5f4c 4f41 4449 4e47 9468  LAMENT_LOADING.h
+00005580: 424e 7494 286a 6a04 0000 8c3d 4341 4c49  BNt.(jj....=CALI
+00005590: 4252 4154 494e 475f 4d4f 544f 525f 4e4f  BRATING_MOTOR_NO
+000055a0: 4953 4520 2869 6e20 6d6f 6475 6c65 2062  ISE (in module b
+000055b0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+000055c0: 6e74 5374 6174 7573 2994 8c31 6261 6d62  ntStatus)..1bamb
+000055d0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+000055e0: 7461 7475 732e 4341 4c49 4252 4154 494e  tatus.CALIBRATIN
+000055f0: 475f 4d4f 544f 525f 4e4f 4953 4594 6842  G_MOTOR_NOISE.hB
+00005600: 4e74 9428 6a6a 0400 008c 3550 4155 5345  Nt.(jj....5PAUSE
+00005610: 445f 414d 535f 4c4f 5354 2028 696e 206d  D_AMS_LOST (in m
+00005620: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
+00005630: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
+00005640: 948c 2962 616d 6275 6c61 6273 5f61 7069  ..)bambulabs_api
+00005650: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
+00005660: 5345 445f 414d 535f 4c4f 5354 9468 424e  SED_AMS_LOST.hBN
+00005670: 7494 286a 6a04 0000 8c45 5041 5553 4544  t.(jj....EPAUSED
+00005680: 5f4c 4f57 5f46 414e 5f53 5045 4544 5f48  _LOW_FAN_SPEED_H
+00005690: 4541 545f 4252 4541 4b20 2869 6e20 6d6f  EAT_BREAK (in mo
+000056a0: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+000056b0: 7069 2e50 7269 6e74 5374 6174 7573 2994  pi.PrintStatus).
+000056c0: 8c39 6261 6d62 756c 6162 735f 6170 692e  .9bambulabs_api.
+000056d0: 5072 696e 7453 7461 7475 732e 5041 5553  PrintStatus.PAUS
+000056e0: 4544 5f4c 4f57 5f46 414e 5f53 5045 4544  ED_LOW_FAN_SPEED
+000056f0: 5f48 4541 545f 4252 4541 4b94 6842 4e74  _HEAT_BREAK.hBNt
+00005700: 9428 6a6a 0400 008c 4e50 4155 5345 445f  .(jj....NPAUSED_
+00005710: 4348 414d 4245 525f 5445 4d50 4552 4154  CHAMBER_TEMPERAT
+00005720: 5552 455f 434f 4e54 524f 4c5f 4552 524f  URE_CONTROL_ERRO
+00005730: 5220 2869 6e20 6d6f 6475 6c65 2062 616d  R (in module bam
+00005740: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00005750: 5374 6174 7573 2994 8c42 6261 6d62 756c  Status)..Bbambul
+00005760: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00005770: 7475 732e 5041 5553 4544 5f43 4841 4d42  tus.PAUSED_CHAMB
+00005780: 4552 5f54 454d 5045 5241 5455 5245 5f43  ER_TEMPERATURE_C
+00005790: 4f4e 5452 4f4c 5f45 5252 4f52 9468 424e  ONTROL_ERROR.hBN
+000057a0: 7494 286a 6a04 0000 8c35 434f 4f4c 494e  t.(jj....5COOLIN
+000057b0: 475f 4348 414d 4245 5220 2869 6e20 6d6f  G_CHAMBER (in mo
+000057c0: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+000057d0: 7069 2e50 7269 6e74 5374 6174 7573 2994  pi.PrintStatus).
+000057e0: 8c29 6261 6d62 756c 6162 735f 6170 692e  .)bambulabs_api.
+000057f0: 5072 696e 7453 7461 7475 732e 434f 4f4c  PrintStatus.COOL
+00005800: 494e 475f 4348 414d 4245 5294 6842 4e74  ING_CHAMBER.hBNt
+00005810: 9428 6a6a 0400 008c 3750 4155 5345 445f  .(jj....7PAUSED_
+00005820: 5553 4552 5f47 434f 4445 2028 696e 206d  USER_GCODE (in m
+00005830: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
+00005840: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
+00005850: 948c 2b62 616d 6275 6c61 6273 5f61 7069  ..+bambulabs_api
+00005860: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
+00005870: 5345 445f 5553 4552 5f47 434f 4445 9468  SED_USER_GCODE.h
+00005880: 424e 7494 286a 6a04 0000 8c39 4d4f 544f  BNt.(jj....9MOTO
+00005890: 525f 4e4f 4953 455f 5348 4f57 4f46 4620  R_NOISE_SHOWOFF 
+000058a0: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+000058b0: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+000058c0: 6174 7573 2994 8c2d 6261 6d62 756c 6162  atus)..-bambulab
+000058d0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+000058e0: 732e 4d4f 544f 525f 4e4f 4953 455f 5348  s.MOTOR_NOISE_SH
+000058f0: 4f57 4f46 4694 6842 4e74 9428 6a6a 0400  OWOFF.hBNt.(jj..
+00005900: 008c 4d50 4155 5345 445f 4e4f 5a5a 4c45  ..MPAUSED_NOZZLE
+00005910: 5f46 494c 414d 454e 545f 434f 5645 5245  _FILAMENT_COVERE
+00005920: 445f 4445 5445 4354 4544 2028 696e 206d  D_DETECTED (in m
+00005930: 6f64 756c 6520 6261 6d62 756c 6162 735f  odule bambulabs_
+00005940: 6170 692e 5072 696e 7453 7461 7475 7329  api.PrintStatus)
+00005950: 948c 4162 616d 6275 6c61 6273 5f61 7069  ..Abambulabs_api
+00005960: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
+00005970: 5345 445f 4e4f 5a5a 4c45 5f46 494c 414d  SED_NOZZLE_FILAM
+00005980: 454e 545f 434f 5645 5245 445f 4445 5445  ENT_COVERED_DETE
+00005990: 4354 4544 9468 424e 7494 286a 6a04 0000  CTED.hBNt.(jj...
+000059a0: 8c39 5041 5553 4544 5f43 5554 5445 525f  .9PAUSED_CUTTER_
+000059b0: 4552 524f 5220 2869 6e20 6d6f 6475 6c65  ERROR (in module
+000059c0: 2062 616d 6275 6c61 6273 5f61 7069 2e50   bambulabs_api.P
+000059d0: 7269 6e74 5374 6174 7573 2994 8c2d 6261  rintStatus)..-ba
+000059e0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+000059f0: 7453 7461 7475 732e 5041 5553 4544 5f43  tStatus.PAUSED_C
+00005a00: 5554 5445 525f 4552 524f 5294 6842 4e74  UTTER_ERROR.hBNt
+00005a10: 9428 6a6a 0400 008c 3e50 4155 5345 445f  .(jj....>PAUSED_
+00005a20: 4649 5253 545f 4c41 5945 525f 4552 524f  FIRST_LAYER_ERRO
+00005a30: 5220 2869 6e20 6d6f 6475 6c65 2062 616d  R (in module bam
+00005a40: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00005a50: 5374 6174 7573 2994 8c32 6261 6d62 756c  Status)..2bambul
+00005a60: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00005a70: 7475 732e 5041 5553 4544 5f46 4952 5354  tus.PAUSED_FIRST
+00005a80: 5f4c 4159 4552 5f45 5252 4f52 9468 424e  _LAYER_ERROR.hBN
+00005a90: 7494 286a 6a04 0000 8c38 5041 5553 4544  t.(jj....8PAUSED
+00005aa0: 5f4e 4f5a 5a4c 455f 434c 4f47 2028 696e  _NOZZLE_CLOG (in
+00005ab0: 206d 6f64 756c 6520 6261 6d62 756c 6162   module bambulab
+00005ac0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00005ad0: 7329 948c 2c62 616d 6275 6c61 6273 5f61  s)..,bambulabs_a
+00005ae0: 7069 2e50 7269 6e74 5374 6174 7573 2e50  pi.PrintStatus.P
+00005af0: 4155 5345 445f 4e4f 5a5a 4c45 5f43 4c4f  AUSED_NOZZLE_CLO
+00005b00: 4794 6842 4e74 9428 6a6a 0400 008c 2d55  G.hBNt.(jj....-U
+00005b10: 4e4b 4e4f 574e 2028 696e 206d 6f64 756c  NKNOWN (in modul
+00005b20: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00005b30: 5072 696e 7453 7461 7475 7329 948c 2162  PrintStatus)..!b
+00005b40: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00005b50: 6e74 5374 6174 7573 2e55 4e4b 4e4f 574e  ntStatus.UNKNOWN
+00005b60: 9468 424e 7494 286a 6a04 0000 8c2a 4944  .hBNt.(jj....*ID
+00005b70: 4c45 2028 696e 206d 6f64 756c 6520 6261  LE (in module ba
+00005b80: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00005b90: 7453 7461 7475 7329 948c 1e62 616d 6275  tStatus)...bambu
+00005ba0: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+00005bb0: 6174 7573 2e49 444c 4594 6842 4e74 9428  atus.IDLE.hBNt.(
+00005bc0: 6a66 0400 008c 206d 6f64 756c 653b 2062  jf.... module; b
+00005bd0: 616d 6275 6c61 6273 5f61 7069 2e47 636f  ambulabs_api.Gco
+00005be0: 6465 5374 6174 6594 8c1f 6d6f 6475 6c65  deState...module
+00005bf0: 2d62 616d 6275 6c61 6273 5f61 7069 2e47  -bambulabs_api.G
+00005c00: 636f 6465 5374 6174 6594 6842 4e74 9428  codeState.hBNt.(
+00005c10: 6a6a 0400 008c 2949 444c 4520 2869 6e20  jj....)IDLE (in 
+00005c20: 6d6f 6475 6c65 2062 616d 6275 6c61 6273  module bambulabs
+00005c30: 5f61 7069 2e47 636f 6465 5374 6174 6529  _api.GcodeState)
+00005c40: 948c 1d62 616d 6275 6c61 6273 5f61 7069  ...bambulabs_api
+00005c50: 2e47 636f 6465 5374 6174 652e 4944 4c45  .GcodeState.IDLE
+00005c60: 9468 424e 7494 286a 6a04 0000 8c2e 5052  .hBNt.(jj.....PR
+00005c70: 4550 4152 494e 4720 2869 6e20 6d6f 6475  EPARING (in modu
+00005c80: 6c65 2062 616d 6275 6c61 6273 5f61 7069  le bambulabs_api
+00005c90: 2e47 636f 6465 5374 6174 6529 948c 2262  .GcodeState).."b
+00005ca0: 616d 6275 6c61 6273 5f61 7069 2e47 636f  ambulabs_api.Gco
+00005cb0: 6465 5374 6174 652e 5052 4550 4152 494e  deState.PREPARIN
+00005cc0: 4794 6842 4e74 9428 6a6a 0400 008c 2c52  G.hBNt.(jj....,R
+00005cd0: 554e 4e49 4e47 2028 696e 206d 6f64 756c  UNNING (in modul
+00005ce0: 6520 6261 6d62 756c 6162 735f 6170 692e  e bambulabs_api.
+00005cf0: 4763 6f64 6553 7461 7465 2994 8c20 6261  GcodeState).. ba
+00005d00: 6d62 756c 6162 735f 6170 692e 4763 6f64  mbulabs_api.Gcod
+00005d10: 6553 7461 7465 2e52 554e 4e49 4e47 9468  eState.RUNNING.h
+00005d20: 424e 7494 286a 6a04 0000 8c2b 5041 5553  BNt.(jj....+PAUS
+00005d30: 4544 2028 696e 206d 6f64 756c 6520 6261  ED (in module ba
+00005d40: 6d62 756c 6162 735f 6170 692e 4763 6f64  mbulabs_api.Gcod
+00005d50: 6553 7461 7465 2994 8c1f 6261 6d62 756c  eState)...bambul
+00005d60: 6162 735f 6170 692e 4763 6f64 6553 7461  abs_api.GcodeSta
+00005d70: 7465 2e50 4155 5345 4494 6842 4e74 9428  te.PAUSED.hBNt.(
+00005d80: 6a6a 0400 008c 2d46 494e 4953 4845 4420  jj....-FINISHED 
+00005d90: 2869 6e20 6d6f 6475 6c65 2062 616d 6275  (in module bambu
+00005da0: 6c61 6273 5f61 7069 2e47 636f 6465 5374  labs_api.GcodeSt
+00005db0: 6174 6529 948c 2162 616d 6275 6c61 6273  ate)..!bambulabs
+00005dc0: 5f61 7069 2e47 636f 6465 5374 6174 652e  _api.GcodeState.
+00005dd0: 4649 4e49 5348 4544 9468 424e 7494 286a  FINISHED.hBNt.(j
+00005de0: 6a04 0000 8c2c 554e 4b4e 4f57 4e20 2869  j....,UNKNOWN (i
+00005df0: 6e20 6d6f 6475 6c65 2062 616d 6275 6c61  n module bambula
+00005e00: 6273 5f61 7069 2e47 636f 6465 5374 6174  bs_api.GcodeStat
+00005e10: 6529 948c 2062 616d 6275 6c61 6273 5f61  e).. bambulabs_a
+00005e20: 7069 2e47 636f 6465 5374 6174 652e 554e  pi.GcodeState.UN
+00005e30: 4b4e 4f57 4e94 6842 4e74 9465 7375 8c02  KNOWN.hBNt.esu..
+00005e40: 6a73 947d 9428 6a49 0400 007d 948c 076d  js.}.(jI...}...m
+00005e50: 6f64 756c 6573 947d 946a b402 0000 4b00  odules.}.j....K.
+00005e60: 758c 046d 6174 6894 7d94 286a 4904 0000  u..math.}.(jI...
+00005e70: 7d94 8c0d 6861 735f 6571 7561 7469 6f6e  }...has_equation
+00005e80: 7394 7d94 6ab3 0200 0089 736a b402 0000  s.}.j.....sj....
+00005e90: 4b00 758c 0270 7994 7d94 286a 4904 0000  K.u..py.}.(jI...
+00005ea0: 7d94 288c 1562 616d 6275 6c61 6273 5f61  }.(..bambulabs_a
+00005eb0: 7069 2e50 7269 6e74 6572 948c 1573 7068  pi.Printer...sph
+00005ec0: 696e 782e 646f 6d61 696e 732e 7079 7468  inx.domains.pyth
+00005ed0: 6f6e 948c 0b4f 626a 6563 7445 6e74 7279  on...ObjectEntry
+00005ee0: 9493 9428 6ab3 0200 006a 6804 0000 8c06  ...(j....jh.....
+00005ef0: 6d6f 6475 6c65 9489 7494 8194 8c27 6261  module..t....'ba
+00005f00: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00005f10: 7465 722e 6361 6c69 6272 6174 655f 7072  ter.calibrate_pr
+00005f20: 696e 7465 7294 6aaa 0500 0028 6ab3 0200  inter.j....(j...
+00005f30: 006a 6c04 0000 8c08 6675 6e63 7469 6f6e  .jl.....function
+00005f40: 9489 7494 8194 8c1d 6261 6d62 756c 6162  ..t.....bambulab
+00005f50: 735f 6170 692e 5072 696e 7465 722e 636f  s_api.Printer.co
+00005f60: 6e6e 6563 7494 6aaa 0500 0028 6ab3 0200  nnect.j....(j...
+00005f70: 006a 6f04 0000 8c08 6675 6e63 7469 6f6e  .jo.....function
+00005f80: 9489 7494 8194 8c21 6261 6d62 756c 6162  ..t....!bambulab
+00005f90: 735f 6170 692e 5072 696e 7465 722e 6465  s_api.Printer.de
+00005fa0: 6c65 7465 5f66 696c 6594 6aaa 0500 0028  lete_file.j....(
+00005fb0: 6ab3 0200 006a 7204 0000 8c08 6675 6e63  j....jr.....func
+00005fc0: 7469 6f6e 9489 7494 8194 8c20 6261 6d62  tion..t.... bamb
+00005fd0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+00005fe0: 722e 6469 7363 6f6e 6e65 6374 946a aa05  r.disconnect.j..
+00005ff0: 0000 286a b302 0000 6a75 0400 008c 0866  ..(j....ju.....f
+00006000: 756e 6374 696f 6e94 8974 9481 948c 2962  unction..t....)b
+00006010: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00006020: 6e74 6572 2e67 6574 5f62 6564 5f74 656d  nter.get_bed_tem
+00006030: 7065 7261 7475 7265 946a aa05 0000 286a  perature.j....(j
+00006040: b302 0000 6a78 0400 008c 0866 756e 6374  ....jx.....funct
+00006050: 696f 6e94 8974 9481 948c 2662 616d 6275  ion..t....&bambu
+00006060: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+00006070: 2e67 6574 5f63 616d 6572 615f 6672 616d  .get_camera_fram
+00006080: 6594 6aaa 0500 0028 6ab3 0200 006a 7b04  e.j....(j....j{.
+00006090: 0000 8c08 6675 6e63 7469 6f6e 9489 7494  ....function..t.
+000060a0: 8194 8c23 6261 6d62 756c 6162 735f 6170  ...#bambulabs_ap
+000060b0: 692e 5072 696e 7465 722e 6765 745f 6669  i.Printer.get_fi
+000060c0: 6c65 5f6e 616d 6594 6aaa 0500 0028 6ab3  le_name.j....(j.
+000060d0: 0200 006a 7e04 0000 8c08 6675 6e63 7469  ...j~.....functi
+000060e0: 6f6e 9489 7494 8194 8c25 6261 6d62 756c  on..t....%bambul
+000060f0: 6162 735f 6170 692e 5072 696e 7465 722e  abs_api.Printer.
+00006100: 6765 745f 6c69 6768 745f 7374 6174 6594  get_light_state.
+00006110: 6aaa 0500 0028 6ab3 0200 006a 8104 0000  j....(j....j....
+00006120: 8c08 6675 6e63 7469 6f6e 9489 7494 8194  ..function..t...
+00006130: 8c2c 6261 6d62 756c 6162 735f 6170 692e  .,bambulabs_api.
+00006140: 5072 696e 7465 722e 6765 745f 6e6f 7a7a  Printer.get_nozz
+00006150: 6c65 5f74 656d 7065 7261 7475 7265 946a  le_temperature.j
+00006160: aa05 0000 286a b302 0000 6a84 0400 008c  ....(j....j.....
+00006170: 0866 756e 6374 696f 6e94 8974 9481 948c  .function..t....
+00006180: 2462 616d 6275 6c61 6273 5f61 7069 2e50  $bambulabs_api.P
+00006190: 7269 6e74 6572 2e67 6574 5f70 6572 6365  rinter.get_perce
+000061a0: 6e74 6167 6594 6aaa 0500 0028 6ab3 0200  ntage.j....(j...
+000061b0: 006a 8704 0000 8c08 6675 6e63 7469 6f6e  .j......function
+000061c0: 9489 7494 8194 8c25 6261 6d62 756c 6162  ..t....%bambulab
+000061d0: 735f 6170 692e 5072 696e 7465 722e 6765  s_api.Printer.ge
+000061e0: 745f 7072 696e 745f 7370 6565 6494 6aaa  t_print_speed.j.
+000061f0: 0500 0028 6ab3 0200 006a 8a04 0000 8c08  ...(j....j......
+00006200: 6675 6e63 7469 6f6e 9489 7494 8194 8c1f  function..t.....
+00006210: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+00006220: 696e 7465 722e 6765 745f 7374 6174 6594  inter.get_state.
+00006230: 6aaa 0500 0028 6ab3 0200 006a 8d04 0000  j....(j....j....
+00006240: 8c08 6675 6e63 7469 6f6e 9489 7494 8194  ..function..t...
+00006250: 8c1e 6261 6d62 756c 6162 735f 6170 692e  ..bambulabs_api.
+00006260: 5072 696e 7465 722e 6765 745f 7469 6d65  Printer.get_time
+00006270: 946a aa05 0000 286a b302 0000 6a90 0400  .j....(j....j...
+00006280: 008c 0866 756e 6374 696f 6e94 8974 9481  ...function..t..
+00006290: 948c 2262 616d 6275 6c61 6273 5f61 7069  .."bambulabs_api
+000062a0: 2e50 7269 6e74 6572 2e68 6f6d 655f 7072  .Printer.home_pr
+000062b0: 696e 7465 7294 6aaa 0500 0028 6ab3 0200  inter.j....(j...
+000062c0: 006a 9304 0000 8c08 6675 6e63 7469 6f6e  .j......function
+000062d0: 9489 7494 8194 8c29 6261 6d62 756c 6162  ..t....)bambulab
+000062e0: 735f 6170 692e 5072 696e 7465 722e 6c6f  s_api.Printer.lo
+000062f0: 6164 5f66 696c 616d 656e 745f 7370 6f6f  ad_filament_spoo
+00006300: 6c94 6aaa 0500 0028 6ab3 0200 006a 9604  l.j....(j....j..
+00006310: 0000 8c08 6675 6e63 7469 6f6e 9489 7494  ....function..t.
+00006320: 8194 8c21 6261 6d62 756c 6162 735f 6170  ...!bambulabs_ap
+00006330: 692e 5072 696e 7465 722e 6d6f 7665 5f7a  i.Printer.move_z
+00006340: 5f61 7869 7394 6aaa 0500 0028 6ab3 0200  _axis.j....(j...
+00006350: 006a 9904 0000 8c08 6675 6e63 7469 6f6e  .j......function
+00006360: 9489 7494 8194 8c21 6261 6d62 756c 6162  ..t....!bambulab
+00006370: 735f 6170 692e 5072 696e 7465 722e 7061  s_api.Printer.pa
+00006380: 7573 655f 7072 696e 7494 6aaa 0500 0028  use_print.j....(
+00006390: 6ab3 0200 006a 9c04 0000 8c08 6675 6e63  j....j......func
+000063a0: 7469 6f6e 9489 7494 8194 8c22 6261 6d62  tion..t...."bamb
+000063b0: 756c 6162 735f 6170 692e 5072 696e 7465  ulabs_api.Printe
+000063c0: 722e 7265 7375 6d65 5f70 7269 6e74 946a  r.resume_print.j
+000063d0: aa05 0000 286a b302 0000 6a9f 0400 008c  ....(j....j.....
+000063e0: 0866 756e 6374 696f 6e94 8974 9481 948c  .function..t....
+000063f0: 2b62 616d 6275 6c61 6273 5f61 7069 2e50  +bambulabs_api.P
+00006400: 7269 6e74 6572 2e72 6574 7279 5f66 696c  rinter.retry_fil
+00006410: 616d 656e 745f 6163 7469 6f6e 946a aa05  ament_action.j..
+00006420: 0000 286a b302 0000 6aa2 0400 008c 0866  ..(j....j......f
+00006430: 756e 6374 696f 6e94 8974 9481 948c 2962  unction..t....)b
+00006440: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00006450: 6e74 6572 2e73 6574 5f62 6564 5f74 656d  nter.set_bed_tem
+00006460: 7065 7261 7475 7265 946a aa05 0000 286a  perature.j....(j
+00006470: b302 0000 6aa5 0400 008c 0866 756e 6374  ....j......funct
+00006480: 696f 6e94 8974 9481 948c 2a62 616d 6275  ion..t....*bambu
+00006490: 6c61 6273 5f61 7069 2e50 7269 6e74 6572  labs_api.Printer
+000064a0: 2e73 6574 5f66 696c 616d 656e 745f 7072  .set_filament_pr
+000064b0: 696e 7465 7294 6aaa 0500 0028 6ab3 0200  inter.j....(j...
+000064c0: 006a a804 0000 8c08 6675 6e63 7469 6f6e  .j......function
+000064d0: 9489 7494 8194 8c2c 6261 6d62 756c 6162  ..t....,bambulab
+000064e0: 735f 6170 692e 5072 696e 7465 722e 7365  s_api.Printer.se
+000064f0: 745f 6e6f 7a7a 6c65 5f74 656d 7065 7261  t_nozzle_tempera
+00006500: 7475 7265 946a aa05 0000 286a b302 0000  ture.j....(j....
+00006510: 6aab 0400 008c 0866 756e 6374 696f 6e94  j......function.
+00006520: 8974 9481 948c 2562 616d 6275 6c61 6273  .t....%bambulabs
+00006530: 5f61 7069 2e50 7269 6e74 6572 2e73 6574  _api.Printer.set
+00006540: 5f70 7269 6e74 5f73 7065 6564 946a aa05  _print_speed.j..
+00006550: 0000 286a b302 0000 6aae 0400 008c 0866  ..(j....j......f
+00006560: 756e 6374 696f 6e94 8974 9481 948c 2162  unction..t....!b
+00006570: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00006580: 6e74 6572 2e73 7461 7274 5f70 7269 6e74  nter.start_print
+00006590: 946a aa05 0000 286a b302 0000 6ab1 0400  .j....(j....j...
+000065a0: 008c 0866 756e 6374 696f 6e94 8974 9481  ...function..t..
+000065b0: 948c 2062 616d 6275 6c61 6273 5f61 7069  .. bambulabs_api
+000065c0: 2e50 7269 6e74 6572 2e73 746f 705f 7072  .Printer.stop_pr
+000065d0: 696e 7494 6aaa 0500 0028 6ab3 0200 006a  int.j....(j....j
+000065e0: b404 0000 8c08 6675 6e63 7469 6f6e 9489  ......function..
+000065f0: 7494 8194 8c24 6261 6d62 756c 6162 735f  t....$bambulabs_
+00006600: 6170 692e 5072 696e 7465 722e 7475 726e  api.Printer.turn
+00006610: 5f6c 6967 6874 5f6f 6666 946a aa05 0000  _light_off.j....
+00006620: 286a b302 0000 6ab7 0400 008c 0866 756e  (j....j......fun
+00006630: 6374 696f 6e94 8974 9481 948c 2362 616d  ction..t....#bam
+00006640: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00006650: 6572 2e74 7572 6e5f 6c69 6768 745f 6f6e  er.turn_light_on
+00006660: 946a aa05 0000 286a b302 0000 6aba 0400  .j....(j....j...
+00006670: 008c 0866 756e 6374 696f 6e94 8974 9481  ...function..t..
+00006680: 948c 2b62 616d 6275 6c61 6273 5f61 7069  ..+bambulabs_api
+00006690: 2e50 7269 6e74 6572 2e75 6e6c 6f61 645f  .Printer.unload_
+000066a0: 6669 6c61 6d65 6e74 5f73 706f 6f6c 946a  filament_spool.j
+000066b0: aa05 0000 286a b302 0000 6abd 0400 008c  ....(j....j.....
+000066c0: 0866 756e 6374 696f 6e94 8974 9481 948c  .function..t....
+000066d0: 2162 616d 6275 6c61 6273 5f61 7069 2e50  !bambulabs_api.P
+000066e0: 7269 6e74 6572 2e75 706c 6f61 645f 6669  rinter.upload_fi
+000066f0: 6c65 946a aa05 0000 286a b302 0000 6ac0  le.j....(j....j.
+00006700: 0400 008c 0866 756e 6374 696f 6e94 8974  .....function..t
+00006710: 9481 948c 1662 616d 6275 6c61 6273 5f61  .....bambulabs_a
+00006720: 7069 2e46 696c 616d 656e 7494 6aaa 0500  pi.Filament.j...
+00006730: 0028 6ab3 0200 006a c304 0000 6aab 0500  .(j....j....j...
+00006740: 0089 7494 8194 8c23 6261 6d62 756c 6162  ..t....#bambulab
+00006750: 735f 6170 692e 4669 6c61 6d65 6e74 2e50  s_api.Filament.P
+00006760: 4f4c 594c 4954 455f 504c 4194 6aaa 0500  OLYLITE_PLA.j...
+00006770: 0028 6ab3 0200 006a c604 0000 8c09 6174  .(j....j......at
+00006780: 7472 6962 7574 6594 8974 9481 948c 2462  tribute..t....$b
+00006790: 616d 6275 6c61 6273 5f61 7069 2e46 696c  ambulabs_api.Fil
+000067a0: 616d 656e 742e 504f 4c59 5445 5252 415f  ament.POLYTERRA_
+000067b0: 504c 4194 6aaa 0500 0028 6ab3 0200 006a  PLA.j....(j....j
+000067c0: c904 0000 8c09 6174 7472 6962 7574 6594  ......attribute.
+000067d0: 8974 9481 948c 2062 616d 6275 6c61 6273  .t.... bambulabs
+000067e0: 5f61 7069 2e46 696c 616d 656e 742e 4241  _api.Filament.BA
+000067f0: 4d42 555f 4142 5394 6aaa 0500 0028 6ab3  MBU_ABS.j....(j.
+00006800: 0200 006a cc04 0000 8c09 6174 7472 6962  ...j......attrib
+00006810: 7574 6594 8974 9481 948c 2262 616d 6275  ute..t...."bambu
+00006820: 6c61 6273 5f61 7069 2e46 696c 616d 656e  labs_api.Filamen
+00006830: 742e 4241 4d42 555f 5041 5f43 4694 6aaa  t.BAMBU_PA_CF.j.
+00006840: 0500 0028 6ab3 0200 006a cf04 0000 8c09  ...(j....j......
+00006850: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
+00006860: 1f62 616d 6275 6c61 6273 5f61 7069 2e46  .bambulabs_api.F
+00006870: 696c 616d 656e 742e 4241 4d42 555f 5043  ilament.BAMBU_PC
+00006880: 946a aa05 0000 286a b302 0000 6ad2 0400  .j....(j....j...
+00006890: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
+000068a0: 8194 8c26 6261 6d62 756c 6162 735f 6170  ...&bambulabs_ap
+000068b0: 692e 4669 6c61 6d65 6e74 2e42 414d 4255  i.Filament.BAMBU
+000068c0: 5f50 4c41 5f42 6173 6963 946a aa05 0000  _PLA_Basic.j....
+000068d0: 286a b302 0000 6ad5 0400 008c 0961 7474  (j....j......att
+000068e0: 7269 6275 7465 9489 7494 8194 8c26 6261  ribute..t....&ba
+000068f0: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
+00006900: 6d65 6e74 2e42 414d 4255 5f50 4c41 5f4d  ment.BAMBU_PLA_M
+00006910: 6174 7465 946a aa05 0000 286a b302 0000  atte.j....(j....
+00006920: 6ad8 0400 008c 0961 7474 7269 6275 7465  j......attribute
+00006930: 9489 7494 8194 8c20 6261 6d62 756c 6162  ..t.... bambulab
+00006940: 735f 6170 692e 4669 6c61 6d65 6e74 2e53  s_api.Filament.S
+00006950: 5550 504f 5254 5f47 946a aa05 0000 286a  UPPORT_G.j....(j
+00006960: b302 0000 6adb 0400 008c 0961 7474 7269  ....j......attri
+00006970: 6275 7465 9489 7494 8194 8c20 6261 6d62  bute..t.... bamb
+00006980: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
+00006990: 6e74 2e53 5550 504f 5254 5f57 946a aa05  nt.SUPPORT_W.j..
+000069a0: 0000 286a b302 0000 6ade 0400 008c 0961  ..(j....j......a
+000069b0: 7474 7269 6275 7465 9489 7494 8194 8c24  ttribute..t....$
+000069c0: 6261 6d62 756c 6162 735f 6170 692e 4669  bambulabs_api.Fi
+000069d0: 6c61 6d65 6e74 2e42 414d 4255 5f54 5055  lament.BAMBU_TPU
+000069e0: 5f39 3541 946a aa05 0000 286a b302 0000  _95A.j....(j....
+000069f0: 6ae1 0400 008c 0961 7474 7269 6275 7465  j......attribute
+00006a00: 9489 7494 8194 8c1a 6261 6d62 756c 6162  ..t.....bambulab
+00006a10: 735f 6170 692e 4669 6c61 6d65 6e74 2e41  s_api.Filament.A
+00006a20: 4253 946a aa05 0000 286a b302 0000 6ae4  BS.j....(j....j.
+00006a30: 0400 008c 0961 7474 7269 6275 7465 9489  .....attribute..
+00006a40: 7494 8194 8c1a 6261 6d62 756c 6162 735f  t.....bambulabs_
+00006a50: 6170 692e 4669 6c61 6d65 6e74 2e41 5341  api.Filament.ASA
+00006a60: 946a aa05 0000 286a b302 0000 6ae7 0400  .j....(j....j...
+00006a70: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
+00006a80: 8194 8c19 6261 6d62 756c 6162 735f 6170  ....bambulabs_ap
+00006a90: 692e 4669 6c61 6d65 6e74 2e50 4194 6aaa  i.Filament.PA.j.
+00006aa0: 0500 0028 6ab3 0200 006a ea04 0000 8c09  ...(j....j......
+00006ab0: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
+00006ac0: 1c62 616d 6275 6c61 6273 5f61 7069 2e46  .bambulabs_api.F
+00006ad0: 696c 616d 656e 742e 5041 5f43 4694 6aaa  ilament.PA_CF.j.
+00006ae0: 0500 0028 6ab3 0200 006a ed04 0000 8c09  ...(j....j......
+00006af0: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
+00006b00: 1962 616d 6275 6c61 6273 5f61 7069 2e46  .bambulabs_api.F
+00006b10: 696c 616d 656e 742e 5043 946a aa05 0000  ilament.PC.j....
+00006b20: 286a b302 0000 6af0 0400 008c 0961 7474  (j....j......att
+00006b30: 7269 6275 7465 9489 7494 8194 8c1b 6261  ribute..t.....ba
+00006b40: 6d62 756c 6162 735f 6170 692e 4669 6c61  mbulabs_api.Fila
+00006b50: 6d65 6e74 2e50 4554 4794 6aaa 0500 0028  ment.PETG.j....(
+00006b60: 6ab3 0200 006a f304 0000 8c09 6174 7472  j....j......attr
+00006b70: 6962 7574 6594 8974 9481 948c 1a62 616d  ibute..t.....bam
+00006b80: 6275 6c61 6273 5f61 7069 2e46 696c 616d  bulabs_api.Filam
+00006b90: 656e 742e 504c 4194 6aaa 0500 0028 6ab3  ent.PLA.j....(j.
+00006ba0: 0200 006a f604 0000 8c09 6174 7472 6962  ...j......attrib
+00006bb0: 7574 6594 8974 9481 948c 1d62 616d 6275  ute..t.....bambu
+00006bc0: 6c61 6273 5f61 7069 2e46 696c 616d 656e  labs_api.Filamen
+00006bd0: 742e 504c 415f 4346 946a aa05 0000 286a  t.PLA_CF.j....(j
+00006be0: b302 0000 6af9 0400 008c 0961 7474 7269  ....j......attri
+00006bf0: 6275 7465 9489 7494 8194 8c1a 6261 6d62  bute..t.....bamb
+00006c00: 756c 6162 735f 6170 692e 4669 6c61 6d65  ulabs_api.Filame
+00006c10: 6e74 2e50 5641 946a aa05 0000 286a b302  nt.PVA.j....(j..
+00006c20: 0000 6afc 0400 008c 0961 7474 7269 6275  ..j......attribu
+00006c30: 7465 9489 7494 8194 8c1a 6261 6d62 756c  te..t.....bambul
+00006c40: 6162 735f 6170 692e 4669 6c61 6d65 6e74  abs_api.Filament
+00006c50: 2e54 5055 946a aa05 0000 286a b302 0000  .TPU.j....(j....
+00006c60: 6aff 0400 008c 0961 7474 7269 6275 7465  j......attribute
+00006c70: 9489 7494 8194 8c21 6261 6d62 756c 6162  ..t....!bambulab
+00006c80: 735f 6170 692e 414d 5346 696c 616d 656e  s_api.AMSFilamen
+00006c90: 7453 6574 7469 6e67 7394 6aaa 0500 0028  tSettings.j....(
+00006ca0: 6ab3 0200 006a 0205 0000 6aab 0500 0089  j....j....j.....
+00006cb0: 7494 8194 8c2f 6261 6d62 756c 6162 735f  t..../bambulabs_
+00006cc0: 6170 692e 414d 5346 696c 616d 656e 7453  api.AMSFilamentS
+00006cd0: 6574 7469 6e67 732e 7472 6179 5f69 6e66  ettings.tray_inf
+00006ce0: 6f5f 6964 7894 6aaa 0500 0028 6ab3 0200  o_idx.j....(j...
+00006cf0: 006a 0505 0000 8c09 6174 7472 6962 7574  .j......attribut
+00006d00: 6594 8974 9481 948c 3162 616d 6275 6c61  e..t....1bambula
+00006d10: 6273 5f61 7069 2e41 4d53 4669 6c61 6d65  bs_api.AMSFilame
+00006d20: 6e74 5365 7474 696e 6773 2e6e 6f7a 7a6c  ntSettings.nozzl
+00006d30: 655f 7465 6d70 5f6d 696e 946a aa05 0000  e_temp_min.j....
+00006d40: 286a b302 0000 6a08 0500 008c 0961 7474  (j....j......att
+00006d50: 7269 6275 7465 9489 7494 8194 8c31 6261  ribute..t....1ba
+00006d60: 6d62 756c 6162 735f 6170 692e 414d 5346  mbulabs_api.AMSF
+00006d70: 696c 616d 656e 7453 6574 7469 6e67 732e  ilamentSettings.
+00006d80: 6e6f 7a7a 6c65 5f74 656d 705f 6d61 7894  nozzle_temp_max.
+00006d90: 6aaa 0500 0028 6ab3 0200 006a 0b05 0000  j....(j....j....
+00006da0: 8c09 6174 7472 6962 7574 6594 8974 9481  ..attribute..t..
+00006db0: 948c 2b62 616d 6275 6c61 6273 5f61 7069  ..+bambulabs_api
+00006dc0: 2e41 4d53 4669 6c61 6d65 6e74 5365 7474  .AMSFilamentSett
+00006dd0: 696e 6773 2e74 7261 795f 7479 7065 946a  ings.tray_type.j
+00006de0: aa05 0000 286a b302 0000 6a0e 0500 008c  ....(j....j.....
+00006df0: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
+00006e00: 8c19 6261 6d62 756c 6162 735f 6170 692e  ..bambulabs_api.
+00006e10: 5072 696e 7453 7461 7475 7394 6aaa 0500  PrintStatus.j...
+00006e20: 0028 6ab3 0200 006a 1105 0000 6aab 0500  .(j....j....j...
+00006e30: 0089 7494 8194 8c22 6261 6d62 756c 6162  ..t...."bambulab
+00006e40: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00006e50: 732e 5052 494e 5449 4e47 946a aa05 0000  s.PRINTING.j....
+00006e60: 286a b302 0000 6a14 0500 008c 0961 7474  (j....j......att
+00006e70: 7269 6275 7465 9489 7494 8194 8c2b 6261  ribute..t....+ba
+00006e80: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00006e90: 7453 7461 7475 732e 4155 544f 5f42 4544  tStatus.AUTO_BED
+00006ea0: 5f4c 4556 454c 494e 4794 6aaa 0500 0028  _LEVELING.j....(
+00006eb0: 6ab3 0200 006a 1705 0000 8c09 6174 7472  j....j......attr
+00006ec0: 6962 7574 6594 8974 9481 948c 2c62 616d  ibute..t....,bam
+00006ed0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00006ee0: 5374 6174 7573 2e48 4541 5442 4544 5f50  Status.HEATBED_P
+00006ef0: 5245 4845 4154 494e 4794 6aaa 0500 0028  REHEATING.j....(
+00006f00: 6ab3 0200 006a 1a05 0000 8c09 6174 7472  j....j......attr
+00006f10: 6962 7574 6594 8974 9481 948c 2f62 616d  ibute..t..../bam
+00006f20: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00006f30: 5374 6174 7573 2e53 5745 4550 494e 475f  Status.SWEEPING_
+00006f40: 5859 5f4d 4543 485f 4d4f 4445 946a aa05  XY_MECH_MODE.j..
+00006f50: 0000 286a b302 0000 6a1d 0500 008c 0961  ..(j....j......a
+00006f60: 7474 7269 6275 7465 9489 7494 8194 8c2b  ttribute..t....+
+00006f70: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+00006f80: 696e 7453 7461 7475 732e 4348 414e 4749  intStatus.CHANGI
+00006f90: 4e47 5f46 494c 414d 454e 5494 6aaa 0500  NG_FILAMENT.j...
+00006fa0: 0028 6ab3 0200 006a 2005 0000 8c09 6174  .(j....j .....at
+00006fb0: 7472 6962 7574 6594 8974 9481 948c 2462  tribute..t....$b
+00006fc0: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00006fd0: 6e74 5374 6174 7573 2e4d 3430 305f 5041  ntStatus.M400_PA
+00006fe0: 5553 4594 6aaa 0500 0028 6ab3 0200 006a  USE.j....(j....j
+00006ff0: 2305 0000 8c09 6174 7472 6962 7574 6594  #.....attribute.
+00007000: 8974 9481 948c 3062 616d 6275 6c61 6273  .t....0bambulabs
+00007010: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
+00007020: 2e50 4155 5345 445f 4649 4c41 4d45 4e54  .PAUSED_FILAMENT
+00007030: 5f52 554e 4f55 5494 6aaa 0500 0028 6ab3  _RUNOUT.j....(j.
+00007040: 0200 006a 2605 0000 8c09 6174 7472 6962  ...j&.....attrib
+00007050: 7574 6594 8974 9481 948c 2862 616d 6275  ute..t....(bambu
+00007060: 6c61 6273 5f61 7069 2e50 7269 6e74 5374  labs_api.PrintSt
+00007070: 6174 7573 2e48 4541 5449 4e47 5f48 4f54  atus.HEATING_HOT
+00007080: 454e 4494 6aaa 0500 0028 6ab3 0200 006a  END.j....(j....j
+00007090: 2905 0000 8c09 6174 7472 6962 7574 6594  ).....attribute.
+000070a0: 8974 9481 948c 2f62 616d 6275 6c61 6273  .t..../bambulabs
+000070b0: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
+000070c0: 2e43 414c 4942 5241 5449 4e47 5f45 5854  .CALIBRATING_EXT
+000070d0: 5255 5349 4f4e 946a aa05 0000 286a b302  RUSION.j....(j..
+000070e0: 0000 6a2c 0500 008c 0961 7474 7269 6275  ..j,.....attribu
+000070f0: 7465 9489 7494 8194 8c2e 6261 6d62 756c  te..t.....bambul
+00007100: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00007110: 7475 732e 5343 414e 4e49 4e47 5f42 4544  tus.SCANNING_BED
+00007120: 5f53 5552 4641 4345 946a aa05 0000 286a  _SURFACE.j....(j
+00007130: b302 0000 6a2f 0500 008c 0961 7474 7269  ....j/.....attri
+00007140: 6275 7465 9489 7494 8194 8c30 6261 6d62  bute..t....0bamb
+00007150: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+00007160: 7461 7475 732e 494e 5350 4543 5449 4e47  tatus.INSPECTING
+00007170: 5f46 4952 5354 5f4c 4159 4552 946a aa05  _FIRST_LAYER.j..
+00007180: 0000 286a b302 0000 6a32 0500 008c 0961  ..(j....j2.....a
+00007190: 7474 7269 6275 7465 9489 7494 8194 8c36  ttribute..t....6
+000071a0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+000071b0: 696e 7453 7461 7475 732e 4944 454e 5449  intStatus.IDENTI
+000071c0: 4659 494e 475f 4255 494c 445f 504c 4154  FYING_BUILD_PLAT
+000071d0: 455f 5459 5045 946a aa05 0000 286a b302  E_TYPE.j....(j..
+000071e0: 0000 6a35 0500 008c 0961 7474 7269 6275  ..j5.....attribu
+000071f0: 7465 9489 7494 8194 8c31 6261 6d62 756c  te..t....1bambul
+00007200: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00007210: 7475 732e 4341 4c49 4252 4154 494e 475f  tus.CALIBRATING_
+00007220: 4d49 4352 4f5f 4c49 4441 5294 6aaa 0500  MICRO_LIDAR.j...
+00007230: 0028 6ab3 0200 006a 3805 0000 8c09 6174  .(j....j8.....at
+00007240: 7472 6962 7574 6594 8974 9481 948c 2962  tribute..t....)b
+00007250: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00007260: 6e74 5374 6174 7573 2e48 4f4d 494e 475f  ntStatus.HOMING_
+00007270: 544f 4f4c 4845 4144 946a aa05 0000 286a  TOOLHEAD.j....(j
+00007280: b302 0000 6a3b 0500 008c 0961 7474 7269  ....j;.....attri
+00007290: 6275 7465 9489 7494 8194 8c2d 6261 6d62  bute..t....-bamb
+000072a0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+000072b0: 7461 7475 732e 434c 4541 4e49 4e47 5f4e  tatus.CLEANING_N
+000072c0: 4f5a 5a4c 455f 5449 5094 6aaa 0500 0028  OZZLE_TIP.j....(
 000072d0: 6ab3 0200 006a 3e05 0000 8c09 6174 7472  j....j>.....attr
-000072e0: 6962 7574 6594 8974 9481 948c 3962 616d  ibute..t....9bam
+000072e0: 6962 7574 6594 8974 9481 948c 3762 616d  ibute..t....7bam
 000072f0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00007300: 5374 6174 7573 2e50 4155 5345 445f 4c4f  Status.PAUSED_LO
-00007310: 575f 4641 4e5f 5350 4545 445f 4845 4154  W_FAN_SPEED_HEAT
-00007320: 5f42 5245 414b 946a 7105 0000 286a b302  _BREAK.jq...(j..
-00007330: 0000 6a41 0500 008c 0961 7474 7269 6275  ..jA.....attribu
-00007340: 7465 9489 7494 8194 8c42 6261 6d62 756c  te..t....Bbambul
-00007350: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
-00007360: 7475 732e 5041 5553 4544 5f43 4841 4d42  tus.PAUSED_CHAMB
-00007370: 4552 5f54 454d 5045 5241 5455 5245 5f43  ER_TEMPERATURE_C
-00007380: 4f4e 5452 4f4c 5f45 5252 4f52 946a 7105  ONTROL_ERROR.jq.
-00007390: 0000 286a b302 0000 6a44 0500 008c 0961  ..(j....jD.....a
-000073a0: 7474 7269 6275 7465 9489 7494 8194 8c29  ttribute..t....)
-000073b0: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
-000073c0: 696e 7453 7461 7475 732e 434f 4f4c 494e  intStatus.COOLIN
-000073d0: 475f 4348 414d 4245 5294 6a71 0500 0028  G_CHAMBER.jq...(
-000073e0: 6ab3 0200 006a 4705 0000 8c09 6174 7472  j....jG.....attr
-000073f0: 6962 7574 6594 8974 9481 948c 2b62 616d  ibute..t....+bam
-00007400: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-00007410: 5374 6174 7573 2e50 4155 5345 445f 5553  Status.PAUSED_US
-00007420: 4552 5f47 434f 4445 946a 7105 0000 286a  ER_GCODE.jq...(j
-00007430: b302 0000 6a4a 0500 008c 0961 7474 7269  ....jJ.....attri
-00007440: 6275 7465 9489 7494 8194 8c2d 6261 6d62  bute..t....-bamb
-00007450: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
-00007460: 7461 7475 732e 4d4f 544f 525f 4e4f 4953  tatus.MOTOR_NOIS
-00007470: 455f 5348 4f57 4f46 4694 6a71 0500 0028  E_SHOWOFF.jq...(
-00007480: 6ab3 0200 006a 4d05 0000 8c09 6174 7472  j....jM.....attr
-00007490: 6962 7574 6594 8974 9481 948c 4162 616d  ibute..t....Abam
-000074a0: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
-000074b0: 5374 6174 7573 2e50 4155 5345 445f 4e4f  Status.PAUSED_NO
-000074c0: 5a5a 4c45 5f46 494c 414d 454e 545f 434f  ZZLE_FILAMENT_CO
-000074d0: 5645 5245 445f 4445 5445 4354 4544 946a  VERED_DETECTED.j
-000074e0: 7105 0000 286a b302 0000 6a50 0500 008c  q...(j....jP....
-000074f0: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
-00007500: 8c2d 6261 6d62 756c 6162 735f 6170 692e  .-bambulabs_api.
-00007510: 5072 696e 7453 7461 7475 732e 5041 5553  PrintStatus.PAUS
-00007520: 4544 5f43 5554 5445 525f 4552 524f 5294  ED_CUTTER_ERROR.
-00007530: 6a71 0500 0028 6ab3 0200 006a 5305 0000  jq...(j....jS...
-00007540: 8c09 6174 7472 6962 7574 6594 8974 9481  ..attribute..t..
-00007550: 948c 3262 616d 6275 6c61 6273 5f61 7069  ..2bambulabs_api
-00007560: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
-00007570: 5345 445f 4649 5253 545f 4c41 5945 525f  SED_FIRST_LAYER_
-00007580: 4552 524f 5294 6a71 0500 0028 6ab3 0200  ERROR.jq...(j...
-00007590: 006a 5605 0000 8c09 6174 7472 6962 7574  .jV.....attribut
-000075a0: 6594 8974 9481 948c 2c62 616d 6275 6c61  e..t....,bambula
-000075b0: 6273 5f61 7069 2e50 7269 6e74 5374 6174  bs_api.PrintStat
-000075c0: 7573 2e50 4155 5345 445f 4e4f 5a5a 4c45  us.PAUSED_NOZZLE
-000075d0: 5f43 4c4f 4794 6a71 0500 0028 6ab3 0200  _CLOG.jq...(j...
+00007300: 5374 6174 7573 2e43 4845 434b 494e 475f  Status.CHECKING_
+00007310: 4558 5452 5544 4552 5f54 454d 5045 5241  EXTRUDER_TEMPERA
+00007320: 5455 5245 946a aa05 0000 286a b302 0000  TURE.j....(j....
+00007330: 6a41 0500 008c 0961 7474 7269 6275 7465  jA.....attribute
+00007340: 9489 7494 8194 8c25 6261 6d62 756c 6162  ..t....%bambulab
+00007350: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00007360: 732e 5041 5553 4544 5f55 5345 5294 6aaa  s.PAUSED_USER.j.
+00007370: 0500 0028 6ab3 0200 006a 4405 0000 8c09  ...(j....jD.....
+00007380: 6174 7472 6962 7574 6594 8974 9481 948c  attribute..t....
+00007390: 3462 616d 6275 6c61 6273 5f61 7069 2e50  4bambulabs_api.P
+000073a0: 7269 6e74 5374 6174 7573 2e50 4155 5345  rintStatus.PAUSE
+000073b0: 445f 4652 4f4e 545f 434f 5645 525f 4641  D_FRONT_COVER_FA
+000073c0: 4c4c 494e 4794 6aaa 0500 0028 6ab3 0200  LLING.j....(j...
+000073d0: 006a 4705 0000 8c09 6174 7472 6962 7574  .jG.....attribut
+000073e0: 6594 8974 9481 948c 2b62 616d 6275 6c61  e..t....+bambula
+000073f0: 6273 5f61 7069 2e50 7269 6e74 5374 6174  bs_api.PrintStat
+00007400: 7573 2e43 414c 4942 5241 5449 4e47 5f4c  us.CALIBRATING_L
+00007410: 4944 4152 946a aa05 0000 286a b302 0000  IDAR.j....(j....
+00007420: 6a4a 0500 008c 0961 7474 7269 6275 7465  jJ.....attribute
+00007430: 9489 7494 8194 8c34 6261 6d62 756c 6162  ..t....4bambulab
+00007440: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00007450: 732e 4341 4c49 4252 4154 494e 475f 4558  s.CALIBRATING_EX
+00007460: 5452 5553 494f 4e5f 464c 4f57 946a aa05  TRUSION_FLOW.j..
+00007470: 0000 286a b302 0000 6a4d 0500 008c 0961  ..(j....jM.....a
+00007480: 7474 7269 6275 7465 9489 7494 8194 8c3f  ttribute..t....?
+00007490: 6261 6d62 756c 6162 735f 6170 692e 5072  bambulabs_api.Pr
+000074a0: 696e 7453 7461 7475 732e 5041 5553 4544  intStatus.PAUSED
+000074b0: 5f4e 4f5a 5a4c 455f 5445 4d50 4552 4154  _NOZZLE_TEMPERAT
+000074c0: 5552 455f 4d41 4c46 554e 4354 494f 4e94  URE_MALFUNCTION.
+000074d0: 6aaa 0500 0028 6ab3 0200 006a 5005 0000  j....(j....jP...
+000074e0: 8c09 6174 7472 6962 7574 6594 8974 9481  ..attribute..t..
+000074f0: 948c 4162 616d 6275 6c61 6273 5f61 7069  ..Abambulabs_api
+00007500: 2e50 7269 6e74 5374 6174 7573 2e50 4155  .PrintStatus.PAU
+00007510: 5345 445f 4845 4154 5f42 4544 5f54 454d  SED_HEAT_BED_TEM
+00007520: 5045 5241 5455 5245 5f4d 414c 4655 4e43  PERATURE_MALFUNC
+00007530: 5449 4f4e 946a aa05 0000 286a b302 0000  TION.j....(j....
+00007540: 6a53 0500 008c 0961 7474 7269 6275 7465  jS.....attribute
+00007550: 9489 7494 8194 8c2c 6261 6d62 756c 6162  ..t....,bambulab
+00007560: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00007570: 732e 4649 4c41 4d45 4e54 5f55 4e4c 4f41  s.FILAMENT_UNLOA
+00007580: 4449 4e47 946a aa05 0000 286a b302 0000  DING.j....(j....
+00007590: 6a56 0500 008c 0961 7474 7269 6275 7465  jV.....attribute
+000075a0: 9489 7494 8194 8c2d 6261 6d62 756c 6162  ..t....-bambulab
+000075b0: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+000075c0: 732e 5041 5553 4544 5f53 4b49 5050 4544  s.PAUSED_SKIPPED
+000075d0: 5f53 5445 5094 6aaa 0500 0028 6ab3 0200  _STEP.j....(j...
 000075e0: 006a 5905 0000 8c09 6174 7472 6962 7574  .jY.....attribut
-000075f0: 6594 8974 9481 948c 2162 616d 6275 6c61  e..t....!bambula
+000075f0: 6594 8974 9481 948c 2a62 616d 6275 6c61  e..t....*bambula
 00007600: 6273 5f61 7069 2e50 7269 6e74 5374 6174  bs_api.PrintStat
-00007610: 7573 2e55 4e4b 4e4f 574e 946a 7105 0000  us.UNKNOWN.jq...
-00007620: 286a b302 0000 6a5c 0500 008c 0961 7474  (j....j\.....att
-00007630: 7269 6275 7465 9489 7494 8194 8c1e 6261  ribute..t.....ba
-00007640: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
-00007650: 7453 7461 7475 732e 4944 4c45 946a 7105  tStatus.IDLE.jq.
-00007660: 0000 286a b302 0000 6a5f 0500 008c 0961  ..(j....j_.....a
-00007670: 7474 7269 6275 7465 9489 7494 8194 756a  ttribute..t...uj
-00007680: 6405 0000 7d94 286a 6e05 0000 6a6f 0500  d...}.(jn...jo..
-00007690: 008c 0b4d 6f64 756c 6545 6e74 7279 9493  ...ModuleEntry..
-000076a0: 9428 6ab3 0200 006a 4404 0000 6842 6842  .(j....jD...hBhB
-000076b0: 8974 9481 946a e905 0000 6aec 0600 0028  .t...j....j....(
-000076c0: 6ab3 0200 006a 9f04 0000 6842 6842 8974  j....j....hBhB.t
-000076d0: 9481 946a 3c06 0000 6aec 0600 0028 6ab3  ...j<...j....(j.
-000076e0: 0200 006a de04 0000 6842 6842 8974 9481  ...j....hBhB.t..
-000076f0: 946a 4f06 0000 6aec 0600 0028 6ab3 0200  .jO...j....(j...
-00007700: 006a ed04 0000 6842 6842 8974 9481 9475  .j....hBhB.t...u
-00007710: 6ab4 0200 004b 0075 8c03 7273 7494 7d94  j....K.u..rst.}.
-00007720: 286a 2504 0000 7d94 6ab4 0200 004b 0075  (j%...}.j....K.u
-00007730: 8c03 7374 6494 7d94 288c 0b70 726f 676f  ..std.}.(..progo
-00007740: 7074 696f 6e73 947d 946a 2504 0000 7d94  ptions.}.j%...}.
-00007750: 8c06 6c61 6265 6c73 947d 9428 8c08 6765  ..labels.}.(..ge
-00007760: 6e69 6e64 6578 946a ff06 0000 6842 8c0d  nindex.j....hB..
-00007770: 7370 6869 6e78 2e6c 6f63 616c 6594 8c11  sphinx.locale...
-00007780: 5f54 7261 6e73 6c61 7469 6f6e 5072 6f78  _TranslationProx
-00007790: 7994 9394 286a 0007 0000 8c0f 5f6c 617a  y...(j......_laz
-000077a0: 795f 7472 616e 736c 6174 6594 9394 8c06  y_translate.....
-000077b0: 7370 6869 6e78 948c 0767 656e 6572 616c  sphinx...general
-000077c0: 948c 0549 6e64 6578 9474 9481 946a 0407  ...Index.t...j..
-000077d0: 0000 6a05 0700 006a 0607 0000 6a07 0700  ..j....j....j...
-000077e0: 0087 9486 9462 8794 8c08 6d6f 6469 6e64  .....b....modind
-000077f0: 6578 948c 0b70 792d 6d6f 6469 6e64 6578  ex...py-modindex
-00007800: 9468 426a 0207 0000 286a 0407 0000 6a05  .hBj....(j....j.
-00007810: 0700 006a 0607 0000 8c0c 4d6f 6475 6c65  ...j......Module
-00007820: 2049 6e64 6578 9474 9481 946a 0407 0000   Index.t...j....
-00007830: 6a05 0700 006a 0607 0000 6a0f 0700 0087  j....j....j.....
-00007840: 9486 9462 8794 8c06 7365 6172 6368 946a  ...b....search.j
-00007850: 1507 0000 6842 6a02 0700 0028 6a04 0700  ....hBj....(j...
-00007860: 006a 0507 0000 6a06 0700 008c 0b53 6561  .j....j......Sea
-00007870: 7263 6820 5061 6765 9474 9481 946a 0407  rch Page.t...j..
-00007880: 0000 6a05 0700 006a 0607 0000 6a16 0700  ..j....j....j...
-00007890: 0087 9486 9462 8794 8c0b 7079 2d6d 6f64  .....b....py-mod
-000078a0: 696e 6465 7894 8c0b 7079 2d6d 6f64 696e  index...py-modin
-000078b0: 6465 7894 6842 8c13 5079 7468 6f6e 204d  dex.hB..Python M
-000078c0: 6f64 756c 6520 496e 6465 7894 8794 758c  odule Index...u.
-000078d0: 0a61 6e6f 6e6c 6162 656c 7394 7d94 286a  .anonlabels.}.(j
-000078e0: ff06 0000 6aff 0600 0068 4286 946a 0d07  ....j....hB..j..
-000078f0: 0000 6a0e 0700 0068 4286 946a 1507 0000  ..j....hB..j....
-00007900: 6a15 0700 0068 4286 946a 1c07 0000 6a1d  j....hB..j....j.
-00007910: 0700 0068 4286 9475 6ab4 0200 004b 008c  ...hB..uj....K..
-00007920: 0574 6572 6d73 947d 9475 758c 0669 6d61  .terms.}.uu..ima
-00007930: 6765 7394 8c0b 7370 6869 6e78 2e75 7469  ges...sphinx.uti
-00007940: 6c94 8c10 4669 6c65 6e61 6d65 556e 6971  l...FilenameUniq
-00007950: 4469 6374 9493 9429 8194 8f94 628c 0764  Dict...)....b..d
-00007960: 6c66 696c 6573 946a 2907 0000 8c0d 446f  lfiles.j).....Do
-00007970: 776e 6c6f 6164 4669 6c65 7394 9394 2981  wnloadFiles...).
-00007980: 948c 126f 7269 6769 6e61 6c5f 696d 6167  ...original_imag
-00007990: 655f 7572 6994 7d94 8c09 7465 6d70 5f64  e_uri.}...temp_d
-000079a0: 6174 6194 7d94 8c0b 7265 665f 636f 6e74  ata.}...ref_cont
-000079b0: 6578 7494 7d94 7562 2e                   ext.}.ub.
+00007610: 7573 2e46 494c 414d 454e 545f 4c4f 4144  us.FILAMENT_LOAD
+00007620: 494e 4794 6aaa 0500 0028 6ab3 0200 006a  ING.j....(j....j
+00007630: 5c05 0000 8c09 6174 7472 6962 7574 6594  \.....attribute.
+00007640: 8974 9481 948c 3162 616d 6275 6c61 6273  .t....1bambulabs
+00007650: 5f61 7069 2e50 7269 6e74 5374 6174 7573  _api.PrintStatus
+00007660: 2e43 414c 4942 5241 5449 4e47 5f4d 4f54  .CALIBRATING_MOT
+00007670: 4f52 5f4e 4f49 5345 946a aa05 0000 286a  OR_NOISE.j....(j
+00007680: b302 0000 6a5f 0500 008c 0961 7474 7269  ....j_.....attri
+00007690: 6275 7465 9489 7494 8194 8c29 6261 6d62  bute..t....)bamb
+000076a0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+000076b0: 7461 7475 732e 5041 5553 4544 5f41 4d53  tatus.PAUSED_AMS
+000076c0: 5f4c 4f53 5494 6aaa 0500 0028 6ab3 0200  _LOST.j....(j...
+000076d0: 006a 6205 0000 8c09 6174 7472 6962 7574  .jb.....attribut
+000076e0: 6594 8974 9481 948c 3962 616d 6275 6c61  e..t....9bambula
+000076f0: 6273 5f61 7069 2e50 7269 6e74 5374 6174  bs_api.PrintStat
+00007700: 7573 2e50 4155 5345 445f 4c4f 575f 4641  us.PAUSED_LOW_FA
+00007710: 4e5f 5350 4545 445f 4845 4154 5f42 5245  N_SPEED_HEAT_BRE
+00007720: 414b 946a aa05 0000 286a b302 0000 6a65  AK.j....(j....je
+00007730: 0500 008c 0961 7474 7269 6275 7465 9489  .....attribute..
+00007740: 7494 8194 8c42 6261 6d62 756c 6162 735f  t....Bbambulabs_
+00007750: 6170 692e 5072 696e 7453 7461 7475 732e  api.PrintStatus.
+00007760: 5041 5553 4544 5f43 4841 4d42 4552 5f54  PAUSED_CHAMBER_T
+00007770: 454d 5045 5241 5455 5245 5f43 4f4e 5452  EMPERATURE_CONTR
+00007780: 4f4c 5f45 5252 4f52 946a aa05 0000 286a  OL_ERROR.j....(j
+00007790: b302 0000 6a68 0500 008c 0961 7474 7269  ....jh.....attri
+000077a0: 6275 7465 9489 7494 8194 8c29 6261 6d62  bute..t....)bamb
+000077b0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
+000077c0: 7461 7475 732e 434f 4f4c 494e 475f 4348  tatus.COOLING_CH
+000077d0: 414d 4245 5294 6aaa 0500 0028 6ab3 0200  AMBER.j....(j...
+000077e0: 006a 6b05 0000 8c09 6174 7472 6962 7574  .jk.....attribut
+000077f0: 6594 8974 9481 948c 2b62 616d 6275 6c61  e..t....+bambula
+00007800: 6273 5f61 7069 2e50 7269 6e74 5374 6174  bs_api.PrintStat
+00007810: 7573 2e50 4155 5345 445f 5553 4552 5f47  us.PAUSED_USER_G
+00007820: 434f 4445 946a aa05 0000 286a b302 0000  CODE.j....(j....
+00007830: 6a6e 0500 008c 0961 7474 7269 6275 7465  jn.....attribute
+00007840: 9489 7494 8194 8c2d 6261 6d62 756c 6162  ..t....-bambulab
+00007850: 735f 6170 692e 5072 696e 7453 7461 7475  s_api.PrintStatu
+00007860: 732e 4d4f 544f 525f 4e4f 4953 455f 5348  s.MOTOR_NOISE_SH
+00007870: 4f57 4f46 4694 6aaa 0500 0028 6ab3 0200  OWOFF.j....(j...
+00007880: 006a 7105 0000 8c09 6174 7472 6962 7574  .jq.....attribut
+00007890: 6594 8974 9481 948c 4162 616d 6275 6c61  e..t....Abambula
+000078a0: 6273 5f61 7069 2e50 7269 6e74 5374 6174  bs_api.PrintStat
+000078b0: 7573 2e50 4155 5345 445f 4e4f 5a5a 4c45  us.PAUSED_NOZZLE
+000078c0: 5f46 494c 414d 454e 545f 434f 5645 5245  _FILAMENT_COVERE
+000078d0: 445f 4445 5445 4354 4544 946a aa05 0000  D_DETECTED.j....
+000078e0: 286a b302 0000 6a74 0500 008c 0961 7474  (j....jt.....att
+000078f0: 7269 6275 7465 9489 7494 8194 8c2d 6261  ribute..t....-ba
+00007900: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00007910: 7453 7461 7475 732e 5041 5553 4544 5f43  tStatus.PAUSED_C
+00007920: 5554 5445 525f 4552 524f 5294 6aaa 0500  UTTER_ERROR.j...
+00007930: 0028 6ab3 0200 006a 7705 0000 8c09 6174  .(j....jw.....at
+00007940: 7472 6962 7574 6594 8974 9481 948c 3262  tribute..t....2b
+00007950: 616d 6275 6c61 6273 5f61 7069 2e50 7269  ambulabs_api.Pri
+00007960: 6e74 5374 6174 7573 2e50 4155 5345 445f  ntStatus.PAUSED_
+00007970: 4649 5253 545f 4c41 5945 525f 4552 524f  FIRST_LAYER_ERRO
+00007980: 5294 6aaa 0500 0028 6ab3 0200 006a 7a05  R.j....(j....jz.
+00007990: 0000 8c09 6174 7472 6962 7574 6594 8974  ....attribute..t
+000079a0: 9481 948c 2c62 616d 6275 6c61 6273 5f61  ....,bambulabs_a
+000079b0: 7069 2e50 7269 6e74 5374 6174 7573 2e50  pi.PrintStatus.P
+000079c0: 4155 5345 445f 4e4f 5a5a 4c45 5f43 4c4f  AUSED_NOZZLE_CLO
+000079d0: 4794 6aaa 0500 0028 6ab3 0200 006a 7d05  G.j....(j....j}.
+000079e0: 0000 8c09 6174 7472 6962 7574 6594 8974  ....attribute..t
+000079f0: 9481 948c 2162 616d 6275 6c61 6273 5f61  ....!bambulabs_a
+00007a00: 7069 2e50 7269 6e74 5374 6174 7573 2e55  pi.PrintStatus.U
+00007a10: 4e4b 4e4f 574e 946a aa05 0000 286a b302  NKNOWN.j....(j..
+00007a20: 0000 6a80 0500 008c 0961 7474 7269 6275  ..j......attribu
+00007a30: 7465 9489 7494 8194 8c1e 6261 6d62 756c  te..t.....bambul
+00007a40: 6162 735f 6170 692e 5072 696e 7453 7461  abs_api.PrintSta
+00007a50: 7475 732e 4944 4c45 946a aa05 0000 286a  tus.IDLE.j....(j
+00007a60: b302 0000 6a83 0500 008c 0961 7474 7269  ....j......attri
+00007a70: 6275 7465 9489 7494 8194 8c18 6261 6d62  bute..t.....bamb
+00007a80: 756c 6162 735f 6170 692e 4763 6f64 6553  ulabs_api.GcodeS
+00007a90: 7461 7465 946a aa05 0000 286a b302 0000  tate.j....(j....
+00007aa0: 6a86 0500 006a ab05 0000 8974 9481 948c  j....j.....t....
+00007ab0: 1d62 616d 6275 6c61 6273 5f61 7069 2e47  .bambulabs_api.G
+00007ac0: 636f 6465 5374 6174 652e 4944 4c45 946a  codeState.IDLE.j
+00007ad0: aa05 0000 286a b302 0000 6a89 0500 008c  ....(j....j.....
+00007ae0: 0961 7474 7269 6275 7465 9489 7494 8194  .attribute..t...
+00007af0: 8c22 6261 6d62 756c 6162 735f 6170 692e  ."bambulabs_api.
+00007b00: 4763 6f64 6553 7461 7465 2e50 5245 5041  GcodeState.PREPA
+00007b10: 5249 4e47 946a aa05 0000 286a b302 0000  RING.j....(j....
+00007b20: 6a8c 0500 008c 0961 7474 7269 6275 7465  j......attribute
+00007b30: 9489 7494 8194 8c20 6261 6d62 756c 6162  ..t.... bambulab
+00007b40: 735f 6170 692e 4763 6f64 6553 7461 7465  s_api.GcodeState
+00007b50: 2e52 554e 4e49 4e47 946a aa05 0000 286a  .RUNNING.j....(j
+00007b60: b302 0000 6a8f 0500 008c 0961 7474 7269  ....j......attri
+00007b70: 6275 7465 9489 7494 8194 8c1f 6261 6d62  bute..t.....bamb
+00007b80: 756c 6162 735f 6170 692e 4763 6f64 6553  ulabs_api.GcodeS
+00007b90: 7461 7465 2e50 4155 5345 4494 6aaa 0500  tate.PAUSED.j...
+00007ba0: 0028 6ab3 0200 006a 9205 0000 8c09 6174  .(j....j......at
+00007bb0: 7472 6962 7574 6594 8974 9481 948c 2162  tribute..t....!b
+00007bc0: 616d 6275 6c61 6273 5f61 7069 2e47 636f  ambulabs_api.Gco
+00007bd0: 6465 5374 6174 652e 4649 4e49 5348 4544  deState.FINISHED
+00007be0: 946a aa05 0000 286a b302 0000 6a95 0500  .j....(j....j...
+00007bf0: 008c 0961 7474 7269 6275 7465 9489 7494  ...attribute..t.
+00007c00: 8194 8c20 6261 6d62 756c 6162 735f 6170  ... bambulabs_ap
+00007c10: 692e 4763 6f64 6553 7461 7465 2e55 4e4b  i.GcodeState.UNK
+00007c20: 4e4f 574e 946a aa05 0000 286a b302 0000  NOWN.j....(j....
+00007c30: 6a98 0500 008c 0961 7474 7269 6275 7465  j......attribute
+00007c40: 9489 7494 8194 756a 9d05 0000 7d94 286a  ..t...uj....}.(j
+00007c50: a705 0000 6aa8 0500 008c 0b4d 6f64 756c  ....j......Modul
+00007c60: 6545 6e74 7279 9493 9428 6ab3 0200 006a  eEntry...(j....j
+00007c70: 6804 0000 6842 6842 8974 9481 946a 2206  h...hBhB.t...j".
+00007c80: 0000 6a40 0700 0028 6ab3 0200 006a c304  ..j@...(j....j..
+00007c90: 0000 6842 6842 8974 9481 946a 7506 0000  ..hBhB.t...ju...
+00007ca0: 6a40 0700 0028 6ab3 0200 006a 0205 0000  j@...(j....j....
+00007cb0: 6842 6842 8974 9481 946a 8806 0000 6a40  hBhB.t...j....j@
+00007cc0: 0700 0028 6ab3 0200 006a 1105 0000 6842  ...(j....j....hB
+00007cd0: 6842 8974 9481 946a 2307 0000 6a40 0700  hB.t...j#...j@..
+00007ce0: 0028 6ab3 0200 006a 8605 0000 6842 6842  .(j....j....hBhB
+00007cf0: 8974 9481 9475 6ab4 0200 004b 0075 8c03  .t...uj....K.u..
+00007d00: 7273 7494 7d94 286a 4904 0000 7d94 6ab4  rst.}.(jI...}.j.
+00007d10: 0200 004b 0075 8c03 7374 6494 7d94 288c  ...K.u..std.}.(.
+00007d20: 0b70 726f 676f 7074 696f 6e73 947d 946a  .progoptions.}.j
+00007d30: 4904 0000 7d94 8c06 6c61 6265 6c73 947d  I...}...labels.}
+00007d40: 9428 8c08 6765 6e69 6e64 6578 946a 5507  .(..genindex.jU.
+00007d50: 0000 6842 8c0d 7370 6869 6e78 2e6c 6f63  ..hB..sphinx.loc
+00007d60: 616c 6594 8c11 5f54 7261 6e73 6c61 7469  ale..._Translati
+00007d70: 6f6e 5072 6f78 7994 9394 286a 5607 0000  onProxy...(jV...
+00007d80: 8c0f 5f6c 617a 795f 7472 616e 736c 6174  .._lazy_translat
+00007d90: 6594 9394 8c06 7370 6869 6e78 948c 0767  e.....sphinx...g
+00007da0: 656e 6572 616c 948c 0549 6e64 6578 9474  eneral...Index.t
+00007db0: 9481 946a 5a07 0000 6a5b 0700 006a 5c07  ...jZ...j[...j\.
+00007dc0: 0000 6a5d 0700 0087 9486 9462 8794 8c08  ..j].......b....
+00007dd0: 6d6f 6469 6e64 6578 948c 0b70 792d 6d6f  modindex...py-mo
+00007de0: 6469 6e64 6578 9468 426a 5807 0000 286a  dindex.hBjX...(j
+00007df0: 5a07 0000 6a5b 0700 006a 5c07 0000 8c0c  Z...j[...j\.....
+00007e00: 4d6f 6475 6c65 2049 6e64 6578 9474 9481  Module Index.t..
+00007e10: 946a 5a07 0000 6a5b 0700 006a 5c07 0000  .jZ...j[...j\...
+00007e20: 6a65 0700 0087 9486 9462 8794 8c06 7365  je.......b....se
+00007e30: 6172 6368 946a 6b07 0000 6842 6a58 0700  arch.jk...hBjX..
+00007e40: 0028 6a5a 0700 006a 5b07 0000 6a5c 0700  .(jZ...j[...j\..
+00007e50: 008c 0b53 6561 7263 6820 5061 6765 9474  ...Search Page.t
+00007e60: 9481 946a 5a07 0000 6a5b 0700 006a 5c07  ...jZ...j[...j\.
+00007e70: 0000 6a6c 0700 0087 9486 9462 8794 8c0b  ..jl.......b....
+00007e80: 7079 2d6d 6f64 696e 6465 7894 8c0b 7079  py-modindex...py
+00007e90: 2d6d 6f64 696e 6465 7894 6842 8c13 5079  -modindex.hB..Py
+00007ea0: 7468 6f6e 204d 6f64 756c 6520 496e 6465  thon Module Inde
+00007eb0: 7894 8794 758c 0a61 6e6f 6e6c 6162 656c  x...u..anonlabel
+00007ec0: 7394 7d94 286a 5507 0000 6a55 0700 0068  s.}.(jU...jU...h
+00007ed0: 4286 946a 6307 0000 6a64 0700 0068 4286  B..jc...jd...hB.
+00007ee0: 946a 6b07 0000 6a6b 0700 0068 4286 946a  .jk...jk...hB..j
+00007ef0: 7207 0000 6a73 0700 0068 4286 9475 6ab4  r...js...hB..uj.
+00007f00: 0200 004b 008c 0574 6572 6d73 947d 9475  ...K...terms.}.u
+00007f10: 758c 0669 6d61 6765 7394 8c0b 7370 6869  u..images...sphi
+00007f20: 6e78 2e75 7469 6c94 8c10 4669 6c65 6e61  nx.util...Filena
+00007f30: 6d65 556e 6971 4469 6374 9493 9429 8194  meUniqDict...)..
+00007f40: 8f94 628c 0764 6c66 696c 6573 946a 7f07  ..b..dlfiles.j..
+00007f50: 0000 8c0d 446f 776e 6c6f 6164 4669 6c65  ....DownloadFile
+00007f60: 7394 9394 2981 948c 126f 7269 6769 6e61  s...)....origina
+00007f70: 6c5f 696d 6167 655f 7572 6994 7d94 8c09  l_image_uri.}...
+00007f80: 7465 6d70 5f64 6174 6194 7d94 8c0b 7265  temp_data.}...re
+00007f90: 665f 636f 6e74 6578 7494 7d94 7562 2e    f_context.}.ub.
```

### Comparing `bambulabs_api-2.1.5/docs/.doctrees/index.doctree` & `bambulabs_api-2.1.6/docs/.doctrees/index.doctree`

 * *Files 1% similar despite different names*

```diff
@@ -12287,15 +12287,15 @@
 0002ffe0: 235d 9428 6a9a 4800 008c 0961 7474 7269  #].(j.H....attri
 0002fff0: 6275 7465 9465 6825 5d94 6827 5d94 6829  bute.eh%].h'].h)
 00030000: 5d94 6a18 0500 006a 9a48 0000 6a19 0500  ].j....j.H..j...
 00030010: 006a c048 0000 6a1a 0500 006a c048 0000  .j.H..j....j.H..
 00030020: 6a1b 0500 0089 7568 2b68 ac68 1c68 0368  j.....uh+h.h.h.h
 00030030: 1b6a b739 0000 681d 4e68 1e4e 7562 687e  .j.9..h.Nh.Nubh~
 00030040: 2981 947d 9428 6805 6806 6807 5d94 681f  )..}.(h.h.h.].h.
-00030050: 7d94 2868 215d 9468 235d 9468 2595 9d5e  }.(h!].h#].h%..^
+00030050: 7d94 2868 215d 9468 235d 9468 2595 728b  }.(h!].h#].h%.r.
 00030060: 0000 0000 0000 5d94 6827 5d94 6829 5d94  ......].h'].h)].
 00030070: 8c07 656e 7472 6965 7394 5d94 2868 a88c  ..entries.].(h..
 00030080: 4550 4155 5345 445f 4c4f 575f 4641 4e5f  EPAUSED_LOW_FAN_
 00030090: 5350 4545 445f 4845 4154 5f42 5245 414b  SPEED_HEAT_BREAK
 000300a0: 2028 696e 206d 6f64 756c 6520 6261 6d62   (in module bamb
 000300b0: 756c 6162 735f 6170 692e 5072 696e 7453  ulabs_api.PrintS
 000300c0: 7461 7475 7329 948c 3962 616d 6275 6c61  tatus)..9bambula
@@ -13370,440 +13370,1157 @@
 00034390: 006a c44e 0000 6a1a 0500 006a c44e 0000  .j.N..j....j.N..
 000343a0: 6a1b 0500 0089 7568 2b68 ac68 1c68 0368  j.....uh+h.h.h.h
 000343b0: 1b6a b739 0000 681d 4e68 1e4e 7562 6568  .j.9..h.Nh.Nubeh
 000343c0: 1f7d 9428 6821 5d94 8c0b 7072 696e 7473  .}.(h!]...prints
 000343d0: 7461 7475 7394 6168 235d 9468 255d 948c  tatus.ah#].h%]..
 000343e0: 0b70 7269 6e74 7374 6174 7573 9461 6827  .printstatus.ah'
 000343f0: 5d94 6829 5d94 7568 2b68 0a68 1b68 0368  ].h)].uh+h.h.h.h
-00034400: 1c68 0368 1d68 2c68 1e4b 1d75 6265 681f  .h.h.h,h.K.ubeh.
-00034410: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00034420: 275d 9468 295d 948c 0673 6f75 7263 6594  '].h)]...source.
-00034430: 682c 7568 2b68 018c 0e63 7572 7265 6e74  h,uh+h...current
-00034440: 5f73 6f75 7263 6594 4e8c 0c63 7572 7265  _source.N..curre
-00034450: 6e74 5f6c 696e 6594 4e8c 0873 6574 7469  nt_line.N..setti
-00034460: 6e67 7394 8c11 646f 6375 7469 6c73 2e66  ngs...docutils.f
-00034470: 726f 6e74 656e 6494 8c06 5661 6c75 6573  rontend...Values
-00034480: 9493 9429 8194 7d94 2868 0f4e 8c09 6765  ...)..}.(h.N..ge
-00034490: 6e65 7261 746f 7294 4e8c 0964 6174 6573  nerator.N..dates
-000344a0: 7461 6d70 944e 8c0b 736f 7572 6365 5f6c  tamp.N..source_l
-000344b0: 696e 6b94 4e8c 0a73 6f75 7263 655f 7572  ink.N..source_ur
-000344c0: 6c94 4e8c 0d74 6f63 5f62 6163 6b6c 696e  l.N..toc_backlin
-000344d0: 6b73 948c 0565 6e74 7279 948c 1266 6f6f  ks...entry...foo
-000344e0: 746e 6f74 655f 6261 636b 6c69 6e6b 7394  tnote_backlinks.
-000344f0: 4b01 8c0d 7365 6374 6e75 6d5f 7866 6f72  K...sectnum_xfor
-00034500: 6d94 4b01 8c0e 7374 7269 705f 636f 6d6d  m.K...strip_comm
-00034510: 656e 7473 944e 8c1b 7374 7269 705f 656c  ents.N..strip_el
-00034520: 656d 656e 7473 5f77 6974 685f 636c 6173  ements_with_clas
-00034530: 7365 7394 4e8c 0d73 7472 6970 5f63 6c61  ses.N..strip_cla
-00034540: 7373 6573 944e 8c0c 7265 706f 7274 5f6c  sses.N..report_l
-00034550: 6576 656c 944b 028c 0a68 616c 745f 6c65  evel.K...halt_le
-00034560: 7665 6c94 4b05 8c11 6578 6974 5f73 7461  vel.K...exit_sta
-00034570: 7475 735f 6c65 7665 6c94 4b05 8c05 6465  tus_level.K...de
-00034580: 6275 6794 4e8c 0e77 6172 6e69 6e67 5f73  bug.N..warning_s
-00034590: 7472 6561 6d94 4e8c 0974 7261 6365 6261  tream.N..traceba
-000345a0: 636b 9488 8c0e 696e 7075 745f 656e 636f  ck....input_enco
-000345b0: 6469 6e67 948c 0975 7466 2d38 2d73 6967  ding...utf-8-sig
-000345c0: 948c 1c69 6e70 7574 5f65 6e63 6f64 696e  ...input_encodin
-000345d0: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
-000345e0: 8c06 7374 7269 6374 948c 0f6f 7574 7075  ..strict...outpu
-000345f0: 745f 656e 636f 6469 6e67 948c 0575 7466  t_encoding...utf
-00034600: 2d38 948c 1d6f 7574 7075 745f 656e 636f  -8...output_enco
-00034610: 6469 6e67 5f65 7272 6f72 5f68 616e 646c  ding_error_handl
-00034620: 6572 946a f34e 0000 8c0e 6572 726f 725f  er.j.N....error_
-00034630: 656e 636f 6469 6e67 948c 0575 7466 2d38  encoding...utf-8
-00034640: 948c 1c65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
-00034650: 675f 6572 726f 725f 6861 6e64 6c65 7294  g_error_handler.
-00034660: 8c10 6261 636b 736c 6173 6872 6570 6c61  ..backslashrepla
-00034670: 6365 948c 0d6c 616e 6775 6167 655f 636f  ce...language_co
-00034680: 6465 948c 0265 6e94 8c13 7265 636f 7264  de...en...record
-00034690: 5f64 6570 656e 6465 6e63 6965 7394 4e8c  _dependencies.N.
-000346a0: 0663 6f6e 6669 6794 4e8c 0969 645f 7072  .config.N..id_pr
-000346b0: 6566 6978 9468 068c 0e61 7574 6f5f 6964  efix.h...auto_id
-000346c0: 5f70 7265 6669 7894 8c02 6964 948c 0d64  _prefix...id...d
-000346d0: 756d 705f 7365 7474 696e 6773 944e 8c0e  ump_settings.N..
-000346e0: 6475 6d70 5f69 6e74 6572 6e61 6c73 944e  dump_internals.N
-000346f0: 8c0f 6475 6d70 5f74 7261 6e73 666f 726d  ..dump_transform
-00034700: 7394 4e8c 0f64 756d 705f 7073 6575 646f  s.N..dump_pseudo
-00034710: 5f78 6d6c 944e 8c10 6578 706f 7365 5f69  _xml.N..expose_i
-00034720: 6e74 6572 6e61 6c73 944e 8c0e 7374 7269  nternals.N..stri
-00034730: 6374 5f76 6973 6974 6f72 944e 8c0f 5f64  ct_visitor.N.._d
-00034740: 6973 6162 6c65 5f63 6f6e 6669 6794 4e8c  isable_config.N.
-00034750: 075f 736f 7572 6365 9468 2c8c 0c5f 6465  ._source.h,.._de
-00034760: 7374 696e 6174 696f 6e94 4e8c 0d5f 636f  stination.N.._co
-00034770: 6e66 6967 5f66 696c 6573 945d 948c 1666  nfig_files.]...f
-00034780: 696c 655f 696e 7365 7274 696f 6e5f 656e  ile_insertion_en
-00034790: 6162 6c65 6494 888c 0b72 6177 5f65 6e61  abled....raw_ena
-000347a0: 626c 6564 944b 018c 116c 696e 655f 6c65  bled.K...line_le
-000347b0: 6e67 7468 5f6c 696d 6974 944d 1027 8c0e  ngth_limit.M.'..
-000347c0: 7065 705f 7265 6665 7265 6e63 6573 944e  pep_references.N
-000347d0: 8c0c 7065 705f 6261 7365 5f75 726c 948c  ..pep_base_url..
-000347e0: 1868 7474 7073 3a2f 2f70 6570 732e 7079  .https://peps.py
-000347f0: 7468 6f6e 2e6f 7267 2f94 8c15 7065 705f  thon.org/...pep_
-00034800: 6669 6c65 5f75 726c 5f74 656d 706c 6174  file_url_templat
-00034810: 6594 8c08 7065 702d 2530 3464 948c 0e72  e...pep-%04d...r
-00034820: 6663 5f72 6566 6572 656e 6365 7394 4e8c  fc_references.N.
-00034830: 0c72 6663 5f62 6173 655f 7572 6c94 8c26  .rfc_base_url..&
-00034840: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
-00034850: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
-00034860: 2f68 746d 6c2f 948c 0974 6162 5f77 6964  /html/...tab_wid
-00034870: 7468 944b 088c 1d74 7269 6d5f 666f 6f74  th.K...trim_foot
-00034880: 6e6f 7465 5f72 6566 6572 656e 6365 5f73  note_reference_s
-00034890: 7061 6365 9489 8c10 7379 6e74 6178 5f68  pace....syntax_h
-000348a0: 6967 686c 6967 6874 948c 046c 6f6e 6794  ighlight...long.
-000348b0: 8c0c 736d 6172 745f 7175 6f74 6573 9488  ..smart_quotes..
-000348c0: 8c13 736d 6172 7471 756f 7465 735f 6c6f  ..smartquotes_lo
-000348d0: 6361 6c65 7394 5d94 8c1d 6368 6172 6163  cales.]...charac
-000348e0: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
-000348f0: 5f6d 6172 6b75 7094 898c 0e64 6f63 7469  _markup....docti
-00034900: 746c 655f 7866 6f72 6d94 898c 0d64 6f63  tle_xform....doc
-00034910: 696e 666f 5f78 666f 726d 944b 018c 1273  info_xform.K...s
-00034920: 6563 7473 7562 7469 746c 655f 7866 6f72  ectsubtitle_xfor
-00034930: 6d94 898c 0d69 6d61 6765 5f6c 6f61 6469  m....image_loadi
-00034940: 6e67 948c 046c 696e 6b94 8c10 656d 6265  ng...link...embe
-00034950: 645f 7374 796c 6573 6865 6574 9489 8c15  d_stylesheet....
-00034960: 636c 6f61 6b5f 656d 6169 6c5f 6164 6472  cloak_email_addr
-00034970: 6573 7365 7394 888c 1173 6563 7469 6f6e  esses....section
-00034980: 5f73 656c 665f 6c69 6e6b 9489 8c03 656e  _self_link....en
-00034990: 7694 4e75 628c 0872 6570 6f72 7465 7294  v.Nub..reporter.
-000349a0: 4e8c 1069 6e64 6972 6563 745f 7461 7267  N..indirect_targ
-000349b0: 6574 7394 5d94 8c11 7375 6273 7469 7475  ets.]...substitu
-000349c0: 7469 6f6e 5f64 6566 7394 7d94 8c12 7375  tion_defs.}...su
-000349d0: 6273 7469 7475 7469 6f6e 5f6e 616d 6573  bstitution_names
-000349e0: 947d 948c 0872 6566 6e61 6d65 7394 7d94  .}...refnames.}.
-000349f0: 8c06 7265 6669 6473 947d 948c 076e 616d  ..refids.}...nam
-00034a00: 6569 6473 947d 9428 6832 682f 685b 6858  eids.}.(h2h/h[hX
-00034a10: 6af2 2b00 006a ef2b 0000 6a33 3700 006a  j.+..j.+..j37..j
-00034a20: 3037 0000 6ab4 3900 006a b139 0000 6acd  07..j.9..j.9..j.
-00034a30: 4e00 006a ca4e 0000 758c 096e 616d 6574  N..j.N..u..namet
-00034a40: 7970 6573 947d 9428 6832 4e68 5b4e 6af2  ypes.}.(h2Nh[Nj.
-00034a50: 2b00 004e 6a33 3700 004e 6ab4 3900 004e  +..Nj37..Nj.9..N
-00034a60: 6acd 4e00 004e 7568 217d 9428 682f 680c  j.N..Nuh!}.(h/h.
-00034a70: 6858 6835 6aef 2b00 0068 5e68 7668 7168  hXh5j.+..h^hvhqh
-00034a80: aa68 b36a 2805 0000 6a2e 0500 006a a305  .h.j(...j....j..
-00034a90: 0000 6aa8 0500 006a 6607 0000 6a6c 0700  ..j....jf...jl..
-00034aa0: 006a e107 0000 6ae6 0700 006a 3f09 0000  .j....j....j?...
-00034ab0: 6a44 0900 006a 4c0a 0000 6a51 0a00 006a  jD...jL...jQ...j
-00034ac0: 590b 0000 6a5e 0b00 006a 660c 0000 6a6b  Y...j^...jf...jk
-00034ad0: 0c00 006a bf0d 0000 6ac4 0d00 006a 7c0f  ...j....j....j|.
-00034ae0: 0000 6a81 0f00 006a 8910 0000 6a8e 1000  ..j....j....j...
-00034af0: 006a 9611 0000 6a9b 1100 006a 5313 0000  .j....j....jS...
-00034b00: 6a58 1300 006a 6014 0000 6a65 1400 006a  jX...j`...je...j
-00034b10: 6d15 0000 6a72 1500 006a 3017 0000 6a35  m...jr...j0...j5
-00034b20: 1700 006a 3d18 0000 6a42 1800 006a 4a19  ...j=...jB...jJ.
-00034b30: 0000 6a4f 1900 006a 571a 0000 6a5c 1a00  ..jO...jW...j\..
-00034b40: 006a 1a1c 0000 6a1f 1c00 006a f51e 0000  .j....j....j....
-00034b50: 6afa 1e00 006a b820 0000 6abd 2000 006a  j....j. ..j. ..j
-00034b60: 7b22 0000 6a80 2200 006a ef24 0000 6af4  {"..j."..j.$..j.
-00034b70: 2400 006a fc25 0000 6a01 2600 006a 0927  $..j.%..j.&..j.'
-00034b80: 0000 6a0e 2700 006a 1628 0000 6a1b 2800  ..j.'..j.(..j.(.
-00034b90: 006a 2329 0000 6a28 2900 006a 3037 0000  .j#)..j()..j07..
-00034ba0: 6af5 2b00 006a 0b2c 0000 6a06 2c00 006a  j.+..j.,..j.,..j
-00034bb0: 492c 0000 6a4e 2c00 006a d62c 0000 6adb  I,..jN,..j.,..j.
-00034bc0: 2c00 006a 622d 0000 6a67 2d00 006a ee2d  ,..jb-..jg-..j.-
-00034bd0: 0000 6af3 2d00 006a 7a2e 0000 6a7f 2e00  ..j.-..jz...j...
-00034be0: 006a 062f 0000 6a0b 2f00 006a 922f 0000  .j./..j./..j./..
-00034bf0: 6a97 2f00 006a 1e30 0000 6a23 3000 006a  j./..j.0..j#0..j
-00034c00: aa30 0000 6aaf 3000 006a 3631 0000 6a3b  .0..j.0..j61..j;
-00034c10: 3100 006a c231 0000 6ac7 3100 006a 4e32  1..j.1..j.1..jN2
-00034c20: 0000 6a53 3200 006a da32 0000 6adf 3200  ..jS2..j.2..j.2.
-00034c30: 006a 6633 0000 6a6b 3300 006a f233 0000  .jf3..jk3..j.3..
-00034c40: 6af7 3300 006a 7e34 0000 6a83 3400 006a  j.3..j~4..j.4..j
-00034c50: 0a35 0000 6a0f 3500 006a 9635 0000 6a9b  .5..j.5..j.5..j.
-00034c60: 3500 006a 2236 0000 6a27 3600 006a ae36  5..j"6..j'6..j.6
-00034c70: 0000 6ab3 3600 006a b139 0000 6a36 3700  ..j.6..j.9..j67.
-00034c80: 006a 4c37 0000 6a47 3700 006a 8a37 0000  .jL7..jG7..j.7..
-00034c90: 6a8f 3700 006a 1738 0000 6a1c 3800 006a  j.7..j.8..j.8..j
-00034ca0: a338 0000 6aa8 3800 006a 2f39 0000 6a34  .8..j.8..j/9..j4
-00034cb0: 3900 006a ca4e 0000 6ab7 3900 006a cd39  9..j.N..j.9..j.9
-00034cc0: 0000 6ac8 3900 006a 0b3a 0000 6a10 3a00  ..j.9..j.:..j.:.
-00034cd0: 006a 983a 0000 6a9d 3a00 006a 243b 0000  .j.:..j.:..j$;..
-00034ce0: 6a29 3b00 006a b03b 0000 6ab5 3b00 006a  j);..j.;..j.;..j
-00034cf0: 3c3c 0000 6a41 3c00 006a c83c 0000 6acd  <<..jA<..j.<..j.
-00034d00: 3c00 006a 543d 0000 6a59 3d00 006a e03d  <..jT=..jY=..j.=
-00034d10: 0000 6ae5 3d00 006a 6c3e 0000 6a71 3e00  ..j.=..jl>..jq>.
-00034d20: 006a f83e 0000 6afd 3e00 006a 843f 0000  .j.>..j.>..j.?..
-00034d30: 6a89 3f00 006a 1040 0000 6a15 4000 006a  j.?..j.@..j.@..j
-00034d40: 9c40 0000 6aa1 4000 006a 2841 0000 6a2d  .@..j.@..j(A..j-
-00034d50: 4100 006a b441 0000 6ab9 4100 006a 4042  A..j.A..j.A..j@B
-00034d60: 0000 6a45 4200 006a cc42 0000 6ad1 4200  ..jEB..j.B..j.B.
-00034d70: 006a 5843 0000 6a5d 4300 006a e443 0000  .jXC..j]C..j.C..
-00034d80: 6ae9 4300 006a 7044 0000 6a75 4400 006a  j.C..jpD..juD..j
-00034d90: fc44 0000 6a01 4500 006a 8845 0000 6a8d  .D..j.E..j.E..j.
-00034da0: 4500 006a 1446 0000 6a19 4600 006a a046  E..j.F..j.F..j.F
-00034db0: 0000 6aa5 4600 006a 2c47 0000 6a31 4700  ..j.F..j,G..j1G.
-00034dc0: 006a b847 0000 6abd 4700 006a 4448 0000  .j.G..j.G..jDH..
-00034dd0: 6a49 4800 006a d048 0000 6ad5 4800 006a  jIH..j.H..j.H..j
-00034de0: 5c49 0000 6a61 4900 006a e849 0000 6aed  \I..jaI..j.I..j.
-00034df0: 4900 006a 744a 0000 6a79 4a00 006a 004b  I..jtJ..jyJ..j.K
-00034e00: 0000 6a05 4b00 006a 8c4b 0000 6a91 4b00  ..j.K..j.K..j.K.
-00034e10: 006a 184c 0000 6a1d 4c00 006a a44c 0000  .j.L..j.L..j.L..
-00034e20: 6aa9 4c00 006a 304d 0000 6a35 4d00 006a  j.L..j0M..j5M..j
-00034e30: bc4d 0000 6ac1 4d00 006a 484e 0000 6a4d  .M..j.M..jHN..jM
-00034e40: 4e00 0075 8c0d 666f 6f74 6e6f 7465 5f72  N..u..footnote_r
-00034e50: 6566 7394 7d94 8c0d 6369 7461 7469 6f6e  efs.}...citation
-00034e60: 5f72 6566 7394 7d94 8c0d 6175 746f 666f  _refs.}...autofo
-00034e70: 6f74 6e6f 7465 7394 5d94 8c11 6175 746f  otnotes.]...auto
-00034e80: 666f 6f74 6e6f 7465 5f72 6566 7394 5d94  footnote_refs.].
-00034e90: 8c10 7379 6d62 6f6c 5f66 6f6f 746e 6f74  ..symbol_footnot
-00034ea0: 6573 945d 948c 1473 796d 626f 6c5f 666f  es.]...symbol_fo
-00034eb0: 6f74 6e6f 7465 5f72 6566 7394 5d94 8c09  otnote_refs.]...
-00034ec0: 666f 6f74 6e6f 7465 7394 5d94 8c09 6369  footnotes.]...ci
-00034ed0: 7461 7469 6f6e 7394 5d94 8c12 6175 746f  tations.]...auto
-00034ee0: 666f 6f74 6e6f 7465 5f73 7461 7274 944b  footnote_start.K
-00034ef0: 018c 1573 796d 626f 6c5f 666f 6f74 6e6f  ...symbol_footno
-00034f00: 7465 5f73 7461 7274 944b 008c 0a69 645f  te_start.K...id_
-00034f10: 636f 756e 7465 7294 8c0b 636f 6c6c 6563  counter...collec
-00034f20: 7469 6f6e 7394 8c07 436f 756e 7465 7294  tions...Counter.
-00034f30: 9394 7d94 8594 5294 8c0e 7061 7273 655f  ..}...R...parse_
-00034f40: 6d65 7373 6167 6573 945d 9428 6809 8c0e  messages.].(h...
-00034f50: 7379 7374 656d 5f6d 6573 7361 6765 9493  system_message..
-00034f60: 9429 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
-00034f70: 6847 2981 947d 9428 6805 6806 6807 5d94  hG)..}.(h.h.h.].
-00034f80: 6816 8c1a 5469 746c 6520 756e 6465 726c  h...Title underl
-00034f90: 696e 6520 746f 6f20 7368 6f72 742e 9485  ine too short...
-00034fa0: 9481 947d 9428 6805 6806 681b 6a59 4f00  ...}.(h.h.h.jYO.
-00034fb0: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00034fc0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
-00034fd0: 6846 681b 6a56 4f00 0075 6268 098c 0d6c  hFh.jVO..ubh...l
-00034fe0: 6974 6572 616c 5f62 6c6f 636b 9493 9429  iteral_block...)
-00034ff0: 8194 7d94 2868 058c 0e50 7269 6e74 6572  ..}.(h...Printer
-00035000: 0a3d 3d3d 3d3d 3d94 6807 5d94 6816 8c0e  .======.h.].h...
-00035010: 5072 696e 7465 720a 3d3d 3d3d 3d3d 9485  Printer.======..
-00035020: 9481 947d 9428 6805 6806 681b 6a68 4f00  ...}.(h.h.h.jhO.
-00035030: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-00035040: 9468 255d 9468 275d 9468 295d 9468 c968  .h%].h'].h)].h.h
-00035050: ca75 682b 6a66 4f00 0068 1b6a 564f 0000  .uh+jfO..h.jVO..
-00035060: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00035070: 6825 5d94 6827 5d94 6829 5d94 8c05 6c65  h%].h'].h)]...le
-00035080: 7665 6c94 4b02 8c04 7479 7065 948c 0757  vel.K...type...W
-00035090: 4152 4e49 4e47 948c 046c 696e 6594 4b0b  ARNING...line.K.
-000350a0: 8c06 736f 7572 6365 9468 2c75 682b 6a54  ..source.h,uh+jT
-000350b0: 4f00 0075 626a 554f 0000 2981 947d 9428  O..ubjUO..)..}.(
-000350c0: 6805 6806 6807 5d94 2868 4729 8194 7d94  h.h.h.].(hG)..}.
-000350d0: 2868 058c 1a54 6974 6c65 2075 6e64 6572  (h...Title under
-000350e0: 6c69 6e65 2074 6f6f 2073 686f 7274 2e94  line too short..
-000350f0: 6807 5d94 6816 8c1a 5469 746c 6520 756e  h.].h...Title un
-00035100: 6465 726c 696e 6520 746f 6f20 7368 6f72  derline too shor
-00035110: 742e 9485 9481 947d 9428 6805 6806 681b  t......}.(h.h.h.
-00035120: 6a84 4f00 0068 1c68 0368 1d4e 681e 4e75  j.O..h.h.h.Nh.Nu
-00035130: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
-00035140: 255d 9468 275d 9468 295d 9475 682b 6846  %].h'].h)].uh+hF
-00035150: 681b 6a81 4f00 0075 626a 674f 0000 2981  h.j.O..ubjgO..).
-00035160: 947d 9428 6805 8c0e 5072 696e 7465 720a  .}.(h...Printer.
-00035170: 3d3d 3d3d 3d3d 9468 075d 9468 168c 0e50  ======.h.].h...P
-00035180: 7269 6e74 6572 0a3d 3d3d 3d3d 3d94 8594  rinter.======...
-00035190: 8194 7d94 2868 0568 0668 1b6a 924f 0000  ..}.(h.h.h.j.O..
-000351a0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-000351b0: 6825 5d94 6827 5d94 6829 5d94 68c9 68ca  h%].h'].h)].h.h.
-000351c0: 7568 2b6a 664f 0000 681b 6a81 4f00 0068  uh+jfO..h.j.O..h
-000351d0: 1d68 2c75 6265 681f 7d94 2868 215d 9468  .h,ubeh.}.(h!].h
-000351e0: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
-000351f0: 056c 6576 656c 944b 028c 0474 7970 6594  .level.K...type.
-00035200: 6a7e 4f00 008c 046c 696e 6594 4b0b 8c06  j~O....line.K...
-00035210: 736f 7572 6365 9468 2c75 682b 6a54 4f00  source.h,uh+jTO.
-00035220: 0068 1b68 5e68 1c68 0368 1d68 2c68 1e4b  .h.h^h.h.h.h,h.K
-00035230: 0b75 626a 554f 0000 2981 947d 9428 6805  .ubjUO..)..}.(h.
-00035240: 6806 6807 5d94 2868 4729 8194 7d94 2868  h.h.].(hG)..}.(h
-00035250: 0568 0668 075d 9468 168c 1a54 6974 6c65  .h.h.].h...Title
-00035260: 2075 6e64 6572 6c69 6e65 2074 6f6f 2073   underline too s
-00035270: 686f 7274 2e94 8594 8194 7d94 2868 0568  hort......}.(h.h
-00035280: 0668 1b6a ad4f 0000 7562 6168 1f7d 9428  .h.j.O..ubah.}.(
-00035290: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-000352a0: 6829 5d94 7568 2b68 4668 1b6a aa4f 0000  h)].uh+hFh.j.O..
-000352b0: 7562 6a67 4f00 0029 8194 7d94 2868 058c  ubjgO..)..}.(h..
-000352c0: 0f46 696c 616d 656e 740a 3d3d 3d3d 3d3d  .Filament.======
-000352d0: 9468 075d 9468 168c 0f46 696c 616d 656e  .h.].h...Filamen
-000352e0: 740a 3d3d 3d3d 3d3d 9485 9481 947d 9428  t.======.....}.(
-000352f0: 6805 6806 681b 6aba 4f00 0075 6261 681f  h.h.h.j.O..ubah.
-00035300: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00035310: 275d 9468 295d 9468 c968 ca75 682b 6a66  '].h)].h.h.uh+jf
-00035320: 4f00 0068 1b6a aa4f 0000 7562 6568 1f7d  O..h.j.O..ubeh.}
-00035330: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00035340: 5d94 6829 5d94 8c05 6c65 7665 6c94 4b02  ].h)]...level.K.
-00035350: 8c04 7479 7065 946a 7e4f 0000 8c04 6c69  ..type.j~O....li
-00035360: 6e65 944b 118c 0673 6f75 7263 6594 682c  ne.K...source.h,
-00035370: 7568 2b6a 544f 0000 7562 6a55 4f00 0029  uh+jTO..ubjUO..)
-00035380: 8194 7d94 2868 0568 0668 075d 9428 6847  ..}.(h.h.h.].(hG
-00035390: 2981 947d 9428 6805 8c1a 5469 746c 6520  )..}.(h...Title 
-000353a0: 756e 6465 726c 696e 6520 746f 6f20 7368  underline too sh
-000353b0: 6f72 742e 9468 075d 9468 168c 1a54 6974  ort..h.].h...Tit
-000353c0: 6c65 2075 6e64 6572 6c69 6e65 2074 6f6f  le underline too
-000353d0: 2073 686f 7274 2e94 8594 8194 7d94 2868   short......}.(h
-000353e0: 0568 0668 1b6a d54f 0000 681c 6803 681d  .h.h.j.O..h.h.h.
-000353f0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-00035400: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-00035410: 7568 2b68 4668 1b6a d24f 0000 7562 6a67  uh+hFh.j.O..ubjg
-00035420: 4f00 0029 8194 7d94 2868 058c 0f46 696c  O..)..}.(h...Fil
-00035430: 616d 656e 740a 3d3d 3d3d 3d3d 9468 075d  ament.======.h.]
-00035440: 9468 168c 0f46 696c 616d 656e 740a 3d3d  .h...Filament.==
-00035450: 3d3d 3d3d 9485 9481 947d 9428 6805 6806  ====.....}.(h.h.
-00035460: 681b 6ae3 4f00 0075 6261 681f 7d94 2868  h.j.O..ubah.}.(h
-00035470: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
-00035480: 295d 9468 c968 ca75 682b 6a66 4f00 0068  )].h.h.uh+jfO..h
-00035490: 1b6a d24f 0000 681d 682c 7562 6568 1f7d  .j.O..h.h,ubeh.}
-000354a0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000354b0: 5d94 6829 5d94 8c05 6c65 7665 6c94 4b02  ].h)]...level.K.
-000354c0: 8c04 7479 7065 946a 7e4f 0000 8c04 6c69  ..type.j~O....li
-000354d0: 6e65 944b 118c 0673 6f75 7263 6594 682c  ne.K...source.h,
-000354e0: 7568 2b6a 544f 0000 681b 6af5 2b00 0068  uh+jTO..h.j.+..h
-000354f0: 1c68 0368 1d68 2c68 1e4b 1175 626a 554f  .h.h.h,h.K.ubjUO
-00035500: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
-00035510: 2868 4729 8194 7d94 2868 0568 0668 075d  (hG)..}.(h.h.h.]
-00035520: 9468 168c 1a54 6974 6c65 2075 6e64 6572  .h...Title under
-00035530: 6c69 6e65 2074 6f6f 2073 686f 7274 2e94  line too short..
-00035540: 8594 8194 7d94 2868 0568 0668 1b6a fe4f  ....}.(h.h.h.j.O
-00035550: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
-00035560: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
-00035570: 2b68 4668 1b6a fb4f 0000 7562 6a67 4f00  +hFh.j.O..ubjgO.
-00035580: 0029 8194 7d94 2868 058c 1a41 4d53 4669  .)..}.(h...AMSFi
-00035590: 6c61 6d65 6e74 5365 7474 696e 6773 0a3d  lamentSettings.=
-000355a0: 3d3d 3d3d 3d94 6807 5d94 6816 8c1a 414d  =====.h.].h...AM
-000355b0: 5346 696c 616d 656e 7453 6574 7469 6e67  SFilamentSetting
-000355c0: 730a 3d3d 3d3d 3d3d 9485 9481 947d 9428  s.======.....}.(
-000355d0: 6805 6806 681b 6a0b 5000 0075 6261 681f  h.h.h.j.P..ubah.
-000355e0: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-000355f0: 275d 9468 295d 9468 c968 ca75 682b 6a66  '].h)].h.h.uh+jf
-00035600: 4f00 0068 1b6a fb4f 0000 7562 6568 1f7d  O..h.j.O..ubeh.}
-00035610: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-00035620: 5d94 6829 5d94 8c05 6c65 7665 6c94 4b02  ].h)]...level.K.
-00035630: 8c04 7479 7065 946a 7e4f 0000 8c04 6c69  ..type.j~O....li
-00035640: 6e65 944b 178c 0673 6f75 7263 6594 682c  ne.K...source.h,
-00035650: 7568 2b6a 544f 0000 7562 6a55 4f00 0029  uh+jTO..ubjUO..)
-00035660: 8194 7d94 2868 0568 0668 075d 9428 6847  ..}.(h.h.h.].(hG
-00035670: 2981 947d 9428 6805 8c1a 5469 746c 6520  )..}.(h...Title 
-00035680: 756e 6465 726c 696e 6520 746f 6f20 7368  underline too sh
-00035690: 6f72 742e 9468 075d 9468 168c 1a54 6974  ort..h.].h...Tit
-000356a0: 6c65 2075 6e64 6572 6c69 6e65 2074 6f6f  le underline too
-000356b0: 2073 686f 7274 2e94 8594 8194 7d94 2868   short......}.(h
-000356c0: 0568 0668 1b6a 2650 0000 681c 6803 681d  .h.h.j&P..h.h.h.
-000356d0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
-000356e0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
-000356f0: 7568 2b68 4668 1b6a 2350 0000 7562 6a67  uh+hFh.j#P..ubjg
-00035700: 4f00 0029 8194 7d94 2868 058c 1a41 4d53  O..)..}.(h...AMS
-00035710: 4669 6c61 6d65 6e74 5365 7474 696e 6773  FilamentSettings
-00035720: 0a3d 3d3d 3d3d 3d94 6807 5d94 6816 8c1a  .======.h.].h...
-00035730: 414d 5346 696c 616d 656e 7453 6574 7469  AMSFilamentSetti
-00035740: 6e67 730a 3d3d 3d3d 3d3d 9485 9481 947d  ngs.======.....}
-00035750: 9428 6805 6806 681b 6a34 5000 0075 6261  .(h.h.h.j4P..uba
-00035760: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00035770: 9468 275d 9468 295d 9468 c968 ca75 682b  .h'].h)].h.h.uh+
-00035780: 6a66 4f00 0068 1b6a 2350 0000 681d 682c  jfO..h.j#P..h.h,
-00035790: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-000357a0: 6825 5d94 6827 5d94 6829 5d94 8c05 6c65  h%].h'].h)]...le
-000357b0: 7665 6c94 4b02 8c04 7479 7065 946a 7e4f  vel.K...type.j~O
-000357c0: 0000 8c04 6c69 6e65 944b 178c 0673 6f75  ....line.K...sou
-000357d0: 7263 6594 682c 7568 2b6a 544f 0000 681b  rce.h,uh+jTO..h.
-000357e0: 6a36 3700 0068 1c68 0368 1d68 2c68 1e4b  j67..h.h.h.h,h.K
-000357f0: 1775 626a 554f 0000 2981 947d 9428 6805  .ubjUO..)..}.(h.
-00035800: 6806 6807 5d94 2868 4729 8194 7d94 2868  h.h.].(hG)..}.(h
-00035810: 0568 0668 075d 9468 168c 1a54 6974 6c65  .h.h.].h...Title
-00035820: 2075 6e64 6572 6c69 6e65 2074 6f6f 2073   underline too s
-00035830: 686f 7274 2e94 8594 8194 7d94 2868 0568  hort......}.(h.h
-00035840: 0668 1b6a 4f50 0000 7562 6168 1f7d 9428  .h.jOP..ubah.}.(
-00035850: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00035860: 6829 5d94 7568 2b68 4668 1b6a 4c50 0000  h)].uh+hFh.jLP..
-00035870: 7562 6a67 4f00 0029 8194 7d94 2868 058c  ubjgO..)..}.(h..
-00035880: 1250 7269 6e74 5374 6174 7573 0a3d 3d3d  .PrintStatus.===
-00035890: 3d3d 3d94 6807 5d94 6816 8c12 5072 696e  ===.h.].h...Prin
-000358a0: 7453 7461 7475 730a 3d3d 3d3d 3d3d 9485  tStatus.======..
-000358b0: 9481 947d 9428 6805 6806 681b 6a5c 5000  ...}.(h.h.h.j\P.
-000358c0: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
-000358d0: 9468 255d 9468 275d 9468 295d 9468 c968  .h%].h'].h)].h.h
-000358e0: ca75 682b 6a66 4f00 0068 1b6a 4c50 0000  .uh+jfO..h.jLP..
-000358f0: 7562 6568 1f7d 9428 6821 5d94 6823 5d94  ubeh.}.(h!].h#].
-00035900: 6825 5d94 6827 5d94 6829 5d94 8c05 6c65  h%].h'].h)]...le
-00035910: 7665 6c94 4b02 8c04 7479 7065 946a 7e4f  vel.K...type.j~O
-00035920: 0000 8c04 6c69 6e65 944b 1d8c 0673 6f75  ....line.K...sou
-00035930: 7263 6594 682c 7568 2b6a 544f 0000 7562  rce.h,uh+jTO..ub
-00035940: 6a55 4f00 0029 8194 7d94 2868 0568 0668  jUO..)..}.(h.h.h
-00035950: 075d 9428 6847 2981 947d 9428 6805 8c1a  .].(hG)..}.(h...
-00035960: 5469 746c 6520 756e 6465 726c 696e 6520  Title underline 
-00035970: 746f 6f20 7368 6f72 742e 9468 075d 9468  too short..h.].h
-00035980: 168c 1a54 6974 6c65 2075 6e64 6572 6c69  ...Title underli
-00035990: 6e65 2074 6f6f 2073 686f 7274 2e94 8594  ne too short....
-000359a0: 8194 7d94 2868 0568 0668 1b6a 7750 0000  ..}.(h.h.h.jwP..
-000359b0: 681c 6803 681d 4e68 1e4e 7562 6168 1f7d  h.h.h.Nh.Nubah.}
-000359c0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
-000359d0: 5d94 6829 5d94 7568 2b68 4668 1b6a 7450  ].h)].uh+hFh.jtP
-000359e0: 0000 7562 6a67 4f00 0029 8194 7d94 2868  ..ubjgO..)..}.(h
-000359f0: 058c 1250 7269 6e74 5374 6174 7573 0a3d  ...PrintStatus.=
-00035a00: 3d3d 3d3d 3d94 6807 5d94 6816 8c12 5072  =====.h.].h...Pr
-00035a10: 696e 7453 7461 7475 730a 3d3d 3d3d 3d3d  intStatus.======
-00035a20: 9485 9481 947d 9428 6805 6806 681b 6a85  .....}.(h.h.h.j.
-00035a30: 5000 0075 6261 681f 7d94 2868 215d 9468  P..ubah.}.(h!].h
-00035a40: 235d 9468 255d 9468 275d 9468 295d 9468  #].h%].h'].h)].h
-00035a50: c968 ca75 682b 6a66 4f00 0068 1b6a 7450  .h.uh+jfO..h.jtP
-00035a60: 0000 681d 682c 7562 6568 1f7d 9428 6821  ..h.h,ubeh.}.(h!
-00035a70: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00035a80: 5d94 8c05 6c65 7665 6c94 4b02 8c04 7479  ]...level.K...ty
-00035a90: 7065 946a 7e4f 0000 8c04 6c69 6e65 944b  pe.j~O....line.K
-00035aa0: 1d8c 0673 6f75 7263 6594 682c 7568 2b6a  ...source.h,uh+j
-00035ab0: 544f 0000 681b 6ab7 3900 0068 1c68 0368  TO..h.j.9..h.h.h
-00035ac0: 1d68 2c68 1e4b 1d75 6265 8c12 7472 616e  .h,h.K.ube..tran
-00035ad0: 7366 6f72 6d5f 6d65 7373 6167 6573 945d  sform_messages.]
-00035ae0: 9428 6a55 4f00 0029 8194 7d94 2868 0568  .(jUO..)..}.(h.h
-00035af0: 0668 075d 9468 4729 8194 7d94 2868 0568  .h.].hG)..}.(h.h
-00035b00: 0668 075d 9468 168c 4248 7970 6572 6c69  .h.].h..BHyperli
-00035b10: 6e6b 2074 6172 6765 7420 226d 6f64 756c  nk target "modul
-00035b20: 652d 6261 6d62 756c 6162 735f 6170 692e  e-bambulabs_api.
-00035b30: 5072 696e 7465 7222 2069 7320 6e6f 7420  Printer" is not 
-00035b40: 7265 6665 7265 6e63 6564 2e94 8594 8194  referenced......
-00035b50: 7d94 2868 0568 0668 1b6a a250 0000 7562  }.(h.h.h.j.P..ub
-00035b60: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
-00035b70: 5d94 6827 5d94 6829 5d94 7568 2b68 4668  ].h'].h)].uh+hFh
-00035b80: 1b6a 9f50 0000 7562 6168 1f7d 9428 6821  .j.P..ubah.}.(h!
-00035b90: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
-00035ba0: 5d94 8c05 6c65 7665 6c94 4b01 8c04 7479  ]...level.K...ty
-00035bb0: 7065 948c 0449 4e46 4f94 8c06 736f 7572  pe...INFO...sour
-00035bc0: 6365 9468 7c8c 046c 696e 6594 4b01 7568  ce.h|..line.K.uh
-00035bd0: 2b6a 544f 0000 7562 6a55 4f00 0029 8194  +jTO..ubjUO..)..
-00035be0: 7d94 2868 0568 0668 075d 9468 4729 8194  }.(h.h.h.].hG)..
-00035bf0: 7d94 2868 0568 0668 075d 9468 168c 4348  }.(h.h.h.].h..CH
-00035c00: 7970 6572 6c69 6e6b 2074 6172 6765 7420  yperlink target 
-00035c10: 226d 6f64 756c 652d 6261 6d62 756c 6162  "module-bambulab
-00035c20: 735f 6170 692e 4669 6c61 6d65 6e74 2220  s_api.Filament" 
-00035c30: 6973 206e 6f74 2072 6566 6572 656e 6365  is not reference
-00035c40: 642e 9485 9481 947d 9428 6805 6806 681b  d......}.(h.h.h.
-00035c50: 6abd 5000 0075 6261 681f 7d94 2868 215d  j.P..ubah.}.(h!]
-00035c60: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
-00035c70: 9475 682b 6846 681b 6aba 5000 0075 6261  .uh+hFh.j.P..uba
-00035c80: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
-00035c90: 9468 275d 9468 295d 948c 056c 6576 656c  .h'].h)]...level
-00035ca0: 944b 018c 0474 7970 6594 6ab7 5000 008c  .K...type.j.P...
-00035cb0: 0673 6f75 7263 6594 6a11 2c00 008c 046c  .source.j.,....l
-00035cc0: 696e 6594 4b01 7568 2b6a 544f 0000 7562  ine.K.uh+jTO..ub
-00035cd0: 6a55 4f00 0029 8194 7d94 2868 0568 0668  jUO..)..}.(h.h.h
-00035ce0: 075d 9468 4729 8194 7d94 2868 0568 0668  .].hG)..}.(h.h.h
-00035cf0: 075d 9468 168c 4e48 7970 6572 6c69 6e6b  .].h..NHyperlink
-00035d00: 2074 6172 6765 7420 226d 6f64 756c 652d   target "module-
-00035d10: 6261 6d62 756c 6162 735f 6170 692e 414d  bambulabs_api.AM
-00035d20: 5346 696c 616d 656e 7453 6574 7469 6e67  SFilamentSetting
-00035d30: 7322 2069 7320 6e6f 7420 7265 6665 7265  s" is not refere
-00035d40: 6e63 6564 2e94 8594 8194 7d94 2868 0568  nced......}.(h.h
-00035d50: 0668 1b6a d750 0000 7562 6168 1f7d 9428  .h.j.P..ubah.}.(
-00035d60: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
-00035d70: 6829 5d94 7568 2b68 4668 1b6a d450 0000  h)].uh+hFh.j.P..
-00035d80: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
-00035d90: 6825 5d94 6827 5d94 6829 5d94 8c05 6c65  h%].h'].h)]...le
-00035da0: 7665 6c94 4b01 8c04 7479 7065 946a b750  vel.K...type.j.P
-00035db0: 0000 8c06 736f 7572 6365 946a 5237 0000  ....source.jR7..
-00035dc0: 8c04 6c69 6e65 944b 0175 682b 6a54 4f00  ..line.K.uh+jTO.
-00035dd0: 0075 626a 554f 0000 2981 947d 9428 6805  .ubjUO..)..}.(h.
-00035de0: 6806 6807 5d94 6847 2981 947d 9428 6805  h.h.].hG)..}.(h.
-00035df0: 6806 6807 5d94 6816 8c46 4879 7065 726c  h.h.].h..FHyperl
-00035e00: 696e 6b20 7461 7267 6574 2022 6d6f 6475  ink target "modu
-00035e10: 6c65 2d62 616d 6275 6c61 6273 5f61 7069  le-bambulabs_api
-00035e20: 2e50 7269 6e74 5374 6174 7573 2220 6973  .PrintStatus" is
-00035e30: 206e 6f74 2072 6566 6572 656e 6365 642e   not referenced.
-00035e40: 9485 9481 947d 9428 6805 6806 681b 6af1  .....}.(h.h.h.j.
-00035e50: 5000 0075 6261 681f 7d94 2868 215d 9468  P..ubah.}.(h!].h
-00035e60: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
-00035e70: 682b 6846 681b 6aee 5000 0075 6261 681f  h+hFh.j.P..ubah.
-00035e80: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
-00035e90: 275d 9468 295d 948c 056c 6576 656c 944b  '].h)]...level.K
-00035ea0: 018c 0474 7970 6594 6ab7 5000 008c 0673  ...type.j.P....s
-00035eb0: 6f75 7263 6594 6ad3 3900 008c 046c 696e  ource.j.9....lin
-00035ec0: 6594 4b01 7568 2b6a 544f 0000 7562 658c  e.K.uh+jTO..ube.
-00035ed0: 0b74 7261 6e73 666f 726d 6572 944e 8c0b  .transformer.N..
-00035ee0: 696e 636c 7564 655f 6c6f 6794 5d94 8c0a  include_log.]...
-00035ef0: 6465 636f 7261 7469 6f6e 944e 681c 6803  decoration.Nh.h.
-00035f00: 7562 2e                                  ub.
+00034400: 1c68 0368 1d68 2c68 1e4b 1d75 6268 0b29  .h.h.h,h.K.ubh.)
+00034410: 8194 7d94 2868 0568 0668 075d 9428 6810  ..}.(h.h.h.].(h.
+00034420: 2981 947d 9428 6805 8c0a 4763 6f64 6553  )..}.(h...GcodeS
+00034430: 7461 7465 9468 075d 9468 168c 0a47 636f  tate.h.].h...Gco
+00034440: 6465 5374 6174 6594 8594 8194 7d94 2868  deState.....}.(h
+00034450: 056a d54e 0000 681b 6ad3 4e00 0068 1c68  .j.N..h.j.N..h.h
+00034460: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00034470: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00034480: 295d 9475 682b 680f 681b 6ad0 4e00 0068  )].uh+h.h.j.N..h
+00034490: 1c68 0368 1d68 2c68 1e4b 2375 6268 7029  .h.h.h,h.K#ubhp)
+000344a0: 8194 7d94 2868 0568 0668 075d 9468 1f7d  ..}.(h.h.h.].h.}
+000344b0: 9428 6821 5d94 8c1f 6d6f 6475 6c65 2d62  .(h!]...module-b
+000344c0: 616d 6275 6c61 6273 5f61 7069 2e47 636f  ambulabs_api.Gco
+000344d0: 6465 5374 6174 6594 6168 235d 9468 255d  deState.ah#].h%]
+000344e0: 9468 275d 9468 295d 948c 0569 736d 6f64  .h'].h)]...ismod
+000344f0: 9488 7568 2b68 6f68 1d8c 8343 3a5c 5573  ..uh+hoh...C:\Us
+00034500: 6572 735c 6369 6372 695c 4465 736b 746f  ers\cicri\Deskto
+00034510: 705c 436f 6469 6e67 5c49 6d70 6572 6961  p\Coding\Imperia
+00034520: 6c5c 6261 6d62 756c 6162 735f 6170 695c  l\bambulabs_api\
+00034530: 6261 6d62 756c 6162 735f 6170 695c 7374  bambulabs_api\st
+00034540: 6174 6573 5f69 6e66 6f2e 7079 3a64 6f63  ates_info.py:doc
+00034550: 7374 7269 6e67 206f 6620 6261 6d62 756c  string of bambul
+00034560: 6162 735f 6170 692e 7374 6174 6573 5f69  abs_api.states_i
+00034570: 6e66 6f2e 4763 6f64 6553 7461 7465 9468  nfo.GcodeState.h
+00034580: 1e4b 0168 1b6a d04e 0000 681c 6803 7562  .K.h.j.N..h.h.ub
+00034590: 687e 2981 947d 9428 6805 6806 6807 5d94  h~)..}.(h.h.h.].
+000345a0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000345b0: 9468 275d 9468 295d 948c 0765 6e74 7269  .h'].h)]...entri
+000345c0: 6573 945d 9428 688a 8c20 6d6f 6475 6c65  es.].(h.. module
+000345d0: 3b20 6261 6d62 756c 6162 735f 6170 692e  ; bambulabs_api.
+000345e0: 4763 6f64 6553 7461 7465 946a e64e 0000  GcodeState.j.N..
+000345f0: 6806 4e74 9461 7568 2b68 7d68 1b6a d04e  h.Nt.auh+h}h.j.N
+00034600: 0000 681c 6803 681d 8c83 433a 5c55 7365  ..h.h.h...C:\Use
+00034610: 7273 5c63 6963 7269 5c44 6573 6b74 6f70  rs\cicri\Desktop
+00034620: 5c43 6f64 696e 675c 496d 7065 7269 616c  \Coding\Imperial
+00034630: 5c62 616d 6275 6c61 6273 5f61 7069 5c62  \bambulabs_api\b
+00034640: 616d 6275 6c61 6273 5f61 7069 5c73 7461  ambulabs_api\sta
+00034650: 7465 735f 696e 666f 2e70 793a 646f 6373  tes_info.py:docs
+00034660: 7472 696e 6720 6f66 2062 616d 6275 6c61  tring of bambula
+00034670: 6273 5f61 7069 2e73 7461 7465 735f 696e  bs_api.states_in
+00034680: 666f 2e47 636f 6465 5374 6174 6594 681e  fo.GcodeState.h.
+00034690: 4b01 7562 6847 2981 947d 9428 6805 8c1e  K.ubhG)..}.(h...
+000346a0: 456e 756d 2063 6c61 7373 2066 6f72 2074  Enum class for t
+000346b0: 6865 2047 636f 6465 2053 7461 7465 9468  he Gcode State.h
+000346c0: 075d 9468 168c 1e45 6e75 6d20 636c 6173  .].h...Enum clas
+000346d0: 7320 666f 7220 7468 6520 4763 6f64 6520  s for the Gcode 
+000346e0: 5374 6174 6594 8594 8194 7d94 2868 056a  State.....}.(h.j
+000346f0: fd4e 0000 681b 6afb 4e00 0068 1c68 0368  .N..h.j.N..h.h.h
+00034700: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00034710: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00034720: 9475 682b 6846 681d 8c83 433a 5c55 7365  .uh+hFh...C:\Use
+00034730: 7273 5c63 6963 7269 5c44 6573 6b74 6f70  rs\cicri\Desktop
+00034740: 5c43 6f64 696e 675c 496d 7065 7269 616c  \Coding\Imperial
+00034750: 5c62 616d 6275 6c61 6273 5f61 7069 5c62  \bambulabs_api\b
+00034760: 616d 6275 6c61 6273 5f61 7069 5c73 7461  ambulabs_api\sta
+00034770: 7465 735f 696e 666f 2e70 793a 646f 6373  tes_info.py:docs
+00034780: 7472 696e 6720 6f66 2062 616d 6275 6c61  tring of bambula
+00034790: 6273 5f61 7069 2e73 7461 7465 735f 696e  bs_api.states_in
+000347a0: 666f 2e47 636f 6465 5374 6174 6594 681e  fo.GcodeState.h.
+000347b0: 4b01 681b 6ad0 4e00 0068 1c68 0375 6268  K.h.j.N..h.h.ubh
+000347c0: 4729 8194 7d94 2868 058c 2747 636f 6465  G)..}.(h..'Gcode
+000347d0: 2053 7461 7465 2074 6861 7420 7468 6520   State that the 
+000347e0: 7072 696e 7465 7220 6361 6e20 6265 2069  printer can be i
+000347f0: 6e2e 9468 075d 9468 168c 2747 636f 6465  n..h.].h..'Gcode
+00034800: 2053 7461 7465 2074 6861 7420 7468 6520   State that the 
+00034810: 7072 696e 7465 7220 6361 6e20 6265 2069  printer can be i
+00034820: 6e2e 9485 9481 947d 9428 6805 6a0c 4f00  n......}.(h.j.O.
+00034830: 0068 1b6a 0a4f 0000 681c 6803 681d 4e68  .h.j.O..h.h.h.Nh
+00034840: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00034850: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00034860: 2b68 4668 1d6a 094f 0000 681e 4b03 681b  +hFh.j.O..h.K.h.
+00034870: 6ad0 4e00 0068 1c68 0375 6268 7e29 8194  j.N..h.h.ubh~)..
+00034880: 7d94 2868 0568 0668 075d 9468 1f7d 9428  }.(h.h.h.].h.}.(
+00034890: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000348a0: 6829 5d94 8c07 656e 7472 6965 7394 5d94  h)]...entries.].
+000348b0: 2868 a88c 2949 444c 4520 2869 6e20 6d6f  (h..)IDLE (in mo
+000348c0: 6475 6c65 2062 616d 6275 6c61 6273 5f61  dule bambulabs_a
+000348d0: 7069 2e47 636f 6465 5374 6174 6529 948c  pi.GcodeState)..
+000348e0: 1d62 616d 6275 6c61 6273 5f61 7069 2e47  .bambulabs_api.G
+000348f0: 636f 6465 5374 6174 652e 4944 4c45 9468  codeState.IDLE.h
+00034900: 064e 7494 6175 682b 687d 681b 6ad0 4e00  .Nt.auh+h}h.j.N.
+00034910: 0068 1c68 0368 1d4e 681e 4e75 6268 ad29  .h.h.h.Nh.Nubh.)
+00034920: 8194 7d94 2868 0568 0668 075d 9428 68b2  ..}.(h.h.h.].(h.
+00034930: 2981 947d 9428 6805 8c04 4944 4c45 9468  )..}.(h...IDLE.h
+00034940: 075d 9428 68b8 2981 947d 9428 6805 8c19  .].(h.)..}.(h...
+00034950: 6261 6d62 756c 6162 735f 6170 692e 4763  bambulabs_api.Gc
+00034960: 6f64 6553 7461 7465 2e94 6807 5d94 6816  odeState..h.].h.
+00034970: 8c19 6261 6d62 756c 6162 735f 6170 692e  ..bambulabs_api.
+00034980: 4763 6f64 6553 7461 7465 2e94 8594 8194  GcodeState......
+00034990: 7d94 2868 0568 0668 1b6a 2d4f 0000 681c  }.(h.h.h.j-O..h.
+000349a0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000349b0: 6821 5d94 6823 5d94 2868 c468 c565 6825  h!].h#].(h.h.eh%
+000349c0: 5d94 6827 5d94 6829 5d94 68c9 68ca 7568  ].h'].h)].h.h.uh
+000349d0: 2b68 b768 1b6a 294f 0000 681c 6803 681d  +h.h.j)O..h.h.h.
+000349e0: 6a09 4f00 0068 1e4b 0a75 6268 cd29 8194  j.O..h.K.ubh.)..
+000349f0: 7d94 2868 056a 2b4f 0000 6807 5d94 6816  }.(h.j+O..h.].h.
+00034a00: 8c04 4944 4c45 9485 9481 947d 9428 6805  ..IDLE.....}.(h.
+00034a10: 6806 681b 6a3b 4f00 0068 1c68 0368 1d4e  h.h.j;O..h.h.h.N
+00034a20: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00034a30: 235d 9428 68d9 68da 6568 255d 9468 275d  #].(h.h.eh%].h']
+00034a40: 9468 295d 9468 c968 ca75 682b 68cc 681b  .h)].h.h.uh+h.h.
+00034a50: 6a29 4f00 0068 1c68 0368 1d6a 094f 0000  j)O..h.h.h.j.O..
+00034a60: 681e 4b0a 7562 6568 1f7d 9428 6821 5d94  h.K.ubeh.}.(h!].
+00034a70: 6a24 4f00 0061 6823 5d94 286a dc02 0000  j$O..ah#].(j....
+00034a80: 6add 0200 0065 6825 5d94 6827 5d94 6829  j....eh%].h'].h)
+00034a90: 5d94 6ae1 0200 008c 1862 616d 6275 6c61  ].j......bambula
+00034aa0: 6273 5f61 7069 2e47 636f 6465 5374 6174  bs_api.GcodeStat
+00034ab0: 6594 6a4b 0100 0068 066a e302 0000 6a2b  e.jK...h.j....j+
+00034ac0: 4f00 0075 682b 68b1 681d 6a09 4f00 0068  O..uh+h.h.j.O..h
+00034ad0: 1e4b 0568 1b6a 264f 0000 681c 6803 7562  .K.h.j&O..h.h.ub
+00034ae0: 6ae5 0200 0029 8194 7d94 2868 0568 0668  j....)..}.(h.h.h
+00034af0: 075d 946a f902 0000 2981 947d 9428 6805  .].j....)..}.(h.
+00034b00: 6806 6807 5d94 6afe 0200 0029 8194 7d94  h.h.].j....)..}.
+00034b10: 2868 0568 0668 075d 9428 6a03 0300 0029  (h.h.h.].(j....)
+00034b20: 8194 7d94 2868 058c 0474 7970 6594 6807  ..}.(h...type.h.
+00034b30: 5d94 6816 8c04 5479 7065 9485 9481 947d  ].h...Type.....}
+00034b40: 9428 6805 6806 681b 6a58 4f00 0068 1c68  .(h.h.h.jXO..h.h
+00034b50: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00034b60: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00034b70: 295d 9475 682b 6a02 0300 0068 1b6a 554f  )].uh+j....h.jUO
+00034b80: 0000 681d 6a09 4f00 0068 1e4b 0075 626a  ..h.j.O..h.K.ubj
+00034b90: 1303 0000 2981 947d 9428 6805 8c14 5468  ....)..}.(h...Th
+00034ba0: 6520 7072 696e 7465 7220 6973 2069 646c  e printer is idl
+00034bb0: 652e 9468 075d 9468 4729 8194 7d94 2868  e..h.].hG)..}.(h
+00034bc0: 056a 684f 0000 6807 5d94 6a3a 0100 0029  .jhO..h.].j:...)
+00034bd0: 8194 7d94 2868 0568 0668 075d 9468 168c  ..}.(h.h.h.].h..
+00034be0: 1454 6865 2070 7269 6e74 6572 2069 7320  .The printer is 
+00034bf0: 6964 6c65 2e94 8594 8194 7d94 2868 0568  idle......}.(h.h
+00034c00: 0668 1b6a 6d4f 0000 681c 6803 681d 4e68  .h.jmO..h.h.h.Nh
+00034c10: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00034c20: 5d94 6825 5d94 6827 5d94 6829 5d94 8c09  ].h%].h'].h)]...
+00034c30: 7265 6664 6f6d 6169 6e94 8c02 7079 948c  refdomain...py..
+00034c40: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+00034c50: 7265 6674 7970 6594 6a4b 0100 008c 0972  reftype.jK.....r
+00034c60: 6566 7461 7267 6574 948c 1454 6865 2070  eftarget...The p
+00034c70: 7269 6e74 6572 2069 7320 6964 6c65 2e94  rinter is idle..
+00034c80: 6a57 0300 0088 6a58 0300 006a 4e4f 0000  jW....jX...jNO..
+00034c90: 6a59 0300 004e 7568 2b6a 3901 0000 681b  jY...Nuh+j9...h.
+00034ca0: 6a6a 4f00 0068 1c68 0368 1d4e 681e 4e75  jjO..h.h.h.Nh.Nu
+00034cb0: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00034cc0: 255d 9468 275d 9468 295d 9475 682b 6846  %].h'].h)].uh+hF
+00034cd0: 681d 6a09 4f00 0068 1e4b 0968 1b6a 664f  h.j.O..h.K.h.jfO
+00034ce0: 0000 7562 6168 1f7d 9428 6821 5d94 6823  ..ubah.}.(h!].h#
+00034cf0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+00034d00: 2b6a 1203 0000 681b 6a55 4f00 0075 6265  +j....h.jUO..ube
+00034d10: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00034d20: 9468 275d 9468 295d 9475 682b 6afd 0200  .h'].h)].uh+j...
+00034d30: 0068 1d6a 094f 0000 681e 4b09 681b 6a52  .h.j.O..h.K.h.jR
+00034d40: 4f00 0068 1c68 0375 6261 681f 7d94 2868  O..h.h.ubah.}.(h
+00034d50: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00034d60: 295d 9475 682b 6af8 0200 0068 1b6a 4f4f  )].uh+j....h.jOO
+00034d70: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00034d80: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00034d90: 6827 5d94 6829 5d94 7568 2b6a e402 0000  h'].h)].uh+j....
+00034da0: 681b 6a26 4f00 0068 1c68 0368 1d6a 094f  h.j&O..h.h.h.j.O
+00034db0: 0000 681e 4b0a 7562 6568 1f7d 9428 6821  ..h.K.ubeh.}.(h!
+00034dc0: 5d94 6823 5d94 286a 7b4f 0000 8c09 6174  ].h#].(j{O....at
+00034dd0: 7472 6962 7574 6594 6568 255d 9468 275d  tribute.eh%].h']
+00034de0: 9468 295d 946a 1805 0000 6a7b 4f00 006a  .h)].j....j{O..j
+00034df0: 1905 0000 6aa1 4f00 006a 1a05 0000 6aa1  ....j.O..j....j.
+00034e00: 4f00 006a 1b05 0000 8975 682b 68ac 681c  O..j.....uh+h.h.
+00034e10: 6803 681b 6ad0 4e00 0068 1d4e 681e 4e75  h.h.j.N..h.Nh.Nu
+00034e20: 6268 7e29 8194 7d94 2868 0568 0668 075d  bh~)..}.(h.h.h.]
+00034e30: 9468 1f7d 9428 6821 5d94 6823 5d94 6825  .h.}.(h!].h#].h%
+00034e40: 5d94 6827 5d94 6829 5d94 8c07 656e 7472  ].h'].h)]...entr
+00034e50: 6965 7394 5d94 2868 a88c 2e50 5245 5041  ies.].(h...PREPA
+00034e60: 5249 4e47 2028 696e 206d 6f64 756c 6520  RING (in module 
+00034e70: 6261 6d62 756c 6162 735f 6170 692e 4763  bambulabs_api.Gc
+00034e80: 6f64 6553 7461 7465 2994 8c22 6261 6d62  odeState).."bamb
+00034e90: 756c 6162 735f 6170 692e 4763 6f64 6553  ulabs_api.GcodeS
+00034ea0: 7461 7465 2e50 5245 5041 5249 4e47 9468  tate.PREPARING.h
+00034eb0: 064e 7494 6175 682b 687d 681b 6ad0 4e00  .Nt.auh+h}h.j.N.
+00034ec0: 0068 1c68 0368 1d4e 681e 4e75 6268 ad29  .h.h.h.Nh.Nubh.)
+00034ed0: 8194 7d94 2868 0568 0668 075d 9428 68b2  ..}.(h.h.h.].(h.
+00034ee0: 2981 947d 9428 6805 8c09 5052 4550 4152  )..}.(h...PREPAR
+00034ef0: 494e 4794 6807 5d94 2868 b829 8194 7d94  ING.h.].(h.)..}.
+00034f00: 2868 058c 1962 616d 6275 6c61 6273 5f61  (h...bambulabs_a
+00034f10: 7069 2e47 636f 6465 5374 6174 652e 9468  pi.GcodeState..h
+00034f20: 075d 9468 168c 1962 616d 6275 6c61 6273  .].h...bambulabs
+00034f30: 5f61 7069 2e47 636f 6465 5374 6174 652e  _api.GcodeState.
+00034f40: 9485 9481 947d 9428 6805 6806 681b 6aba  .....}.(h.h.h.j.
+00034f50: 4f00 0068 1c68 0368 1d4e 681e 4e75 6261  O..h.h.h.Nh.Nuba
+00034f60: 681f 7d94 2868 215d 9468 235d 9428 68c4  h.}.(h!].h#].(h.
+00034f70: 68c5 6568 255d 9468 275d 9468 295d 9468  h.eh%].h'].h)].h
+00034f80: c968 ca75 682b 68b7 681b 6ab6 4f00 0068  .h.uh+h.h.j.O..h
+00034f90: 1c68 0368 1d6a 094f 0000 681e 4b10 7562  .h.h.j.O..h.K.ub
+00034fa0: 68cd 2981 947d 9428 6805 6ab8 4f00 0068  h.)..}.(h.j.O..h
+00034fb0: 075d 9468 168c 0950 5245 5041 5249 4e47  .].h...PREPARING
+00034fc0: 9485 9481 947d 9428 6805 6806 681b 6ac8  .....}.(h.h.h.j.
+00034fd0: 4f00 0068 1c68 0368 1d4e 681e 4e75 6261  O..h.h.h.Nh.Nuba
+00034fe0: 681f 7d94 2868 215d 9468 235d 9428 68d9  h.}.(h!].h#].(h.
+00034ff0: 68da 6568 255d 9468 275d 9468 295d 9468  h.eh%].h'].h)].h
+00035000: c968 ca75 682b 68cc 681b 6ab6 4f00 0068  .h.uh+h.h.j.O..h
+00035010: 1c68 0368 1d6a 094f 0000 681e 4b10 7562  .h.h.j.O..h.K.ub
+00035020: 6568 1f7d 9428 6821 5d94 6ab1 4f00 0061  eh.}.(h!].j.O..a
+00035030: 6823 5d94 286a dc02 0000 6add 0200 0065  h#].(j....j....e
+00035040: 6825 5d94 6827 5d94 6829 5d94 6ae1 0200  h%].h'].h)].j...
+00035050: 006a 4e4f 0000 6a4b 0100 0068 066a e302  .jNO..jK...h.j..
+00035060: 0000 6ab8 4f00 0075 682b 68b1 681d 6a09  ..j.O..uh+h.h.j.
+00035070: 4f00 0068 1e4b 0b68 1b6a b34f 0000 681c  O..h.K.h.j.O..h.
+00035080: 6803 7562 6ae5 0200 0029 8194 7d94 2868  h.ubj....)..}.(h
+00035090: 0568 0668 075d 946a f902 0000 2981 947d  .h.h.].j....)..}
+000350a0: 9428 6805 6806 6807 5d94 6afe 0200 0029  .(h.h.h.].j....)
+000350b0: 8194 7d94 2868 0568 0668 075d 9428 6a03  ..}.(h.h.h.].(j.
+000350c0: 0300 0029 8194 7d94 2868 058c 0474 7970  ...)..}.(h...typ
+000350d0: 6594 6807 5d94 6816 8c04 5479 7065 9485  e.h.].h...Type..
+000350e0: 9481 947d 9428 6805 6806 681b 6ae4 4f00  ...}.(h.h.h.j.O.
+000350f0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00035100: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00035110: 275d 9468 295d 9475 682b 6a02 0300 0068  '].h)].uh+j....h
+00035120: 1b6a e14f 0000 681d 6a09 4f00 0068 1e4b  .j.O..h.j.O..h.K
+00035130: 0075 626a 1303 0000 2981 947d 9428 6805  .ubj....)..}.(h.
+00035140: 8c27 5468 6520 7072 696e 7465 7220 6973  .'The printer is
+00035150: 2070 7265 7061 7269 6e67 2028 4669 6c65   preparing (File
+00035160: 2075 706c 6f61 6429 2e94 6807 5d94 6847   upload)..h.].hG
+00035170: 2981 947d 9428 6805 6af4 4f00 0068 075d  )..}.(h.j.O..h.]
+00035180: 9428 6a3a 0100 0029 8194 7d94 2868 0568  .(j:...)..}.(h.h
+00035190: 0668 075d 9468 168c 1854 6865 2070 7269  .h.].h...The pri
+000351a0: 6e74 6572 2069 7320 7072 6570 6172 696e  nter is preparin
+000351b0: 6794 8594 8194 7d94 2868 0568 0668 1b6a  g.....}.(h.h.h.j
+000351c0: f94f 0000 681c 6803 681d 4e68 1e4e 7562  .O..h.h.h.Nh.Nub
+000351d0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000351e0: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
+000351f0: 6f6d 6169 6e94 8c02 7079 948c 0b72 6566  omain...py...ref
+00035200: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+00035210: 7970 6594 6a4b 0100 008c 0972 6566 7461  ype.jK.....refta
+00035220: 7267 6574 948c 1854 6865 2070 7269 6e74  rget...The print
+00035230: 6572 2069 7320 7072 6570 6172 696e 6794  er is preparing.
+00035240: 6a57 0300 0088 6a58 0300 006a 4e4f 0000  jW....jX...jNO..
+00035250: 6a59 0300 004e 7568 2b6a 3901 0000 681b  jY...Nuh+j9...h.
+00035260: 6af6 4f00 0068 1c68 0368 1d4e 681e 4e75  j.O..h.h.h.Nh.Nu
+00035270: 6268 168c 0220 2894 8594 8194 7d94 2868  bh... (.....}.(h
+00035280: 0568 0668 1b6a f64f 0000 681c 6803 681d  .h.h.j.O..h.h.h.
+00035290: 4e68 1e4e 7562 6a3a 0100 0029 8194 7d94  Nh.Nubj:...)..}.
+000352a0: 2868 0568 0668 075d 9468 168c 0b46 696c  (h.h.h.].h...Fil
+000352b0: 6520 7570 6c6f 6164 9485 9481 947d 9428  e upload.....}.(
+000352c0: 6805 6806 681b 6a10 5000 0068 1c68 0368  h.h.h.j.P..h.h.h
+000352d0: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+000352e0: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+000352f0: 948c 0972 6566 646f 6d61 696e 946a 0750  ...refdomain.j.P
+00035300: 0000 8c0b 7265 6665 7870 6c69 6369 7494  ....refexplicit.
+00035310: 898c 0772 6566 7479 7065 946a 4b01 0000  ...reftype.jK...
+00035320: 8c09 7265 6674 6172 6765 7494 8c0b 4669  ..reftarget...Fi
+00035330: 6c65 2075 706c 6f61 6494 6a57 0300 0088  le upload.jW....
+00035340: 6a58 0300 006a 4e4f 0000 6a59 0300 004e  jX...jNO..jY...N
+00035350: 7568 2b6a 3901 0000 681b 6af6 4f00 0068  uh+j9...h.j.O..h
+00035360: 1c68 0368 1d4e 681e 4e75 6268 168c 0129  .h.h.Nh.Nubh...)
+00035370: 9485 9481 947d 9428 6805 6806 681b 6af6  .....}.(h.h.h.j.
+00035380: 4f00 0068 1c68 0368 1d4e 681e 4e75 626a  O..h.h.h.Nh.Nubj
+00035390: 3a01 0000 2981 947d 9428 6805 6806 6807  :...)..}.(h.h.h.
+000353a0: 5d94 6816 8c01 2e94 8594 8194 7d94 2868  ].h.........}.(h
+000353b0: 0568 0668 1b6a 2650 0000 681c 6803 681d  .h.h.j&P..h.h.h.
+000353c0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+000353d0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000353e0: 8c09 7265 6664 6f6d 6169 6e94 6a07 5000  ..refdomain.j.P.
+000353f0: 008c 0b72 6566 6578 706c 6963 6974 9489  ...refexplicit..
+00035400: 8c07 7265 6674 7970 6594 6a4b 0100 008c  ..reftype.jK....
+00035410: 0972 6566 7461 7267 6574 948c 012e 946a  .reftarget.....j
+00035420: 5703 0000 886a 5803 0000 6a4e 4f00 006a  W....jX...jNO..j
+00035430: 5903 0000 4e75 682b 6a39 0100 0068 1b6a  Y...Nuh+j9...h.j
+00035440: f64f 0000 681c 6803 681d 4e68 1e4e 7562  .O..h.h.h.Nh.Nub
+00035450: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+00035460: 5d94 6827 5d94 6829 5d94 7568 2b68 4668  ].h'].h)].uh+hFh
+00035470: 1d6a 094f 0000 681e 4b0f 681b 6af2 4f00  .j.O..h.K.h.j.O.
+00035480: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+00035490: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+000354a0: 6a12 0300 0068 1b6a e14f 0000 7562 6568  j....h.j.O..ubeh
+000354b0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+000354c0: 6827 5d94 6829 5d94 7568 2b6a fd02 0000  h'].h)].uh+j....
+000354d0: 681d 6a09 4f00 0068 1e4b 0f68 1b6a de4f  h.j.O..h.K.h.j.O
+000354e0: 0000 681c 6803 7562 6168 1f7d 9428 6821  ..h.h.ubah.}.(h!
+000354f0: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00035500: 5d94 7568 2b6a f802 0000 681b 6adb 4f00  ].uh+j....h.j.O.
+00035510: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+00035520: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00035530: 275d 9468 295d 9475 682b 6ae4 0200 0068  '].h)].uh+j....h
+00035540: 1b6a b34f 0000 681c 6803 681d 6a09 4f00  .j.O..h.h.h.j.O.
+00035550: 0068 1e4b 1075 6265 681f 7d94 2868 215d  .h.K.ubeh.}.(h!]
+00035560: 9468 235d 9428 6a07 5000 008c 0961 7474  .h#].(j.P....att
+00035570: 7269 6275 7465 9465 6825 5d94 6827 5d94  ribute.eh%].h'].
+00035580: 6829 5d94 6a18 0500 006a 0750 0000 6a19  h)].j....j.P..j.
+00035590: 0500 006a 5950 0000 6a1a 0500 006a 5950  ...jYP..j....jYP
+000355a0: 0000 6a1b 0500 0089 7568 2b68 ac68 1c68  ..j.....uh+h.h.h
+000355b0: 0368 1b6a d04e 0000 681d 4e68 1e4e 7562  .h.j.N..h.Nh.Nub
+000355c0: 687e 2981 947d 9428 6805 6806 6807 5d94  h~)..}.(h.h.h.].
+000355d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000355e0: 9468 275d 9468 295d 948c 0765 6e74 7269  .h'].h)]...entri
+000355f0: 6573 945d 9428 68a8 8c2c 5255 4e4e 494e  es.].(h..,RUNNIN
+00035600: 4720 2869 6e20 6d6f 6475 6c65 2062 616d  G (in module bam
+00035610: 6275 6c61 6273 5f61 7069 2e47 636f 6465  bulabs_api.Gcode
+00035620: 5374 6174 6529 948c 2062 616d 6275 6c61  State).. bambula
+00035630: 6273 5f61 7069 2e47 636f 6465 5374 6174  bs_api.GcodeStat
+00035640: 652e 5255 4e4e 494e 4794 6806 4e74 9461  e.RUNNING.h.Nt.a
+00035650: 7568 2b68 7d68 1b6a d04e 0000 681c 6803  uh+h}h.j.N..h.h.
+00035660: 681d 4e68 1e4e 7562 68ad 2981 947d 9428  h.Nh.Nubh.)..}.(
+00035670: 6805 6806 6807 5d94 2868 b229 8194 7d94  h.h.h.].(h.)..}.
+00035680: 2868 058c 0752 554e 4e49 4e47 9468 075d  (h...RUNNING.h.]
+00035690: 9428 68b8 2981 947d 9428 6805 8c19 6261  .(h.)..}.(h...ba
+000356a0: 6d62 756c 6162 735f 6170 692e 4763 6f64  mbulabs_api.Gcod
+000356b0: 6553 7461 7465 2e94 6807 5d94 6816 8c19  eState..h.].h...
+000356c0: 6261 6d62 756c 6162 735f 6170 692e 4763  bambulabs_api.Gc
+000356d0: 6f64 6553 7461 7465 2e94 8594 8194 7d94  odeState......}.
+000356e0: 2868 0568 0668 1b6a 7250 0000 681c 6803  (h.h.h.jrP..h.h.
+000356f0: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00035700: 5d94 6823 5d94 2868 c468 c565 6825 5d94  ].h#].(h.h.eh%].
+00035710: 6827 5d94 6829 5d94 68c9 68ca 7568 2b68  h'].h)].h.h.uh+h
+00035720: b768 1b6a 6e50 0000 681c 6803 681d 6a09  .h.jnP..h.h.h.j.
+00035730: 4f00 0068 1e4b 1675 6268 cd29 8194 7d94  O..h.K.ubh.)..}.
+00035740: 2868 056a 7050 0000 6807 5d94 6816 8c07  (h.jpP..h.].h...
+00035750: 5255 4e4e 494e 4794 8594 8194 7d94 2868  RUNNING.....}.(h
+00035760: 0568 0668 1b6a 8050 0000 681c 6803 681d  .h.h.j.P..h.h.h.
+00035770: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00035780: 6823 5d94 2868 d968 da65 6825 5d94 6827  h#].(h.h.eh%].h'
+00035790: 5d94 6829 5d94 68c9 68ca 7568 2b68 cc68  ].h)].h.h.uh+h.h
+000357a0: 1b6a 6e50 0000 681c 6803 681d 6a09 4f00  .jnP..h.h.h.j.O.
+000357b0: 0068 1e4b 1675 6265 681f 7d94 2868 215d  .h.K.ubeh.}.(h!]
+000357c0: 946a 6950 0000 6168 235d 9428 6adc 0200  .jiP..ah#].(j...
+000357d0: 006a dd02 0000 6568 255d 9468 275d 9468  .j....eh%].h'].h
+000357e0: 295d 946a e102 0000 6a4e 4f00 006a 4b01  )].j....jNO..jK.
+000357f0: 0000 6806 6ae3 0200 006a 7050 0000 7568  ..h.j....jpP..uh
+00035800: 2b68 b168 1d6a 094f 0000 681e 4b11 681b  +h.h.j.O..h.K.h.
+00035810: 6a6b 5000 0068 1c68 0375 626a e502 0000  jkP..h.h.ubj....
+00035820: 2981 947d 9428 6805 6806 6807 5d94 6af9  )..}.(h.h.h.].j.
+00035830: 0200 0029 8194 7d94 2868 0568 0668 075d  ...)..}.(h.h.h.]
+00035840: 946a fe02 0000 2981 947d 9428 6805 6806  .j....)..}.(h.h.
+00035850: 6807 5d94 286a 0303 0000 2981 947d 9428  h.].(j....)..}.(
+00035860: 6805 8c04 7479 7065 9468 075d 9468 168c  h...type.h.].h..
+00035870: 0454 7970 6594 8594 8194 7d94 2868 0568  .Type.....}.(h.h
+00035880: 0668 1b6a 9c50 0000 681c 6803 681d 4e68  .h.j.P..h.h.h.Nh
+00035890: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+000358a0: 5d94 6825 5d94 6827 5d94 6829 5d94 7568  ].h%].h'].h)].uh
+000358b0: 2b6a 0203 0000 681b 6a99 5000 0068 1d6a  +j....h.j.P..h.j
+000358c0: 094f 0000 681e 4b00 7562 6a13 0300 0029  .O..h.K.ubj....)
+000358d0: 8194 7d94 2868 058c 1754 6865 2070 7269  ..}.(h...The pri
+000358e0: 6e74 6572 2069 7320 7275 6e6e 696e 672e  nter is running.
+000358f0: 9468 075d 9468 4729 8194 7d94 2868 056a  .h.].hG)..}.(h.j
+00035900: ac50 0000 6807 5d94 6a3a 0100 0029 8194  .P..h.].j:...)..
+00035910: 7d94 2868 0568 0668 075d 9468 168c 1754  }.(h.h.h.].h...T
+00035920: 6865 2070 7269 6e74 6572 2069 7320 7275  he printer is ru
+00035930: 6e6e 696e 672e 9485 9481 947d 9428 6805  nning......}.(h.
+00035940: 6806 681b 6ab1 5000 0068 1c68 0368 1d4e  h.h.j.P..h.h.h.N
+00035950: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00035960: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00035970: 0972 6566 646f 6d61 696e 948c 0270 7994  .refdomain...py.
+00035980: 8c0b 7265 6665 7870 6c69 6369 7494 898c  ..refexplicit...
+00035990: 0772 6566 7479 7065 946a 4b01 0000 8c09  .reftype.jK.....
+000359a0: 7265 6674 6172 6765 7494 8c17 5468 6520  reftarget...The 
+000359b0: 7072 696e 7465 7220 6973 2072 756e 6e69  printer is runni
+000359c0: 6e67 2e94 6a57 0300 0088 6a58 0300 006a  ng..jW....jX...j
+000359d0: 4e4f 0000 6a59 0300 004e 7568 2b6a 3901  NO..jY...Nuh+j9.
+000359e0: 0000 681b 6aae 5000 0068 1c68 0368 1d4e  ..h.j.P..h.h.h.N
+000359f0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00035a00: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00035a10: 682b 6846 681d 6a09 4f00 0068 1e4b 1568  h+hFh.j.O..h.K.h
+00035a20: 1b6a aa50 0000 7562 6168 1f7d 9428 6821  .j.P..ubah.}.(h!
+00035a30: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00035a40: 5d94 7568 2b6a 1203 0000 681b 6a99 5000  ].uh+j....h.j.P.
+00035a50: 0075 6265 681f 7d94 2868 215d 9468 235d  .ubeh.}.(h!].h#]
+00035a60: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00035a70: 6afd 0200 0068 1d6a 094f 0000 681e 4b15  j....h.j.O..h.K.
+00035a80: 681b 6a96 5000 0068 1c68 0375 6261 681f  h.j.P..h.h.ubah.
+00035a90: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00035aa0: 275d 9468 295d 9475 682b 6af8 0200 0068  '].h)].uh+j....h
+00035ab0: 1b6a 9350 0000 681c 6803 681d 4e68 1e4e  .j.P..h.h.h.Nh.N
+00035ac0: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00035ad0: 6825 5d94 6827 5d94 6829 5d94 7568 2b6a  h%].h'].h)].uh+j
+00035ae0: e402 0000 681b 6a6b 5000 0068 1c68 0368  ....h.jkP..h.h.h
+00035af0: 1d6a 094f 0000 681e 4b16 7562 6568 1f7d  .j.O..h.K.ubeh.}
+00035b00: 9428 6821 5d94 6823 5d94 286a bf50 0000  .(h!].h#].(j.P..
+00035b10: 8c09 6174 7472 6962 7574 6594 6568 255d  ..attribute.eh%]
+00035b20: 9468 275d 9468 295d 946a 1805 0000 6abf  .h'].h)].j....j.
+00035b30: 5000 006a 1905 0000 6ae5 5000 006a 1a05  P..j....j.P..j..
+00035b40: 0000 6ae5 5000 006a 1b05 0000 8975 682b  ..j.P..j.....uh+
+00035b50: 68ac 681c 6803 681b 6ad0 4e00 0068 1d4e  h.h.h.h.j.N..h.N
+00035b60: 681e 4e75 6268 7e29 8194 7d94 2868 0568  h.Nubh~)..}.(h.h
+00035b70: 0668 075d 9468 1f7d 9428 6821 5d94 6823  .h.].h.}.(h!].h#
+00035b80: 5d94 6825 5d94 6827 5d94 6829 5d94 8c07  ].h%].h'].h)]...
+00035b90: 656e 7472 6965 7394 5d94 2868 a88c 2b50  entries.].(h..+P
+00035ba0: 4155 5345 4420 2869 6e20 6d6f 6475 6c65  AUSED (in module
+00035bb0: 2062 616d 6275 6c61 6273 5f61 7069 2e47   bambulabs_api.G
+00035bc0: 636f 6465 5374 6174 6529 948c 1f62 616d  codeState)...bam
+00035bd0: 6275 6c61 6273 5f61 7069 2e47 636f 6465  bulabs_api.Gcode
+00035be0: 5374 6174 652e 5041 5553 4544 9468 064e  State.PAUSED.h.N
+00035bf0: 7494 6175 682b 687d 681b 6ad0 4e00 0068  t.auh+h}h.j.N..h
+00035c00: 1c68 0368 1d4e 681e 4e75 6268 ad29 8194  .h.h.Nh.Nubh.)..
+00035c10: 7d94 2868 0568 0668 075d 9428 68b2 2981  }.(h.h.h.].(h.).
+00035c20: 947d 9428 6805 8c06 5041 5553 4544 9468  .}.(h...PAUSED.h
+00035c30: 075d 9428 68b8 2981 947d 9428 6805 8c19  .].(h.)..}.(h...
+00035c40: 6261 6d62 756c 6162 735f 6170 692e 4763  bambulabs_api.Gc
+00035c50: 6f64 6553 7461 7465 2e94 6807 5d94 6816  odeState..h.].h.
+00035c60: 8c19 6261 6d62 756c 6162 735f 6170 692e  ..bambulabs_api.
+00035c70: 4763 6f64 6553 7461 7465 2e94 8594 8194  GcodeState......
+00035c80: 7d94 2868 0568 0668 1b6a fe50 0000 681c  }.(h.h.h.j.P..h.
+00035c90: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00035ca0: 6821 5d94 6823 5d94 2868 c468 c565 6825  h!].h#].(h.h.eh%
+00035cb0: 5d94 6827 5d94 6829 5d94 68c9 68ca 7568  ].h'].h)].h.h.uh
+00035cc0: 2b68 b768 1b6a fa50 0000 681c 6803 681d  +h.h.j.P..h.h.h.
+00035cd0: 6a09 4f00 0068 1e4b 1c75 6268 cd29 8194  j.O..h.K.ubh.)..
+00035ce0: 7d94 2868 056a fc50 0000 6807 5d94 6816  }.(h.j.P..h.].h.
+00035cf0: 8c06 5041 5553 4544 9485 9481 947d 9428  ..PAUSED.....}.(
+00035d00: 6805 6806 681b 6a0c 5100 0068 1c68 0368  h.h.h.j.Q..h.h.h
+00035d10: 1d4e 681e 4e75 6261 681f 7d94 2868 215d  .Nh.Nubah.}.(h!]
+00035d20: 9468 235d 9428 68d9 68da 6568 255d 9468  .h#].(h.h.eh%].h
+00035d30: 275d 9468 295d 9468 c968 ca75 682b 68cc  '].h)].h.h.uh+h.
+00035d40: 681b 6afa 5000 0068 1c68 0368 1d6a 094f  h.j.P..h.h.h.j.O
+00035d50: 0000 681e 4b1c 7562 6568 1f7d 9428 6821  ..h.K.ubeh.}.(h!
+00035d60: 5d94 6af5 5000 0061 6823 5d94 286a dc02  ].j.P..ah#].(j..
+00035d70: 0000 6add 0200 0065 6825 5d94 6827 5d94  ..j....eh%].h'].
+00035d80: 6829 5d94 6ae1 0200 006a 4e4f 0000 6a4b  h)].j....jNO..jK
+00035d90: 0100 0068 066a e302 0000 6afc 5000 0075  ...h.j....j.P..u
+00035da0: 682b 68b1 681d 6a09 4f00 0068 1e4b 1768  h+h.h.j.O..h.K.h
+00035db0: 1b6a f750 0000 681c 6803 7562 6ae5 0200  .j.P..h.h.ubj...
+00035dc0: 0029 8194 7d94 2868 0568 0668 075d 946a  .)..}.(h.h.h.].j
+00035dd0: f902 0000 2981 947d 9428 6805 6806 6807  ....)..}.(h.h.h.
+00035de0: 5d94 6afe 0200 0029 8194 7d94 2868 0568  ].j....)..}.(h.h
+00035df0: 0668 075d 9428 6a03 0300 0029 8194 7d94  .h.].(j....)..}.
+00035e00: 2868 058c 0474 7970 6594 6807 5d94 6816  (h...type.h.].h.
+00035e10: 8c04 5479 7065 9485 9481 947d 9428 6805  ..Type.....}.(h.
+00035e20: 6806 681b 6a28 5100 0068 1c68 0368 1d4e  h.h.j(Q..h.h.h.N
+00035e30: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+00035e40: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00035e50: 682b 6a02 0300 0068 1b6a 2551 0000 681d  h+j....h.j%Q..h.
+00035e60: 6a09 4f00 0068 1e4b 0075 626a 1303 0000  j.O..h.K.ubj....
+00035e70: 2981 947d 9428 6805 8c16 5468 6520 7072  )..}.(h...The pr
+00035e80: 696e 7465 7220 6973 2070 6175 7365 642e  inter is paused.
+00035e90: 9468 075d 9468 4729 8194 7d94 2868 056a  .h.].hG)..}.(h.j
+00035ea0: 3851 0000 6807 5d94 6a3a 0100 0029 8194  8Q..h.].j:...)..
+00035eb0: 7d94 2868 0568 0668 075d 9468 168c 1654  }.(h.h.h.].h...T
+00035ec0: 6865 2070 7269 6e74 6572 2069 7320 7061  he printer is pa
+00035ed0: 7573 6564 2e94 8594 8194 7d94 2868 0568  used......}.(h.h
+00035ee0: 0668 1b6a 3d51 0000 681c 6803 681d 4e68  .h.j=Q..h.h.h.Nh
+00035ef0: 1e4e 7562 6168 1f7d 9428 6821 5d94 6823  .Nubah.}.(h!].h#
+00035f00: 5d94 6825 5d94 6827 5d94 6829 5d94 8c09  ].h%].h'].h)]...
+00035f10: 7265 6664 6f6d 6169 6e94 8c02 7079 948c  refdomain...py..
+00035f20: 0b72 6566 6578 706c 6963 6974 9489 8c07  .refexplicit....
+00035f30: 7265 6674 7970 6594 6a4b 0100 008c 0972  reftype.jK.....r
+00035f40: 6566 7461 7267 6574 948c 1654 6865 2070  eftarget...The p
+00035f50: 7269 6e74 6572 2069 7320 7061 7573 6564  rinter is paused
+00035f60: 2e94 6a57 0300 0088 6a58 0300 006a 4e4f  ..jW....jX...jNO
+00035f70: 0000 6a59 0300 004e 7568 2b6a 3901 0000  ..jY...Nuh+j9...
+00035f80: 681b 6a3a 5100 0068 1c68 0368 1d4e 681e  h.j:Q..h.h.h.Nh.
+00035f90: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00035fa0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00035fb0: 6846 681d 6a09 4f00 0068 1e4b 1b68 1b6a  hFh.j.O..h.K.h.j
+00035fc0: 3651 0000 7562 6168 1f7d 9428 6821 5d94  6Q..ubah.}.(h!].
+00035fd0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00035fe0: 7568 2b6a 1203 0000 681b 6a25 5100 0075  uh+j....h.j%Q..u
+00035ff0: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00036000: 255d 9468 275d 9468 295d 9475 682b 6afd  %].h'].h)].uh+j.
+00036010: 0200 0068 1d6a 094f 0000 681e 4b1b 681b  ...h.j.O..h.K.h.
+00036020: 6a22 5100 0068 1c68 0375 6261 681f 7d94  j"Q..h.h.ubah.}.
+00036030: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00036040: 9468 295d 9475 682b 6af8 0200 0068 1b6a  .h)].uh+j....h.j
+00036050: 1f51 0000 681c 6803 681d 4e68 1e4e 7562  .Q..h.h.h.Nh.Nub
+00036060: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00036070: 5d94 6827 5d94 6829 5d94 7568 2b6a e402  ].h'].h)].uh+j..
+00036080: 0000 681b 6af7 5000 0068 1c68 0368 1d6a  ..h.j.P..h.h.h.j
+00036090: 094f 0000 681e 4b1c 7562 6568 1f7d 9428  .O..h.K.ubeh.}.(
+000360a0: 6821 5d94 6823 5d94 286a 4b51 0000 8c09  h!].h#].(jKQ....
+000360b0: 6174 7472 6962 7574 6594 6568 255d 9468  attribute.eh%].h
+000360c0: 275d 9468 295d 946a 1805 0000 6a4b 5100  '].h)].j....jKQ.
+000360d0: 006a 1905 0000 6a71 5100 006a 1a05 0000  .j....jqQ..j....
+000360e0: 6a71 5100 006a 1b05 0000 8975 682b 68ac  jqQ..j.....uh+h.
+000360f0: 681c 6803 681b 6ad0 4e00 0068 1d4e 681e  h.h.h.j.N..h.Nh.
+00036100: 4e75 6268 7e29 8194 7d94 2868 0568 0668  Nubh~)..}.(h.h.h
+00036110: 075d 9468 1f7d 9428 6821 5d94 6823 5d94  .].h.}.(h!].h#].
+00036120: 6825 5d94 6827 5d94 6829 5d94 8c07 656e  h%].h'].h)]...en
+00036130: 7472 6965 7394 5d94 2868 a88c 2d46 494e  tries.].(h..-FIN
+00036140: 4953 4845 4420 2869 6e20 6d6f 6475 6c65  ISHED (in module
+00036150: 2062 616d 6275 6c61 6273 5f61 7069 2e47   bambulabs_api.G
+00036160: 636f 6465 5374 6174 6529 948c 2162 616d  codeState)..!bam
+00036170: 6275 6c61 6273 5f61 7069 2e47 636f 6465  bulabs_api.Gcode
+00036180: 5374 6174 652e 4649 4e49 5348 4544 9468  State.FINISHED.h
+00036190: 064e 7494 6175 682b 687d 681b 6ad0 4e00  .Nt.auh+h}h.j.N.
+000361a0: 0068 1c68 0368 1d4e 681e 4e75 6268 ad29  .h.h.h.Nh.Nubh.)
+000361b0: 8194 7d94 2868 0568 0668 075d 9428 68b2  ..}.(h.h.h.].(h.
+000361c0: 2981 947d 9428 6805 8c08 4649 4e49 5348  )..}.(h...FINISH
+000361d0: 4544 9468 075d 9428 68b8 2981 947d 9428  ED.h.].(h.)..}.(
+000361e0: 6805 8c19 6261 6d62 756c 6162 735f 6170  h...bambulabs_ap
+000361f0: 692e 4763 6f64 6553 7461 7465 2e94 6807  i.GcodeState..h.
+00036200: 5d94 6816 8c19 6261 6d62 756c 6162 735f  ].h...bambulabs_
+00036210: 6170 692e 4763 6f64 6553 7461 7465 2e94  api.GcodeState..
+00036220: 8594 8194 7d94 2868 0568 0668 1b6a 8a51  ....}.(h.h.h.j.Q
+00036230: 0000 681c 6803 681d 4e68 1e4e 7562 6168  ..h.h.h.Nh.Nubah
+00036240: 1f7d 9428 6821 5d94 6823 5d94 2868 c468  .}.(h!].h#].(h.h
+00036250: c565 6825 5d94 6827 5d94 6829 5d94 68c9  .eh%].h'].h)].h.
+00036260: 68ca 7568 2b68 b768 1b6a 8651 0000 681c  h.uh+h.h.j.Q..h.
+00036270: 6803 681d 6a09 4f00 0068 1e4b 2275 6268  h.h.j.O..h.K"ubh
+00036280: cd29 8194 7d94 2868 056a 8851 0000 6807  .)..}.(h.j.Q..h.
+00036290: 5d94 6816 8c08 4649 4e49 5348 4544 9485  ].h...FINISHED..
+000362a0: 9481 947d 9428 6805 6806 681b 6a98 5100  ...}.(h.h.h.j.Q.
+000362b0: 0068 1c68 0368 1d4e 681e 4e75 6261 681f  .h.h.h.Nh.Nubah.
+000362c0: 7d94 2868 215d 9468 235d 9428 68d9 68da  }.(h!].h#].(h.h.
+000362d0: 6568 255d 9468 275d 9468 295d 9468 c968  eh%].h'].h)].h.h
+000362e0: ca75 682b 68cc 681b 6a86 5100 0068 1c68  .uh+h.h.j.Q..h.h
+000362f0: 0368 1d6a 094f 0000 681e 4b22 7562 6568  .h.j.O..h.K"ubeh
+00036300: 1f7d 9428 6821 5d94 6a81 5100 0061 6823  .}.(h!].j.Q..ah#
+00036310: 5d94 286a dc02 0000 6add 0200 0065 6825  ].(j....j....eh%
+00036320: 5d94 6827 5d94 6829 5d94 6ae1 0200 006a  ].h'].h)].j....j
+00036330: 4e4f 0000 6a4b 0100 0068 066a e302 0000  NO..jK...h.j....
+00036340: 6a88 5100 0075 682b 68b1 681d 6a09 4f00  j.Q..uh+h.h.j.O.
+00036350: 0068 1e4b 1d68 1b6a 8351 0000 681c 6803  .h.K.h.j.Q..h.h.
+00036360: 7562 6ae5 0200 0029 8194 7d94 2868 0568  ubj....)..}.(h.h
+00036370: 0668 075d 946a f902 0000 2981 947d 9428  .h.].j....)..}.(
+00036380: 6805 6806 6807 5d94 6afe 0200 0029 8194  h.h.h.].j....)..
+00036390: 7d94 2868 0568 0668 075d 9428 6a03 0300  }.(h.h.h.].(j...
+000363a0: 0029 8194 7d94 2868 058c 0474 7970 6594  .)..}.(h...type.
+000363b0: 6807 5d94 6816 8c04 5479 7065 9485 9481  h.].h...Type....
+000363c0: 947d 9428 6805 6806 681b 6ab4 5100 0068  .}.(h.h.h.j.Q..h
+000363d0: 1c68 0368 1d4e 681e 4e75 6261 681f 7d94  .h.h.Nh.Nubah.}.
+000363e0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000363f0: 9468 295d 9475 682b 6a02 0300 0068 1b6a  .h)].uh+j....h.j
+00036400: b151 0000 681d 6a09 4f00 0068 1e4b 0075  .Q..h.j.O..h.K.u
+00036410: 626a 1303 0000 2981 947d 9428 6805 8c19  bj....)..}.(h...
+00036420: 5468 6520 7072 696e 7465 7220 6861 7320  The printer has 
+00036430: 6669 6e69 7368 6564 2e94 6807 5d94 6847  finished..h.].hG
+00036440: 2981 947d 9428 6805 6ac4 5100 0068 075d  )..}.(h.j.Q..h.]
+00036450: 946a 3a01 0000 2981 947d 9428 6805 6806  .j:...)..}.(h.h.
+00036460: 6807 5d94 6816 8c19 5468 6520 7072 696e  h.].h...The prin
+00036470: 7465 7220 6861 7320 6669 6e69 7368 6564  ter has finished
+00036480: 2e94 8594 8194 7d94 2868 0568 0668 1b6a  ......}.(h.h.h.j
+00036490: c951 0000 681c 6803 681d 4e68 1e4e 7562  .Q..h.h.h.Nh.Nub
+000364a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000364b0: 5d94 6827 5d94 6829 5d94 8c09 7265 6664  ].h'].h)]...refd
+000364c0: 6f6d 6169 6e94 8c02 7079 948c 0b72 6566  omain...py...ref
+000364d0: 6578 706c 6963 6974 9489 8c07 7265 6674  explicit....reft
+000364e0: 7970 6594 6a4b 0100 008c 0972 6566 7461  ype.jK.....refta
+000364f0: 7267 6574 948c 1954 6865 2070 7269 6e74  rget...The print
+00036500: 6572 2068 6173 2066 696e 6973 6865 642e  er has finished.
+00036510: 946a 5703 0000 886a 5803 0000 6a4e 4f00  .jW....jX...jNO.
+00036520: 006a 5903 0000 4e75 682b 6a39 0100 0068  .jY...Nuh+j9...h
+00036530: 1b6a c651 0000 681c 6803 681d 4e68 1e4e  .j.Q..h.h.h.Nh.N
+00036540: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00036550: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00036560: 4668 1d6a 094f 0000 681e 4b21 681b 6ac2  Fh.j.O..h.K!h.j.
+00036570: 5100 0075 6261 681f 7d94 2868 215d 9468  Q..ubah.}.(h!].h
+00036580: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00036590: 682b 6a12 0300 0068 1b6a b151 0000 7562  h+j....h.j.Q..ub
+000365a0: 6568 1f7d 9428 6821 5d94 6823 5d94 6825  eh.}.(h!].h#].h%
+000365b0: 5d94 6827 5d94 6829 5d94 7568 2b6a fd02  ].h'].h)].uh+j..
+000365c0: 0000 681d 6a09 4f00 0068 1e4b 2168 1b6a  ..h.j.O..h.K!h.j
+000365d0: ae51 0000 681c 6803 7562 6168 1f7d 9428  .Q..h.h.ubah.}.(
+000365e0: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+000365f0: 6829 5d94 7568 2b6a f802 0000 681b 6aab  h)].uh+j....h.j.
+00036600: 5100 0068 1c68 0368 1d4e 681e 4e75 6261  Q..h.h.h.Nh.Nuba
+00036610: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00036620: 9468 275d 9468 295d 9475 682b 6ae4 0200  .h'].h)].uh+j...
+00036630: 0068 1b6a 8351 0000 681c 6803 681d 6a09  .h.j.Q..h.h.h.j.
+00036640: 4f00 0068 1e4b 2275 6265 681f 7d94 2868  O..h.K"ubeh.}.(h
+00036650: 215d 9468 235d 9428 6ad7 5100 008c 0961  !].h#].(j.Q....a
+00036660: 7474 7269 6275 7465 9465 6825 5d94 6827  ttribute.eh%].h'
+00036670: 5d94 6829 5d94 6a18 0500 006a d751 0000  ].h)].j....j.Q..
+00036680: 6a19 0500 006a fd51 0000 6a1a 0500 006a  j....j.Q..j....j
+00036690: fd51 0000 6a1b 0500 0089 7568 2b68 ac68  .Q..j.....uh+h.h
+000366a0: 1c68 0368 1b6a d04e 0000 681d 4e68 1e4e  .h.h.j.N..h.Nh.N
+000366b0: 7562 687e 2981 947d 9428 6805 6806 6807  ubh~)..}.(h.h.h.
+000366c0: 5d94 681f 7d94 2868 215d 9468 235d 9468  ].h.}.(h!].h#].h
+000366d0: 255d 9468 275d 9468 295d 948c 0765 6e74  %].h'].h)]...ent
+000366e0: 7269 6573 945d 9428 68a8 8c2c 554e 4b4e  ries.].(h..,UNKN
+000366f0: 4f57 4e20 2869 6e20 6d6f 6475 6c65 2062  OWN (in module b
+00036700: 616d 6275 6c61 6273 5f61 7069 2e47 636f  ambulabs_api.Gco
+00036710: 6465 5374 6174 6529 948c 2062 616d 6275  deState).. bambu
+00036720: 6c61 6273 5f61 7069 2e47 636f 6465 5374  labs_api.GcodeSt
+00036730: 6174 652e 554e 4b4e 4f57 4e94 6806 4e74  ate.UNKNOWN.h.Nt
+00036740: 9461 7568 2b68 7d68 1b6a d04e 0000 681c  .auh+h}h.j.N..h.
+00036750: 6803 681d 4e68 1e4e 7562 68ad 2981 947d  h.h.Nh.Nubh.)..}
+00036760: 9428 6805 6806 6807 5d94 2868 b229 8194  .(h.h.h.].(h.)..
+00036770: 7d94 2868 058c 0755 4e4b 4e4f 574e 9468  }.(h...UNKNOWN.h
+00036780: 075d 9428 68b8 2981 947d 9428 6805 8c19  .].(h.)..}.(h...
+00036790: 6261 6d62 756c 6162 735f 6170 692e 4763  bambulabs_api.Gc
+000367a0: 6f64 6553 7461 7465 2e94 6807 5d94 6816  odeState..h.].h.
+000367b0: 8c19 6261 6d62 756c 6162 735f 6170 692e  ..bambulabs_api.
+000367c0: 4763 6f64 6553 7461 7465 2e94 8594 8194  GcodeState......
+000367d0: 7d94 2868 0568 0668 1b6a 1652 0000 681c  }.(h.h.h.j.R..h.
+000367e0: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+000367f0: 6821 5d94 6823 5d94 2868 c468 c565 6825  h!].h#].(h.h.eh%
+00036800: 5d94 6827 5d94 6829 5d94 68c9 68ca 7568  ].h'].h)].h.h.uh
+00036810: 2b68 b768 1b6a 1252 0000 681c 6803 681d  +h.h.j.R..h.h.h.
+00036820: 6a09 4f00 0068 1e4b 2875 6268 cd29 8194  j.O..h.K(ubh.)..
+00036830: 7d94 2868 056a 1452 0000 6807 5d94 6816  }.(h.j.R..h.].h.
+00036840: 8c07 554e 4b4e 4f57 4e94 8594 8194 7d94  ..UNKNOWN.....}.
+00036850: 2868 0568 0668 1b6a 2452 0000 681c 6803  (h.h.h.j$R..h.h.
+00036860: 681d 4e68 1e4e 7562 6168 1f7d 9428 6821  h.Nh.Nubah.}.(h!
+00036870: 5d94 6823 5d94 2868 d968 da65 6825 5d94  ].h#].(h.h.eh%].
+00036880: 6827 5d94 6829 5d94 68c9 68ca 7568 2b68  h'].h)].h.h.uh+h
+00036890: cc68 1b6a 1252 0000 681c 6803 681d 6a09  .h.j.R..h.h.h.j.
+000368a0: 4f00 0068 1e4b 2875 6265 681f 7d94 2868  O..h.K(ubeh.}.(h
+000368b0: 215d 946a 0d52 0000 6168 235d 9428 6adc  !].j.R..ah#].(j.
+000368c0: 0200 006a dd02 0000 6568 255d 9468 275d  ...j....eh%].h']
+000368d0: 9468 295d 946a e102 0000 6a4e 4f00 006a  .h)].j....jNO..j
+000368e0: 4b01 0000 6806 6ae3 0200 006a 1452 0000  K...h.j....j.R..
+000368f0: 7568 2b68 b168 1d6a 094f 0000 681e 4b23  uh+h.h.j.O..h.K#
+00036900: 681b 6a0f 5200 0068 1c68 0375 626a e502  h.j.R..h.h.ubj..
+00036910: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00036920: 6af9 0200 0029 8194 7d94 2868 0568 0668  j....)..}.(h.h.h
+00036930: 075d 946a fe02 0000 2981 947d 9428 6805  .].j....)..}.(h.
+00036940: 6806 6807 5d94 286a 0303 0000 2981 947d  h.h.].(j....)..}
+00036950: 9428 6805 8c04 7479 7065 9468 075d 9468  .(h...type.h.].h
+00036960: 168c 0454 7970 6594 8594 8194 7d94 2868  ...Type.....}.(h
+00036970: 0568 0668 1b6a 4052 0000 681c 6803 681d  .h.h.j@R..h.h.h.
+00036980: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00036990: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+000369a0: 7568 2b6a 0203 0000 681b 6a3d 5200 0068  uh+j....h.j=R..h
+000369b0: 1d6a 094f 0000 681e 4b00 7562 6a13 0300  .j.O..h.K.ubj...
+000369c0: 0029 8194 7d94 2868 058c 1d54 6865 2070  .)..}.(h...The p
+000369d0: 7269 6e74 6572 2073 7461 7465 2069 7320  rinter state is 
+000369e0: 756e 6b6e 6f77 6e2e 9468 075d 9468 4729  unknown..h.].hG)
+000369f0: 8194 7d94 2868 056a 5052 0000 6807 5d94  ..}.(h.jPR..h.].
+00036a00: 6a3a 0100 0029 8194 7d94 2868 0568 0668  j:...)..}.(h.h.h
+00036a10: 075d 9468 168c 1d54 6865 2070 7269 6e74  .].h...The print
+00036a20: 6572 2073 7461 7465 2069 7320 756e 6b6e  er state is unkn
+00036a30: 6f77 6e2e 9485 9481 947d 9428 6805 6806  own......}.(h.h.
+00036a40: 681b 6a55 5200 0068 1c68 0368 1d4e 681e  h.jUR..h.h.h.Nh.
+00036a50: 4e75 6261 681f 7d94 2868 215d 9468 235d  Nubah.}.(h!].h#]
+00036a60: 9468 255d 9468 275d 9468 295d 948c 0972  .h%].h'].h)]...r
+00036a70: 6566 646f 6d61 696e 948c 0270 7994 8c0b  efdomain...py...
+00036a80: 7265 6665 7870 6c69 6369 7494 898c 0772  refexplicit....r
+00036a90: 6566 7479 7065 946a 4b01 0000 8c09 7265  eftype.jK.....re
+00036aa0: 6674 6172 6765 7494 8c1d 5468 6520 7072  ftarget...The pr
+00036ab0: 696e 7465 7220 7374 6174 6520 6973 2075  inter state is u
+00036ac0: 6e6b 6e6f 776e 2e94 6a57 0300 0088 6a58  nknown..jW....jX
+00036ad0: 0300 006a 4e4f 0000 6a59 0300 004e 7568  ...jNO..jY...Nuh
+00036ae0: 2b6a 3901 0000 681b 6a52 5200 0068 1c68  +j9...h.jRR..h.h
+00036af0: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+00036b00: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00036b10: 295d 9475 682b 6846 681d 6a09 4f00 0068  )].uh+hFh.j.O..h
+00036b20: 1e4b 2768 1b6a 4e52 0000 7562 6168 1f7d  .K'h.jNR..ubah.}
+00036b30: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00036b40: 5d94 6829 5d94 7568 2b6a 1203 0000 681b  ].h)].uh+j....h.
+00036b50: 6a3d 5200 0075 6265 681f 7d94 2868 215d  j=R..ubeh.}.(h!]
+00036b60: 9468 235d 9468 255d 9468 275d 9468 295d  .h#].h%].h'].h)]
+00036b70: 9475 682b 6afd 0200 0068 1d6a 094f 0000  .uh+j....h.j.O..
+00036b80: 681e 4b27 681b 6a3a 5200 0068 1c68 0375  h.K'h.j:R..h.h.u
+00036b90: 6261 681f 7d94 2868 215d 9468 235d 9468  bah.}.(h!].h#].h
+00036ba0: 255d 9468 275d 9468 295d 9475 682b 6af8  %].h'].h)].uh+j.
+00036bb0: 0200 0068 1b6a 3752 0000 681c 6803 681d  ...h.j7R..h.h.h.
+00036bc0: 4e68 1e4e 7562 6168 1f7d 9428 6821 5d94  Nh.Nubah.}.(h!].
+00036bd0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00036be0: 7568 2b6a e402 0000 681b 6a0f 5200 0068  uh+j....h.j.R..h
+00036bf0: 1c68 0368 1d6a 094f 0000 681e 4b28 7562  .h.h.j.O..h.K(ub
+00036c00: 6568 1f7d 9428 6821 5d94 6823 5d94 286a  eh.}.(h!].h#].(j
+00036c10: 6352 0000 8c09 6174 7472 6962 7574 6594  cR....attribute.
+00036c20: 6568 255d 9468 275d 9468 295d 946a 1805  eh%].h'].h)].j..
+00036c30: 0000 6a63 5200 006a 1905 0000 6a89 5200  ..jcR..j....j.R.
+00036c40: 006a 1a05 0000 6a89 5200 006a 1b05 0000  .j....j.R..j....
+00036c50: 8975 682b 68ac 681c 6803 681b 6ad0 4e00  .uh+h.h.h.h.j.N.
+00036c60: 0068 1d4e 681e 4e75 6265 681f 7d94 2868  .h.Nh.Nubeh.}.(h
+00036c70: 215d 948c 0a67 636f 6465 7374 6174 6594  !]...gcodestate.
+00036c80: 6168 235d 9468 255d 948c 0a67 636f 6465  ah#].h%]...gcode
+00036c90: 7374 6174 6594 6168 275d 9468 295d 9475  state.ah'].h)].u
+00036ca0: 682b 680a 681b 6803 681c 6803 681d 682c  h+h.h.h.h.h.h.h,
+00036cb0: 681e 4b23 7562 6568 1f7d 9428 6821 5d94  h.K#ubeh.}.(h!].
+00036cc0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00036cd0: 8c06 736f 7572 6365 9468 2c75 682b 6801  ..source.h,uh+h.
+00036ce0: 8c0e 6375 7272 656e 745f 736f 7572 6365  ..current_source
+00036cf0: 944e 8c0c 6375 7272 656e 745f 6c69 6e65  .N..current_line
+00036d00: 944e 8c08 7365 7474 696e 6773 948c 1164  .N..settings...d
+00036d10: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
+00036d20: 948c 0656 616c 7565 7394 9394 2981 947d  ...Values...)..}
+00036d30: 9428 680f 4e8c 0967 656e 6572 6174 6f72  .(h.N..generator
+00036d40: 944e 8c09 6461 7465 7374 616d 7094 4e8c  .N..datestamp.N.
+00036d50: 0b73 6f75 7263 655f 6c69 6e6b 944e 8c0a  .source_link.N..
+00036d60: 736f 7572 6365 5f75 726c 944e 8c0d 746f  source_url.N..to
+00036d70: 635f 6261 636b 6c69 6e6b 7394 8c05 656e  c_backlinks...en
+00036d80: 7472 7994 8c12 666f 6f74 6e6f 7465 5f62  try...footnote_b
+00036d90: 6163 6b6c 696e 6b73 944b 018c 0d73 6563  acklinks.K...sec
+00036da0: 746e 756d 5f78 666f 726d 944b 018c 0e73  tnum_xform.K...s
+00036db0: 7472 6970 5f63 6f6d 6d65 6e74 7394 4e8c  trip_comments.N.
+00036dc0: 1b73 7472 6970 5f65 6c65 6d65 6e74 735f  .strip_elements_
+00036dd0: 7769 7468 5f63 6c61 7373 6573 944e 8c0d  with_classes.N..
+00036de0: 7374 7269 705f 636c 6173 7365 7394 4e8c  strip_classes.N.
+00036df0: 0c72 6570 6f72 745f 6c65 7665 6c94 4b02  .report_level.K.
+00036e00: 8c0a 6861 6c74 5f6c 6576 656c 944b 058c  ..halt_level.K..
+00036e10: 1165 7869 745f 7374 6174 7573 5f6c 6576  .exit_status_lev
+00036e20: 656c 944b 058c 0564 6562 7567 944e 8c0e  el.K...debug.N..
+00036e30: 7761 726e 696e 675f 7374 7265 616d 944e  warning_stream.N
+00036e40: 8c09 7472 6163 6562 6163 6b94 888c 0e69  ..traceback....i
+00036e50: 6e70 7574 5f65 6e63 6f64 696e 6794 8c09  nput_encoding...
+00036e60: 7574 662d 382d 7369 6794 8c1c 696e 7075  utf-8-sig...inpu
+00036e70: 745f 656e 636f 6469 6e67 5f65 7272 6f72  t_encoding_error
+00036e80: 5f68 616e 646c 6572 948c 0673 7472 6963  _handler...stric
+00036e90: 7494 8c0f 6f75 7470 7574 5f65 6e63 6f64  t...output_encod
+00036ea0: 696e 6794 8c05 7574 662d 3894 8c1d 6f75  ing...utf-8...ou
+00036eb0: 7470 7574 5f65 6e63 6f64 696e 675f 6572  tput_encoding_er
+00036ec0: 726f 725f 6861 6e64 6c65 7294 6ab8 5200  ror_handler.j.R.
+00036ed0: 008c 0e65 7272 6f72 5f65 6e63 6f64 696e  ...error_encodin
+00036ee0: 6794 8c05 7574 662d 3894 8c1c 6572 726f  g...utf-8...erro
+00036ef0: 725f 656e 636f 6469 6e67 5f65 7272 6f72  r_encoding_error
+00036f00: 5f68 616e 646c 6572 948c 1062 6163 6b73  _handler...backs
+00036f10: 6c61 7368 7265 706c 6163 6594 8c0d 6c61  lashreplace...la
+00036f20: 6e67 7561 6765 5f63 6f64 6594 8c02 656e  nguage_code...en
+00036f30: 948c 1372 6563 6f72 645f 6465 7065 6e64  ...record_depend
+00036f40: 656e 6369 6573 944e 8c06 636f 6e66 6967  encies.N..config
+00036f50: 944e 8c09 6964 5f70 7265 6669 7894 6806  .N..id_prefix.h.
+00036f60: 8c0e 6175 746f 5f69 645f 7072 6566 6978  ..auto_id_prefix
+00036f70: 948c 0269 6494 8c0d 6475 6d70 5f73 6574  ...id...dump_set
+00036f80: 7469 6e67 7394 4e8c 0e64 756d 705f 696e  tings.N..dump_in
+00036f90: 7465 726e 616c 7394 4e8c 0f64 756d 705f  ternals.N..dump_
+00036fa0: 7472 616e 7366 6f72 6d73 944e 8c0f 6475  transforms.N..du
+00036fb0: 6d70 5f70 7365 7564 6f5f 786d 6c94 4e8c  mp_pseudo_xml.N.
+00036fc0: 1065 7870 6f73 655f 696e 7465 726e 616c  .expose_internal
+00036fd0: 7394 4e8c 0e73 7472 6963 745f 7669 7369  s.N..strict_visi
+00036fe0: 746f 7294 4e8c 0f5f 6469 7361 626c 655f  tor.N.._disable_
+00036ff0: 636f 6e66 6967 944e 8c07 5f73 6f75 7263  config.N.._sourc
+00037000: 6594 682c 8c0c 5f64 6573 7469 6e61 7469  e.h,.._destinati
+00037010: 6f6e 944e 8c0d 5f63 6f6e 6669 675f 6669  on.N.._config_fi
+00037020: 6c65 7394 5d94 8c16 6669 6c65 5f69 6e73  les.]...file_ins
+00037030: 6572 7469 6f6e 5f65 6e61 626c 6564 9488  ertion_enabled..
+00037040: 8c0b 7261 775f 656e 6162 6c65 6494 4b01  ..raw_enabled.K.
+00037050: 8c11 6c69 6e65 5f6c 656e 6774 685f 6c69  ..line_length_li
+00037060: 6d69 7494 4d10 278c 0e70 6570 5f72 6566  mit.M.'..pep_ref
+00037070: 6572 656e 6365 7394 4e8c 0c70 6570 5f62  erences.N..pep_b
+00037080: 6173 655f 7572 6c94 8c18 6874 7470 733a  ase_url...https:
+00037090: 2f2f 7065 7073 2e70 7974 686f 6e2e 6f72  //peps.python.or
+000370a0: 672f 948c 1570 6570 5f66 696c 655f 7572  g/...pep_file_ur
+000370b0: 6c5f 7465 6d70 6c61 7465 948c 0870 6570  l_template...pep
+000370c0: 2d25 3034 6494 8c0e 7266 635f 7265 6665  -%04d...rfc_refe
+000370d0: 7265 6e63 6573 944e 8c0c 7266 635f 6261  rences.N..rfc_ba
+000370e0: 7365 5f75 726c 948c 2668 7474 7073 3a2f  se_url..&https:/
+000370f0: 2f64 6174 6174 7261 636b 6572 2e69 6574  /datatracker.iet
+00037100: 662e 6f72 672f 646f 632f 6874 6d6c 2f94  f.org/doc/html/.
+00037110: 8c09 7461 625f 7769 6474 6894 4b08 8c1d  ..tab_width.K...
+00037120: 7472 696d 5f66 6f6f 746e 6f74 655f 7265  trim_footnote_re
+00037130: 6665 7265 6e63 655f 7370 6163 6594 898c  ference_space...
+00037140: 1073 796e 7461 785f 6869 6768 6c69 6768  .syntax_highligh
+00037150: 7494 8c04 6c6f 6e67 948c 0c73 6d61 7274  t...long...smart
+00037160: 5f71 756f 7465 7394 888c 1373 6d61 7274  _quotes....smart
+00037170: 7175 6f74 6573 5f6c 6f63 616c 6573 945d  quotes_locales.]
+00037180: 948c 1d63 6861 7261 6374 6572 5f6c 6576  ...character_lev
+00037190: 656c 5f69 6e6c 696e 655f 6d61 726b 7570  el_inline_markup
+000371a0: 9489 8c0e 646f 6374 6974 6c65 5f78 666f  ....doctitle_xfo
+000371b0: 726d 9489 8c0d 646f 6369 6e66 6f5f 7866  rm....docinfo_xf
+000371c0: 6f72 6d94 4b01 8c12 7365 6374 7375 6274  orm.K...sectsubt
+000371d0: 6974 6c65 5f78 666f 726d 9489 8c0d 696d  itle_xform....im
+000371e0: 6167 655f 6c6f 6164 696e 6794 8c04 6c69  age_loading...li
+000371f0: 6e6b 948c 1065 6d62 6564 5f73 7479 6c65  nk...embed_style
+00037200: 7368 6565 7494 898c 1563 6c6f 616b 5f65  sheet....cloak_e
+00037210: 6d61 696c 5f61 6464 7265 7373 6573 9488  mail_addresses..
+00037220: 8c11 7365 6374 696f 6e5f 7365 6c66 5f6c  ..section_self_l
+00037230: 696e 6b94 898c 0365 6e76 944e 7562 8c08  ink....env.Nub..
+00037240: 7265 706f 7274 6572 944e 8c10 696e 6469  reporter.N..indi
+00037250: 7265 6374 5f74 6172 6765 7473 945d 948c  rect_targets.]..
+00037260: 1173 7562 7374 6974 7574 696f 6e5f 6465  .substitution_de
+00037270: 6673 947d 948c 1273 7562 7374 6974 7574  fs.}...substitut
+00037280: 696f 6e5f 6e61 6d65 7394 7d94 8c08 7265  ion_names.}...re
+00037290: 666e 616d 6573 947d 948c 0672 6566 6964  fnames.}...refid
+000372a0: 7394 7d94 8c07 6e61 6d65 6964 7394 7d94  s.}...nameids.}.
+000372b0: 2868 3268 2f68 5b68 586a f22b 0000 6aef  (h2h/h[hXj.+..j.
+000372c0: 2b00 006a 3337 0000 6a30 3700 006a b439  +..j37..j07..j.9
+000372d0: 0000 6ab1 3900 006a cd4e 0000 6aca 4e00  ..j.9..j.N..j.N.
+000372e0: 006a 9252 0000 6a8f 5200 0075 8c09 6e61  .j.R..j.R..u..na
+000372f0: 6d65 7479 7065 7394 7d94 2868 324e 685b  metypes.}.(h2Nh[
+00037300: 4e6a f22b 0000 4e6a 3337 0000 4e6a b439  Nj.+..Nj37..Nj.9
+00037310: 0000 4e6a cd4e 0000 4e6a 9252 0000 4e75  ..Nj.N..Nj.R..Nu
+00037320: 6821 7d94 2868 2f68 0c68 5868 356a ef2b  h!}.(h/h.hXh5j.+
+00037330: 0000 685e 6876 6871 68aa 68b3 6a28 0500  ..h^hvhqh.h.j(..
+00037340: 006a 2e05 0000 6aa3 0500 006a a805 0000  .j....j....j....
+00037350: 6a66 0700 006a 6c07 0000 6ae1 0700 006a  jf...jl...j....j
+00037360: e607 0000 6a3f 0900 006a 4409 0000 6a4c  ....j?...jD...jL
+00037370: 0a00 006a 510a 0000 6a59 0b00 006a 5e0b  ...jQ...jY...j^.
+00037380: 0000 6a66 0c00 006a 6b0c 0000 6abf 0d00  ..jf...jk...j...
+00037390: 006a c40d 0000 6a7c 0f00 006a 810f 0000  .j....j|...j....
+000373a0: 6a89 1000 006a 8e10 0000 6a96 1100 006a  j....j....j....j
+000373b0: 9b11 0000 6a53 1300 006a 5813 0000 6a60  ....jS...jX...j`
+000373c0: 1400 006a 6514 0000 6a6d 1500 006a 7215  ...je...jm...jr.
+000373d0: 0000 6a30 1700 006a 3517 0000 6a3d 1800  ..j0...j5...j=..
+000373e0: 006a 4218 0000 6a4a 1900 006a 4f19 0000  .jB...jJ...jO...
+000373f0: 6a57 1a00 006a 5c1a 0000 6a1a 1c00 006a  jW...j\...j....j
+00037400: 1f1c 0000 6af5 1e00 006a fa1e 0000 6ab8  ....j....j....j.
+00037410: 2000 006a bd20 0000 6a7b 2200 006a 8022   ..j. ..j{"..j."
+00037420: 0000 6aef 2400 006a f424 0000 6afc 2500  ..j.$..j.$..j.%.
+00037430: 006a 0126 0000 6a09 2700 006a 0e27 0000  .j.&..j.'..j.'..
+00037440: 6a16 2800 006a 1b28 0000 6a23 2900 006a  j.(..j.(..j#)..j
+00037450: 2829 0000 6a30 3700 006a f52b 0000 6a0b  ()..j07..j.+..j.
+00037460: 2c00 006a 062c 0000 6a49 2c00 006a 4e2c  ,..j.,..jI,..jN,
+00037470: 0000 6ad6 2c00 006a db2c 0000 6a62 2d00  ..j.,..j.,..jb-.
+00037480: 006a 672d 0000 6aee 2d00 006a f32d 0000  .jg-..j.-..j.-..
+00037490: 6a7a 2e00 006a 7f2e 0000 6a06 2f00 006a  jz...j....j./..j
+000374a0: 0b2f 0000 6a92 2f00 006a 972f 0000 6a1e  ./..j./..j./..j.
+000374b0: 3000 006a 2330 0000 6aaa 3000 006a af30  0..j#0..j.0..j.0
+000374c0: 0000 6a36 3100 006a 3b31 0000 6ac2 3100  ..j61..j;1..j.1.
+000374d0: 006a c731 0000 6a4e 3200 006a 5332 0000  .j.1..jN2..jS2..
+000374e0: 6ada 3200 006a df32 0000 6a66 3300 006a  j.2..j.2..jf3..j
+000374f0: 6b33 0000 6af2 3300 006a f733 0000 6a7e  k3..j.3..j.3..j~
+00037500: 3400 006a 8334 0000 6a0a 3500 006a 0f35  4..j.4..j.5..j.5
+00037510: 0000 6a96 3500 006a 9b35 0000 6a22 3600  ..j.5..j.5..j"6.
+00037520: 006a 2736 0000 6aae 3600 006a b336 0000  .j'6..j.6..j.6..
+00037530: 6ab1 3900 006a 3637 0000 6a4c 3700 006a  j.9..j67..jL7..j
+00037540: 4737 0000 6a8a 3700 006a 8f37 0000 6a17  G7..j.7..j.7..j.
+00037550: 3800 006a 1c38 0000 6aa3 3800 006a a838  8..j.8..j.8..j.8
+00037560: 0000 6a2f 3900 006a 3439 0000 6aca 4e00  ..j/9..j49..j.N.
+00037570: 006a b739 0000 6acd 3900 006a c839 0000  .j.9..j.9..j.9..
+00037580: 6a0b 3a00 006a 103a 0000 6a98 3a00 006a  j.:..j.:..j.:..j
+00037590: 9d3a 0000 6a24 3b00 006a 293b 0000 6ab0  .:..j$;..j);..j.
+000375a0: 3b00 006a b53b 0000 6a3c 3c00 006a 413c  ;..j.;..j<<..jA<
+000375b0: 0000 6ac8 3c00 006a cd3c 0000 6a54 3d00  ..j.<..j.<..jT=.
+000375c0: 006a 593d 0000 6ae0 3d00 006a e53d 0000  .jY=..j.=..j.=..
+000375d0: 6a6c 3e00 006a 713e 0000 6af8 3e00 006a  jl>..jq>..j.>..j
+000375e0: fd3e 0000 6a84 3f00 006a 893f 0000 6a10  .>..j.?..j.?..j.
+000375f0: 4000 006a 1540 0000 6a9c 4000 006a a140  @..j.@..j.@..j.@
+00037600: 0000 6a28 4100 006a 2d41 0000 6ab4 4100  ..j(A..j-A..j.A.
+00037610: 006a b941 0000 6a40 4200 006a 4542 0000  .j.A..j@B..jEB..
+00037620: 6acc 4200 006a d142 0000 6a58 4300 006a  j.B..j.B..jXC..j
+00037630: 5d43 0000 6ae4 4300 006a e943 0000 6a70  ]C..j.C..j.C..jp
+00037640: 4400 006a 7544 0000 6afc 4400 006a 0145  D..juD..j.D..j.E
+00037650: 0000 6a88 4500 006a 8d45 0000 6a14 4600  ..j.E..j.E..j.F.
+00037660: 006a 1946 0000 6aa0 4600 006a a546 0000  .j.F..j.F..j.F..
+00037670: 6a2c 4700 006a 3147 0000 6ab8 4700 006a  j,G..j1G..j.G..j
+00037680: bd47 0000 6a44 4800 006a 4948 0000 6ad0  .G..jDH..jIH..j.
+00037690: 4800 006a d548 0000 6a5c 4900 006a 6149  H..j.H..j\I..jaI
+000376a0: 0000 6ae8 4900 006a ed49 0000 6a74 4a00  ..j.I..j.I..jtJ.
+000376b0: 006a 794a 0000 6a00 4b00 006a 054b 0000  .jyJ..j.K..j.K..
+000376c0: 6a8c 4b00 006a 914b 0000 6a18 4c00 006a  j.K..j.K..j.L..j
+000376d0: 1d4c 0000 6aa4 4c00 006a a94c 0000 6a30  .L..j.L..j.L..j0
+000376e0: 4d00 006a 354d 0000 6abc 4d00 006a c14d  M..j5M..j.M..j.M
+000376f0: 0000 6a48 4e00 006a 4d4e 0000 6a8f 5200  ..jHN..jMN..j.R.
+00037700: 006a d04e 0000 6ae6 4e00 006a e14e 0000  .j.N..j.N..j.N..
+00037710: 6a24 4f00 006a 294f 0000 6ab1 4f00 006a  j$O..j)O..j.O..j
+00037720: b64f 0000 6a69 5000 006a 6e50 0000 6af5  .O..jiP..jnP..j.
+00037730: 5000 006a fa50 0000 6a81 5100 006a 8651  P..j.P..j.Q..j.Q
+00037740: 0000 6a0d 5200 006a 1252 0000 758c 0d66  ..j.R..j.R..u..f
+00037750: 6f6f 746e 6f74 655f 7265 6673 947d 948c  ootnote_refs.}..
+00037760: 0d63 6974 6174 696f 6e5f 7265 6673 947d  .citation_refs.}
+00037770: 948c 0d61 7574 6f66 6f6f 746e 6f74 6573  ...autofootnotes
+00037780: 945d 948c 1161 7574 6f66 6f6f 746e 6f74  .]...autofootnot
+00037790: 655f 7265 6673 945d 948c 1073 796d 626f  e_refs.]...symbo
+000377a0: 6c5f 666f 6f74 6e6f 7465 7394 5d94 8c14  l_footnotes.]...
+000377b0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
+000377c0: 7265 6673 945d 948c 0966 6f6f 746e 6f74  refs.]...footnot
+000377d0: 6573 945d 948c 0963 6974 6174 696f 6e73  es.]...citations
+000377e0: 945d 948c 1261 7574 6f66 6f6f 746e 6f74  .]...autofootnot
+000377f0: 655f 7374 6172 7494 4b01 8c15 7379 6d62  e_start.K...symb
+00037800: 6f6c 5f66 6f6f 746e 6f74 655f 7374 6172  ol_footnote_star
+00037810: 7494 4b00 8c0a 6964 5f63 6f75 6e74 6572  t.K...id_counter
+00037820: 948c 0b63 6f6c 6c65 6374 696f 6e73 948c  ...collections..
+00037830: 0743 6f75 6e74 6572 9493 947d 9485 9452  .Counter...}...R
+00037840: 948c 0e70 6172 7365 5f6d 6573 7361 6765  ...parse_message
+00037850: 7394 5d94 2868 098c 0e73 7973 7465 6d5f  s.].(h...system_
+00037860: 6d65 7373 6167 6594 9394 2981 947d 9428  message...)..}.(
+00037870: 6805 6806 6807 5d94 2868 4729 8194 7d94  h.h.h.].(hG)..}.
+00037880: 2868 0568 0668 075d 9468 168c 1a54 6974  (h.h.h.].h...Tit
+00037890: 6c65 2075 6e64 6572 6c69 6e65 2074 6f6f  le underline too
+000378a0: 2073 686f 7274 2e94 8594 8194 7d94 2868   short......}.(h
+000378b0: 0568 0668 1b6a 1e53 0000 7562 6168 1f7d  .h.h.j.S..ubah.}
+000378c0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000378d0: 5d94 6829 5d94 7568 2b68 4668 1b6a 1b53  ].h)].uh+hFh.j.S
+000378e0: 0000 7562 6809 8c0d 6c69 7465 7261 6c5f  ..ubh...literal_
+000378f0: 626c 6f63 6b94 9394 2981 947d 9428 6805  block...)..}.(h.
+00037900: 8c0e 5072 696e 7465 720a 3d3d 3d3d 3d3d  ..Printer.======
+00037910: 9468 075d 9468 168c 0e50 7269 6e74 6572  .h.].h...Printer
+00037920: 0a3d 3d3d 3d3d 3d94 8594 8194 7d94 2868  .======.....}.(h
+00037930: 0568 0668 1b6a 2d53 0000 7562 6168 1f7d  .h.h.j-S..ubah.}
+00037940: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+00037950: 5d94 6829 5d94 68c9 68ca 7568 2b6a 2b53  ].h)].h.h.uh+j+S
+00037960: 0000 681b 6a1b 5300 0075 6265 681f 7d94  ..h.j.S..ubeh.}.
+00037970: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00037980: 9468 295d 948c 056c 6576 656c 944b 028c  .h)]...level.K..
+00037990: 0474 7970 6594 8c07 5741 524e 494e 4794  .type...WARNING.
+000379a0: 8c04 6c69 6e65 944b 0b8c 0673 6f75 7263  ..line.K...sourc
+000379b0: 6594 682c 7568 2b6a 1953 0000 7562 6a1a  e.h,uh+j.S..ubj.
+000379c0: 5300 0029 8194 7d94 2868 0568 0668 075d  S..)..}.(h.h.h.]
+000379d0: 9428 6847 2981 947d 9428 6805 8c1a 5469  .(hG)..}.(h...Ti
+000379e0: 746c 6520 756e 6465 726c 696e 6520 746f  tle underline to
+000379f0: 6f20 7368 6f72 742e 9468 075d 9468 168c  o short..h.].h..
+00037a00: 1a54 6974 6c65 2075 6e64 6572 6c69 6e65  .Title underline
+00037a10: 2074 6f6f 2073 686f 7274 2e94 8594 8194   too short......
+00037a20: 7d94 2868 0568 0668 1b6a 4953 0000 681c  }.(h.h.h.jIS..h.
+00037a30: 6803 681d 4e68 1e4e 7562 6168 1f7d 9428  h.h.Nh.Nubah.}.(
+00037a40: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00037a50: 6829 5d94 7568 2b68 4668 1b6a 4653 0000  h)].uh+hFh.jFS..
+00037a60: 7562 6a2c 5300 0029 8194 7d94 2868 058c  ubj,S..)..}.(h..
+00037a70: 0e50 7269 6e74 6572 0a3d 3d3d 3d3d 3d94  .Printer.======.
+00037a80: 6807 5d94 6816 8c0e 5072 696e 7465 720a  h.].h...Printer.
+00037a90: 3d3d 3d3d 3d3d 9485 9481 947d 9428 6805  ======.....}.(h.
+00037aa0: 6806 681b 6a57 5300 0075 6261 681f 7d94  h.h.jWS..ubah.}.
+00037ab0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00037ac0: 9468 295d 9468 c968 ca75 682b 6a2b 5300  .h)].h.h.uh+j+S.
+00037ad0: 0068 1b6a 4653 0000 681d 682c 7562 6568  .h.jFS..h.h,ubeh
+00037ae0: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00037af0: 6827 5d94 6829 5d94 8c05 6c65 7665 6c94  h'].h)]...level.
+00037b00: 4b02 8c04 7479 7065 946a 4353 0000 8c04  K...type.jCS....
+00037b10: 6c69 6e65 944b 0b8c 0673 6f75 7263 6594  line.K...source.
+00037b20: 682c 7568 2b6a 1953 0000 681b 685e 681c  h,uh+j.S..h.h^h.
+00037b30: 6803 681d 682c 681e 4b0b 7562 6a1a 5300  h.h.h,h.K.ubj.S.
+00037b40: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00037b50: 6847 2981 947d 9428 6805 6806 6807 5d94  hG)..}.(h.h.h.].
+00037b60: 6816 8c1a 5469 746c 6520 756e 6465 726c  h...Title underl
+00037b70: 696e 6520 746f 6f20 7368 6f72 742e 9485  ine too short...
+00037b80: 9481 947d 9428 6805 6806 681b 6a72 5300  ...}.(h.h.h.jrS.
+00037b90: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+00037ba0: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00037bb0: 6846 681b 6a6f 5300 0075 626a 2c53 0000  hFh.joS..ubj,S..
+00037bc0: 2981 947d 9428 6805 8c0f 4669 6c61 6d65  )..}.(h...Filame
+00037bd0: 6e74 0a3d 3d3d 3d3d 3d94 6807 5d94 6816  nt.======.h.].h.
+00037be0: 8c0f 4669 6c61 6d65 6e74 0a3d 3d3d 3d3d  ..Filament.=====
+00037bf0: 3d94 8594 8194 7d94 2868 0568 0668 1b6a  =.....}.(h.h.h.j
+00037c00: 7f53 0000 7562 6168 1f7d 9428 6821 5d94  .S..ubah.}.(h!].
+00037c10: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00037c20: 68c9 68ca 7568 2b6a 2b53 0000 681b 6a6f  h.h.uh+j+S..h.jo
+00037c30: 5300 0075 6265 681f 7d94 2868 215d 9468  S..ubeh.}.(h!].h
+00037c40: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00037c50: 056c 6576 656c 944b 028c 0474 7970 6594  .level.K...type.
+00037c60: 6a43 5300 008c 046c 696e 6594 4b11 8c06  jCS....line.K...
+00037c70: 736f 7572 6365 9468 2c75 682b 6a19 5300  source.h,uh+j.S.
+00037c80: 0075 626a 1a53 0000 2981 947d 9428 6805  .ubj.S..)..}.(h.
+00037c90: 6806 6807 5d94 2868 4729 8194 7d94 2868  h.h.].(hG)..}.(h
+00037ca0: 058c 1a54 6974 6c65 2075 6e64 6572 6c69  ...Title underli
+00037cb0: 6e65 2074 6f6f 2073 686f 7274 2e94 6807  ne too short..h.
+00037cc0: 5d94 6816 8c1a 5469 746c 6520 756e 6465  ].h...Title unde
+00037cd0: 726c 696e 6520 746f 6f20 7368 6f72 742e  rline too short.
+00037ce0: 9485 9481 947d 9428 6805 6806 681b 6a9a  .....}.(h.h.h.j.
+00037cf0: 5300 0068 1c68 0368 1d4e 681e 4e75 6261  S..h.h.h.Nh.Nuba
+00037d00: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00037d10: 9468 275d 9468 295d 9475 682b 6846 681b  .h'].h)].uh+hFh.
+00037d20: 6a97 5300 0075 626a 2c53 0000 2981 947d  j.S..ubj,S..)..}
+00037d30: 9428 6805 8c0f 4669 6c61 6d65 6e74 0a3d  .(h...Filament.=
+00037d40: 3d3d 3d3d 3d94 6807 5d94 6816 8c0f 4669  =====.h.].h...Fi
+00037d50: 6c61 6d65 6e74 0a3d 3d3d 3d3d 3d94 8594  lament.======...
+00037d60: 8194 7d94 2868 0568 0668 1b6a a853 0000  ..}.(h.h.h.j.S..
+00037d70: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00037d80: 6825 5d94 6827 5d94 6829 5d94 68c9 68ca  h%].h'].h)].h.h.
+00037d90: 7568 2b6a 2b53 0000 681b 6a97 5300 0068  uh+j+S..h.j.S..h
+00037da0: 1d68 2c75 6265 681f 7d94 2868 215d 9468  .h,ubeh.}.(h!].h
+00037db0: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00037dc0: 056c 6576 656c 944b 028c 0474 7970 6594  .level.K...type.
+00037dd0: 6a43 5300 008c 046c 696e 6594 4b11 8c06  jCS....line.K...
+00037de0: 736f 7572 6365 9468 2c75 682b 6a19 5300  source.h,uh+j.S.
+00037df0: 0068 1b6a f52b 0000 681c 6803 681d 682c  .h.j.+..h.h.h.h,
+00037e00: 681e 4b11 7562 6a1a 5300 0029 8194 7d94  h.K.ubj.S..)..}.
+00037e10: 2868 0568 0668 075d 9428 6847 2981 947d  (h.h.h.].(hG)..}
+00037e20: 9428 6805 6806 6807 5d94 6816 8c1a 5469  .(h.h.h.].h...Ti
+00037e30: 746c 6520 756e 6465 726c 696e 6520 746f  tle underline to
+00037e40: 6f20 7368 6f72 742e 9485 9481 947d 9428  o short......}.(
+00037e50: 6805 6806 681b 6ac3 5300 0075 6261 681f  h.h.h.j.S..ubah.
+00037e60: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00037e70: 275d 9468 295d 9475 682b 6846 681b 6ac0  '].h)].uh+hFh.j.
+00037e80: 5300 0075 626a 2c53 0000 2981 947d 9428  S..ubj,S..)..}.(
+00037e90: 6805 8c1a 414d 5346 696c 616d 656e 7453  h...AMSFilamentS
+00037ea0: 6574 7469 6e67 730a 3d3d 3d3d 3d3d 9468  ettings.======.h
+00037eb0: 075d 9468 168c 1a41 4d53 4669 6c61 6d65  .].h...AMSFilame
+00037ec0: 6e74 5365 7474 696e 6773 0a3d 3d3d 3d3d  ntSettings.=====
+00037ed0: 3d94 8594 8194 7d94 2868 0568 0668 1b6a  =.....}.(h.h.h.j
+00037ee0: d053 0000 7562 6168 1f7d 9428 6821 5d94  .S..ubah.}.(h!].
+00037ef0: 6823 5d94 6825 5d94 6827 5d94 6829 5d94  h#].h%].h'].h)].
+00037f00: 68c9 68ca 7568 2b6a 2b53 0000 681b 6ac0  h.h.uh+j+S..h.j.
+00037f10: 5300 0075 6265 681f 7d94 2868 215d 9468  S..ubeh.}.(h!].h
+00037f20: 235d 9468 255d 9468 275d 9468 295d 948c  #].h%].h'].h)]..
+00037f30: 056c 6576 656c 944b 028c 0474 7970 6594  .level.K...type.
+00037f40: 6a43 5300 008c 046c 696e 6594 4b17 8c06  jCS....line.K...
+00037f50: 736f 7572 6365 9468 2c75 682b 6a19 5300  source.h,uh+j.S.
+00037f60: 0075 626a 1a53 0000 2981 947d 9428 6805  .ubj.S..)..}.(h.
+00037f70: 6806 6807 5d94 2868 4729 8194 7d94 2868  h.h.].(hG)..}.(h
+00037f80: 058c 1a54 6974 6c65 2075 6e64 6572 6c69  ...Title underli
+00037f90: 6e65 2074 6f6f 2073 686f 7274 2e94 6807  ne too short..h.
+00037fa0: 5d94 6816 8c1a 5469 746c 6520 756e 6465  ].h...Title unde
+00037fb0: 726c 696e 6520 746f 6f20 7368 6f72 742e  rline too short.
+00037fc0: 9485 9481 947d 9428 6805 6806 681b 6aeb  .....}.(h.h.h.j.
+00037fd0: 5300 0068 1c68 0368 1d4e 681e 4e75 6261  S..h.h.h.Nh.Nuba
+00037fe0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+00037ff0: 9468 275d 9468 295d 9475 682b 6846 681b  .h'].h)].uh+hFh.
+00038000: 6ae8 5300 0075 626a 2c53 0000 2981 947d  j.S..ubj,S..)..}
+00038010: 9428 6805 8c1a 414d 5346 696c 616d 656e  .(h...AMSFilamen
+00038020: 7453 6574 7469 6e67 730a 3d3d 3d3d 3d3d  tSettings.======
+00038030: 9468 075d 9468 168c 1a41 4d53 4669 6c61  .h.].h...AMSFila
+00038040: 6d65 6e74 5365 7474 696e 6773 0a3d 3d3d  mentSettings.===
+00038050: 3d3d 3d94 8594 8194 7d94 2868 0568 0668  ===.....}.(h.h.h
+00038060: 1b6a f953 0000 7562 6168 1f7d 9428 6821  .j.S..ubah.}.(h!
+00038070: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00038080: 5d94 68c9 68ca 7568 2b6a 2b53 0000 681b  ].h.h.uh+j+S..h.
+00038090: 6ae8 5300 0068 1d68 2c75 6265 681f 7d94  j.S..h.h,ubeh.}.
+000380a0: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+000380b0: 9468 295d 948c 056c 6576 656c 944b 028c  .h)]...level.K..
+000380c0: 0474 7970 6594 6a43 5300 008c 046c 696e  .type.jCS....lin
+000380d0: 6594 4b17 8c06 736f 7572 6365 9468 2c75  e.K...source.h,u
+000380e0: 682b 6a19 5300 0068 1b6a 3637 0000 681c  h+j.S..h.j67..h.
+000380f0: 6803 681d 682c 681e 4b17 7562 6a1a 5300  h.h.h,h.K.ubj.S.
+00038100: 0029 8194 7d94 2868 0568 0668 075d 9428  .)..}.(h.h.h.].(
+00038110: 6847 2981 947d 9428 6805 6806 6807 5d94  hG)..}.(h.h.h.].
+00038120: 6816 8c1a 5469 746c 6520 756e 6465 726c  h...Title underl
+00038130: 696e 6520 746f 6f20 7368 6f72 742e 9485  ine too short...
+00038140: 9481 947d 9428 6805 6806 681b 6a14 5400  ...}.(h.h.h.j.T.
+00038150: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+00038160: 9468 255d 9468 275d 9468 295d 9475 682b  .h%].h'].h)].uh+
+00038170: 6846 681b 6a11 5400 0075 626a 2c53 0000  hFh.j.T..ubj,S..
+00038180: 2981 947d 9428 6805 8c12 5072 696e 7453  )..}.(h...PrintS
+00038190: 7461 7475 730a 3d3d 3d3d 3d3d 9468 075d  tatus.======.h.]
+000381a0: 9468 168c 1250 7269 6e74 5374 6174 7573  .h...PrintStatus
+000381b0: 0a3d 3d3d 3d3d 3d94 8594 8194 7d94 2868  .======.....}.(h
+000381c0: 0568 0668 1b6a 2154 0000 7562 6168 1f7d  .h.h.j!T..ubah.}
+000381d0: 9428 6821 5d94 6823 5d94 6825 5d94 6827  .(h!].h#].h%].h'
+000381e0: 5d94 6829 5d94 68c9 68ca 7568 2b6a 2b53  ].h)].h.h.uh+j+S
+000381f0: 0000 681b 6a11 5400 0075 6265 681f 7d94  ..h.j.T..ubeh.}.
+00038200: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00038210: 9468 295d 948c 056c 6576 656c 944b 028c  .h)]...level.K..
+00038220: 0474 7970 6594 6a43 5300 008c 046c 696e  .type.jCS....lin
+00038230: 6594 4b1d 8c06 736f 7572 6365 9468 2c75  e.K...source.h,u
+00038240: 682b 6a19 5300 0075 626a 1a53 0000 2981  h+j.S..ubj.S..).
+00038250: 947d 9428 6805 6806 6807 5d94 2868 4729  .}.(h.h.h.].(hG)
+00038260: 8194 7d94 2868 058c 1a54 6974 6c65 2075  ..}.(h...Title u
+00038270: 6e64 6572 6c69 6e65 2074 6f6f 2073 686f  nderline too sho
+00038280: 7274 2e94 6807 5d94 6816 8c1a 5469 746c  rt..h.].h...Titl
+00038290: 6520 756e 6465 726c 696e 6520 746f 6f20  e underline too 
+000382a0: 7368 6f72 742e 9485 9481 947d 9428 6805  short......}.(h.
+000382b0: 6806 681b 6a3c 5400 0068 1c68 0368 1d4e  h.h.j<T..h.h.h.N
+000382c0: 681e 4e75 6261 681f 7d94 2868 215d 9468  h.Nubah.}.(h!].h
+000382d0: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+000382e0: 682b 6846 681b 6a39 5400 0075 626a 2c53  h+hFh.j9T..ubj,S
+000382f0: 0000 2981 947d 9428 6805 8c12 5072 696e  ..)..}.(h...Prin
+00038300: 7453 7461 7475 730a 3d3d 3d3d 3d3d 9468  tStatus.======.h
+00038310: 075d 9468 168c 1250 7269 6e74 5374 6174  .].h...PrintStat
+00038320: 7573 0a3d 3d3d 3d3d 3d94 8594 8194 7d94  us.======.....}.
+00038330: 2868 0568 0668 1b6a 4a54 0000 7562 6168  (h.h.h.jJT..ubah
+00038340: 1f7d 9428 6821 5d94 6823 5d94 6825 5d94  .}.(h!].h#].h%].
+00038350: 6827 5d94 6829 5d94 68c9 68ca 7568 2b6a  h'].h)].h.h.uh+j
+00038360: 2b53 0000 681b 6a39 5400 0068 1d68 2c75  +S..h.j9T..h.h,u
+00038370: 6265 681f 7d94 2868 215d 9468 235d 9468  beh.}.(h!].h#].h
+00038380: 255d 9468 275d 9468 295d 948c 056c 6576  %].h'].h)]...lev
+00038390: 656c 944b 028c 0474 7970 6594 6a43 5300  el.K...type.jCS.
+000383a0: 008c 046c 696e 6594 4b1d 8c06 736f 7572  ...line.K...sour
+000383b0: 6365 9468 2c75 682b 6a19 5300 0068 1b6a  ce.h,uh+j.S..h.j
+000383c0: b739 0000 681c 6803 681d 682c 681e 4b1d  .9..h.h.h.h,h.K.
+000383d0: 7562 6a1a 5300 0029 8194 7d94 2868 0568  ubj.S..)..}.(h.h
+000383e0: 0668 075d 9428 6847 2981 947d 9428 6805  .h.].(hG)..}.(h.
+000383f0: 6806 6807 5d94 6816 8c1a 5469 746c 6520  h.h.].h...Title 
+00038400: 756e 6465 726c 696e 6520 746f 6f20 7368  underline too sh
+00038410: 6f72 742e 9485 9481 947d 9428 6805 6806  ort......}.(h.h.
+00038420: 681b 6a65 5400 0075 6261 681f 7d94 2868  h.jeT..ubah.}.(h
+00038430: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+00038440: 295d 9475 682b 6846 681b 6a62 5400 0075  )].uh+hFh.jbT..u
+00038450: 626a 2c53 0000 2981 947d 9428 6805 8c11  bj,S..)..}.(h...
+00038460: 4763 6f64 6553 7461 7465 0a3d 3d3d 3d3d  GcodeState.=====
+00038470: 3d94 6807 5d94 6816 8c11 4763 6f64 6553  =.h.].h...GcodeS
+00038480: 7461 7465 0a3d 3d3d 3d3d 3d94 8594 8194  tate.======.....
+00038490: 7d94 2868 0568 0668 1b6a 7254 0000 7562  }.(h.h.h.jrT..ub
+000384a0: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+000384b0: 5d94 6827 5d94 6829 5d94 68c9 68ca 7568  ].h'].h)].h.h.uh
+000384c0: 2b6a 2b53 0000 681b 6a62 5400 0075 6265  +j+S..h.jbT..ube
+000384d0: 681f 7d94 2868 215d 9468 235d 9468 255d  h.}.(h!].h#].h%]
+000384e0: 9468 275d 9468 295d 948c 056c 6576 656c  .h'].h)]...level
+000384f0: 944b 028c 0474 7970 6594 6a43 5300 008c  .K...type.jCS...
+00038500: 046c 696e 6594 4b23 8c06 736f 7572 6365  .line.K#..source
+00038510: 9468 2c75 682b 6a19 5300 0075 626a 1a53  .h,uh+j.S..ubj.S
+00038520: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+00038530: 2868 4729 8194 7d94 2868 058c 1a54 6974  (hG)..}.(h...Tit
+00038540: 6c65 2075 6e64 6572 6c69 6e65 2074 6f6f  le underline too
+00038550: 2073 686f 7274 2e94 6807 5d94 6816 8c1a   short..h.].h...
+00038560: 5469 746c 6520 756e 6465 726c 696e 6520  Title underline 
+00038570: 746f 6f20 7368 6f72 742e 9485 9481 947d  too short......}
+00038580: 9428 6805 6806 681b 6a8d 5400 0068 1c68  .(h.h.h.j.T..h.h
+00038590: 0368 1d4e 681e 4e75 6261 681f 7d94 2868  .h.Nh.Nubah.}.(h
+000385a0: 215d 9468 235d 9468 255d 9468 275d 9468  !].h#].h%].h'].h
+000385b0: 295d 9475 682b 6846 681b 6a8a 5400 0075  )].uh+hFh.j.T..u
+000385c0: 626a 2c53 0000 2981 947d 9428 6805 8c11  bj,S..)..}.(h...
+000385d0: 4763 6f64 6553 7461 7465 0a3d 3d3d 3d3d  GcodeState.=====
+000385e0: 3d94 6807 5d94 6816 8c11 4763 6f64 6553  =.h.].h...GcodeS
+000385f0: 7461 7465 0a3d 3d3d 3d3d 3d94 8594 8194  tate.======.....
+00038600: 7d94 2868 0568 0668 1b6a 9b54 0000 7562  }.(h.h.h.j.T..ub
+00038610: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00038620: 5d94 6827 5d94 6829 5d94 68c9 68ca 7568  ].h'].h)].h.h.uh
+00038630: 2b6a 2b53 0000 681b 6a8a 5400 0068 1d68  +j+S..h.j.T..h.h
+00038640: 2c75 6265 681f 7d94 2868 215d 9468 235d  ,ubeh.}.(h!].h#]
+00038650: 9468 255d 9468 275d 9468 295d 948c 056c  .h%].h'].h)]...l
+00038660: 6576 656c 944b 028c 0474 7970 6594 6a43  evel.K...type.jC
+00038670: 5300 008c 046c 696e 6594 4b23 8c06 736f  S....line.K#..so
+00038680: 7572 6365 9468 2c75 682b 6a19 5300 0068  urce.h,uh+j.S..h
+00038690: 1b6a d04e 0000 681c 6803 681d 682c 681e  .j.N..h.h.h.h,h.
+000386a0: 4b23 7562 658c 1274 7261 6e73 666f 726d  K#ube..transform
+000386b0: 5f6d 6573 7361 6765 7394 5d94 286a 1a53  _messages.].(j.S
+000386c0: 0000 2981 947d 9428 6805 6806 6807 5d94  ..)..}.(h.h.h.].
+000386d0: 6847 2981 947d 9428 6805 6806 6807 5d94  hG)..}.(h.h.h.].
+000386e0: 6816 8c42 4879 7065 726c 696e 6b20 7461  h..BHyperlink ta
+000386f0: 7267 6574 2022 6d6f 6475 6c65 2d62 616d  rget "module-bam
+00038700: 6275 6c61 6273 5f61 7069 2e50 7269 6e74  bulabs_api.Print
+00038710: 6572 2220 6973 206e 6f74 2072 6566 6572  er" is not refer
+00038720: 656e 6365 642e 9485 9481 947d 9428 6805  enced......}.(h.
+00038730: 6806 681b 6ab8 5400 0075 6261 681f 7d94  h.h.j.T..ubah.}.
+00038740: 2868 215d 9468 235d 9468 255d 9468 275d  (h!].h#].h%].h']
+00038750: 9468 295d 9475 682b 6846 681b 6ab5 5400  .h)].uh+hFh.j.T.
+00038760: 0075 6261 681f 7d94 2868 215d 9468 235d  .ubah.}.(h!].h#]
+00038770: 9468 255d 9468 275d 9468 295d 948c 056c  .h%].h'].h)]...l
+00038780: 6576 656c 944b 018c 0474 7970 6594 8c04  evel.K...type...
+00038790: 494e 464f 948c 0673 6f75 7263 6594 687c  INFO...source.h|
+000387a0: 8c04 6c69 6e65 944b 0175 682b 6a19 5300  ..line.K.uh+j.S.
+000387b0: 0075 626a 1a53 0000 2981 947d 9428 6805  .ubj.S..)..}.(h.
+000387c0: 6806 6807 5d94 6847 2981 947d 9428 6805  h.h.].hG)..}.(h.
+000387d0: 6806 6807 5d94 6816 8c43 4879 7065 726c  h.h.].h..CHyperl
+000387e0: 696e 6b20 7461 7267 6574 2022 6d6f 6475  ink target "modu
+000387f0: 6c65 2d62 616d 6275 6c61 6273 5f61 7069  le-bambulabs_api
+00038800: 2e46 696c 616d 656e 7422 2069 7320 6e6f  .Filament" is no
+00038810: 7420 7265 6665 7265 6e63 6564 2e94 8594  t referenced....
+00038820: 8194 7d94 2868 0568 0668 1b6a d354 0000  ..}.(h.h.h.j.T..
+00038830: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00038840: 6825 5d94 6827 5d94 6829 5d94 7568 2b68  h%].h'].h)].uh+h
+00038850: 4668 1b6a d054 0000 7562 6168 1f7d 9428  Fh.j.T..ubah.}.(
+00038860: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00038870: 6829 5d94 8c05 6c65 7665 6c94 4b01 8c04  h)]...level.K...
+00038880: 7479 7065 946a cd54 0000 8c06 736f 7572  type.j.T....sour
+00038890: 6365 946a 112c 0000 8c04 6c69 6e65 944b  ce.j.,....line.K
+000388a0: 0175 682b 6a19 5300 0075 626a 1a53 0000  .uh+j.S..ubj.S..
+000388b0: 2981 947d 9428 6805 6806 6807 5d94 6847  )..}.(h.h.h.].hG
+000388c0: 2981 947d 9428 6805 6806 6807 5d94 6816  )..}.(h.h.h.].h.
+000388d0: 8c4e 4879 7065 726c 696e 6b20 7461 7267  .NHyperlink targ
+000388e0: 6574 2022 6d6f 6475 6c65 2d62 616d 6275  et "module-bambu
+000388f0: 6c61 6273 5f61 7069 2e41 4d53 4669 6c61  labs_api.AMSFila
+00038900: 6d65 6e74 5365 7474 696e 6773 2220 6973  mentSettings" is
+00038910: 206e 6f74 2072 6566 6572 656e 6365 642e   not referenced.
+00038920: 9485 9481 947d 9428 6805 6806 681b 6aed  .....}.(h.h.h.j.
+00038930: 5400 0075 6261 681f 7d94 2868 215d 9468  T..ubah.}.(h!].h
+00038940: 235d 9468 255d 9468 275d 9468 295d 9475  #].h%].h'].h)].u
+00038950: 682b 6846 681b 6aea 5400 0075 6261 681f  h+hFh.j.T..ubah.
+00038960: 7d94 2868 215d 9468 235d 9468 255d 9468  }.(h!].h#].h%].h
+00038970: 275d 9468 295d 948c 056c 6576 656c 944b  '].h)]...level.K
+00038980: 018c 0474 7970 6594 6acd 5400 008c 0673  ...type.j.T....s
+00038990: 6f75 7263 6594 6a52 3700 008c 046c 696e  ource.jR7....lin
+000389a0: 6594 4b01 7568 2b6a 1953 0000 7562 6a1a  e.K.uh+j.S..ubj.
+000389b0: 5300 0029 8194 7d94 2868 0568 0668 075d  S..)..}.(h.h.h.]
+000389c0: 9468 4729 8194 7d94 2868 0568 0668 075d  .hG)..}.(h.h.h.]
+000389d0: 9468 168c 4648 7970 6572 6c69 6e6b 2074  .h..FHyperlink t
+000389e0: 6172 6765 7420 226d 6f64 756c 652d 6261  arget "module-ba
+000389f0: 6d62 756c 6162 735f 6170 692e 5072 696e  mbulabs_api.Prin
+00038a00: 7453 7461 7475 7322 2069 7320 6e6f 7420  tStatus" is not 
+00038a10: 7265 6665 7265 6e63 6564 2e94 8594 8194  referenced......
+00038a20: 7d94 2868 0568 0668 1b6a 0755 0000 7562  }.(h.h.h.j.U..ub
+00038a30: 6168 1f7d 9428 6821 5d94 6823 5d94 6825  ah.}.(h!].h#].h%
+00038a40: 5d94 6827 5d94 6829 5d94 7568 2b68 4668  ].h'].h)].uh+hFh
+00038a50: 1b6a 0455 0000 7562 6168 1f7d 9428 6821  .j.U..ubah.}.(h!
+00038a60: 5d94 6823 5d94 6825 5d94 6827 5d94 6829  ].h#].h%].h'].h)
+00038a70: 5d94 8c05 6c65 7665 6c94 4b01 8c04 7479  ]...level.K...ty
+00038a80: 7065 946a cd54 0000 8c06 736f 7572 6365  pe.j.T....source
+00038a90: 946a d339 0000 8c04 6c69 6e65 944b 0175  .j.9....line.K.u
+00038aa0: 682b 6a19 5300 0075 626a 1a53 0000 2981  h+j.S..ubj.S..).
+00038ab0: 947d 9428 6805 6806 6807 5d94 6847 2981  .}.(h.h.h.].hG).
+00038ac0: 947d 9428 6805 6806 6807 5d94 6816 8c45  .}.(h.h.h.].h..E
+00038ad0: 4879 7065 726c 696e 6b20 7461 7267 6574  Hyperlink target
+00038ae0: 2022 6d6f 6475 6c65 2d62 616d 6275 6c61   "module-bambula
+00038af0: 6273 5f61 7069 2e47 636f 6465 5374 6174  bs_api.GcodeStat
+00038b00: 6522 2069 7320 6e6f 7420 7265 6665 7265  e" is not refere
+00038b10: 6e63 6564 2e94 8594 8194 7d94 2868 0568  nced......}.(h.h
+00038b20: 0668 1b6a 2155 0000 7562 6168 1f7d 9428  .h.j!U..ubah.}.(
+00038b30: 6821 5d94 6823 5d94 6825 5d94 6827 5d94  h!].h#].h%].h'].
+00038b40: 6829 5d94 7568 2b68 4668 1b6a 1e55 0000  h)].uh+hFh.j.U..
+00038b50: 7562 6168 1f7d 9428 6821 5d94 6823 5d94  ubah.}.(h!].h#].
+00038b60: 6825 5d94 6827 5d94 6829 5d94 8c05 6c65  h%].h'].h)]...le
+00038b70: 7665 6c94 4b01 8c04 7479 7065 946a cd54  vel.K...type.j.T
+00038b80: 0000 8c06 736f 7572 6365 946a ec4e 0000  ....source.j.N..
+00038b90: 8c04 6c69 6e65 944b 0175 682b 6a19 5300  ..line.K.uh+j.S.
+00038ba0: 0075 6265 8c0b 7472 616e 7366 6f72 6d65  .ube..transforme
+00038bb0: 7294 4e8c 0b69 6e63 6c75 6465 5f6c 6f67  r.N..include_log
+00038bc0: 945d 948c 0a64 6563 6f72 6174 696f 6e94  .]...decoration.
+00038bd0: 4e68 1c68 0375 622e                      Nh.h.ub.
```

### Comparing `bambulabs_api-2.1.5/docs/_sources/index.rst.txt` & `bambulabs_api-2.1.6/docs/_sources/index.rst.txt`

 * *Files 19% similar despite different names*

```diff
@@ -25,8 +25,14 @@
   :members:
   :imported-members:
 
 PrintStatus
 ======
 .. automodule:: bambulabs_api.PrintStatus
   :members:
+  :imported-members:
+
+GcodeState
+======
+.. automodule:: bambulabs_api.GcodeState
+  :members:
   :imported-members:
```

### Comparing `bambulabs_api-2.1.5/docs/_static/_sphinx_javascript_frameworks_compat.js` & `bambulabs_api-2.1.6/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/basic.css` & `bambulabs_api-2.1.6/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/badge_only.css` & `bambulabs_api-2.1.6/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.eot` & `bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.svg` & `bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.ttf` & `bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff2` & `bambulabs_api-2.1.6/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/css/theme.css` & `bambulabs_api-2.1.6/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/doctools.js` & `bambulabs_api-2.1.6/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/jquery-3.6.0.js` & `bambulabs_api-2.1.6/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/jquery.js` & `bambulabs_api-2.1.6/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/js/badge_only.js` & `bambulabs_api-2.1.6/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/js/html5shiv-printshiv.min.js` & `bambulabs_api-2.1.6/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/js/html5shiv.min.js` & `bambulabs_api-2.1.6/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/js/theme.js` & `bambulabs_api-2.1.6/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/language_data.js` & `bambulabs_api-2.1.6/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/pygments.css` & `bambulabs_api-2.1.6/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/searchtools.js` & `bambulabs_api-2.1.6/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/underscore-1.13.1.js` & `bambulabs_api-2.1.6/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/_static/underscore.js` & `bambulabs_api-2.1.6/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/doc_conf/index.rst` & `bambulabs_api-2.1.6/docs/doc_conf/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -25,8 +25,14 @@
   :members:
   :imported-members:
 
 PrintStatus
 ======
 .. automodule:: bambulabs_api.PrintStatus
   :members:
+  :imported-members:
+
+GcodeState
+======
+.. automodule:: bambulabs_api.GcodeState
+  :members:
   :imported-members:
```

### Comparing `bambulabs_api-2.1.5/docs/genindex.html` & `bambulabs_api-2.1.6/docs/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,21 @@
     bambulabs_api.Filament
 
       <ul>
         <li><a href="index.html#module-bambulabs_api.Filament">module</a>
 </li>
       </ul></li>
       <li>
+    bambulabs_api.GcodeState
+
+      <ul>
+        <li><a href="index.html#module-bambulabs_api.GcodeState">module</a>
+</li>
+      </ul></li>
+      <li>
     bambulabs_api.Printer
 
       <ul>
         <li><a href="index.html#module-bambulabs_api.Printer">module</a>
 </li>
       </ul></li>
       <li>
@@ -191,14 +198,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.PrintStatus.FILAMENT_LOADING">FILAMENT_LOADING (in module bambulabs_api.PrintStatus)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.PrintStatus.FILAMENT_UNLOADING">FILAMENT_UNLOADING (in module bambulabs_api.PrintStatus)</a>
 </li>
+      <li><a href="index.html#bambulabs_api.GcodeState.FINISHED">FINISHED (in module bambulabs_api.GcodeState)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="G">G</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.Printer.get_bed_temperature">get_bed_temperature() (in module bambulabs_api.Printer)</a>
@@ -241,18 +250,22 @@
 </tr></table>
 
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.PrintStatus.IDENTIFYING_BUILD_PLATE_TYPE">IDENTIFYING_BUILD_PLATE_TYPE (in module bambulabs_api.PrintStatus)</a>
 </li>
+      <li><a href="index.html#bambulabs_api.GcodeState.IDLE">IDLE (in module bambulabs_api.GcodeState)</a>
+
+      <ul>
+        <li><a href="index.html#bambulabs_api.PrintStatus.IDLE">(in module bambulabs_api.PrintStatus)</a>
+</li>
+      </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="index.html#bambulabs_api.PrintStatus.IDLE">IDLE (in module bambulabs_api.PrintStatus)</a>
-</li>
       <li><a href="index.html#bambulabs_api.PrintStatus.INSPECTING_FIRST_LAYER">INSPECTING_FIRST_LAYER (in module bambulabs_api.PrintStatus)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="L">L</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -271,14 +284,16 @@
     module
 
       <ul>
         <li><a href="index.html#module-bambulabs_api.AMSFilamentSettings">bambulabs_api.AMSFilamentSettings</a>
 </li>
         <li><a href="index.html#module-bambulabs_api.Filament">bambulabs_api.Filament</a>
 </li>
+        <li><a href="index.html#module-bambulabs_api.GcodeState">bambulabs_api.GcodeState</a>
+</li>
         <li><a href="index.html#module-bambulabs_api.Printer">bambulabs_api.Printer</a>
 </li>
         <li><a href="index.html#module-bambulabs_api.PrintStatus">bambulabs_api.PrintStatus</a>
 </li>
       </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
@@ -306,14 +321,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.Filament.PA">PA (in module bambulabs_api.Filament)</a>
 </li>
       <li><a href="index.html#bambulabs_api.Filament.PA_CF">PA_CF (in module bambulabs_api.Filament)</a>
 </li>
       <li><a href="index.html#bambulabs_api.Printer.pause_print">pause_print() (in module bambulabs_api.Printer)</a>
 </li>
+      <li><a href="index.html#bambulabs_api.GcodeState.PAUSED">PAUSED (in module bambulabs_api.GcodeState)</a>
+</li>
       <li><a href="index.html#bambulabs_api.PrintStatus.PAUSED_AMS_LOST">PAUSED_AMS_LOST (in module bambulabs_api.PrintStatus)</a>
 </li>
       <li><a href="index.html#bambulabs_api.PrintStatus.PAUSED_CHAMBER_TEMPERATURE_CONTROL_ERROR">PAUSED_CHAMBER_TEMPERATURE_CONTROL_ERROR (in module bambulabs_api.PrintStatus)</a>
 </li>
       <li><a href="index.html#bambulabs_api.PrintStatus.PAUSED_CUTTER_ERROR">PAUSED_CUTTER_ERROR (in module bambulabs_api.PrintStatus)</a>
 </li>
       <li><a href="index.html#bambulabs_api.PrintStatus.PAUSED_FILAMENT_RUNOUT">PAUSED_FILAMENT_RUNOUT (in module bambulabs_api.PrintStatus)</a>
@@ -348,14 +365,16 @@
 </li>
       <li><a href="index.html#bambulabs_api.Filament.PLA_CF">PLA_CF (in module bambulabs_api.Filament)</a>
 </li>
       <li><a href="index.html#bambulabs_api.Filament.POLYLITE_PLA">POLYLITE_PLA (in module bambulabs_api.Filament)</a>
 </li>
       <li><a href="index.html#bambulabs_api.Filament.POLYTERRA_PLA">POLYTERRA_PLA (in module bambulabs_api.Filament)</a>
 </li>
+      <li><a href="index.html#bambulabs_api.GcodeState.PREPARING">PREPARING (in module bambulabs_api.GcodeState)</a>
+</li>
       <li><a href="index.html#bambulabs_api.PrintStatus.PRINTING">PRINTING (in module bambulabs_api.PrintStatus)</a>
 </li>
       <li><a href="index.html#bambulabs_api.Filament.PVA">PVA (in module bambulabs_api.Filament)</a>
 </li>
   </ul></td>
 </tr></table>
 
@@ -364,14 +383,16 @@
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.Printer.resume_print">resume_print() (in module bambulabs_api.Printer)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.Printer.retry_filament_action">retry_filament_action() (in module bambulabs_api.Printer)</a>
 </li>
+      <li><a href="index.html#bambulabs_api.GcodeState.RUNNING">RUNNING (in module bambulabs_api.GcodeState)</a>
+</li>
   </ul></td>
 </tr></table>
 
 <h2 id="S">S</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.PrintStatus.SCANNING_BED_SURFACE">SCANNING_BED_SURFACE (in module bambulabs_api.PrintStatus)</a>
@@ -416,16 +437,20 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="U">U</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="index.html#bambulabs_api.PrintStatus.UNKNOWN">UNKNOWN (in module bambulabs_api.PrintStatus)</a>
+      <li><a href="index.html#bambulabs_api.GcodeState.UNKNOWN">UNKNOWN (in module bambulabs_api.GcodeState)</a>
+
+      <ul>
+        <li><a href="index.html#bambulabs_api.PrintStatus.UNKNOWN">(in module bambulabs_api.PrintStatus)</a>
 </li>
+      </ul></li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="index.html#bambulabs_api.Printer.unload_filament_spool">unload_filament_spool() (in module bambulabs_api.Printer)</a>
 </li>
       <li><a href="index.html#bambulabs_api.Printer.upload_file">upload_file() (in module bambulabs_api.Printer)</a>
 </li>
   </ul></td>
```

#### html2text {}

```diff
@@ -8,20 +8,20 @@
 ********** AA **********
     * _A_B_S_ _(_i_n_ _m_o_d_u_l_e              * _A_S_A_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)     * _A_U_T_O___B_E_D___L_E_V_E_L_I_N_G_ _(_i_n_ _m_o_d_u_l_e
                                     _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
 ********** BB **********
     * _B_A_M_B_U___A_B_S_ _(_i_n_ _m_o_d_u_l_e                  * bambulabs_api.Filament
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)                     o _m_o_d_u_l_e
-    * _B_A_M_B_U___P_A___C_F_ _(_i_n_ _m_o_d_u_l_e                * bambulabs_api.Printer
+    * _B_A_M_B_U___P_A___C_F_ _(_i_n_ _m_o_d_u_l_e                * bambulabs_api.GcodeState
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)                     o _m_o_d_u_l_e
-    * _B_A_M_B_U___P_C_ _(_i_n_ _m_o_d_u_l_e                   * bambulabs_api.PrintStatus
+    * _B_A_M_B_U___P_C_ _(_i_n_ _m_o_d_u_l_e                   * bambulabs_api.Printer
+      _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)                     o _m_o_d_u_l_e
+    * _B_A_M_B_U___P_L_A___B_a_s_i_c_ _(_i_n_ _m_o_d_u_l_e            * bambulabs_api.PrintStatus
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)                     o _m_o_d_u_l_e
-    * _B_A_M_B_U___P_L_A___B_a_s_i_c_ _(_i_n_ _m_o_d_u_l_e
-      _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
     * _B_A_M_B_U___P_L_A___M_a_t_t_e_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
     * _B_A_M_B_U___T_P_U___9_5_A_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
     * bambulabs_api.AMSFilamentSettings
           o _m_o_d_u_l_e
 ********** CC **********
@@ -39,14 +39,16 @@
                                               _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
 ********** DD **********
     * _d_e_l_e_t_e___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e     * _d_i_s_c_o_n_n_e_c_t_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)         _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
 ********** FF **********
     * _F_I_L_A_M_E_N_T___L_O_A_D_I_N_G_ _(_i_n_ _m_o_d_u_l_e     * _F_I_L_A_M_E_N_T___U_N_L_O_A_D_I_N_G_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)        _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
+                                      * _F_I_N_I_S_H_E_D_ _(_i_n_ _m_o_d_u_l_e
+                                        _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e_)
 ********** GG **********
     * _g_e_t___b_e_d___t_e_m_p_e_r_a_t_u_r_e_(_)_ _(_i_n_ _m_o_d_u_l_e     * _g_e_t___n_o_z_z_l_e___t_e_m_p_e_r_a_t_u_r_e_(_)_ _(_i_n
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)                 _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
     * _g_e_t___c_a_m_e_r_a___f_r_a_m_e_(_)_ _(_i_n_ _m_o_d_u_l_e        * _g_e_t___p_e_r_c_e_n_t_a_g_e_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)                 _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
     * _g_e_t___f_i_l_e___n_a_m_e_(_)_ _(_i_n_ _m_o_d_u_l_e           * _g_e_t___p_r_i_n_t___s_p_e_e_d_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)                 _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
@@ -56,57 +58,64 @@
                                              _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
 ********** HH **********
     * _H_E_A_T_B_E_D___P_R_E_H_E_A_T_I_N_G_ _(_i_n_ _m_o_d_u_l_e     * _h_o_m_e___p_r_i_n_t_e_r_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)          _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
     * _H_E_A_T_I_N_G___H_O_T_E_N_D_ _(_i_n_ _m_o_d_u_l_e         * _H_O_M_I_N_G___T_O_O_L_H_E_A_D_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)          _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
 ********** II **********
-    * _I_D_E_N_T_I_F_Y_I_N_G___B_U_I_L_D___P_L_A_T_E___T_Y_P_E_ _(_i_n      * _I_D_L_E_ _(_i_n_ _m_o_d_u_l_e
+    * _I_D_E_N_T_I_F_Y_I_N_G___B_U_I_L_D___P_L_A_T_E___T_Y_P_E_ _(_i_n      * _I_N_S_P_E_C_T_I_N_G___F_I_R_S_T___L_A_Y_E_R_ _(_i_n_ _m_o_d_u_l_e
       _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
-                                            * _I_N_S_P_E_C_T_I_N_G___F_I_R_S_T___L_A_Y_E_R_ _(_i_n_ _m_o_d_u_l_e
-                                              _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
+    * _I_D_L_E_ _(_i_n_ _m_o_d_u_l_e
+      _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e_)
+          o _(_i_n_ _m_o_d_u_l_e
+            _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
 ********** LL **********
     * _l_o_a_d___f_i_l_a_m_e_n_t___s_p_o_o_l_(_)_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
 ********** MM **********
     * _M_4_0_0___P_A_U_S_E_ _(_i_n_ _m_o_d_u_l_e                       * _M_O_T_O_R___N_O_I_S_E___S_H_O_W_O_F_F_ _(_i_n
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                    _m_o_d_u_l_e
     * module                                        _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
           o _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s     * _m_o_v_e___z___a_x_i_s_(_)_ _(_i_n_ _m_o_d_u_l_e
           o _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t                  _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
+          o _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e
           o _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r
           o _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s
 ********** NN **********
     * _n_o_z_z_l_e___t_e_m_p___m_a_x_ _(_i_n_ _m_o_d_u_l_e             * _n_o_z_z_l_e___t_e_m_p___m_i_n_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s_)       _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s_)
 ********** PP **********
     * _P_A_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)        * _P_A_U_S_E_D___N_O_Z_Z_L_E___F_I_L_A_M_E_N_T___C_O_V_E_R_E_D___D_E_T_E_C_T_E_D
     * _P_A___C_F_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)       _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
     * _p_a_u_s_e___p_r_i_n_t_(_)_ _(_i_n_ _m_o_d_u_l_e                     * _P_A_U_S_E_D___N_O_Z_Z_L_E___T_E_M_P_E_R_A_T_U_R_E___M_A_L_F_U_N_C_T_I_O_N_ 
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)                         _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
-    * _P_A_U_S_E_D___A_M_S___L_O_S_T_ _(_i_n_ _m_o_d_u_l_e                   * _P_A_U_S_E_D___S_K_I_P_P_E_D___S_T_E_P_ _(_i_n_ _m_o_d_u_l_e
+    * _P_A_U_S_E_D_ _(_i_n_ _m_o_d_u_l_e                            * _P_A_U_S_E_D___S_K_I_P_P_E_D___S_T_E_P_ _(_i_n_ _m_o_d_u_l_e
+      _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e_)                      _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
+    * _P_A_U_S_E_D___A_M_S___L_O_S_T_ _(_i_n_ _m_o_d_u_l_e                   * _P_A_U_S_E_D___U_S_E_R_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                     _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
-    * _P_A_U_S_E_D___C_H_A_M_B_E_R___T_E_M_P_E_R_A_T_U_R_E___C_O_N_T_R_O_L___E_R_R_O_R     * _P_A_U_S_E_D___U_S_E_R_ _(_i_n_ _m_o_d_u_l_e
+    * _P_A_U_S_E_D___C_H_A_M_B_E_R___T_E_M_P_E_R_A_T_U_R_E___C_O_N_T_R_O_L___E_R_R_O_R     * _P_A_U_S_E_D___U_S_E_R___G_C_O_D_E_ _(_i_n_ _m_o_d_u_l_e
       _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)          _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
-    * _P_A_U_S_E_D___C_U_T_T_E_R___E_R_R_O_R_ _(_i_n_ _m_o_d_u_l_e               * _P_A_U_S_E_D___U_S_E_R___G_C_O_D_E_ _(_i_n_ _m_o_d_u_l_e
-      _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                     _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
-    * _P_A_U_S_E_D___F_I_L_A_M_E_N_T___R_U_N_O_U_T_ _(_i_n_ _m_o_d_u_l_e            * _P_C_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
+    * _P_A_U_S_E_D___C_U_T_T_E_R___E_R_R_O_R_ _(_i_n_ _m_o_d_u_l_e               * _P_C_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                   * _P_E_T_G_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
-    * _P_A_U_S_E_D___F_I_R_S_T___L_A_Y_E_R___E_R_R_O_R_ _(_i_n_ _m_o_d_u_l_e          * _P_L_A_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
+    * _P_A_U_S_E_D___F_I_L_A_M_E_N_T___R_U_N_O_U_T_ _(_i_n_ _m_o_d_u_l_e            * _P_L_A_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                   * _P_L_A___C_F_ _(_i_n_ _m_o_d_u_l_e
-    * _P_A_U_S_E_D___F_R_O_N_T___C_O_V_E_R___F_A_L_L_I_N_G_ _(_i_n_ _m_o_d_u_l_e          _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
+    * _P_A_U_S_E_D___F_I_R_S_T___L_A_Y_E_R___E_R_R_O_R_ _(_i_n_ _m_o_d_u_l_e            _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                   * _P_O_L_Y_L_I_T_E___P_L_A_ _(_i_n_ _m_o_d_u_l_e
+    * _P_A_U_S_E_D___F_R_O_N_T___C_O_V_E_R___F_A_L_L_I_N_G_ _(_i_n_ _m_o_d_u_l_e          _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
+      _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                   * _P_O_L_Y_T_E_R_R_A___P_L_A_ _(_i_n_ _m_o_d_u_l_e
     * _P_A_U_S_E_D___H_E_A_T___B_E_D___T_E_M_P_E_R_A_T_U_R_E___M_A_L_F_U_N_C_T_I_O_N_        _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
-      _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)        * _P_O_L_Y_T_E_R_R_A___P_L_A_ _(_i_n_ _m_o_d_u_l_e
-    * _P_A_U_S_E_D___L_O_W___F_A_N___S_P_E_E_D___H_E_A_T___B_R_E_A_K_ _(_i_n            _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
+      _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)        * _P_R_E_P_A_R_I_N_G_ _(_i_n_ _m_o_d_u_l_e
+    * _P_A_U_S_E_D___L_O_W___F_A_N___S_P_E_E_D___H_E_A_T___B_R_E_A_K_ _(_i_n            _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e_)
       _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)            * _P_R_I_N_T_I_N_G_ _(_i_n_ _m_o_d_u_l_e
     * _P_A_U_S_E_D___N_O_Z_Z_L_E___C_L_O_G_ _(_i_n_ _m_o_d_u_l_e                  _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)                   * _P_V_A_ _(_i_n_ _m_o_d_u_l_e_ _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
 ********** RR **********
     * _r_e_s_u_m_e___p_r_i_n_t_(_)_ _(_i_n_ _m_o_d_u_l_e     * _r_e_t_r_y___f_i_l_a_m_e_n_t___a_c_t_i_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)          _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
+                                    * _R_U_N_N_I_N_G_ _(_i_n_ _m_o_d_u_l_e
+                                      _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e_)
 ********** SS **********
     * _S_C_A_N_N_I_N_G___B_E_D___S_U_R_F_A_C_E_ _(_i_n_ _m_o_d_u_l_e       * _s_t_a_r_t___p_r_i_n_t_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)              _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
     * _s_e_t___b_e_d___t_e_m_p_e_r_a_t_u_r_e_(_)_ _(_i_n_ _m_o_d_u_l_e      * _s_t_o_p___p_r_i_n_t_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)                  _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
     * _s_e_t___f_i_l_a_m_e_n_t___p_r_i_n_t_e_r_(_)_ _(_i_n_ _m_o_d_u_l_e     * _S_U_P_P_O_R_T___G_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)                  _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)
@@ -118,14 +127,14 @@
     * _T_P_U_ _(_i_n_ _m_o_d_u_l_e                         * _t_r_a_y___t_y_p_e_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t_)                  _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s_)
     * _t_r_a_y___i_n_f_o___i_d_x_ _(_i_n_ _m_o_d_u_l_e               * _t_u_r_n___l_i_g_h_t___o_f_f_(_)_ _(_i_n_ _m_o_d_u_l_e
       _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s_)       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
                                              * _t_u_r_n___l_i_g_h_t___o_n_(_)_ _(_i_n_ _m_o_d_u_l_e
                                                _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
 ********** UU **********
-    * _U_N_K_N_O_W_N_ _(_i_n_ _m_o_d_u_l_e             * _u_n_l_o_a_d___f_i_l_a_m_e_n_t___s_p_o_o_l_(_)_ _(_i_n_ _m_o_d_u_l_e
-      _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
-                                     * _u_p_l_o_a_d___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e
-                                       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
+    * _U_N_K_N_O_W_N_ _(_i_n_ _m_o_d_u_l_e                   * _u_n_l_o_a_d___f_i_l_a_m_e_n_t___s_p_o_o_l_(_)_ _(_i_n_ _m_o_d_u_l_e
+      _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e_)              _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
+          o _(_i_n_ _m_o_d_u_l_e                     * _u_p_l_o_a_d___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e
+            _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s_)       _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r_)
 ===============================================================================
 © Copyright .
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `bambulabs_api-2.1.5/docs/index.html` & `bambulabs_api-2.1.6/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
               <div class="local-toc"><ul>
 <li><a class="reference internal" href="#">BambuLabs API</a></li>
 <li><a class="reference internal" href="#description">Description</a></li>
 <li><a class="reference internal" href="#printer">Printer</a></li>
 <li><a class="reference internal" href="#filament">Filament</a></li>
 <li><a class="reference internal" href="#amsfilamentsettings">AMSFilamentSettings</a></li>
 <li><a class="reference internal" href="#printstatus">PrintStatus</a></li>
+<li><a class="reference internal" href="#gcodestate">GcodeState</a></li>
 </ul>
 </div>
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -1155,14 +1156,79 @@
 <dt class="field-odd">Type</dt>
 <dd class="field-odd"><p>The printer is idle.</p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
+<section id="gcodestate">
+<h1>GcodeState<a class="headerlink" href="#gcodestate" title="Permalink to this heading"></a></h1>
+<span class="target" id="module-bambulabs_api.GcodeState"></span><p>Enum class for the Gcode State</p>
+<p>Gcode State that the printer can be in.</p>
+<dl class="py attribute">
+<dt class="sig sig-object py" id="bambulabs_api.GcodeState.IDLE">
+<span class="sig-prename descclassname"><span class="pre">bambulabs_api.GcodeState.</span></span><span class="sig-name descname"><span class="pre">IDLE</span></span><a class="headerlink" href="#bambulabs_api.GcodeState.IDLE" title="Permalink to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Type</dt>
+<dd class="field-odd"><p>The printer is idle.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="bambulabs_api.GcodeState.PREPARING">
+<span class="sig-prename descclassname"><span class="pre">bambulabs_api.GcodeState.</span></span><span class="sig-name descname"><span class="pre">PREPARING</span></span><a class="headerlink" href="#bambulabs_api.GcodeState.PREPARING" title="Permalink to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Type</dt>
+<dd class="field-odd"><p>The printer is preparing (File upload).</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="bambulabs_api.GcodeState.RUNNING">
+<span class="sig-prename descclassname"><span class="pre">bambulabs_api.GcodeState.</span></span><span class="sig-name descname"><span class="pre">RUNNING</span></span><a class="headerlink" href="#bambulabs_api.GcodeState.RUNNING" title="Permalink to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Type</dt>
+<dd class="field-odd"><p>The printer is running.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="bambulabs_api.GcodeState.PAUSED">
+<span class="sig-prename descclassname"><span class="pre">bambulabs_api.GcodeState.</span></span><span class="sig-name descname"><span class="pre">PAUSED</span></span><a class="headerlink" href="#bambulabs_api.GcodeState.PAUSED" title="Permalink to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Type</dt>
+<dd class="field-odd"><p>The printer is paused.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="bambulabs_api.GcodeState.FINISHED">
+<span class="sig-prename descclassname"><span class="pre">bambulabs_api.GcodeState.</span></span><span class="sig-name descname"><span class="pre">FINISHED</span></span><a class="headerlink" href="#bambulabs_api.GcodeState.FINISHED" title="Permalink to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Type</dt>
+<dd class="field-odd"><p>The printer has finished.</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="bambulabs_api.GcodeState.UNKNOWN">
+<span class="sig-prename descclassname"><span class="pre">bambulabs_api.GcodeState.</span></span><span class="sig-name descname"><span class="pre">UNKNOWN</span></span><a class="headerlink" href="#bambulabs_api.GcodeState.UNKNOWN" title="Permalink to this definition"></a></dt>
+<dd><dl class="field-list simple">
+<dt class="field-odd">Type</dt>
+<dd class="field-odd"><p>The printer state is unknown.</p>
+</dd>
+</dl>
+</dd></dl>
+
+</section>
 
 
            </div>
           </div>
           <footer>
 
   <hr/>
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 [q                   ]
     * _B_a_m_b_u_L_a_b_s_ _A_P_I
     * _D_e_s_c_r_i_p_t_i_o_n
     * _P_r_i_n_t_e_r
     * _F_i_l_a_m_e_n_t
     * _A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s
     * _P_r_i_n_t_S_t_a_t_u_s
+    * _G_c_o_d_e_S_t_a_t_e
 _B_a_m_b_u_L_a_b_s_ _A_P_I
     * BambuLabs API
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ BBaammbbuuLLaabbss AAPPII_? ************
 ************ DDeessccrriippttiioonn_? ************
 API for accessing information for a printer, including the status of the
@@ -408,10 +409,31 @@
             The printer is paused due to a nozzle clog.
   bambulabs_api.PrintStatus.UNKNOWN_
         Type
             The printer status is unknown.
   bambulabs_api.PrintStatus.IDLE_
         Type
             The printer is idle.
+************ GGccooddeeSSttaattee_? ************
+Enum class for the Gcode State
+Gcode State that the printer can be in.
+  bambulabs_api.GcodeState.IDLE_
+        Type
+            The printer is idle.
+  bambulabs_api.GcodeState.PREPARING_
+        Type
+            The printer is preparing (File upload).
+  bambulabs_api.GcodeState.RUNNING_
+        Type
+            The printer is running.
+  bambulabs_api.GcodeState.PAUSED_
+        Type
+            The printer is paused.
+  bambulabs_api.GcodeState.FINISHED_
+        Type
+            The printer has finished.
+  bambulabs_api.GcodeState.UNKNOWN_
+        Type
+            The printer state is unknown.
 ===============================================================================
 © Copyright .
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `bambulabs_api-2.1.5/docs/py-modindex.html` & `bambulabs_api-2.1.6/docs/py-modindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,19 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="index.html#module-bambulabs_api.Filament"><code class="xref">bambulabs_api.Filament</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="index.html#module-bambulabs_api.GcodeState"><code class="xref">bambulabs_api.GcodeState</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="index.html#module-bambulabs_api.Printer"><code class="xref">bambulabs_api.Printer</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="index.html#module-bambulabs_api.PrintStatus"><code class="xref">bambulabs_api.PrintStatus</code></a></td><td>
        <em></em></td></tr>
```

#### html2text {}

```diff
@@ -6,12 +6,13 @@
 ************ PPyytthhoonn MMoodduullee IInnddeexx ************
 _bb
      
     bb
 [-] bambulabs_api
         _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s
         _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t
+        _b_a_m_b_u_l_a_b_s___a_p_i_._G_c_o_d_e_S_t_a_t_e
         _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r
         _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s
 ===============================================================================
 © Copyright .
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `bambulabs_api-2.1.5/docs/search.html` & `bambulabs_api-2.1.6/docs/search.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/docs/searchindex.js` & `bambulabs_api-2.1.6/docs/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -146,15 +146,15 @@
         "enum": 0,
         "red": [],
         "blue": [],
         "green": [],
         "them": [],
         "attribut": [],
         "lookup": [],
-        "can": [],
+        "can": 0,
         "iter": [],
         "over": [],
         "know": [],
         "how": [],
         "mani": [],
         "member": [],
         "thei": [],
@@ -287,20 +287,25 @@
         "paused_nozzle_filament_covered_detect": 0,
         "detect": 0,
         "paused_cutter_error": 0,
         "cutter": 0,
         "paused_first_layer_error": 0,
         "paused_nozzle_clog": 0,
         "clog": 0,
-        "idl": 0
+        "idl": 0,
+        "prepar": 0,
+        "run": 0,
+        "finish": 0,
+        "ha": 0
     },
     "objects": {
         "bambulabs_api": [
             [0, 0, 0, "-", "AMSFilamentSettings"],
             [0, 0, 0, "-", "Filament"],
+            [0, 0, 0, "-", "GcodeState"],
             [0, 0, 0, "-", "PrintStatus"],
             [0, 0, 0, "-", "Printer"]
         ],
         "bambulabs_api.AMSFilamentSettings": [
             [0, 1, 1, "", "nozzle_temp_max"],
             [0, 1, 1, "", "nozzle_temp_min"],
             [0, 1, 1, "", "tray_info_idx"],
@@ -324,14 +329,22 @@
             [0, 1, 1, "", "POLYLITE_PLA"],
             [0, 1, 1, "", "POLYTERRA_PLA"],
             [0, 1, 1, "", "PVA"],
             [0, 1, 1, "", "SUPPORT_G"],
             [0, 1, 1, "", "SUPPORT_W"],
             [0, 1, 1, "", "TPU"]
         ],
+        "bambulabs_api.GcodeState": [
+            [0, 1, 1, "", "FINISHED"],
+            [0, 1, 1, "", "IDLE"],
+            [0, 1, 1, "", "PAUSED"],
+            [0, 1, 1, "", "PREPARING"],
+            [0, 1, 1, "", "RUNNING"],
+            [0, 1, 1, "", "UNKNOWN"]
+        ],
         "bambulabs_api.PrintStatus": [
             [0, 1, 1, "", "AUTO_BED_LEVELING"],
             [0, 1, 1, "", "CALIBRATING_EXTRUSION"],
             [0, 1, 1, "", "CALIBRATING_EXTRUSION_FLOW"],
             [0, 1, 1, "", "CALIBRATING_LIDAR"],
             [0, 1, 1, "", "CALIBRATING_MICRO_LIDAR"],
             [0, 1, 1, "", "CALIBRATING_MOTOR_NOISE"],
@@ -414,15 +427,16 @@
         "bambulab": 0,
         "api": 0,
         "descript": 0,
         "client": [],
         "printer": 0,
         "filament": 0,
         "amsfilamentset": 0,
-        "printstatu": 0
+        "printstatu": 0,
+        "gcodest": 0
     },
     "envversion": {
         "sphinx.domains.c": 2,
         "sphinx.domains.changeset": 1,
         "sphinx.domains.citation": 1,
         "sphinx.domains.cpp": 6,
         "sphinx.domains.index": 1,
```

### Comparing `bambulabs_api-2.1.5/examples/Basic/basic.py` & `bambulabs_api-2.1.6/examples/Basic/basic.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.5/pyproject.toml` & `bambulabs_api-2.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bambulabs_api"
-version = "2.1.5"
+version = "2.1.6"
 authors = [
   { name="Chris Ioannidis", email="chris.ioannidis23@imperial.ac.uk" },
 ]
 description = "API for BambuLabs 3D Printers over MQTT"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `bambulabs_api-2.1.5/setup.py` & `bambulabs_api-2.1.6/setup.py`

 * *Files identical despite different names*

