# Comparing `tmp/bambulabs_api-2.0.0.tar.gz` & `tmp/bambulabs_api-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambulabs_api-2.0.0.tar", last modified: Fri Apr 12 15:39:08 2024, max compression
+gzip compressed data, was "bambulabs_api-2.1.tar", last modified: Fri Apr 12 17:26:11 2024, max compression
```

## Comparing `bambulabs_api-2.0.0.tar` & `bambulabs_api-2.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.193301 bambulabs_api-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.197301 bambulabs_api-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/.github/workflows/pytest-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.197301 bambulabs_api-2.0.0/bambulabs_api/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/camera_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/filament_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/ftp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/bambulabs_api/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/bambulabs_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-12 15:39:08.000000 bambulabs_api-2.0.0/bambulabs_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-12 15:39:08.000000 bambulabs_api-2.0.0/bambulabs_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:39:08.000000 bambulabs_api-2.0.0/bambulabs_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 15:39:08.000000 bambulabs_api-2.0.0/bambulabs_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.201301 bambulabs_api-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.201301 bambulabs_api-2.0.0/docs/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (127)    17592 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   114695 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/.doctrees/index.doctree
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.201301 bambulabs_api-2.0.0/docs/_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_sources/index.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.205301 bambulabs_api-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.205301 bambulabs_api-2.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.209301 bambulabs_api-2.0.0/docs/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/_static/underscore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/docs/doc_conf/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/doc_conf/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/doc_conf/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/genindex.html
--rw-r--r--   0 runner    (1001) docker     (127)    40258 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/objects.inv
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/search.html
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/docs/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.197301 bambulabs_api-2.0.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/examples/Basic/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/examples/Basic/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:39:08.213302 bambulabs_api-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 15:39:01.000000 bambulabs_api-2.0.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.411842 bambulabs_api-2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.387842 bambulabs_api-2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.391842 bambulabs_api-2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 17:26:04.000000 bambulabs_api-2.1/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-12 17:26:04.000000 bambulabs_api-2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 17:26:04.000000 bambulabs_api-2.1/.github/workflows/pytest-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-12 17:26:04.000000 bambulabs_api-2.1/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-12 17:26:04.000000 bambulabs_api-2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 17:26:04.000000 bambulabs_api-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-12 17:26:11.411842 bambulabs_api-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-12 17:26:04.000000 bambulabs_api-2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.391842 bambulabs_api-2.1/bambulabs_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/camera_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11939 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/filament_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/ftp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-12 17:26:04.000000 bambulabs_api-2.1/bambulabs_api/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.411842 bambulabs_api-2.1/bambulabs_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-12 17:26:11.000000 bambulabs_api-2.1/bambulabs_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-12 17:26:11.000000 bambulabs_api-2.1/bambulabs_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:26:11.000000 bambulabs_api-2.1/bambulabs_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 17:26:11.000000 bambulabs_api-2.1/bambulabs_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.395842 bambulabs_api-2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.395842 bambulabs_api-2.1/docs/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (127)    31161 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   220931 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/.doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.395842 bambulabs_api-2.1/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.399842 bambulabs_api-2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.399842 bambulabs_api-2.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/badge_only.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.407842 bambulabs_api-2.1/docs/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    87624 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    86288 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    66444 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   131657 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)    89501 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.407842 bambulabs_api-2.1/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68420 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19530 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/_static/underscore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.407842 bambulabs_api-2.1/docs/doc_conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/doc_conf/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/doc_conf/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)    74797 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-04-12 17:26:04.000000 bambulabs_api-2.1/docs/searchindex.js
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 17:26:04.000000 bambulabs_api-2.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.387842 bambulabs_api-2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.407842 bambulabs_api-2.1/examples/Basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 17:26:04.000000 bambulabs_api-2.1/examples/Basic/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-12 17:26:04.000000 bambulabs_api-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 17:26:04.000000 bambulabs_api-2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:26:11.411842 bambulabs_api-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 17:26:04.000000 bambulabs_api-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:11.407842 bambulabs_api-2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 17:26:04.000000 bambulabs_api-2.1/tests/test_client.py
```

### Comparing `bambulabs_api-2.0.0/.github/workflows/flake8.yml` & `bambulabs_api-2.1/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/.github/workflows/publish.yml` & `bambulabs_api-2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/.github/workflows/pytest-unit-tests.yml` & `bambulabs_api-2.1/.github/workflows/pytest-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/.github/workflows/static.yml` & `bambulabs_api-2.1/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/.gitignore` & `bambulabs_api-2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/LICENSE` & `bambulabs_api-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/PKG-INFO` & `bambulabs_api-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.0.0
+Version: 2.1.0
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
```

### Comparing `bambulabs_api-2.0.0/README.md` & `bambulabs_api-2.1/README.md`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/bambulabs_api/camera_client.py` & `bambulabs_api-2.1/bambulabs_api/camera_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/bambulabs_api/client.py` & `bambulabs_api-2.1/bambulabs_api/client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/bambulabs_api/ftp_client.py` & `bambulabs_api-2.1/bambulabs_api/ftp_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/bambulabs_api/mqtt_client.py` & `bambulabs_api-2.1/bambulabs_api/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/bambulabs_api.egg-info/PKG-INFO` & `bambulabs_api-2.1/bambulabs_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambulabs_api
-Version: 2.0.0
+Version: 2.1.0
 Summary: API for BambuLabs 3D Printers over MQTT
 Home-page: https://github.com/acse-ci223/bambulabs_api
 Author: Chris Ioannidis
 Author-email: Chris Ioannidis <chris.ioannidis23@imperial.ac.uk>
 Project-URL: Homepage, https://github.com/acse-ci223/bambulabs_api
 Project-URL: Docs, https://acse-ci223.github.io/bambulabs_api/
 Project-URL: Issues, https://github.com/acse-ci223/bambulabs_api/issues
```

