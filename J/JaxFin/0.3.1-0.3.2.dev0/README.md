# Comparing `tmp/JaxFin-0.3.1.tar.gz` & `tmp/JaxFin-0.3.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JaxFin-0.3.1.tar", last modified: Sat Apr  6 09:48:20 2024, max compression
+gzip compressed data, was "JaxFin-0.3.2.dev0.tar", last modified: Fri Apr 12 16:00:42 2024, max compression
```

## Comparing `JaxFin-0.3.1.tar` & `JaxFin-0.3.2.dev0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.829982 JaxFin-0.3.1/
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.562607 JaxFin-0.3.1/.github/
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.615667 JaxFin-0.3.1/.github/workflows/
--rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 JaxFin-0.3.1/.github/workflows/linting.yml
--rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.3.1/.github/workflows/pytest.yml
--rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.3.1/.github/workflows/quality_check.yml
--rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 JaxFin-0.3.1/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.635396 JaxFin-0.3.1/.idea/
--rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/.gitignore
--rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.3.1/.idea/aws.xml
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.639024 JaxFin-0.3.1/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.3.1/.idea/misc.xml
--rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.3.1/.idea/other.xml
--rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.3.1/.idea/py-exopricer.iml
--rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.3.1/.idea/vcs.xml
--rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.3.1/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.824372 JaxFin-0.3.1/JaxFin.egg-info/
--rw-rw-rw-   0        0        0     7516 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 09:48:20.000000 JaxFin-0.3.1/JaxFin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      637 2024-04-03 15:58:34.000000 JaxFin-0.3.1/Makefile
--rw-rw-rw-   0        0        0     7516 2024-04-06 09:48:20.824889 JaxFin-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 JaxFin-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.688881 JaxFin-0.3.1/jaxfin/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.1/jaxfin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.697180 JaxFin-0.3.1/jaxfin/models/
--rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.3.1/jaxfin/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.704643 JaxFin-0.3.1/jaxfin/models/gbm/
--rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.3.1/jaxfin/models/gbm/__init__.py
--rw-rw-rw-   0        0        0     7604 2024-03-07 14:43:03.000000 JaxFin-0.3.1/jaxfin/models/gbm/gbm.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.708969 JaxFin-0.3.1/jaxfin/models/heston/
--rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 JaxFin-0.3.1/jaxfin/models/heston/__init__.py
--rw-rw-rw-   0        0        0    13095 2024-04-06 09:45:45.000000 JaxFin-0.3.1/jaxfin/models/heston/heston.py
--rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 JaxFin-0.3.1/jaxfin/models/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.714704 JaxFin-0.3.1/jaxfin/price_engine/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.1/jaxfin/price_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.721935 JaxFin-0.3.1/jaxfin/price_engine/black/
--rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.3.1/jaxfin/price_engine/black/__init__.py
--rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/black/black_model.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.727440 JaxFin-0.3.1/jaxfin/price_engine/black_scholes/
--rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.3.1/jaxfin/price_engine/black_scholes/__init__.py
--rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/black_scholes/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.733550 JaxFin-0.3.1/jaxfin/price_engine/fft/
--rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 JaxFin-0.3.1/jaxfin/price_engine/fft/__init__.py
--rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 JaxFin-0.3.1/jaxfin/price_engine/fft/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.746681 JaxFin-0.3.1/jaxfin/price_engine/math/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/math/__init__.py
--rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/math/bs_common.py
--rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/math/norm.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.750194 JaxFin-0.3.1/jaxfin/price_engine/utils/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/utils/__init__.py
--rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/utils/arrays.py
--rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.3.1/jaxfin/price_engine/utils/vect.py
--rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.3.1/noxfile.py
--rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 JaxFin-0.3.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.763558 JaxFin-0.3.1/requirements/
--rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 JaxFin-0.3.1/requirements/build.txt
--rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 JaxFin-0.3.1/requirements/dev.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.798155 JaxFin-0.3.1/scripts/
--rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.3.1/scripts/basedir.bat
--rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.3.1/scripts/black-reformat.bat
--rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.3.1/scripts/check-black.bat
--rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.3.1/scripts/configure-python.bat
--rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.3.1/scripts/create-new-version.bat
--rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.3.1/scripts/get-tests-cov.bat
--rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 JaxFin-0.3.1/scripts/run-linter.bat
--rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.3.1/scripts/run-mypy.bat
--rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.3.1/scripts/run-tests.bat
--rw-rw-rw-   0        0        0       42 2024-04-06 09:48:20.831192 JaxFin-0.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.800184 JaxFin-0.3.1/tests/
--rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.3.1/tests/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.800184 JaxFin-0.3.1/tests/models/
--rw-rw-rw-   0        0        0     1760 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/models/test_gbm.py
--rw-rw-rw-   0        0        0     3374 2024-04-06 09:45:45.000000 JaxFin-0.3.1/tests/models/test_heston.py
-drwxrwxrwx   0        0        0        0 2024-04-06 09:48:20.818668 JaxFin-0.3.1/tests/price_engine/
--rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/price_engine/test_black.py
--rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/price_engine/test_bs.py
--rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 JaxFin-0.3.1/tests/price_engine/test_fft.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.726980 JaxFin-0.3.2.dev0/
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.230162 JaxFin-0.3.2.dev0/.github/
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.331615 JaxFin-0.3.2.dev0/.github/workflows/
+-rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 JaxFin-0.3.2.dev0/.github/workflows/linting.yml
+-rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.3.2.dev0/.github/workflows/pytest.yml
+-rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/.github/workflows/quality_check.yml
+-rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 JaxFin-0.3.2.dev0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.402893 JaxFin-0.3.2.dev0/.idea/
+-rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/.gitignore
+-rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.3.2.dev0/.idea/aws.xml
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.414401 JaxFin-0.3.2.dev0/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.3.2.dev0/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.3.2.dev0/.idea/other.xml
+-rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.3.2.dev0/.idea/py-exopricer.iml
+-rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.3.2.dev0/.idea/vcs.xml
+-rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.3.2.dev0/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.715816 JaxFin-0.3.2.dev0/JaxFin.egg-info/
+-rw-rw-rw-   0        0        0     7521 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-04-12 16:00:42.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-12 16:00:41.000000 JaxFin-0.3.2.dev0/JaxFin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.3.2.dev0/LICENSE
+-rw-rw-rw-   0        0        0      660 2024-04-12 15:55:17.000000 JaxFin-0.3.2.dev0/Makefile
+-rw-rw-rw-   0        0        0     7521 2024-04-12 16:00:42.715816 JaxFin-0.3.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.470896 JaxFin-0.3.2.dev0/jaxfin/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.2.dev0/jaxfin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.476555 JaxFin-0.3.2.dev0/jaxfin/models/
+-rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.3.2.dev0/jaxfin/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.510543 JaxFin-0.3.2.dev0/jaxfin/models/gbm/
+-rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.3.2.dev0/jaxfin/models/gbm/__init__.py
+-rw-rw-rw-   0        0        0     7604 2024-03-07 14:43:03.000000 JaxFin-0.3.2.dev0/jaxfin/models/gbm/gbm.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.515813 JaxFin-0.3.2.dev0/jaxfin/models/heston/
+-rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 JaxFin-0.3.2.dev0/jaxfin/models/heston/__init__.py
+-rw-rw-rw-   0        0        0    11977 2024-04-12 15:56:31.000000 JaxFin-0.3.2.dev0/jaxfin/models/heston/heston.py
+-rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 JaxFin-0.3.2.dev0/jaxfin/models/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.518954 JaxFin-0.3.2.dev0/jaxfin/price_engine/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.525551 JaxFin-0.3.2.dev0/jaxfin/price_engine/black/
+-rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black/__init__.py
+-rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black/black_model.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.531700 JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/
+-rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/__init__.py
+-rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.537226 JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/
+-rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/__init__.py
+-rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.546009 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/__init__.py
+-rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/bs_common.py
+-rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/math/norm.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.552376 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/__init__.py
+-rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/arrays.py
+-rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/vect.py
+-rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.3.2.dev0/noxfile.py
+-rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 JaxFin-0.3.2.dev0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.577593 JaxFin-0.3.2.dev0/requirements/
+-rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 JaxFin-0.3.2.dev0/requirements/build.txt
+-rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 JaxFin-0.3.2.dev0/requirements/dev.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.692484 JaxFin-0.3.2.dev0/scripts/
+-rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.3.2.dev0/scripts/basedir.bat
+-rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.3.2.dev0/scripts/black-reformat.bat
+-rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.3.2.dev0/scripts/check-black.bat
+-rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.3.2.dev0/scripts/configure-python.bat
+-rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.3.2.dev0/scripts/create-new-version.bat
+-rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.3.2.dev0/scripts/get-tests-cov.bat
+-rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 JaxFin-0.3.2.dev0/scripts/run-linter.bat
+-rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.3.2.dev0/scripts/run-mypy.bat
+-rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.3.2.dev0/scripts/run-tests.bat
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:00:42.726980 JaxFin-0.3.2.dev0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.692484 JaxFin-0.3.2.dev0/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.3.2.dev0/tests/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.705422 JaxFin-0.3.2.dev0/tests/models/
+-rw-rw-rw-   0        0        0     1760 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/models/test_gbm.py
+-rw-rw-rw-   0        0        0     3396 2024-04-12 15:50:02.000000 JaxFin-0.3.2.dev0/tests/models/test_heston.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:00:42.715433 JaxFin-0.3.2.dev0/tests/price_engine/
+-rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/price_engine/test_black.py
+-rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/price_engine/test_bs.py
+-rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 JaxFin-0.3.2.dev0/tests/price_engine/test_fft.py
```

### Comparing `JaxFin-0.3.1/.github/workflows/linting.yml` & `JaxFin-0.3.2.dev0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/.github/workflows/pytest.yml` & `JaxFin-0.3.2.dev0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/.github/workflows/quality_check.yml` & `JaxFin-0.3.2.dev0/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/CONTRIBUTING.md` & `JaxFin-0.3.2.dev0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/JaxFin.egg-info/PKG-INFO` & `JaxFin-0.3.2.dev0/JaxFin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.3.1
+Version: 0.3.2.dev0
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `JaxFin-0.3.1/JaxFin.egg-info/SOURCES.txt` & `JaxFin-0.3.2.dev0/JaxFin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/LICENSE` & `JaxFin-0.3.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/Makefile` & `JaxFin-0.3.2.dev0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 SHELL=/bin/bash
 LINT_PATHS=jaxfin/ tests/
 
 pytest:
 	python -m pytest --no-header -vv --html=test_report.html --self-contained-html
 
+pylint:
+	pylint jaxfin --output-format=text:pylint_res.txt,colorized
+
 type: 
 	mypy ${LINT_PATHS}
 
 lint:
 	ruff check jaxfin --output-format=full
 
-complete-lint:
-	lint
-	pylint jaxfin --output-format=text:pylint_res.txt,colorized
+lint-complete: lint pylint
 
 format:
 	isort ${LINT_PATHS}
 	black ${LINT_PATHS}
 
 check-codestyle:
 	black ${LINT_PATHS} --check
@@ -27,8 +28,8 @@
 	python -m build
 	twine upload dist/*
 
 test-release: 
 	python -m build
 	twine upload dist/* -r testpypi
 
-.PHONY: clean spelling doc lint format check-codestyle commit-checks
+.PHONY: clean spelling doc lint format check-codestyle commit-checks pylint
```

