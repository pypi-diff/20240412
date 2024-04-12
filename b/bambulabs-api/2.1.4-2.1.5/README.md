# Comparing `tmp/bambulabs_api-2.1.4.tar.gz` & `tmp/bambulabs_api-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambulabs_api-2.1.4.tar", last modified: Fri Apr 12 18:41:32 2024, max compression
+gzip compressed data, was "bambulabs_api-2.1.5.tar", last modified: Fri Apr 12 19:00:22 2024, max compression
```

## Comparing `bambulabs_api-2.1.4.tar` & `bambulabs_api-2.1.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.682098 bambulabs_api-2.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.658098 bambulabs_api-2.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.662098 bambulabs_api-2.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/.github/workflows/pytest-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 18:41:32.682098 bambulabs_api-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.666098 bambulabs_api-2.1.4/bambulabs_api/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/camera_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/filament_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/ftp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/bambulabs_api/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.678098 bambulabs_api-2.1.4/bambulabs_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 18:41:32.000000 bambulabs_api-2.1.4/bambulabs_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 18:41:32.000000 bambulabs_api-2.1.4/bambulabs_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:41:32.000000 bambulabs_api-2.1.4/bambulabs_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 18:41:32.000000 bambulabs_api-2.1.4/bambulabs_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 18:41:32.000000 bambulabs_api-2.1.4/bambulabs_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.666098 bambulabs_api-2.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.666098 bambulabs_api-2.1.4/docs/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   220931 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/.doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.666098 bambulabs_api-2.1.4/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.670098 bambulabs_api-2.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.670098 bambulabs_api-2.1.4/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.678098 bambulabs_api-2.1.4/docs/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.678098 bambulabs_api-2.1.4/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.678098 bambulabs_api-2.1.4/docs/doc_conf/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/doc_conf/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/doc_conf/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    74797 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/docs/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.662098 bambulabs_api-2.1.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.678098 bambulabs_api-2.1.4/examples/Basic/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/examples/Basic/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:41:32.682098 bambulabs_api-2.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:41:32.678098 bambulabs_api-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 18:41:25.000000 bambulabs_api-2.1.4/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.822347 bambulabs_api-2.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.826347 bambulabs_api-2.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/pytest-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.826347 bambulabs_api-2.1.5/bambulabs_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/filament_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/ftp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12376 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/bambulabs_api/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/bambulabs_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 19:00:22.000000 bambulabs_api-2.1.5/bambulabs_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.830347 bambulabs_api-2.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.830347 bambulabs_api-2.1.5/docs/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   220931 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/.doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.830347 bambulabs_api-2.1.5/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.834347 bambulabs_api-2.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.834347 bambulabs_api-2.1.5/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.838347 bambulabs_api-2.1.5/docs/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/docs/doc_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/doc_conf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/doc_conf/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    74797 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/docs/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.826347 bambulabs_api-2.1.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/examples/Basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/examples/Basic/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:00:22.842347 bambulabs_api-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 19:00:15.000000 bambulabs_api-2.1.5/tests/test_client.py
```

### Comparing `bambulabs_api-2.1.4/.github/workflows/flake8.yml` & `bambulabs_api-2.1.5/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/.github/workflows/publish.yml` & `bambulabs_api-2.1.5/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,18 @@
         with:
           inputs: ./dist/*.tar.gz ./dist/*.whl
       - name: Install dependencies
         run: python3 -m pip install toml
       - name: Get version from pyproject.toml file
         id: get_version
         run: |
+          cd $GITHUB_WORKSPACE
           version=$(python3 -c "import toml; print(toml.load('pyproject.toml')['project']['version'])")
           echo "VERSION=${version}" >> $GITHUB_ENV
       - name: Create GitHub Release
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: gh release create "${{ env.VERSION }}" --repo "${{ github.repository }}" --notes ""
       - name: Upload artifact signatures to GitHub Release
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: gh release upload "${{ env.VERSION }}" dist/** --repo "${{ github.repository }}"
-
```

### Comparing `bambulabs_api-2.1.4/.github/workflows/pytest-unit-tests.yml` & `bambulabs_api-2.1.5/.github/workflows/pytest-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/.github/workflows/static.yml` & `bambulabs_api-2.1.5/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/.gitignore` & `bambulabs_api-2.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/LICENSE` & `bambulabs_api-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/PKG-INFO` & `bambulabs_api-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.1.4
+Version: 2.1.5
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
```

### Comparing `bambulabs_api-2.1.4/README.md` & `bambulabs_api-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/bambulabs_api/camera_client.py` & `bambulabs_api-2.1.5/bambulabs_api/camera_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/bambulabs_api/client.py` & `bambulabs_api-2.1.5/bambulabs_api/client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/bambulabs_api/filament_info.py` & `bambulabs_api-2.1.5/bambulabs_api/filament_info.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/bambulabs_api/ftp_client.py` & `bambulabs_api-2.1.5/bambulabs_api/ftp_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/bambulabs_api/mqtt_client.py` & `bambulabs_api-2.1.5/bambulabs_api/mqtt_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         Get the remaining time for the print
 
         Returns:
             int | str | None: The remaining time for the print
         """
         return self.__get("mc_remaining_time", None)
 
-    def get_printer_state(self) -> PrintStatus:
+    def get_printer_state(self) -> GcodeState:
         """
         Get the printer state
 
         Returns:
             PrintStatus: printer state
         """
         return GcodeState(self.__get("gcode_state", -1))
@@ -227,26 +227,26 @@
     def pause_print(self) -> bool:
         """
         Pause the print
 
         Returns:
             str: print_status
         """
-        if self.get_printer_state() == "PAUSED":
+        if self.get_printer_state() == GcodeState.PAUSED:
             return True
         return self.__publish_command({"print": {"command": "pause"}})
 
     def resume_print(self) -> bool:
         """
         Resume the print
 
         Returns:
             str: print_status
         """
-        if self.get_printer_state() == "RUNNING":
+        if self.get_printer_state() == GcodeState.RUNNING:
             return True
         return self.__publish_command({"print": {"command": "resume"}})
 
     def __send_gcode_line(self, gcode_command: str) -> bool:
         """
         Send a G-code line command to the printer
```

### Comparing `bambulabs_api-2.1.4/bambulabs_api/states_info.py` & `bambulabs_api-2.1.5/bambulabs_api/states_info.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/bambulabs_api.egg-info/PKG-INFO` & `bambulabs_api-2.1.5/bambulabs_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.1.4
+Version: 2.1.5
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
```

### Comparing `bambulabs_api-2.1.4/bambulabs_api.egg-info/SOURCES.txt` & `bambulabs_api-2.1.5/bambulabs_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/.doctrees/environment.pickle` & `bambulabs_api-2.1.5/docs/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/.doctrees/index.doctree` & `bambulabs_api-2.1.5/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_sources/index.rst.txt` & `bambulabs_api-2.1.5/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/_sphinx_javascript_frameworks_compat.js` & `bambulabs_api-2.1.5/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/basic.css` & `bambulabs_api-2.1.5/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/badge_only.css` & `bambulabs_api-2.1.5/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.eot` & `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.svg` & `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.ttf` & `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/fontawesome-webfont.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold-italic.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold-italic.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-bold.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal-italic.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal-italic.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal.woff` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/fonts/lato-normal.woff2` & `bambulabs_api-2.1.5/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/css/theme.css` & `bambulabs_api-2.1.5/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/doctools.js` & `bambulabs_api-2.1.5/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/jquery-3.6.0.js` & `bambulabs_api-2.1.5/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/jquery.js` & `bambulabs_api-2.1.5/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/js/badge_only.js` & `bambulabs_api-2.1.5/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/js/html5shiv-printshiv.min.js` & `bambulabs_api-2.1.5/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/js/html5shiv.min.js` & `bambulabs_api-2.1.5/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/js/theme.js` & `bambulabs_api-2.1.5/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/language_data.js` & `bambulabs_api-2.1.5/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/pygments.css` & `bambulabs_api-2.1.5/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/searchtools.js` & `bambulabs_api-2.1.5/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/underscore-1.13.1.js` & `bambulabs_api-2.1.5/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/_static/underscore.js` & `bambulabs_api-2.1.5/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/doc_conf/index.rst` & `bambulabs_api-2.1.5/docs/doc_conf/index.rst`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/genindex.html` & `bambulabs_api-2.1.5/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/index.html` & `bambulabs_api-2.1.5/docs/index.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/objects.inv` & `bambulabs_api-2.1.5/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/py-modindex.html` & `bambulabs_api-2.1.5/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/search.html` & `bambulabs_api-2.1.5/docs/search.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/docs/searchindex.js` & `bambulabs_api-2.1.5/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/examples/Basic/basic.py` & `bambulabs_api-2.1.5/examples/Basic/basic.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.1.4/pyproject.toml` & `bambulabs_api-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bambulabs_api"
-version = "2.1.4"
+version = "2.1.5"
 authors = [
   { name="Chris Ioannidis", email="chris.ioannidis23@imperial.ac.uk" },
 ]
 description = "API for BambuLabs 3D Printers over MQTT"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `bambulabs_api-2.1.4/setup.py` & `bambulabs_api-2.1.5/setup.py`

 * *Files identical despite different names*