### Comparing `bambulabs_api-2.0.0/bambulabs_api.egg-info/SOURCES.txt` & `bambulabs_api-2.1/bambulabs_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/_sphinx_javascript_frameworks_compat.js` & `bambulabs_api-2.1/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/basic.css` & `bambulabs_api-2.1/docs/_static/basic.css`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,24 @@
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
+a.brackets:before,
+span.brackets > a:before{
+    content: "[";
+}
+
+a.brackets:after,
+span.brackets > a:after {
+    content: "]";
+}
+
 
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
@@ -320,25 +330,19 @@
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
-nav.contents,
-aside.topic,
-
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
-nav.contents,
-aside.topic,
-
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -369,27 +373,21 @@
     margin-top: 25px;
 }
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
 aside.sidebar > :last-child,
-nav.contents > :last-child,
-aside.topic > :last-child,
-
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
 aside.sidebar::after,
-nav.contents::after,
-aside.topic::after,
-
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
```

### Comparing `bambulabs_api-2.0.0/docs/_static/css/badge_only.css` & `bambulabs_api-2.1/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.eot` & `bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.svg` & `bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.ttf` & `bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/fontawesome-webfont.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold-italic.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold-italic.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-bold.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal-italic.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal-italic.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal.woff` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/fonts/lato-normal.woff2` & `bambulabs_api-2.1/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/css/theme.css` & `bambulabs_api-2.1/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/doctools.js` & `bambulabs_api-2.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/jquery-3.6.0.js` & `bambulabs_api-2.1/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/jquery.js` & `bambulabs_api-2.1/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/js/badge_only.js` & `bambulabs_api-2.1/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/js/html5shiv-printshiv.min.js` & `bambulabs_api-2.1/docs/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/js/html5shiv.min.js` & `bambulabs_api-2.1/docs/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/js/theme.js` & `bambulabs_api-2.1/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/language_data.js` & `bambulabs_api-2.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/pygments.css` & `bambulabs_api-2.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/searchtools.js` & `bambulabs_api-2.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/underscore-1.13.1.js` & `bambulabs_api-2.1/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/_static/underscore.js` & `bambulabs_api-2.1/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/docs/py-modindex.html` & `bambulabs_api-2.1/docs/py-modindex.html`

 * *Files 15% similar despite different names*

```diff
@@ -79,16 +79,31 @@
               id="toggle-1" style="display: none" alt="-" /></td>
        <td>
        <code class="xref">bambulabs_api</code></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="index.html#module-bambulabs_api.AMSFilamentSettings"><code class="xref">bambulabs_api.AMSFilamentSettings</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="index.html#module-bambulabs_api.Filament"><code class="xref">bambulabs_api.Filament</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="index.html#module-bambulabs_api.Printer"><code class="xref">bambulabs_api.Printer</code></a></td><td>
        <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="index.html#module-bambulabs_api.PrintStatus"><code class="xref">bambulabs_api.PrintStatus</code></a></td><td>
+       <em></em></td></tr>
    </table>
 
 
            </div>
           </div>
           <footer>
```

#### html2text {}

```diff
@@ -4,11 +4,14 @@
     * Python Module Index
 ===============================================================================
 ************ PPyytthhoonn MMoodduullee IInnddeexx ************
 _bb
      
     bb
 [-] bambulabs_api
+        _b_a_m_b_u_l_a_b_s___a_p_i_._A_M_S_F_i_l_a_m_e_n_t_S_e_t_t_i_n_g_s
+        _b_a_m_b_u_l_a_b_s___a_p_i_._F_i_l_a_m_e_n_t
         _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_e_r
+        _b_a_m_b_u_l_a_b_s___a_p_i_._P_r_i_n_t_S_t_a_t_u_s
 ===============================================================================
 © Copyright .
 Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `bambulabs_api-2.0.0/docs/search.html` & `bambulabs_api-2.1/docs/search.html`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/examples/Basic/basic.py` & `bambulabs_api-2.1/examples/Basic/basic.py`

 * *Files identical despite different names*

### Comparing `bambulabs_api-2.0.0/pyproject.toml` & `bambulabs_api-2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bambulabs_api"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Chris Ioannidis", email="chris.ioannidis23@imperial.ac.uk" },
 ]
 description = "API for BambuLabs 3D Printers over MQTT"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