### Comparing `JaxFin-0.3.1/PKG-INFO` & `JaxFin-0.3.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.3.1
+Version: 0.3.2.dev0
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `JaxFin-0.3.1/README.md` & `JaxFin-0.3.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/models/gbm/gbm.py` & `JaxFin-0.3.2.dev0/jaxfin/models/gbm/gbm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/models/heston/heston.py` & `JaxFin-0.3.2.dev0/jaxfin/models/heston/heston.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Heston model class implementation
 """
 from typing import Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
-from jax import jit, random
+import numpy as np
 
 from ..utils import check_symmetric
 
 
 class UnivHestonModel:
     """
     Univariate Heston Model
@@ -132,42 +132,59 @@
 
         Returns:
             jax.numpy.dtype: The underlying dtype of the Heston model
         """
         return self._dtype
 
     def sample_paths(
-        self, seed: int, maturity: float, n: int, n_sim: int
+        self, maturity: float, n: int, n_sim: int
     ) -> Tuple[jax.Array, jax.Array]:
         """
         Sample of paths from the Univariate Heston model
 
         Args:
             seed (int): the seed for the random number generator
             maturity (float): The time in years
             n (int): Number of steps (discretization points)
             n_sim (int): The number of simulations
 
         Returns:
             Tuple[jax.Array, jax.Array]: The simulated paths of the asset and the variance process
         """
-        key = random.PRNGKey(seed)
+        dt = maturity / (n - 1)
+        dt_sq = np.sqrt(dt)
 
-        dt = maturity / n
+        assert 2 * self.kappa * self.theta > self.sigma**2  # Feller condition
 
-        W = random.normal(key, shape=(n_sim, n)).T
-        Z = (
-            self._rho
-            * W
-            * jnp.sqrt(1 - self._rho**2)
-            * random.normal(key, shape=(n_sim, n)).T
-        )
+        # Generate random Brownian Motions for all paths and time steps
+        W_1 = np.random.normal(loc=0, scale=1, size=(n_sim, n - 1))
+        W_2 = np.random.normal(loc=0, scale=1, size=(n_sim, n - 1))
+        W_v = W_1
+        W_S = self._rho * W_1 + np.sqrt(1 - self._rho**2) * W_2
+
+        # Initialize arrays to store trajectories
+        v_paths = np.zeros((n_sim, n))
+        S_paths = np.zeros((n_sim, n))
+        v_paths[:, 0] = self._v0
+        S_paths[:, 0] = self._s0
+
+        # Compute trajectories of v and S using vectorized operations
+        for t in range(1, n):
+            v_paths[:, t] = np.abs(
+                v_paths[:, t - 1]
+                + self._kappa * (self._theta - v_paths[:, t - 1]) * dt
+                + self._sigma * np.sqrt(v_paths[:, t - 1]) * dt_sq * W_v[:, t - 1]
+            )
+            S_paths[:, t] = S_paths[:, t - 1] * np.exp(
+                (self._mean - 0.5 * v_paths[:, t - 1]) * dt
+                + np.sqrt(v_paths[:, t - 1]) * dt_sq * W_S[:, t - 1]
+            )
 
-        return _sample_paths(
-            self.s0, self.v0, self.mean, self.kappa, self.theta, self.sigma, dt, W, Z, n
+        return jnp.asarray(S_paths.T, dtype=self._dtype), jnp.asarray(
+            v_paths.T, dtype=self._dtype
         )
 
 
 class MultiHestonModel:
     """Multivariate Heston Model
 
     Represent a multi-dimensional Heston model
@@ -290,131 +307,48 @@
 
         Returns:
             jax.numpy.dtype: The underlying dtype of the Heston model
         """
         return self._dtype
 
     def sample_paths(
-        self, seed: int, maturity: float, n: int, n_sim: int
+        self, maturity: float, n: int, n_sim: int
     ) -> Tuple[jax.Array, jax.Array]:
         """Sample paths from the Multivariate Heston model
 
         Args:
             seed (int): The seed for the random number generator
             maturity (float): The time in years
             n (int): The number of steps
             n_sim (int): The number of simulations
 
         Returns:
             Tuple[jax.Array, jax.Array]: The simulated paths and the variance processes of the assets
         """
-        key = random.PRNGKey(seed)
-
         dt = maturity / n
+        dt_sq = np.sqrt(dt)
 
-        W = random.normal(key, shape=(n_sim, n * self._dim))
-        Z = random.normal(key, shape=(n_sim, n * self._dim))
-        W = jnp.reshape(W, (n_sim, n, self._dim)).transpose((1, 0, 2))
-        Z = jnp.reshape(Z, (n_sim, n, self._dim)).transpose((1, 0, 2))
-
-        L = jnp.linalg.cholesky(self._corr)
-
-        epsilon_S = W @ L
-        epsilon_v = epsilon_S @ self._corr + Z @ jnp.sqrt(1 - self._corr**2)
-
-        return _sample_paths(
-            self.s0,
-            self.v0,
-            self.mean,
-            self.kappa,
-            self.theta,
-            self.sigma,
-            dt,
-            epsilon_S,
-            epsilon_v,
-            n,
-        )
-
-
-# Helpers
-
+        W_1 = np.random.normal(loc=0, scale=1, size=(n_sim, n - 1, self._dim))
+        W_2 = np.random.normal(loc=0, scale=1, size=(n_sim, n - 1, self._dim))
+        W_v = W_1
+        W_S = W_1 @ self._corr + W_2 @ np.sqrt(1 - self._corr**2)
+
+        v_paths = np.zeros((n_sim, n, self._dim))
+        S_paths = np.zeros((n_sim, n, self._dim))
+        v_paths[:, 0, :] = self._v0
+        S_paths[:, 0, :] = self._s0
+
+        # Compute trajectories of v and S using vectorized operations
+        for t in range(1, n):
+            v_paths[:, t, :] = np.abs(
+                v_paths[:, t - 1, :]
+                + self._kappa * (self._theta - v_paths[:, t - 1, :]) * dt
+                + self._sigma * np.sqrt(v_paths[:, t - 1, :]) * dt_sq * W_v[:, t - 1, :]
+            )
+            S_paths[:, t, :] = S_paths[:, t - 1, :] * np.exp(
+                (self._mean - 0.5 * v_paths[:, t - 1, :]) * dt
+                + np.sqrt(v_paths[:, t - 1, :]) * dt_sq * W_S[:, t - 1, :]
+            )
 
-def _variance_process_step(
-    v: jax.Array,
-    kappa: jax.Array,
-    theta: jax.Array,
-    sigma: jax.Array,
-    dt: jax.Array,
-    dZ: jax.Array,
-) -> jax.Array:
-    return (
-        v
-        + kappa * (theta - jnp.maximum(v, 0.0)) * dt
-        + sigma * jnp.sqrt(jnp.maximum(v, 0.0)) * jnp.sqrt(dt) * dZ
-    )
-
-
-@jit
-def _sample_paths(
-    s0: jax.Array,
-    v0: jax.Array,
-    mean: jax.Array,
-    kappa: jax.Array,
-    theta: jax.Array,
-    sigma: jax.Array,
-    dt: jax.Array,
-    W: jax.Array,
-    Z: jax.Array,
-    N: int,
-) -> Tuple[jax.Array, jax.Array]:
-    """Main function that simulate the path of the Heston model leveragin the
-       jax.lax.while_loop function that allows to perform a loop in a jax makes
-       it useful for reducing compilation times for jit-compiled functions,
-       since native Python loop constructs in an @jit function are unrolled,
-       leading to large XLA computations.
-
-    Args:
-        s0 (jax.Array): The initial price of the stock(s)
-        v0 (jax.Array): The initial variance of the stock(s)
-        mean (jax.Array): The mean of the stock(s)
-        kappa (jax.Array): The speed of the mean-reversion of the variance
-        theta (jax.Array): The long-term mean of the variance
-        sigma (jax.Array): The volatility of the variance of the stock(s)
-        dt (jax.Array): The time step
-        W (jax.Array): The Weiner process of the stock(s)
-        Z (jax.Array): The (correlated) Weiner process of the variance of the stock(s)
-        N (int): The number of steps
-
-    Returns:
-        Tuple[jax.Array, jax.Array]: The simulated paths of the stock(s), and the variance process(es)
-    """
-
-    def init_fn(W, Z):
-        W_ = W
-        Z_ = Z
-
-        S = jnp.full_like(W_, s0)
-        v = jnp.full_like(W_, v0)
-
-        return 0, S, v, W_, Z_
-
-    def cond_fn(val):
-        i, *_ = val
-        return i < N
-
-    def body_val(val):
-        i, S, v, W, Z = val
-        dW = W[i]
-        dZ = Z[i]
-
-        S = S.at[i + 1].set(
-            S[i]
-            * jnp.exp((mean - 0.5 * v[i]) * dt + jnp.sqrt(v[i]) * jnp.sqrt(dt) * dW)
+        return jnp.asarray(S_paths.transpose(1, 0, 2)), jnp.asarray(
+            v_paths.transpose(1, 0, 2)
         )
-
-        v = v.at[i + 1].set(_variance_process_step(v[i], kappa, theta, sigma, dt, dZ))
-
-        return i + 1, S, v, W, Z
-
-    _, S, v, _, _ = jax.lax.while_loop(cond_fn, body_val, init_fn(W, Z))
-
-    return S, v
```

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/black/black_model.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/black/black_model.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/black_scholes/vanilla_options.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/black_scholes/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/fft/vanilla_options.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/fft/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/math/bs_common.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/math/bs_common.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/math/norm.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/math/norm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/utils/arrays.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/jaxfin/price_engine/utils/vect.py` & `JaxFin-0.3.2.dev0/jaxfin/price_engine/utils/vect.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/pyproject.toml` & `JaxFin-0.3.2.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/requirements/dev.txt` & `JaxFin-0.3.2.dev0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/scripts/create-new-version.bat` & `JaxFin-0.3.2.dev0/scripts/create-new-version.bat`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/tests/models/test_gbm.py` & `JaxFin-0.3.2.dev0/tests/models/test_gbm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/tests/models/test_heston.py` & `JaxFin-0.3.2.dev0/tests/models/test_heston.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import jax.numpy as jnp
+import numpy as np
 
 from jaxfin.models.heston.heston import MultiHestonModel, UnivHestonModel
 
 SEED: int = 42
 
+np.random.seed(SEED)
+
 
 class TestUnivHestonModel:
     def test_init(self):
         s0 = 100
         v0 = 0.2
         mean = 0.2
         kappa = 2.0
@@ -38,15 +41,15 @@
         sigma = jnp.array(0.3, dtype=jnp.float32)
         rho = jnp.array(-0.7, dtype=jnp.float32)
 
         heston_model = UnivHestonModel(
             s0, v0, mean, kappa, theta, sigma, rho, dtype=jnp.float32
         )
         paths, variance_process = heston_model.sample_paths(
-            seed=SEED, maturity=1.0, n=100, n_sim=100
+            maturity=1.0, n=100, n_sim=100
         )
 
         assert paths.shape == (100, 100)
         assert variance_process.shape == (100, 100)
 
 
 class TestMultiHestonModel:
@@ -82,12 +85,12 @@
         sigma = jnp.array([0.3, 0.3], dtype=jnp.float32)
         corr = jnp.array([[1.0, 0.5], [0.5, 1.0]], dtype=jnp.float32)
 
         heston_model = MultiHestonModel(
             s0, v0, mean, kappa, theta, sigma, corr, dtype=jnp.float32
         )
         paths, variance_processes = heston_model.sample_paths(
-            seed=SEED, maturity=1.0, n=100, n_sim=100
+            maturity=1.0, n=100, n_sim=100
         )
 
         assert paths.shape == (100, 100, 2)
         assert variance_processes.shape == (100, 100, 2)
```

### Comparing `JaxFin-0.3.1/tests/price_engine/test_black.py` & `JaxFin-0.3.2.dev0/tests/price_engine/test_black.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/tests/price_engine/test_bs.py` & `JaxFin-0.3.2.dev0/tests/price_engine/test_bs.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.3.1/tests/price_engine/test_fft.py` & `JaxFin-0.3.2.dev0/tests/price_engine/test_fft.py`

 * *Files identical despite different names*

