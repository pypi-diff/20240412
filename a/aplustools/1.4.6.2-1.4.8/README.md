# Comparing `tmp/aplustools-1.4.6.2.tar.gz` & `tmp/aplustools-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplustools-1.4.6.2.tar", last modified: Wed Mar 27 19:05:20 2024, max compression
+gzip compressed data, was "aplustools-1.4.8.tar", last modified: Fri Apr 12 10:00:48 2024, max compression
```

## Comparing `aplustools-1.4.6.2.tar` & `aplustools-1.4.8.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.982368 aplustools-1.4.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-03-27 19:05:20.982368 aplustools-1.4.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15617 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.974368 aplustools-1.4.6.2/aplustools/
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/adultswork.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/childsplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.974368 aplustools-1.4.6.2/aplustools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28345 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/advanced_imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/github-updater-cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/github-updater-gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/github-updater-none.py
--rw-r--r--   0 runner    (1001) docker     (127)    29692 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/data/updaters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.974368 aplustools-1.4.6.2/aplustools/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/io/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/io/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.978368 aplustools-1.4.6.2/aplustools/package/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/package/argu_mint_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    18660 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/package/argumint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/package/lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/package/timid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.978368 aplustools-1.4.6.2/aplustools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/tests/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.978368 aplustools-1.4.6.2/aplustools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/genpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    30629 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/hasher.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/utils/mappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.978368 aplustools-1.4.6.2/aplustools/web/
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/web/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)   221086 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/web/actual_webtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/web/new_webtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/web/web_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/aplustools/web/webtools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:05:20.978368 aplustools-1.4.6.2/aplustools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-03-27 19:05:20.000000 aplustools-1.4.6.2/aplustools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-27 19:05:20.000000 aplustools-1.4.6.2/aplustools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:05:20.000000 aplustools-1.4.6.2/aplustools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-27 19:05:20.000000 aplustools-1.4.6.2/aplustools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 19:05:20.000000 aplustools-1.4.6.2/aplustools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 19:05:20.000000 aplustools-1.4.6.2/aplustools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-27 19:05:16.000000 aplustools-1.4.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:05:20.982368 aplustools-1.4.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.797835 aplustools-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 10:00:44.000000 aplustools-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-12 10:00:48.797835 aplustools-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19343 2024-04-12 10:00:44.000000 aplustools-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.789835 aplustools-1.4.8/aplustools/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.789835 aplustools-1.4.8/aplustools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28389 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/advanced_imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/database_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/github-updater-cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/github-updater-gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/github-updater-none.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/updaters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.789835 aplustools-1.4.8/aplustools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/system_Test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/argu_mint_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/argumint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/timid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/genpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/new_webtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-12 10:00:44.000000 aplustools-1.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:00:48.797835 aplustools-1.4.8/setup.cfg
```

### Comparing `aplustools-1.4.6.2/LICENSE` & `aplustools-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/PKG-INFO` & `aplustools-1.4.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.6.2
+Version: 1.4.8
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -17,23 +17,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: BeautifulSoup4>=4.12.2
 Requires-Dist: winreg; os_name != "nt"
 Provides-Extra: data
 Requires-Dist: PySide6>=6.6.1; extra == "data"
-Requires-Dist: Pillow>=10.1.0; extra == "data"
+Requires-Dist: Pillow>=10.3.0; extra == "data"
 Requires-Dist: aiohttp>=3.9.3; extra == "data"
 Requires-Dist: opencv-python>=4.9.0.80; extra == "data"
 Requires-Dist: pillow_heif==0.15.0; extra == "data"
 Provides-Extra: web
 Requires-Dist: duckduckgo_search>=3.9.6; extra == "web"
 Provides-Extra: utils
-Requires-Dist: rich>=13.7.0; extra == "utils"
-Requires-Dist: pycryptodome>=3.19.0; extra == "utils"
+Requires-Dist: cryptography>=42.0.5; extra == "utils"
 Requires-Dist: brotli>=1.1.0; extra == "utils"
 Requires-Dist: zstandard>=0.22.0; extra == "utils"
 Requires-Dist: py7zr>=0.21.0; extra == "utils"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # aplustools
@@ -71,62 +70,88 @@
 
 ## Usage
 
 Here are a few quick examples of how to use aplustools:
 
 ### Search Engine usage
 ```python
-from aplustools.web import new_webtools as wt
+from aplustools.web.search import Search, GoogleSearchCore
 
-# Call the `google_search` function with a query
-result = wt.search.google_provider.google_search("Cute puppies", wt.get_useragent(), 1)
+# Call the `google_provider` function with a query
+searcher = Search(GoogleSearchCore(advanced=True))
+results = searcher.search("Cute puppies", num_results=10)
 
 # Print the result
-print(result)
-```
+print(results)
 
-### Search Engine usage 2
-```python
-from aplustools.web import webtools as wt
+from aplustools.web.utils import WebPage
 
-# Call the `google_provider` function with a query
-searcher = wt.Search()
-result = searcher.google_provider("Cute puppies")
+web_page = WebPage(results[0].get("url"))
+
+response = None
+if web_page.crawlable:  # Google search does this automatically at the moment
+    response = web_page.page.content
+print(response)
 
-# Print the result
-print(result)
 ```
 
-### Logger
+### web requests
 ```python
-from aplustools.io import environment as env
-from aplustools.io import loggers
+from aplustools.web.request import UnifiedRequestHandler, UnifiedRequestHandlerAdvanced
+import os
 
-# Set the current working directory to the main script or executable
-env.set_working_dir_to_main_script_location()
+# Default request handler
+handler = UnifiedRequestHandler()
 
-# Create an instance of Logger
-p_logger = loggers.PrintLogger("my_logs_file.log", show_time=True, capture_print=False, 
-                     overwrite_print=True, print_passthrough=False, print_log_to_stdout=True)
-# Shows the time in the logs (Like this [12:33:21]) and overwrites the normal sys.stdout
+# Synchronous request
+handler.fetch('http://example.com', async_mode=False)
+# Asynchronous request
+handler.fetch('http://example.com', async_mode=True)
 
-# Call the `monitor_stdout` method and pass the logger object, this will overwrite sys.stdout from Text I/O to the logger object
-logger = loggers.monitor_stdout(logger=p_logger) # Return sys.stdout, so you can make sure it worked
+# Advanced request handler (you can pass extra keyword arguments, and it automatically raises for status)
+adv_handler = UnifiedRequestHandlerAdvanced()  # It can also handle image content
 
-# Log something
-p_logger.log("Hello, world!")
+# Synchronous GET request
+adv_handler.request('GET', 'http://example.com', async_mode=False)
+# Asynchronous GET request
+adv_handler.request('GET', 'http://example.com', async_mode=True)
 
-# Print something, it won't get captured or displayed
-print("Hello, beautiful world!")
+folder_path = "./test_data/images"
+os.makedirs(folder_path, exist_ok=True)
+
+# Synchronous binary request (e.g., image)
+image_content = adv_handler.request('GET', 'http://example.com/image.png', async_mode=False, return_type='binary')
+with open(os.path.join(folder_path, './image.png'), 'wb') as file:
+    file.write(image_content)
+
+# Asynchronous binary request (e.g., image)
+image_content_async = adv_handler.request('GET', 'http://example.com/image.png', async_mode=True, return_type='binary')
+with open(os.path.join(folder_path, './image_async.png'), 'wb') as file:
+    file.write(image_content_async)
 
-# Close the Logger object (returns sys.stdout to it's normal state)
-p_logger.close()
 ```
 
-### OnlineImage
+### ImageManager
+````python
+from aplustools.data.imagetools import ImageManager, OnlineImage
+import os
+
+os.makedirs("./test", exist_ok=True)
+manager = ImageManager("./test", use_async=True)
+image_index = manager.add_image(OnlineImage, "somewhere.com/image.jpg")
+
+manager.execute_func(image_index, "download_image")
+manager.execute_func(image_index, "convert_to_grayscale")
+manager.execute_func(image_index, "apply_filter")  # Default is blur
+manager.execute_func(image_index, "rotate_image", 12)
+manager.execute_func(image_index, "save_image_to_disk")  # Overwrites downloaded file
+
+````
+
+### ImageTypes
 ```python
 from aplustools.data.imagetools import OnlineImage, OfflineImage, ImageFilter, SVGCompatibleImage
 import os
 
 # Setup
 folder_path = "./images"
 os.makedirs(folder_path, exist_ok=True)
@@ -156,92 +181,25 @@
 offline_image.save_image_to_disk(os.path.join(folder_path, "transformed_image.png"))
 
 # Example svg image usage
 image_processor = SVGCompatibleImage("someSvg.svg", 300,
                                      (667, 800), magick_path=r".\ImageMagick",
                                      base_location='./')
 image_processor.save_image_to_disk()
-```
-
-### Git-Updater
-```python
-from aplustools.data.updaters import GithubUpdater, VersionNumber
-from aplustools.io.environment import get_temp
-from aplustools import set_dir_to_ex
-import sys
-import os
-
-set_dir_to_ex()
-
-__version__ = VersionNumber("0.0.1")
-
-# Initialize an updater
-updater = GithubUpdater("Adalfarus", "unicode-writer", "py")  # If you want to use exe
-latest_version = updater.get_latest_tag_version()             # you need to compile them
-                                                              # yourself, otherwise it
-# Check if an update is needed                                # won't work
-if __version__ >= latest_version:
-    sys.exit()
-
-# Updater method
-path, zip_path = os.path.join(os.getcwd(), "update"), os.path.join(get_temp(), f"apt-update_{latest_version}")
-
-os.makedirs(path, exist_ok=True)
-os.makedirs(zip_path, exist_ok=True)
-
-# Start the update in a separate thread
-update_thread = updater.update(path, zip_path, latest_version, implementation="none", 
-                               host="localhost", port=1264, non_blocking=True, wait_for_connection=True)
-update_thread.start()
-
-# Receive the update status generator and print them
-progress_bar = 1
-for i in updater.receive_update_status():
-    print(f"{i}%", end=f" PB{progress_bar}\n")
-    if i == 100:
-        progress_bar += 1  # Switch to second progress bar, when the downloading is finished
-update_thread.join()
-```
-
-### Webtools
-```python
-... # Continuing the first two examples
-
-# Print the result
-print(result)
 
-from aplustools.web.webtools import check_url, is_crawlable
-import requests
-
-if check_url(result, ''): # Not really nessesary, search does this automatically
-	response = requests.get(result)
-	...
-```
-
-### Environment
-```python
-... # Continuing the image example
-
-_, img_name, img_path = image2.download_image(base_path=str(folder_path))  # Make sure this directory exists
 
 from aplustools.io.environment import absolute_path, remv, copy
-from aplustools.childsplay import ImportClass  # Could be switched out to adultswork, but the string would need to get converted
-
-importer = ImportClass(hard=True)
-importer.import_all()  # Destroys your runtime python
 
-a_img_path = absolute_path(img_path)
+a_img_path = absolute_path(os.path.join(folder_path, "downloaded_image.jpg"))
 
-try:
-    copy(a_img_path, str(folder_path) + str(img_name).remove(".png") + str(" - Copy.png"))
-except ValueError:
-    copy(a_img_path, str(folder_path) + str(img_name.split(".")[-1]) + str(" - Copy.png"))
+copy(a_img_path, str(folder_path) + "downloaded_image" + " - Copy.jpg")
 
 remv(a_img_path)  # Remove the original image
-remv(str(folder_path))  # Remove the base directory
+remv(folder_path)  # Remove the base directory
+
 ```
 
 ### Faker
 ```python
 from aplustools.data.faker import TestDataGenerator
 
 test_data = TestDataGenerator()
@@ -250,20 +208,21 @@
 print("\n", end="")
 print(test_data.generate_random_name())
 print(test_data.generate_random_email())
 print(test_data.generate_random_password())
 print(test_data.generate_random_phone_number())
 print(test_data.generate_random_address())
 print(test_data.generate_random_birth_date())
+
 ```
 
 ### Dummy
 ```python
-from aplustools.utils.dummy import Dummy3 # Dummy3 is for Python 3
-import math, sys
+from aplustools.utils.dummy import Dummy3  # Dummy3 is for Python 3
+import math
 
 dummy = Dummy3()
 
 # Do a bunch of operations that would normally throw errors
 dummy.attr.func("", int3="")
 dummy["Hello"] = 1
 del dummy[1]
@@ -289,23 +248,24 @@
 dummy << dummy
 dummy >> dummy
 dummy -= 1_000_000
 num = 1
 num *= dummy
 
 if dummy:
-	print(True)
+    print(True)
 else:
-	print(False)
+    print(False)
 
 for x in dummy:
-	print(x)
+    print(x)
 
 type(dummy)
 print(dummy, "->", int(dummy), list(dummy), tuple(dummy), float(dummy))
+
 ```
 
 ### Hasher
 ```python
 from aplustools.utils.hasher import hashed_latest, hashed_wrapper_latest, reducer, big_reducer, num_hasher
 
 inp = "Hello beautiful world, how are you today, lovely star?"
@@ -325,62 +285,128 @@
 
 acceptable_chars = range(100, 200)
 
 num_hashed_inp_uni = num_hasher(inp, desired_length, acceptable_chars)
 num_hashed_inp_uni_2 = num_hasher(inp2, desired_length, acceptable_chars)
 
 print(f"{inp} ({len(inp)}) -> {num_hashed_inp_uni} ({len(num_hashed_inp_uni)})\n{inp2} ({len(inp2)}) -> {num_hashed_inp_uni_2} ({len(num_hashed_inp_uni_2)})")
+
 ```
 
 ### GenPass
 ```python
-from aplustools.utils.genpass import GeneratePasswords
+from aplustools.utils.genpass import SecurePasswordManager, GeneratePasswords
+
+manager = SecurePasswordManager()
+password = manager.generate_ratio_based_password_v2(length=26, letters_ratio=0.5, numbers_ratio=0.3,
+                                                    punctuations_ratio=0.2, exclude_similar=True)
+manager.add_password("example.com", "json-the-greatest", password)
+manager.store_in_buffer("example.com", 0)  # Stores unencrypted password in a buffer
+print(manager.get_password("example.com"), "|", manager.use_from_buffer(0))  # for faster access.
+
+print(GeneratePasswords.generate_custom_sentence_based_password_v1(
+    "Exploring the unknown -- discovering new horizons...", random_case=True, extra_char="_",
+    char_position="keep" or 0, num_length=5, special_chars_length=2))
+# "keep" just sets it to 0
+
+# These classes are mostly meant for secure interprocess bidirectional
+# communication using networks.
+from aplustools.utils.genpass import ControlCodeProtocol, SecureSocketServer, SecureSocketClient
+
+# Initialize the protocol
+prot = ControlCodeProtocol()
+
+# Create a client and a server
+client = SecureSocketClient(prot)
+sock = client.get_socket()
+server = SecureSocketServer(sock, prot)
+
+# Start key exchange and communication between server and client
+client.start_and_exchange_keys()  # Client has to start first
+server.start_and_exchange_keys()
+
+# Client sends a message and a control code to the server
+client.add_control_code("shutdown")
+client.add_message("HELLO SERVER")
+client.sendall()  # The message is still received as it sends one chunk here
+# which then get's decoded in one piece. The decoder decodes everything
+# into chunks and control codes are always put behind messages.
+
+# Server shuts down the client connection
+server.shutdown_client()
+print("DONE1")
+
+# There are also classes for one directional communication that are
+# more integrated.
+from aplustools.utils.genpass import ControlCodeProtocol, ServerMessageHandler, ClientMessageHandler
+import threading
+
+prot = ControlCodeProtocol()
+
+# Create message handlers for server and client
+encoder = ClientMessageHandler(prot)
+
+# Make a connection using the clients host and chosen port
+connection = encoder.get_socket()
+
+decoder = ServerMessageHandler(connection, prot)
+
+# Client prepares and sends a message
+encoder.add_message("Hello Server")
+encoder.send_control_message("shutdown")
+
+# Server receives and processes each chunk
+encoder.start()
+threading.Thread(decoder.listen_for_messages()).start()  # Blocking
+encoder.flush()  # Blocking until connection is established
 
-gen = GeneratePasswords(debug=True)
-password = gen.generate_ratio_based_password_v2(length=10, letters_ratio=0.5, numbers_ratio=0.3, punctuations_ratio=0.2, secure_random=True, exclude_similar=True)
-print(password)
 ```
 
-### web_requests
+### Github-Updater
 ```python
-from aplustools.web.web_request import UnifiedRequestHandler, UnifiedRequestHandlerAdvanced
+from aplustools.data.updaters import GithubUpdater, VersionNumber
+from aplustools.io.environment import get_temp
+from aplustools import set_dir_to_ex
+import sys
 import os
 
-# Default request handler
-handler = UnifiedRequestHandler()
+set_dir_to_ex()
 
-# Synchronous request
-handler.fetch('http://example.com', async_mode=False)
-# Asynchronous request
-handler.fetch('http://example.com', async_mode=True)
+__version__ = VersionNumber("0.0.1")
 
-# Advanced request handler (you can pass extra keyword arguments, and it automatically raises for status)
-adv_handler = UnifiedRequestHandlerAdvanced()  # It can also handle image content
+# Initialize an updater
+updater = GithubUpdater("Adalfarus", "unicode-writer", "py")  # If you want to use exe
+latest_version = updater.get_latest_tag_version()             # you need to compile them
+                                                              # yourself, otherwise it
+# Check if an update is needed                                # won't work
+if __version__ >= latest_version:
+    sys.exit()
 
-# Synchronous GET request
-adv_handler.request('GET', 'http://example.com', async_mode=False)
-# Asynchronous GET request
-adv_handler.request('GET', 'http://example.com', async_mode=True)
+# Updater method
+path, zip_path = os.path.join(os.getcwd(), "update"), os.path.join(get_temp(), f"apt-update_{latest_version}")
 
-folder_path = "../test_data/images"
-os.makedirs(folder_path, exist_ok=True)
+os.makedirs(path, exist_ok=True)
+os.makedirs(zip_path, exist_ok=True)
 
-# Synchronous binary request (e.g., image)
-image_content = adv_handler.request('GET', 'http://example.com/image.png', async_mode=False, return_type='binary')
-with open(os.path.join(folder_path, './image.png'), 'wb') as file:
-    file.write(image_content)
+# Start the update in a separate thread
+update_thread = updater.update(path, zip_path, latest_version, implementation="none", 
+                               host="localhost", port=1264, non_blocking=True, wait_for_connection=True)
+update_thread.start()
+
+# Receive the update status generator and print them
+progress_bar = 1
+for i in updater.receive_update_status():
+    print(f"{i}%", end=f" PB{progress_bar}\n")
+    if i == 100:
+        progress_bar += 1  # Switch to second progress bar, when the downloading is finished
+update_thread.join()
 
-# Asynchronous binary request (e.g., image)
-image_content_async = adv_handler.request('GET', 'http://example.com/image.png', async_mode=True, return_type='binary')
-with open(os.path.join(folder_path, './image_async.png'), 'wb') as file:
-    file.write(image_content_async)
 ```
 
 ### ArguMint
-
 ```python
 from aplustools.package.argumint import ArgStruct, ArguMint
 from typing import Literal
 import sys
 
 
 def sorry(*args, **kwargs):
@@ -430,73 +456,163 @@
 sys.argv[0] = "apt"
 
 # Testing
 # sys.argv = ["apt", "help"]
 # sys.argv = ["apt", "build", "file", "./file.py", "--num=19"]
 parser.parse_cli(sys, "native_light")
 print(timer.end())
+
+```
+
+### compressor
+```python
+from aplustools.data.compressor import FileContainerV3, BrotliChunkCompressor
+import os
+
+
+compressor = BrotliChunkCompressor()
+container = FileContainerV3(compressor, block_size=2048*2048)
+
+image_data = {}
+for file in os.listdir("./images"):
+    if file.lower().endswith(".png"):
+        with open(os.path.join("./images", file), "rb") as f:
+            image_file_data = b''.join(f.readlines())
+            image_data[file] = image_file_data
+
+for file_name, image in image_data.items():
+    container.add_file(file_name, image)
+
+# Get the compressed data
+compressed_data = container.get_compressed_container()
+
+print("Compression done")
+
+with open("./files.bin", "wb") as f:
+    f.write(compressed_data)
+
+print("Wrote bin")
+
+# To extract a specific file from the compressed data
+try:
+    decompressed_images = []
+    for i in range(len(image_data)):
+        decompressed_image = container.extract_file(compressed_data, i)
+        decompressed_images.append(decompressed_image)
+except Exception as e:
+    print("Indexing not possible, error", e, "\n")
+    decompressed_images = []
+    for file_name in image_data.keys():
+        decompressed_image = container.extract_file(compressed_data, file_name)
+        decompressed_images.append(decompressed_image)
+compression_ratio = len(compressed_data) / sum(len(x) for x in image_data.values())
+
+print(f"Original size: {sum(len(x) for x in image_data.values())} bytes")
+print(f"Compressed size: {len(compressed_data)} bytes")
+print(f"Compression ratio: {compression_ratio:.2f}")
+
+for i, decompressed_image in enumerate(decompressed_images):
+    with open(f"./decompressed_images/image{i}.png", "wb") as f:
+        f.write(decompressed_image)
+
+```
+
+### Logger
+```python
+from aplustools.io import environment as env
+from aplustools.io import loggers
+
+# Set the current working directory to the main script or executable
+env.set_working_dir_to_main_script_location()
+
+# Create an instance of Logger
+p_logger = loggers.PrintLogger("my_logs_file.log", show_time=True, capture_print=False, 
+                     overwrite_print=True, print_passthrough=False, print_log_to_stdout=True)
+# Shows the time in the logs (Like this [12:33:21]) and overwrites the normal sys.stdout
+
+# Call the `monitor_stdout` method and pass the logger object, this will overwrite sys.stdout from Text I/O to the logger object
+logger = loggers.monitor_stdout(logger=p_logger) # Return sys.stdout, so you can make sure it worked
+
+# Log something
+p_logger.log("Hello, world!")
+
+# Print something, it won't get captured or displayed
+print("Hello, beautiful world!")
+
+# Close the Logger object (returns sys.stdout to it's normal state)
+p_logger.close()
+
 ```
+
 (Correct shortform for aplustools is apt, so please use ```import aplustools as apt``` for consistency)
 
 There are multiple clis added through this package:
 
 ### pype (python pipe)
 ```bash
 C:\Users\user_>pype
-Enter Python expression: 1+2
+Enter Python expression: 1 + 2
 3
 
-C:\Users\user_>pype 1//3
+C:\Users\user_>pype 1 // 3
 0
 ```
 ### upype (unified python pipe)
 ```bash
 C:\Users\user_>upype import aplustools; print(aplustools.__version__)
 1.4.4
 
 C:\Users\user_>upype
 Enter Python code (type 'end' on a new line to finish):
 ... class Test:
 ...     def hello_word(self):
-...             print("Hello, ya dunce!")
+...             print("Hello, you!")
 ... test = Test()
 ... test.hello_word()
 ... end
-Hello, ya dunce!
+Hello, you!
 ```
 ### apt
 Can currently run tests with ```apt tests run``` and show a basic help using ```apt help```.
 
 
 For more detailed usage and examples, check out our [documentation](https://github.com/adalfarus/aplustools/wiki).
 
 ## Naming convention, dependencies and more
 [PEP 8 -- Style Guide for Python Code](https://peps.python.org/pep-0008/#naming-conventions)
 
 For modules I use 'lowercase', classes are 'CapitalizedWords' and functions and methods are 'lower_case_with_underscores'.
 
-Dependencies (except for the standart libraries) are: 
-- data.database, io.environment, io.loggers, utils.mappers, data.faker, utils.dummy, utils.hasher, package.lazy_loader, package.timid, adultswork, childsplay - none
-- data.github-updater-cmd - requests
-- data.github-updater-gui - requests, PySide6
-- data.github-updater, data.updaters - requests
-- data.imagetools - Pillow, aiohttp, requests, wand
-- data.advanced_imagetools - opencv-python, aiohttp, wand, pillow_heif
-- web.webtools - requests, duckduckgo_search, BeautifulSoup4 - duckduckgo_search is only used for Search.duckduckgo_provider, if you don't want to use it, use Search._duckduckgo_provider instead.
-- utils.genpass - pycryptodome, rich
-- web.new_webtools, web.actual_webtools - requests, BeautifulSoup4
-- web.web_request - requests, aiohttp
-- utils.compressor - brotli, zstandard, py7zr
+Dependencies (except for the standard libraries) are: 
+- [`none`]
+  - data.database
+  - io.environment
+  - io.loggers
+  - data.faker
+  - utils.dummy
+  - utils.hasher
+  - package.lazy_loader
+  - package.timid
+- [`requests`]
+  - data.github-updater-none
+  - data.updaters
+  - data.github-updater-cmd
+- data.github-updater-gui - [`requests`, `PySide6`]
+- data.imagetools - [`Pillow`, `aiohttp`, `requests`, `wand`]
+- data.advanced_imagetools - [`opencv-python`, `aiohttp`, `wand`, `pillow_heif`]
+- web.search, web.utils - [`requests`, `BeautifulSoup4`]
+- utils.genpass - [`cryptography`]
+- web.request - [`requests`, `aiohttp`]
+- utils.compressor - [`brotli`, `zstandard`, `py7zr`]
+- io.gui - [`PySide6`]
 
 Sub-Modules that may be removed in future updates due to being hard to support or simply unneeded.
 
-- database (maybe unneeded and hard to support if more dbs are added)
-- actual_webtools, new_webtools, webtools search-machines (hard to support)
+- database (maybe unneeded and hard to support if more dbs are added -> new_database is being developed)
 - loggers (maybe unneeded)
-- childsplay & adultswork (maybe unneeded)
 
 ## Contributing
 
 We welcome contributions! Please see our [contributing guidelines](https://github.com/adalfarus/aplustools/blob/main/CONTRIBUTING.md) for more details on how you can contribute to aplustools.
 
 1. Fork the repository
 2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
```

### Comparing `aplustools-1.4.6.2/aplustools/_direct_functions.py` & `aplustools-1.4.8/aplustools/_direct_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,49 @@
-import subprocess
-import sys
-import os
-import warnings
+import subprocess as _subprocess
+import sys as _sys
+import os as _os
+import warnings as _warnings
+from aplustools.package import install_dependencies_lst as _install_dependencies_lst
 
 
-def execute_python_command(arguments: list = None, *args, **kwargs) -> subprocess.CompletedProcess[str]:
+def execute_python_command(arguments: list = None, *args, **kwargs) -> _subprocess.CompletedProcess[str]:
     if arguments is None:
         arguments = []
-    print(' '.join([sys.executable] + arguments))
+    print(' '.join([_sys.executable] + arguments))
     # Added to remain consistent with executing in the same python environment
-    return subprocess.run([sys.executable] + arguments, *args, **kwargs)
+    return _subprocess.run([_sys.executable] + arguments, *args, **kwargs)
 
 
 def interruptCTRL():
     """Simulates a hard user CTRL+C exit. This means it skips any try ... except KeyboardInterrupts"""
     exit(-1073741510)  # 130 / 0xC000013A
 
 
 def install_all_dependencies():
-    for dep in ["requests==2.31.0",
-                "Pillow==10.2.0",
-                "BeautifulSoup4==4.12.3",
-                "duckduckgo_search==3.9.3",
-                "rich==13.7.0",
-                "pycryptodome==3.20.0",
-                "PySide6==6.6.1",
-                "aiohttp==3.9.3",
-                "opencv-python==4.9.0.80",
-                "brotli==1.1.0",
-                "zstandard==0.22.0",
-                "py7zr==0.21.0",
-                "pillow_heif==0.15.0"]:
-        try:
-            proc = execute_python_command(arguments=
-                                          ["-m", "pip", "install", dep])
-            if proc.returncode != 0:
-                raise
-        except Exception as e:
-            print("An error occurred:" + str(e))
-
+    success = _install_dependencies_lst(["requests==2.31.0", "Pillow==10.3.0", "BeautifulSoup4==4.12.3",
+                                         "duckduckgo_search==3.9.3", "cryptography==42.0.5", "PySide6==6.6.1",
+                                         "aiohttp==3.9.3", "opencv-python==4.9.0.80", "brotli==1.1.0",
+                                         "zstandard==0.22.0", "py7zr==0.21.0", "pillow_heif==0.15.0"])
+    if not success:
+        return
     print("Done, all possible dependencies installed ...")
 
 
 def set_dir_to_ex():
     import __main__
     # Get the directory where the main script (or frozen exe) is located
-    if getattr(sys, 'frozen', False):
+    if getattr(_sys, 'frozen', False):
         # If the script is running as a bundled executable created by e.g. PyInstaller
-        main_dir = os.path.dirname(sys.executable)
+        main_dir = _os.path.dirname(_sys.executable)
     else:
         # If the script is running as a normal Python script
         if hasattr(__main__, '__file__'):
-            main_dir = os.path.dirname(os.path.abspath(__main__.__file__))
+            main_dir = _os.path.dirname(_os.path.abspath(__main__.__file__))
         else:
-            main_dir = os.path.dirname(os.getcwd())
-            warnings.warn(
+            main_dir = _os.path.dirname(_os.getcwd())
+            _warnings.warn(
                 "Could not set the current working directory to the location of the main script or executable",
                 RuntimeWarning,
                 stacklevel=2
             )
     # Change the current working directory to the main script directory
-    os.chdir(main_dir)
+    _os.chdir(main_dir)
```

### Comparing `aplustools-1.4.6.2/aplustools/cli.py` & `aplustools-1.4.8/aplustools/cli.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/aplustools/data/advanced_imagetools.py` & `aplustools-1.4.8/aplustools/data/advanced_imagetools.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,17 +437,16 @@
 
     # Save as HEIC
     heif_image = pillow_heif.from_pillow(pil_img)
     heif_image.save(os.path.join(output_dir_path, os.path.basename(image_path).rsplit(".", 1)[0] + ".HEIC"))
 
 
 class SVGImage:
-    raise NotImplementedError
-
     def __init__(self, file_path=None, svg_content=None):
+        raise NotImplementedError
         ET.register_namespace('', 'http://www.w3.org/2000/svg')
         if file_path:
             self.tree = ET.parse(file_path)
         elif svg_content:
             self.tree = ET.ElementTree(ET.fromstring(svg_content))
         else:
             svg_root = ET.Element('svg', xmlns="http://www.w3.org/2000/svg")
@@ -600,13 +599,13 @@
         # svg_img.rotate(45)
         # svg_img.convert_to_grayscale()
         # svg_img.save('./modified_file.svg')
 
     except Exception as e:
         print(f"An exception occurred during testing: {e}")
         return False
-
+    print("Test completed successfully.")
     return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/data/database.py` & `aplustools-1.4.8/aplustools/data/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,13 +85,12 @@
         print(f"{settings == {'test': 'value'}}")
         update_data(db, {"test": "value2"})
         settings = fetch_data(db)
         print(f"{settings != {'test': 'value'}}")
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
     
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/data/faker.py` & `aplustools-1.4.8/aplustools/data/faker.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,63 +74,29 @@
         email = self.generate_random_email()
         password = self.generate_random_password()
         phone_number = self.generate_random_phone_number()
         address = self.generate_random_address()
         birth_date = self.generate_random_birth_date()
         return Identity(name, last_name, email, password, phone_number, address, birth_date)
 
-    def insert_test_data(self, num_accounts=10, num_events=5):
-        return
-        """
-        Inserts test data into the system.
-        :param num_accounts: Number of test accounts to generate.
-        :param num_events: Number of test events to generate.
-        """
-        emails = [self.generate_random_email() for _ in range(num_accounts)]
-        passwords = [self.generate_random_password() for _ in range(num_accounts)]
-
-        test_accounts = [
-            # Assuming account structure: (account_id, role, first_name, last_name, email, phone, address, birth_date, gender)
-            # Generate and add more test accounts as needed
-        ]
-
-        test_events = [
-            # Assuming event structure: (event_id, organizer_id, title, description, date)
-            # Generate and add more test events as needed
-        ]
-
-        # Insert test accounts
-        try:
-            for account in test_accounts:
-                self.update_account_info(account[0], account[1:])
-        except Exception as e:
-            print(f"Error inserting accounts: {e}")
-
-        # Insert test events
-        try:
-            for event in test_events:
-                self.update_event_info(event[0], event[1:])
-        except Exception as e:
-            print(f"Error inserting events: {e}")
-
 
 def local_test():
     try:
         test_data = TestDataGenerator()
-        print(f"{", \n".join([str(test_data.generate_random_identity()) for _ in range(9000)])}")  # 900000 takes ~5 sec
+        lst_string = ', \n'.join([str(test_data.generate_random_identity()) for _ in range(9000)])
+        print(lst_string)  # 900000 takes ~5 sec
         print("\n", end="")
         print(test_data.generate_random_name())
         print(test_data.generate_random_email())
         print(test_data.generate_random_password())
         print(test_data.generate_random_phone_number())
         print(test_data.generate_random_address())
         print(test_data.generate_random_birth_date())
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/data/github-updater-cmd.py` & `aplustools-1.4.8/aplustools/data/github-updater-cmd.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/aplustools/data/github-updater-gui.py` & `aplustools-1.4.8/aplustools/data/github-updater-gui.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/aplustools/data/github-updater-none.py` & `aplustools-1.4.8/aplustools/data/github-updater-none.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/aplustools/data/imagetools.py` & `aplustools-1.4.8/aplustools/data/imagetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Type, Union, Tuple, Optional, List
-from aplustools.web.webtools import get_useragent
+from aplustools.web.utils import get_user_agent
 from concurrent.futures import ThreadPoolExecutor
 from urllib.parse import urlparse, urljoin
 from PIL import Image, ImageFilter
 from aiohttp import ClientSession
 from requests import Session
 from io import BytesIO
 import functools
@@ -487,15 +487,15 @@
         #         img.save(output, format='PNG')
         #         return output.getvalue()
         # else:
         #     return img
 
     def download_image(self, url):
         try:
-            user_agent = get_useragent()
+            user_agent = get_user_agent()
             headers = {"User-Agent": user_agent}
             response = requests.get(url, headers=headers)
             response.raise_for_status()
             file_name = os.path.basename(urlparse(url).path)
             file_path = os.path.join(self.base_location, file_name)
             with open(file_path, 'wb') as file:
                 file.write(response.content)
@@ -592,14 +592,13 @@
                                              (667, 800), magick_path=r"C:\Program Files\ImageMagick-7.1.1-Q16-HDRI",
                                              base_location='./')
         image_processor.save_image_to_disk()
 
     except Exception as e:
         print(f"Exception occurred: {e}")
         return False
-    else:
-        print("All tests completed successfully.")
-        return True
+    print("All tests completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/data/updaters.py` & `aplustools-1.4.8/aplustools/data/updaters.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,13 @@
             print(f"{i}%", end=f" PB{progress_bar}\n")
             if i == 100:
                 progress_bar += 1  # Switch to second progress bar, when the downloading is finished
         update_thread.join()
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/io/environment.py` & `aplustools-1.4.8/aplustools/io/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # environment.py
-from typing import Union, Optional, Callable
+from typing import Union, Optional, Callable, Any, Type, cast
+from types import FrameType
 import subprocess
 import warnings
 import platform
 import tempfile
 import inspect
 import shutil
 import sys
@@ -257,140 +258,133 @@
         return True
     except Exception as e:
         print(f"An error occurred while renaming: {e}")
         return False
 
 
 def functionize(cls):
-    warnings.warn("This is still experimental and may not be working as expected. A finished version should be available in release 0.1.5.", 
+    warnings.warn("This is still experimental and may not be working as expected. A finished version should be available in release 1.5",
                   UserWarning, 
                   stacklevel=2)
+
     def wrapper(*args, **kwargs):
         # Creating an instance of the class
         instance = cls(*args, **kwargs)
+
         # Collecting the instance attributes (variables) and their values
-        attrs = {attr: getattr(instance, attr) for attr in instance.__dict__}
+        attrs = {attr: getattr(instance, attr) for attr in instance.__dict__ if not attr.startswith("_")}  # instance.__dict__.copy()
+
         # Collecting methods and converting them to standalone functions
         methods = {
-            name: (lambda method: lambda *args, **kwargs: method(instance, *args, **kwargs))(method)
-            for name, method in cls.__dict__.items()
-            if inspect.isfunction(method)
+            name: getattr(instance, name)
+            for name, method in inspect.getmembers(cls, predicate=inspect.isfunction) if not name.startswith("_")
         }
+
         # Combining attributes and methods
         return {**attrs, **methods}
+
     return wrapper
 
-def old_strict(cls):
-    warnings.warn("This is still experimental and may not be working as expected. A finished version should be available in release 0.1.5.", 
-                  UserWarning, 
-                  stacklevel=2)
-    # Create the new class with the same name
-    class_name = cls.__name__
-    def create_method(name):
-        def method(self, *args, **kwargs):
-            return getattr(self._inner_instance, name)(*args, **kwargs)
-        return method
-    def create_property(name):
-        def getter(self):
-            return getattr(self._inner_instance, name)
-        return property(getter)
-    outer_class_attrs = {
-        '__init__': lambda self, *args, **kwargs: setattr(self, '_inner_instance', cls(*args, **kwargs))
-    }
-    # Add public methods and properties from the original class
-    for attr_name in dir(cls):
-        if not attr_name.startswith('_'):
-            attr = getattr(cls, attr_name)
-            if callable(attr):
-                outer_class_attrs[attr_name] = create_method(attr_name)
-            else:
-                outer_class_attrs[attr_name] = create_property(attr_name)
-    # Create the new class
-    OuterClass = type(class_name, (object,), outer_class_attrs)
-    def newgetattr(self, name):
-        if callable(name):
-            outer_class_attrs[attr_name] = create_method(attr_name)
-        else:
-            outer_class_attrs[attr_name] = create_property(attr_name)
-    return OuterClass
 
-def strict(cls):
-    warnings.warn("This is still experimental and may not be working as expected. A finished version should be available in release 0.1.5.", 
-                  UserWarning, 
-                  stacklevel=2)
-    # Create the new class with the same name
-    class_name = cls.__name__
-    def create_method(name):
-        def method(self, *args, **kwargs):
-            return getattr(self._inner_instance, name)(*args, **kwargs)
-        return method
-    def create_property(name):
-        def getter(self):
-            return getattr(self._inner_instance, name)
-        return property(getter)
-    def init_wrapper(self, *args, **kwargs):
-        self.__dict__['_inner_instance'] = cls(*args, **kwargs)
-    def setattr_wrapper(self, name, value):
-        if name in self.__dict__ or name == '_inner_instance':
-            object.__setattr__(self, name, value)
+def strict(cls: Type[Any]):
+    class_name = cls.__name__ + "Cover"
+    original_setattr = cls.__setattr__
+
+    # Overridden __setattr__ for the original class
+    def new_setattr(self, name, value):
+        original_setattr(self, name, value)
+        # Update the cover class if attribute is public
+        if not name.startswith('_') and hasattr(self, '_cover') and getattr(self._cover, name) != value:
+            setattr(self._cover, name, value)
+
+    # Replace __setattr__ in the original class
+    cls.__setattr__ = new_setattr
+
+    # Define new __init__ for the cover class
+    def new_init(self, *args, **kwargs):
+        # Create an instance of the original class
+        original_instance = cls(*args, **kwargs)
+        original_instance._cover = self  # Reference to the cover class
+
+        # Bind public methods and attributes to the cover class instance
+        for attr_name in dir(original_instance):
+            if not attr_name.startswith('_'):  # or attr_name in ('__dict__', '__module__'):
+                attr_value = getattr(original_instance, attr_name)
+                if inspect.isfunction(attr_value):
+                    setattr(self, attr_name, attr_value.__get__(self, cls))
+                else:
+                    setattr(self, attr_name, attr_value)
+
+        def custom_setattr(instance, name, value):
+            object.__setattr__(instance, name, value)
+            if not name.startswith('_') and getattr(original_instance, name) != value:
+                setattr(original_instance, name, value)
+
+        self._dynamic_setattr = custom_setattr
+
+        # Remove reference to original instance
+        # del original_instance
+
+    def setattr_overwrite(self, name, value):
+        if hasattr(self, '_dynamic_setattr'):
+            self._dynamic_setattr(self, name, value)
         else:
-            setattr(self._inner_instance, name, value)
-    def getattr_wrapper(self, name):
-        if name in self.__dict__:
-            return object.__getattribute__(self, name)
-        return getattr(self._inner_instance, name)
-    outer_class_attrs = {
-        '__init__': init_wrapper, 
-        '__setattr__': setattr_wrapper, 
-        '__getattr__': getattr_wrapper
+            object.__setattr__(self, name, value)
+
+    # Create a new cover class with the new __init__ and other methods/attributes
+    cover_class_attrs = {
+        '__init__': new_init,
+        '__class__': cls,
+        '__setattr__': setattr_overwrite,
     }
-    # Add public methods and properties from the original class
     for attr_name in dir(cls):
-        if not attr_name.startswith('_'):
-            attr = getattr(cls, attr_name)
-            if callable(attr):
-                outer_class_attrs[attr_name] = create_method(attr_name)
-            else:
-                outer_class_attrs[attr_name] = create_property(attr_name)
-    # Create the new class
-    OuterClass = type(class_name, (object,), outer_class_attrs)
-    return OuterClass
-"""
-@strict
-class Hello:
-    def __init__(self):
-        self.counter = 0
-    def _hell(self):
-        print(1)
-    def hell(self):
-        self._hell()
-        self.counter += 1
-    
-@functionize
-class Hello2:
-    def __init__(self):
-        pass
-    def _hell(self):
-        print("self")
-    def hell(self):
-        self._hell()
-        
-class Hello3:
-    def __init__(self):
-        pass
-    def _hell(self):
-        print(1)
-    def hell(self):
-        self._hell()
-
-ins = Hello()
-ins.hell()
-print(ins.counter)
-ins._hell()
-"""
+        if callable(getattr(cls, attr_name)) and not attr_name.startswith('_'):
+            cover_class_attrs[attr_name] = getattr(cls, attr_name)
+
+    CoverClass = type(class_name, (object,), cover_class_attrs)
+    return CoverClass
+
+
+def privatize(cls: Type[Any]):
+    """A class decorator that protects private attributes."""
+
+    original_getattr = cls.__getattribute__
+    original_setattr = cls.__setattr__
+
+    def _get_caller_name() -> str:
+        """Return the calling function's name."""
+        return cast(FrameType, cast(FrameType, inspect.currentframe()).f_back).f_code.co_name
+
+    def protected_getattr(self, name: str) -> Any:
+        if name.startswith('_') and _get_caller_name() not in dir(cls):
+            raise AttributeError(f"Access to private attribute {name} is forbidden")
+        return original_getattr(self, name)
+
+    def protected_setattr(self, name: str, value: Any) -> None:
+        if name.startswith('_') and _get_caller_name() not in dir(cls):
+            raise AttributeError(f"Modification of private attribute {name} is forbidden")
+        original_setattr(self, name, value)
+
+    cls.__getattribute__ = protected_getattr
+    cls.__setattr__ = protected_setattr
+
+    return cls
+
+
+def auto_repr(cls):
+    """
+    Decorator that automatically generates a __repr__ method for a class.
+    """
+    if cls.__repr__ is object.__repr__:
+        def __repr__(self):
+            attributes = ', '.join(f"{key}={getattr(self, key)}" for key in self.__dict__)
+            return f"{cls.__name__}({attributes})"
+
+        cls.__repr__ = __repr__
+    return cls
 
 
 class System:
     def __init__(self):
         self.os = self.get_os()
         self.os_version = self.get_os_version()
         self.cpu_arch = self.get_cpu_arch()
@@ -473,17 +467,44 @@
     print(f"CPU Brand: {sys_info.cpu_brand}")
     print(f"System Theme: {sys_info.theme}")
 
 
 def local_test():
     try:
         print_system_info()
+
+        @strict
+        class MyCls:
+            _attr = ""
+        var = MyCls()._attr
+
+        # @functionize
+        # class MyClass:
+        #     def __init__(self, value):
+        #         self.my_attribute = value
+        #         self._my_attr = 1
+
+        #     def adder(self):
+        #         self.my_attribute = 3
+
+        #     def my_method(self, plus):
+        #         return "The value is " + str(self.my_attribute + plus)
+
+        # Creating an instance as a function
+        # my_instance = MyClass(10)
+
+        # print(my_instance['my_attribute'])  # Accessing attribute
+        # print(my_instance['my_method'](3))  # Calling method
+        # my_instance['adder']()
+        # print(my_instance['my_attribute'])
+    except AttributeError:
+        print("Test completed successfully.")
+        return True
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Strict decorator not working.")
+    return False
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/io/loggers.py` & `aplustools-1.4.8/aplustools/io/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,14 +271,13 @@
         print("Do not do this, you need a ref to close it")
         ref.log("Hello World [Warn]", LogType.WARN, LogType.WARN)
         ref.close()
         print("DONE")
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/package/argu_mint_old.py` & `aplustools-1.4.8/aplustools/package/argu_mint_old.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/aplustools/package/argumint.py` & `aplustools-1.4.8/aplustools/package/argumint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional, Callable, Union, Literal, List, get_type_hints
+from typing import Optional, Callable, Union, Literal, List, get_type_hints, Any
 from pydantic import BaseModel, ValidationError, Field, create_model
 from argparse import ArgumentParser
 import sys
 import re
 
 
 class ArgumentParsingError(Exception):
-    def __init__(self, message, index):
+    def __init__(self, message: str, index: int):
         super().__init__(message)
         self.index = index
 
 
 class Argument:
     def __init__(self, name: str,
                  type_: Optional[type] = None,
@@ -35,28 +35,28 @@
         # self.is_optional = default  # Meaning true if there is a default
 
     @property
     def default(self):
         return self._default
 
     @default.setter
-    def default(self, value):
+    def default(self, value: type):
         self._default = value
         self.is_optional = value
         #if value in self.choices:
         #    self._default = value
         #else:
         #    raise ValueError(f"The default argument has to be present in the argument choices.")
 
     @property
     def help(self):
         return self._help
 
     @help.setter
-    def help(self, value):
+    def help(self, value: str):
         self._help = value or ""
 
     def __repr__(self):
         return f"Argument(name={self.name}, \
 type={self.type}, \
 choices={self.choices}, \
 default={self.default}, \
@@ -139,28 +139,28 @@
         cmd22
             cmd221
         cmd23
             ..."""
     def __init__(self):
         self.commands = {}
 
-    def add_command(self, command, subcommands=None):
+    def add_command(self, command: str, subcommands: Optional[dict] = None):
         if subcommands is None:
             subcommands = {}
         self.commands[command] = subcommands
 
-    def add_subcommand(self, parent, subcommand):
+    def add_subcommand(self, parent: str, subcommand: str):
         if parent not in self.commands:
             raise ValueError(f"Command '{parent}' not found.")
         if isinstance(self.commands[parent], dict):
             self.commands[parent][subcommand] = {}
         else:
             raise ValueError(f"Command '{parent}' cannot have subcommands.")
 
-    def add_nested_command(self, parent, command, subcommand=None):
+    def add_nested_command(self, parent: str, command: str, subcommand: Optional[Union[str, dict]] = None):
         if subcommand is None:
             subcommand = {}
 
         # Navigate to the correct parent level
         parts = parent.split('.')
         current_level = self.commands
         for part in parts:
@@ -175,15 +175,15 @@
 
     def get_structure(self):
         return self.commands
 
 
 class ArguMint:
     @staticmethod
-    def error(i, command_string):
+    def _error(i, command_string):
         print(command_string)
         print(" "*i+"^")
 
     @staticmethod
     def _lst_error(i, arg_i, command_lst, do_exit=False):
         length = sum(len(item) for item in command_lst[:i]) + i
         print(' '.join(command_lst) + "\n" +
@@ -192,20 +192,24 @@
             sys.exit(1)
 
     def __init__(self, default_endpoint: Union[EndPoint, Callable],
                  description: Optional[str] = None,
                  arg_struct: Optional[Union[ArgStruct, dict]] = None):
         self.default_endpoint = self._ender(default_endpoint)
         self.description = description or ""
+        if isinstance(arg_struct, ArgStruct):
+            arg_struct = arg_struct.get_structure()
         self.arg_struct = arg_struct or {}
         self.endpoints = {}
 
         self.formats = {1: "Usage: nuisco <subcommand> [--args]", 2: "Usage: nuisco create-template [project_name] [--args]"}
 
-    def _check_path(self, path: str, overwrite_pre_args: Optional[ArgStruct] = None):
+    def _check_path(self, path: str, overwrite_pre_args: Optional[Union[ArgStruct, dict]] = None):
+        if isinstance(overwrite_pre_args, ArgStruct):
+            overwrite_pre_args = overwrite_pre_args.get_structure()
         current_level = overwrite_pre_args or self.arg_struct
         for point in path.split("."):
             if point not in current_level or not isinstance(current_level[point], dict):
                 return False
             current_level = current_level[point]
         return True
 
@@ -213,15 +217,17 @@
     def _ender(potential_endpoint: Union[EndPoint, Callable]):
         if type(potential_endpoint) is EndPoint:
             endpoint = potential_endpoint
         else:
             endpoint = EndPoint(potential_endpoint)
         return endpoint
 
-    def replace_pre_args(self, new_pre_args):
+    def replace_pre_args(self, new_pre_args: Union[ArgStruct, dict]):
+        if isinstance(new_pre_args, ArgStruct):
+            new_pre_args = new_pre_args.get_structure()
         to_del = []
         for path, endpoint in self.endpoints.items():
             if self._check_path(endpoint, new_pre_args):
                 continue
             else:
                 to_del.append(path)
         print(f"Removed {len([self.endpoints.pop(epPath) for epPath in to_del])} endpoints.")
@@ -399,56 +405,66 @@
         path = '.'.join(pre_args)
         args = arguments[arguments.index(pre_args[-1])+1:]  # Will return an empty list, if [i:] is longer than the list
         endpoint = self.endpoints.get(path) or self.default_endpoint
         arguments = self._parse_args(args, endpoint, mode)
         endpoint.call(**arguments)
 
 
-if __name__ == "__main__":
-    def sorry(*args, **kwargs):
-        print("Not implemented yet, sorry!")
-
-    def help_text():
-        print("Build -> dir/file or help.")
-
-    def build_file(path: Literal["./main.py", "./file.py"] = "./main.py", num: int = 0):
-        """
-        build_file
-        :param path: The path to the file that should be built.
-        :param num:
-        :return None:
-        """
-        print(f"Building file {path} ..., {num}")
-
-    from aplustools.package import timid
-
-    timer = timid.TimidTimer()
-
-    arg_struct = {'apt': {'build': {'file': {}, 'dir': {'main': {}, 'all': {}}}, 'help': {}}}
-
-    # Example usage
-    builder = ArgStruct()
-    builder.add_command("apt")
-    builder.add_nested_command("apt", "build", "file")
+def local_test():
+    try:
+        def sorry(*args, **kwargs):
+            print("Not implemented yet, sorry!")
+
+        def help_text():
+            print("Build -> dir/file or help.")
+
+        def build_file(path: Literal["./main.py", "./file.py"] = "./main.py", num: int = 0):
+            """
+            build_file
+            :param path: The path to the file that should be built.
+            :param num:
+            :return None:
+            """
+            print(f"Building file {path} ..., {num}")
+
+        from aplustools.package import timid
+
+        timer = timid.TimidTimer()
+
+        arg_struct = {'apt': {'build': {'file': {}, 'dir': {'main': {}, 'all': {}}}, 'help': {}}}
+
+        # Example usage
+        builder = ArgStruct()
+        builder.add_command("apt")
+        builder.add_nested_command("apt", "build", "file")
+
+        builder.add_nested_command("apt.build", "dir", {'main': {}, 'all': {}})
+        # builder.add_subcommand("apt.build", "dir")
+        # builder.add_nested_command("apt.build.dir", "main")
+        # builder.add_nested_command("apt.build.dir", "all")
+
+        builder.add_command("apt.help")
+        # builder.add_nested_command("apt", "help")
+
+        print(builder.get_structure())  # Best to cache this for better times (by ~15 microseconds)
+
+        parser = ArguMint(default_endpoint=sorry, arg_struct=arg_struct)
+        parser.add_endpoint("apt.help", help_text)
+
+        parser.add_endpoint("apt.build.file", build_file)
+
+        sys.argv[0] = "apt"
+
+        # Testing
+        # sys.argv = ["apt", "help"]
+        sys.argv = ["apt", "build", "file", "./file.py", "--num=19"]
+        parser.parse_cli(sys, "native_light")
+        print(timer.end())
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return False
+    print("Test completed successfully.")
+    return True
 
-    builder.add_nested_command("apt.build", "dir", {'main': {}, 'all': {}})
-    # builder.add_subcommand("apt.build", "dir")
-    # builder.add_nested_command("apt.build.dir", "main")
-    # builder.add_nested_command("apt.build.dir", "all")
 
-    builder.add_command("apt.help")
-    # builder.add_nested_command("apt", "help")
-
-    print(builder.get_structure())  # Best to cache this for better times (by ~15 microseconds)
-
-    parser = ArguMint(default_endpoint=sorry, arg_struct=arg_struct)
-    parser.add_endpoint("apt.help", help_text)
-
-    parser.add_endpoint("apt.build.file", build_file)
-
-    sys.argv[0] = "apt"
-
-    # Testing
-    # sys.argv = ["apt", "help"]
-    # sys.argv = ["apt", "build", "file", "./file.py", "--num=19"]
-    parser.parse_cli(sys, "native_light")
-    print(timer.end())
+if __name__ == "__main__":
+    local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/package/timid.py` & `aplustools-1.4.8/aplustools/package/timid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import time, perf_counter_ns, monotonic_ns
 from datetime import timedelta, datetime
-from typing import Optional, Type
+from typing import Optional, Type, Union
 from timeit import default_timer
 
 
 class TimidTimer:
     """Uses the timeit.default_timer function to calculate passed time."""
     def __init__(self, start_seconds: Optional[int] = 0,
                  start_now: Optional[bool] = True):
@@ -15,31 +15,31 @@
         if start_now:
             self.start()
 
     def start(self) -> float:
         self.starter = default_timer() + self.starter
         return self.starter
 
-    def end(self, return_end_time: Optional[bool] = False) -> timedelta | float:
+    def end(self, return_end_time: Optional[bool] = False) -> Union[timedelta, float]:
         self.ender = default_timer()
         self.timedelta = timedelta(seconds=self.ender - self.starter)
 
         if not return_end_time:
             return self.timedelta
         else:
             return self.ender
 
-    def tick(self, return_time: Optional[bool] = False) -> timedelta | float:
+    def tick(self, return_time: Optional[bool] = False) -> Union[timedelta, float]:
         """Return how much time has passed till the start."""
         if not return_time:
             return timedelta(seconds=default_timer() - self.starter)
         else:
             return default_timer()
 
-    def tock(self, return_time: Optional[bool] = False) -> timedelta | float:
+    def tock(self, return_time: Optional[bool] = False) -> Union[timedelta, float]:
         """Returns how much time has passed till the last tock."""
         last_time = self.ender or self.starter
         self.ender = default_timer()
 
         if not return_time:
             return timedelta(seconds=self.ender - last_time)
         else:
@@ -71,31 +71,31 @@
         if start_now:
             self.start()
 
     def start(self) -> int:
         self.starter = perf_counter_ns() + int(self.starter * 1e+9)
         return self.starter
 
-    def end(self, return_end_time: Optional[bool] = False) -> timedelta | int:
+    def end(self, return_end_time: Optional[bool] = False) -> Union[timedelta, int]:
         self.ender = perf_counter_ns()
         self.timedelta = timedelta(microseconds=(self.ender - self.starter) / 1000)
 
         if not return_end_time:
             return self.timedelta
         else:
             return self.ender
 
-    def tick(self, return_time: Optional[bool] = False) -> timedelta | int:
+    def tick(self, return_time: Optional[bool] = False) -> Union[timedelta, int]:
         """Return how much time has passed till the start."""
         if not return_time:
             return timedelta(microseconds=(perf_counter_ns() - self.starter) / 1000)
         else:
             return perf_counter_ns()
 
-    def tock(self, return_time: Optional[bool] = False) -> timedelta | int:
+    def tock(self, return_time: Optional[bool] = False) -> Union[timedelta, int]:
         """Returns how much time has passed till the last tock."""
         last_time = self.ender or self.starter
         self.ender = perf_counter_ns()
 
         if not return_time:
             return timedelta(microseconds=(self.ender - last_time) / 1000)
         else:
@@ -188,14 +188,15 @@
     SECONDS = 4
     MILISEC = 5
     MICROSEC = 6
 
 
 class TimeDisplay:
     def __init__(self, td: timedelta, out: TimerOut):
+        raise NotImplementedError("This class isn't implemented yet, please visit back in version 1.5 or later.")
         self.microsec = td.microseconds
         self.seconds = td.seconds
         self.days = td.days
 
         self.repr = ""
 
     def __repr__(self):
@@ -203,14 +204,15 @@
                 \
                 )"
 
 
 class Timer:
     def __init__(self, output_target: Optional[TimerOut] = TimerOut.SECONDS,
                  start_now: Optional[bool] = True):
+        raise NotImplementedError("This class isn't implemented yet, please visit back in version 1.5 or later.")
         self.output_target = output_target
 
         self.start_t = None
         self.stop_t = None
         self.t_d = None
 
         if start_now:
@@ -226,54 +228,54 @@
         return self.start_t
 
     @staticmethod
     def time() -> float:
         return
         return timer()
 
-    def tick(self, return_time: Optional[bool] = False) -> timedelta | float:
+    def tick(self, return_time: Optional[bool] = False) -> Union[timedelta, float]:
         return
         """Return how much time has passed till the start."""
         if not return_time:
             return timedelta(seconds=timer() - self.start_t)
         else:
             return timer()
 
-    def tock(self, return_time: Optional[bool] = False) -> timedelta | float:
+    def tock(self, return_time: Optional[bool] = False) -> Union[timedelta, float]:
         return
         """Returns how much time has passed till the last tock."""
         time = self.stop_t or self.start_t
         self.stop_t = time()
 
         if not return_time:
             return timedelta(seconds=time - self.stop_t)
         else:
             return time
 
-    def end(self, return_end_time: Optional[bool] = False) -> timedelta | float:
+    def end(self, return_end_time: Optional[bool] = False) -> Union[timedelta, float]:
         return
         self.stop_t = timer()
         self.t_d = timedelta(seconds=self.stop_t-self.start_t)
 
         if not return_end_time:
             return self.t_d
         else:
             return self.stop_t
 
 
 def local_test():
     try:
-        def test_delay(cls: Type[NormalTimer] | Type[LazyTimer]):
+        def test_delay(cls: Type[Union[NormalTimer, LazyTimer]]):
             timer = TimidTimer2()
             cls().stop()
             return timer.end() - timedelta(microseconds=1)
 
         print("TimidTimerDelay", TimidTimer.test_delay())
         print("TimidTimer2Delay", TimidTimer2.test_delay())
-        print("All other delays are too small as to measure them with themselves, \
+        print("All other timers are too inaccurate as to measure them with themselves, \
 so we measure them with TimidTimer2 and subtract the average delay.")
         print("NormalTimerDelay", test_delay(NormalTimer))
         print("LazyTimerDelay", test_delay(LazyTimer))
 
         print("\nTimer Test, using 1 million passes.")
         t_timer = TimidTimer()
         t_timer2 = TimidTimer2()
@@ -316,14 +318,13 @@
         print("\nLazyTimer delay test 2")
         lazy_t = LazyTimer()
         for i in range(10):
             print(lazy_t.round())
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/tests/test_data.py` & `aplustools-1.4.8/aplustools/tests/test_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from aplustools.data import database, imagetools, updaters, faker
+from aplustools.data import database, imagetools, updaters, faker, advanced_imagetools, compressor
 
 
 class TestUpdaters:
     def test_get_last_version(self):
         updater = updaters.GithubUpdater("adalfarus", "unicode-writer")
         assert (updater.get_latest_tag_version(), updater.get_latest_release_title_version()) == ("0.0.2", "0.0.2")
         
@@ -19,7 +19,17 @@
     def test_local(self):
         assert faker.local_test()
 
 
 class TestImagetools:
     def test_local(self):
         assert imagetools.local_test()
+
+
+class TestAdvancedImagetools:
+    def test_local(self):
+        assert advanced_imagetools.local_test()
+
+
+class TestCompressor:
+    def test_local(self):
+        assert compressor.local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/utils/compressor.py` & `aplustools-1.4.8/aplustools/data/compressor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 import lzma
 import brotli
 import json
 import os
 import zstandard as zstd
 import py7zr
 import io
+from typing import Type, Union, Tuple
 
 
 class FileContainer:
-    def __init__(self, compressor, block_size=1024 * 1024):  # Block size of 1 MB
+    def __init__(self, compressor: "ChunkCompressorBase", block_size: int = 1024 * 1024):  # Block size of 1 MB
         self.compressor = compressor
         self.block_size = block_size
         self.current_block = bytearray()
         self.compressed_data = bytearray()
         self.files = {}
         self.block_offsets = []
 
     def _compress_current_block(self):
         if self.current_block:
             compressed_block = self.compressor.compress(self.current_block)
             self.block_offsets.append({'start': len(self.compressed_data), 'length': len(compressed_block)})
             self.compressed_data.extend(compressed_block)
             self.current_block = bytearray()
 
-    def add_file(self, filename, data):
+    def add_file(self, filename: str, data: bytes):
         if len(self.current_block) + len(data) > self.block_size:
             self._compress_current_block()
 
         file_info = {
             'block_index': len(self.block_offsets),
             'start': len(self.current_block),
             'length': len(data)
         }
         self.current_block.extend(data)
         self.files[filename] = file_info
 
         if len(self.current_block) >= self.block_size:
             self._compress_current_block()
 
-    def get_compressed_container(self):
+    def get_compressed_container(self) -> bytes:
         self._compress_current_block()  # Compress any remaining data in the current block
         index_data = json.dumps({'files': self.files, 'blocks': self.block_offsets}).encode()
         index_length = len(index_data).to_bytes(4, 'big')
         return index_length + index_data + self.compressed_data
 
-    def extract_file(self, compressed_container, filename):
+    def extract_file(self, compressed_container: bytes, filename: str) -> bytes:
         index_length = int.from_bytes(compressed_container[:4], 'big')
         index_data = compressed_container[4:4 + index_length]
         index = json.loads(index_data)
 
         file_info = index['files'][filename]
         block_info = index['blocks'][file_info['block_index']]
 
@@ -61,15 +62,15 @@
 
         start_file = file_info['start']
         length_file = file_info['length']
         return decompressed_block[start_file:start_file + length_file]
 
 
 class FileContainerV2:
-    def __init__(self, compressor, block_size=1024 * 1024):  # Block size of 1 MB
+    def __init__(self, compressor: "ChunkCompressorBase", block_size: int = 1024 * 1024):  # Block size of 1 MB
         self.compressor = compressor
         self.block_size = block_size
         self.current_block = bytearray()
         self.compressed_data = bytearray()
         self.file_info = {}  # Stores info about files by filename
         self.index_to_name = []  # Maps numeric indexes to filenames
         self.block_offsets = []
@@ -77,15 +78,15 @@
     def _compress_current_block(self):
         if self.current_block:
             compressed_block = self.compressor.compress(self.current_block)
             self.block_offsets.append({'start': len(self.compressed_data), 'length': len(compressed_block)})
             self.compressed_data.extend(compressed_block)
             self.current_block = bytearray()
 
-    def add_file(self, filename, data):
+    def add_file(self, filename: str, data: bytes) -> int:
         if len(self.current_block) + len(data) > self.block_size:
             self._compress_current_block()
 
         file_index = len(self.index_to_name)
         self.index_to_name.append(filename)
         self.file_info[filename] = {
             'index': file_index,
@@ -94,21 +95,23 @@
             'length': len(data)
         }
         self.current_block.extend(data)
 
         if len(self.current_block) >= self.block_size:
             self._compress_current_block()
 
-    def get_compressed_container(self):
+        return file_index
+
+    def get_compressed_container(self) -> bytes:
         self._compress_current_block()  # Compress any remaining data in the current block
         index_data = json.dumps({'file_info': self.file_info, 'block_offsets': self.block_offsets, 'index_to_name': self.index_to_name}).encode()
         index_length = len(index_data).to_bytes(4, 'big')
         return index_length + index_data + self.compressed_data
 
-    def extract_file(self, compressed_container, file_identifier):
+    def extract_file(self, compressed_container: bytes, file_identifier: Union[str, int]) -> bytes:
         index_length = int.from_bytes(compressed_container[:4], 'big')
         index_data = compressed_container[4:4 + index_length]
         index = json.loads(index_data)
 
         filename = file_identifier if isinstance(file_identifier, str) else index['index_to_name'][file_identifier]
         file_info = index['file_info'][filename]
         block_info = index['block_offsets'][file_info['block_index']]
@@ -121,15 +124,15 @@
 
         start_file = file_info['start']
         length_file = file_info['length']
         return decompressed_block[start_file:start_file + length_file]
 
 
 class FileContainerV3:
-    def __init__(self, compressor, block_size=1024 * 1024):  # Block size of 1 MB
+    def __init__(self, compressor: "ChunkCompressorBase", block_size: int = 1024 * 1024):  # Block size of 1 MB
         self.compressor = compressor
         self.block_size = block_size
         self.current_block = bytearray()
         self.compressed_data = bytearray()
         self.file_info = {}  # Stores info about files by filename
         self.index_to_name = []  # Maps numeric indexes to filenames
         self.block_offsets = []
@@ -137,15 +140,15 @@
     def _compress_current_block(self):
         if self.current_block:
             compressed_block = self.compressor.compress(self.current_block)
             self.block_offsets.append({'start': len(self.compressed_data), 'length': len(compressed_block)})
             self.compressed_data.extend(compressed_block)
             self.current_block = bytearray()
 
-    def add_file(self, filename, data):
+    def add_file(self, filename: str, data: bytes) -> int:
         if len(self.current_block) + len(data) > self.block_size:
             self._compress_current_block()
 
         file_index = len(self.index_to_name)
         self.index_to_name.append(filename)
         self.file_info[filename] = {
             'index': file_index,
@@ -154,22 +157,24 @@
             'length': len(data)
         }
         self.current_block.extend(data)
 
         if len(self.current_block) >= self.block_size:
             self._compress_current_block()
 
-    def get_compressed_container(self):
+        return file_index
+
+    def get_compressed_container(self) -> bytes:
         self._compress_current_block()  # Compress any remaining data in the current block
         index_data = json.dumps({'file_info': self.file_info, 'block_offsets': self.block_offsets, 'index_to_name': self.index_to_name}).encode()
         compressed_index_data = self.compressor.compress(index_data)
         index_length = len(compressed_index_data).to_bytes(4, 'big')
         return index_length + compressed_index_data + self.compressed_data
 
-    def extract_file(self, compressed_container, file_identifier):
+    def extract_file(self, compressed_container: bytes, file_identifier: Union[str, int]) -> bytes:
         compressed_index_length = int.from_bytes(compressed_container[:4], 'big')
         compressed_index_data = compressed_container[4:4 + compressed_index_length]
         index_data = self.compressor.decompress(compressed_index_data)
         index = json.loads(index_data)
 
         filename = file_identifier if isinstance(file_identifier, str) else index['index_to_name'][file_identifier]
         file_info = index['file_info'][filename]
@@ -181,121 +186,140 @@
 
         decompressed_block = self.compressor.decompress(compressed_block)
 
         start_file = file_info['start']
         length_file = file_info['length']
         return decompressed_block[start_file:start_file + length_file]
 
+    def get_compressed_container_info(self, compressed_container: bytes) -> Tuple[int, dict, list]:
+        """Returns a tuple(Number of Files, Index to name dictionary and an in-order name list)"""
+        compressed_index_length = int.from_bytes(compressed_container[:4], 'big')
+        compressed_index_data = compressed_container[4:4 + compressed_index_length]
+        index_data = self.compressor.decompress(compressed_index_data)
+        index = json.loads(index_data)
+        return (len(index['file_info']),
+                {i: name for i, name in enumerate(index['index_to_name'])}, index['index_to_name'])
+
 
 class ChunkCompressorBase:
-    def compress(self, data_chunk):
+    def compress(self, data_chunk: bytes) -> bytes:
         return data_chunk
 
-    def decompress(self, compressed_chunk):
+    def decompress(self, compressed_chunk: bytes) -> bytes:
         return compressed_chunk
 
 
 class BrotliChunkCompressor(ChunkCompressorBase):
-    def __init__(self, quality=11):  # Maximum compression quality
+    def __init__(self, quality: int = 11):  # Maximum compression quality
         self.quality = quality
 
-    def compress(self, data_chunk):
+    def compress(self, data_chunk: bytes) -> bytes:
         # Compress the data chunk with Brotli
         return brotli.compress(data_chunk, quality=self.quality)
 
-    def decompress(self, compressed_chunk):
+    def decompress(self, compressed_chunk: bytes) -> bytes:
         # Decompress the data chunk with Brotli
         return brotli.decompress(compressed_chunk)
 
     @staticmethod
     def add_markers(data, start_marker, end_marker):
         # Add start and end markers to the data
         return start_marker + data + end_marker
 
 
 class LZMAChunkCompressor(ChunkCompressorBase):
     def __init__(self, preset=lzma.PRESET_EXTREME):
         self.preset = preset
 
-    def compress(self, data_chunk):
+    def compress(self, data_chunk: bytes) -> bytes:
         # Compress the data chunk with LZMA
         return lzma.compress(data_chunk, preset=self.preset)
 
-    def decompress(self, compressed_chunk):
+    def decompress(self, compressed_chunk: bytes) -> bytes:
         # Decompress the data chunk with LZMA
         return lzma.decompress(compressed_chunk)
 
 
 class ZstdCompressor(ChunkCompressorBase):
-    def __init__(self, level=3):
+    def __init__(self, level: int=3):
         self.compressor = zstd.ZstdCompressor(level=level)
         self.decompressor = zstd.ZstdDecompressor()
 
-    def compress(self, data_chunk):
+    def compress(self, data_chunk: bytes) -> bytes:
         return self.compressor.compress(data_chunk)
 
-    def decompress(self, compressed_chunk):
+    def decompress(self, compressed_chunk: bytes) -> bytes:
         return self.decompressor.decompress(compressed_chunk)
 
 
 class LZMA2Compressor(ChunkCompressorBase):
-    def compress(self, data_chunk):
+    def compress(self, data_chunk: bytes) -> bytes:
         with io.BytesIO() as buffer, py7zr.SevenZipFile(buffer, 'w', filters=[{'id': py7zr.FILTER_LZMA2}]) as archive:
             # Create a file-like object from data_chunk
             file_like_data = io.BytesIO(data_chunk)
             archive.write({"data": file_like_data})
             buffer.seek(0)  # Reset buffer position to the beginning
             return buffer.getvalue()
 
-    def decompress(self, compressed_chunk):
+    def decompress(self, compressed_chunk: bytes) -> bytes:
         with io.BytesIO(compressed_chunk) as input_buffer, py7zr.SevenZipFile(input_buffer, 'r') as archive:
             output_buffer = io.BytesIO()
             archive.extractall(path=output_buffer)
             output_buffer.seek(0)  # Reset buffer position to the beginning
             return output_buffer.read()
 
 
-if __name__ == "__main__":
-    compressor = BrotliChunkCompressor()
-    container = FileContainerV3(compressor, block_size=2048*2048)
-
-    image_data = {}
-    for file in os.listdir("./images_htfs"):
-        if file.endswith(".HTSF"):
-            with open(os.path.join("./images_htfs", file), "rb") as f:
-                image_file_data = b''.join(f.readlines())
-                image_data[file] = image_file_data
-
-    for file_name, image in image_data.items():
-        container.add_file(file_name, image)
-
-    # Get the compressed data
-    compressed_data = container.get_compressed_container()
-
-    print("Compression done")
+def local_test():
+    try:
+        compressor = BrotliChunkCompressor()
+        container = FileContainerV3(compressor, block_size=2048 * 2048)
 
-    with open("./htfs_files.bin", "wb") as f:
-        f.write(compressed_data)
+        data = {}
+        for root, dirs, files in os.walk("./test_data"):
+            for file in files:
+                with open(os.path.join(root, file), "rb") as f:
+                    image_file_data = b''.join(f.readlines())
+                    data[file] = image_file_data
+
+        for file_name, image in data.items():
+            container.add_file(file_name, image)
+
+        # Get the compressed data
+        compressed_data = container.get_compressed_container()
+
+        print("Compression done")
+
+        with open("./test_data/files.bin", "wb") as f:
+            f.write(compressed_data)
+
+        print("Wrote bin")
+
+        # To extract a specific file from the compressed data
+        try:
+            decompressed_files = []
+            for i in range(len(data)):
+                decompressed_file = container.extract_file(compressed_data, i)
+                decompressed_files.append(decompressed_file)
+        except Exception as e:
+            print("Indexing not possible, error", e, "\n")
+            decompressed_files = []
+            for file_name in data.keys():
+                decompressed_file = container.extract_file(compressed_data, file_name)
+                decompressed_files.append(decompressed_file)
+        compression_ratio = len(compressed_data) / sum(len(x) for x in data.values())
+
+        print(f"Original size: {sum(len(x) for x in data.values())} bytes")
+        print(f"Compressed size: {len(compressed_data)} bytes")
+        print(f"Compression ratio: {compression_ratio:.2f}")
+
+        for i, decompressed_file in enumerate(decompressed_files):
+            with open(f"./test_data/file_{i}.ext", "wb") as f:
+                f.write(decompressed_file)
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return False
+    print("Test completed successfully.")
+    return True
 
-    print("Wrote bin")
 
-    # To extract a specific file from the compressed data
-    try:
-        decompressed_images = []
-        for i in range(len(image_data)):
-            decompressed_image = container.extract_file(compressed_data, i)
-            decompressed_images.append(decompressed_image)
-    except Exception as e:
-        print("Indexing not possible, error", e, "\n")
-        decompressed_images = []
-        for file_name in image_data.keys():
-            decompressed_image = container.extract_file(compressed_data, file_name)
-            decompressed_images.append(decompressed_image)
-    compression_ratio = len(compressed_data) / sum(len(x) for x in image_data.values())
-
-    print(f"Original size: {sum(len(x) for x in image_data.values())} bytes")
-    print(f"Compressed size: {len(compressed_data)} bytes")
-    print(f"Compression ratio: {compression_ratio:.2f}")
-
-    for i, decompressed_image in enumerate(decompressed_images):
-        with open(f"./decompressed_images/image{i}.HTSF", "wb") as f:
-            f.write(decompressed_image)
+if __name__ == "__main__":
+    local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/utils/dummy.py` & `aplustools-1.4.8/aplustools/utils/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         yield
     def __enter__(self):
         return self
     def __exit__(self, exc_type, exc_val, exc_tb):
         return True
     def __getitem__(self, item):
         return self
+    def __setitem__(self, key, new_value):
+        return
     def __delitem__(self, key):
         return None
         
     # Type dunder methods
     def __int__(self):
         return int()
     def __float__(self):
@@ -183,14 +185,13 @@
         for x in dummy:
             print("HELLO")
         type(dummy)
         print(dummy, str(dummy), int(dummy), list(dummy), tuple(dummy), float(dummy))
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/utils/hasher.py` & `aplustools-1.4.8/aplustools/utils/hasher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import random
+from typing import Optional, List, Callable
+
 
 class UM:
     """
     All the methods in this class are designed to change a given list
     so that all elements aren't at the same index as before and don't
     have the same neighbors as before. Some like umreihen have a second
     to make it hard to get the original input from the output.
     
     Generally a higher number means the function has improved by either
     the output quality or the efficiency.
     """
     @staticmethod
-    def umreihen(num_lst, depth):
-        if not num_lst: # Check if the list is empty
+    def umreihen(num_lst: list, depth: int) -> list:
+        if not num_lst:  # Check if the list is empty
             return []
         
         curr_num_lst = num_lst
         for _ in range(depth):
             new_num_lst = []
             for num in curr_num_lst:
                 if num != 0:
@@ -24,15 +26,15 @@
                     new_num_lst.append(curr_num_lst[index - 1 if index > 0 else index])
                 else:
                     new_num_lst.append(curr_num_lst[num])
             curr_num_lst = new_num_lst
         return curr_num_lst
         
     @staticmethod
-    def umreihenTWO(num_lst, depth):
+    def umreihenTWO(num_lst: list, depth: int) -> list:
         if not num_lst:  # Check if the list is empty
             return []
 
         curr_num_lst = num_lst
         for _ in range(depth):
             new_num_lst, index = [], 0
             while len(curr_num_lst) > 0:
@@ -43,15 +45,15 @@
                 else:
                     new_num_lst.append(curr_num_lst[num])
                 index += 1
             curr_num_lst = new_num_lst
         return curr_num_lst
     
     @staticmethod
-    def umreihenTHREE(num_lst, depth):
+    def umreihenTHREE(num_lst: list, depth: int) -> list:
         if not num_lst:  # Check if the list is empty
             return []
 
         curr_num_lst = num_lst[:]
         print(len(num_lst))
         for _ in range(depth):
             new_num_lst, index = [], 0
@@ -66,15 +68,15 @@
                 index += 1
             new_num_lst.insert(0, curr_num_lst.pop(0))
             curr_num_lst = new_num_lst
             num_lst = curr_num_lst[:]
         return curr_num_lst
     
     @staticmethod
-    def umreihenFOUR(num_lst, depth):
+    def umreihenFOUR(num_lst: list, depth: int) -> list:
         if not num_lst:  # Check if the list is empty
             return []
 
         curr_num_lst = num_lst[:]
         #print(len(num_lst))
         for _ in range(depth):
             new_num_lst, index = [curr_num_lst.pop(-1)], 0
@@ -87,15 +89,15 @@
                     new_num_lst.append(curr_num_lst.pop(index))
                 index += 1
             curr_num_lst = new_num_lst
             num_lst = curr_num_lst[:]
         return curr_num_lst
     
     @staticmethod
-    def umsplitten(num_lst, width=2):
+    def umsplitten(num_lst: list, width: int = 2) -> Optional[list]:
         try:
             raise DeprecationWarning("This function is deprecated, please use umsplittedTWO or umsplittenCH")
         except Exception as e:
             print("Exec Error:", e)
             return # This doesn't work
         if len(num_lst) // 2 < width or len(num_lst) % 2 != 0: # Otherwise pairs don't match
             return None
@@ -106,41 +108,41 @@
         for i, x in enumerate(num_lst[split_point:]):
             pairs.append([x, num_lst[((x + width) % len(num_lst)) - 1]])
             
         lst_1, lst_2 = zip(*pairs)
         return lst_1 + lst_2
         
     @staticmethod
-    def umsplittenCH(num_lst, width=2):
+    def umsplittenCH(num_lst: list) -> Optional[list]:
         if len(num_lst) % 2 != 0:  # Ensure the list has an even number of elements
             return None
 
         split_point = len(num_lst) // 2
         lst_1 = num_lst[:split_point]
         lst_2 = num_lst[split_point:]
 
         result = []
         for a, b in zip(lst_1, lst_2):
             result.extend([a, b])
 
         return result
         
     @staticmethod
-    def umsplittenTWO(num_lst, width=2):
-        if width > len(num_lst) // 2:# or len(num_lst) % 2 != 0:
+    def umsplittenTWO(num_lst: list, width: int = 2) -> Optional[list]:
+        if width > len(num_lst) // 2:  # or len(num_lst) % 2 != 0:
             return None
 
         result = []
         for start in range(width):
             result.extend(num_lst[start::width])
 
         return result
         
     @staticmethod
-    def umsetzen(lst):
+    def umsetzen(lst: list) -> list:
         """
         The umsetzen function is designed to 
         move each element to a new spot and 
         make sure they don't have the same
         neighbor as before.
         """
         Dummy = type('Dummy', (object,), {'__init__': lambda self, *args, **kwargs: None,
@@ -159,24 +161,25 @@
                     new_lst.insert(0, filtered_list[0])
         #if len(new_lst) < len(lst):
         #    pass # Fix
             #for x, y in zip(lst[len(new_lst):], [0, 2, 4, 1, 5, 3][:len(lst) - len(new_lst)]):
             #    new_lst.append(x
         return new_lst
 
-def hashed_old(input, length, debug=False):
+
+def hashed_old(input_str: str, length: int, debug: bool = False):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
-    original_length = len(input)
+    original_length = len(input_str)
     if original_length > length: return "Please only input inputs shorter than length"
-    elif not isinstance(input, str): return "Please only pass strings as input"
-    filled_input = input.ljust(length, "0")
+    elif not isinstance(input_str, str): return "Please only pass strings as input"
+    filled_input = input_str.ljust(length, "0")
     debug_print("Filled: " + filled_input)
-    seed, input_lst = input, list(input)
+    seed, input_lst = input_str, list(input_str)
     shuffled_input = ""
     for i, char in enumerate(filled_input):
         if char == "0":
             random.seed(seed)
             rand_char = random.choice(input_lst)
             char = rand_char
             seed_lst = list(seed)
@@ -203,26 +206,27 @@
             split_lst[i2] = str1
             split_lst.insert(i2+1, str2)
         random.seed(param)
         random.shuffle(split_lst)
         i += 1
     return ''.join(split_lst)
 
-def hashed(input, length, debug=False):
+
+def hashed(input_str: str, length: int, debug: bool = False):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
-    original_length = len(input)
+    original_length = len(input_str)
     if original_length > length: return "Please only input inputs shorter than length"
-    elif not isinstance(input, str): return "Please only pass strings as input"
-    filled_input = input.ljust(length, "0")
+    elif not isinstance(input_str, str): return "Please only pass strings as input"
+    filled_input = input_str.ljust(length, "0")
     debug_print("Filled: " + filled_input)
-    seed, input_lst = input, list(input)
+    seed, input_lst = input_str, list(input_str)
     shuffled_input = ""
-    ord_lst = [ord(x) + original_length for x in input]
+    ord_lst = [ord(x) + original_length for x in input_str]
     print(ord_lst)
     for i, char in enumerate(filled_input):
         if char == "0":
             random.seed(seed)
             rand_char = random.choice(input_lst)
             char = rand_char
             seed_lst = list(seed)
@@ -249,15 +253,16 @@
             split_lst[i2] = str1
             split_lst.insert(i2+1, str2)
         random.seed(param)
         random.shuffle(split_lst)
         i += 1
     return ''.join(split_lst)
 
-def hashed_LS(input, length, debug=False):
+
+def hashed_LS(input_str: str, length: int, debug: bool = False):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
     def order_lst(original_length, input, seed1=200, seed2=30):
         ord_lst = [ord(x) + (i + 1) * (ord(x) + i) * (2 if x.islower() else 3 if x.isupper() else 1) for i, x in enumerate(input)]
         ord_lst = [str(int(original_length + sum(val * (ord(x) / 10 if i == j else ord(x) / 5) for j, x in enumerate(input)))) for i, val in enumerate(ord_lst)]
         # Splitting and reducing the values
@@ -278,22 +283,22 @@
     def reduce_lst(lst):
         import math
 
         # Apply logarithmic scaling and then modular reduction
         reduced_lst = [int(math.log(x + 1)) % 100 for x in lst]
 
         return reduced_lst
-    original_length = len(input)
+    original_length = len(input_str)
     if original_length > length: return "Please only input inputs shorter than length"
-    elif not isinstance(input, str): return "Please only pass strings as input"
-    filled_input = input.ljust(length, "0")
+    elif not isinstance(input_str, str): return "Please only pass strings as input"
+    filled_input = input_str.ljust(length, "0")
     debug_print("Filled: " + filled_input)
-    seed, input_lst = input, list(input)
+    seed, input_lst = input_str, list(input_str)
     shuffled_input = ""
-    ord_lst = order_lst(original_length, input) #[ord(x) + original_length for x in input]
+    ord_lst = order_lst(original_length, input_str) #[ord(x) + original_length for x in input]
     debug_print("Ord List: ", ord_lst)
     ord_lst = reduce_lst(ord_lst)
     for i, char in enumerate(filled_input):
         if char == "0":
             random.seed(seed)
             rand_char = random.choice(input_lst)
             char = rand_char
@@ -321,15 +326,16 @@
             split_lst[i2] = str1
             split_lst.insert(i2+1, str2)
         random.seed(param)
         random.shuffle(split_lst)
         i += 1
     return ''.join(split_lst)
 
-def hashed_LS2(input, length, debug=False):
+
+def hashed_LS2(input_str: str, length: int, debug: bool = False):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
     def order_lst(original_length, input, seed1=200, seed2=30):
         ord_lst = [ord(x) + (i + 1) * (ord(x) + i) * (2 if x.islower() else 3 if x.isupper() else 1) for i, x in enumerate(input)]
         ord_lst = [str(int(original_length + sum(val * (ord(x) / 10 if i == j else ord(x) / 5) for j, x in enumerate(input)))) for i, val in enumerate(ord_lst)]
         # Splitting and reducing the values
@@ -350,22 +356,22 @@
     def reduce_lst(lst):
         import math
 
         # Apply logarithmic scaling and then modular reduction
         reduced_lst = [int(math.log(x + 1)) % 100 for x in lst]
 
         return reduced_lst
-    original_length = len(input)
+    original_length = len(input_str)
     if original_length > length: return "Please only input inputs shorter than length"
-    elif not isinstance(input, str): return "Please only pass strings as input"
-    filled_input = input.ljust(length, "0")
+    elif not isinstance(input_str, str): return "Please only pass strings as input"
+    filled_input = input_str.ljust(length, "0")
     debug_print("Filled: " + filled_input)
-    seed, input_lst = input, list(input)
+    seed, input_lst = input_str, list(input_str)
     shuffled_input = ""
-    ord_lst = order_lst(original_length, input) #[ord(x) + original_length for x in input]
+    ord_lst = order_lst(original_length, input_str) #[ord(x) + original_length for x in input]
     debug_print("Ord List: ", ord_lst)
     #ord_lst = reduce_lst(ord_lst)
     for i, char in enumerate(filled_input):
         if char == "0":
             random.seed(seed)
             rand_char = random.choice(input_lst)
             char = rand_char
@@ -393,15 +399,16 @@
             split_lst[i2] = str1
             split_lst.insert(i2+1, str2)
         random.seed(param)
         random.shuffle(split_lst)
         i += 1
     return ''.join(split_lst)
 
-def hashed_latest(input_str, length, debug=False):
+
+def hashed_latest(input_str: str, length: int, debug: bool = False):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
     original_length = len(input_str)
     
     if original_length > length:
         return "Please only input strings shorter than length"
@@ -457,29 +464,31 @@
             split_lst[i2] = str1
             split_lst.insert(i2 + 1, str2)
             
         random.seed(param)
         random.shuffle(split_lst)
         i += 1
     return "".join(split_lst)
-    
-def hashed_wrapper(input, length, debug=False, sub_debug=False, sub_sub_debug=False, hash_func=lambda x, y, z: None):
+
+
+def hashed_wrapper(input_str: str, length: int, debug: bool = False, sub_debug: bool = False,
+                   sub_sub_debug: bool = False, hash_func: Callable[[str, int, bool], str] = lambda x, y, z: None):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
-    if len(input) <= length:
+    if len(input_str) <= length:
         debug_print("No need to chunk, hashing now ...")
-        final_hash = hash_func(input, length, sub_debug)
+        final_hash = hash_func(input_str, length, sub_debug)
     else:
         debug_print("Input is longer than requested length, chunking needed ...")
-        if len(input) % length != 0:
-            filled_input = input.ljust(((len(input)//length)+1)*length, "0") # What if it's exactly e.g. 3*length? Fixed
-            input = filled_input
+        if len(input_str) % length != 0:
+            filled_input = input_str.ljust(((len(input_str) // length) + 1) * length, "0") # What if it's exactly e.g. 3*length? Fixed
+            input_str = filled_input
             debug_print("Filled input: ", filled_input)
-        input_chunks = list(map(''.join, zip(*[iter(input)]*length))) # https://stackoverflow.com/questions/22571259/split-a-string-into-n-equal-parts from comment: This method comes straight from the docs for zip().
+        input_chunks = list(map(''.join, zip(*[iter(input_str)] * length))) # https://stackoverflow.com/questions/22571259/split-a-string-into-n-equal-parts from comment: This method comes straight from the docs for zip().
         debug_print("Input chunks: ", input_chunks)
         hashes_lst = []
         for inp_chunk in input_chunks:
             new_hash = hash_func(inp_chunk, length, sub_sub_debug)
             hashes_lst.append(new_hash)
             debug_print(f"Finished hashing chunk:{repr(new_hash)},Hashing next chunk ...")
         chunks = len(input_chunks)
@@ -492,28 +501,31 @@
         debug_print("New lengths", lengths) # x[y:y+y] x[-y:-2*y:-1]
         final_input = ''.join([x[i:y+i] if i % 2 == 0 else x[y+i:y+y+i] for i, (x, y) in enumerate(zip(hashes_lst, lengths))]) # How to get something unique from every hash and hash the result (should be smaller or equal to length) Fixed
         debug_print(f"Finished hashing all chunks. Hashing combined chunk ({repr(final_input)}) now ...")
         final_hash = hash_func(final_input, length, sub_debug)
         debug_print(final_hash, "<-", final_input, "\n", len(final_hash), "<-", len(final_input))
     return final_hash
 
-def hashed_wrapper_latest(input, length, debug=False, sub_debug=False, sub_sub_debug=False, hash_func=lambda x, y, z: None):
+
+def hashed_wrapper_latest(input_str: str, length: int, debug: bool = False, sub_debug: bool = False,
+                          sub_sub_debug: bool = False,
+                          hash_func: Callable[[str, int, bool], str] = lambda x, y, z: None):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
-    if len(input) <= length:
+    if len(input_str) <= length:
         debug_print("No need to chunk, hashing now ...")
-        final_hash = hash_func(input, length, sub_debug)
+        final_hash = hash_func(input_str, length, sub_debug)
     else:
         debug_print("Input is longer than requested length, chunking needed ...")
-        if len(input) % length != 0:
-            filled_input = input.ljust(((len(input)//length)+1)*length, "0") # What if it's exactly e.g. 3*length? Fixed
-            input = filled_input
+        if len(input_str) % length != 0:
+            filled_input = input_str.ljust(((len(input_str) // length) + 1) * length, "0") # What if it's exactly e.g. 3*length? Fixed
+            input_str = filled_input
             debug_print("Filled input: ", filled_input)
-        input_chunks = list(map(''.join, zip(*[iter(input)]*length))) # https://stackoverflow.com/questions/22571259/split-a-string-into-n-equal-parts from comment: This method comes straight from the docs for zip().
+        input_chunks = list(map(''.join, zip(*[iter(input_str)] * length))) # https://stackoverflow.com/questions/22571259/split-a-string-into-n-equal-parts from comment: This method comes straight from the docs for zip().
         debug_print("Input chunks: ", input_chunks)
         hashes_lst = []
         for inp_chunk in input_chunks:
             new_hash = hash_func(inp_chunk, length, sub_sub_debug)
             hashes_lst.append(new_hash)
             debug_print(f"Finished hashing chunk:{repr(new_hash)},Hashing next chunk ...")
         chunks = len(input_chunks)
@@ -526,36 +538,38 @@
         debug_print("New lengths", lengths) # x[y:y+y] x[-y:-2*y:-1]
         final_input = ''.join([x[i:y+i] if i % 2 == 0 else x[y+i:y+y+i] for i, (x, y) in enumerate(zip(hashes_lst, lengths))]) # How to get something unique from every hash and hash the result (should be smaller or equal to length) Fixed
         debug_print(f"Finished hashing all chunks. Hashing combined chunk ({repr(final_input)}) now ...")
         final_hash = hash_func(final_input, length, sub_debug)
         debug_print(final_hash, "<-", final_input, "\n", len(final_hash), "<-", len(final_input))
     return final_hash
 
-def reducer(input, ord_range, jump_size, debug=False):
+
+def reducer(input_str: str, ord_range: List[range], jump_size: int, debug: bool = False):
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs)
     max_range, min_range = max(ord_range), min(ord_range)
     output = ""
-    for i in input:
+    for i in input_str:
         ord_i = ord(i)
         debug_print(f"Char {repr(i)} -> Ord {ord_i}")
         if ord_i not in ord_range: # Just send it through both
             while ord_i > max_range:
                 ord_i -= jump_size
             i = chr(ord_i) # To make sure it's within chars allowed range
             ord_i = ord(i)
             debug_print(f"New char {repr(i)} -> Ord {ord_i}")
             while ord_i < min_range:
                 ord_i += jump_size
             i = chr(ord_i)
         output += i
     return output
 
-def big_reducer(input_str, ord_ranges, jump_size, tries, debug=False): # It works, but it's very ugly ...
+
+def big_reducer(input_str: str, ord_ranges: List[range], jump_size: int, tries: int, debug: bool = False): # It works, but it's very ugly ...
     def debug_print(*args, **kwargs):
         if debug:
             print(*args, **kwargs) # Maybe don't prepare ranges? Iterating over a dict is probably also more expensive than accessing the attributes of a range object
     def prepare_ranges(ranges): # NEVER use max, as it gets .stop-1, because that's how ranges work, but .stop is also more efficient
         return {k: v for k, v in sorted({range: [range.start, range.stop] for range in ranges}.items(), key=lambda r: r[0].start)}
     def within_ranges(ord_val, ranges): # Just prepare lists with all valid characters?
         in_range_lst = []
@@ -620,15 +634,15 @@
             ord_i = adjust_to_nearest_range(ord_i, ranges, jump_size, tries)
             char = chr(ord_i)
             debug_print(f"New char {repr(char)} -> Ord {ord_i}")
         output += char
     return output
     
 
-def num_hasher(input_str: str, length: int, char_range: range=range(32, 126), seed: int=1):
+def num_hasher(input_str: str, length: int, char_range: range = range(32, 126), seed: int = 1):
     """
     This hasher function hashes an input and gives out something
     with around the same length. This can be changed by appending
     random range chars using random.seed result.
 
     :str input_str:
     :int desired_length:
@@ -692,14 +706,13 @@
         print(num_hasher(input_string, desired_length, acceptable_chars))
 
         inp = "To hash: "
         print(num_hasher(inp, len(inp)))
     except Exception as e:
         print(f"Exception occurred {e}.")
         return False
-    else:
-        print("Test completed successfully.")
-        return True
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/web/actual_webtools.py` & `aplustools-1.4.8/aplustools/web/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,12 @@
-# actual_webtools - By me :)
-import requests
-from bs4 import BeautifulSoup
 import random
 from typing import List, Union, Optional, Generator, Dict
+from bs4 import BeautifulSoup, element
+import requests
 from urllib.parse import quote_plus, urlparse, urljoin
-import time
-
-
-import warnings
-warnings.warn("This module is new and not usable yet. Please use aplustools.web.webtools instead till release 1.5.0",
-              UserWarning,
-              stacklevel=2)
 
 
 def get_user_agent() -> str:
     _user_agent_list = [
         'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:66.0) Gecko/20100101 Firefox/66.0',
         'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
         'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
@@ -1776,193 +1768,151 @@
         "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.101 Safari/537.36",
         "Mozilla/5.0 (Windows NT 6.1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/86.0.4240.78 Safari/537.36",
         "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.102 Safari/537.36",
         "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_8_5) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.101 Safari/537.36"]
     return random.choice(_user_agent_list)
 
 
-def generate_user_agent():
-    # Define possible components of a user agent string
-    platforms = [
-        "Windows NT 10.0; Win64; x64",
-        "Macintosh; Intel Mac OS X 10_15_7",
-        "X11; Linux x86_64"
-    ]
-
-    browsers = [
-        "Mozilla/5.0 ({platform}) Gecko/20100101 Firefox/{firefox_version}",
-        "Mozilla/5.0 ({platform}) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{chrome_version} Safari/537.36",
-        "Mozilla/5.0 ({platform}) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{chrome_version} Safari/537.36 Edg/{edge_version}"
-    ]
-
-    # Randomly select components
-    platform = random.choice(platforms)
-    browser_template = random.choice(browsers)
-    firefox_version = f"{random.randint(50, 80)}.0"
-    chrome_version = f"{random.randint(70, 100)}.0.0.0"
-    edge_version = f"{random.randint(70, 100)}.0.1661.62"
-
-    # Generate the final user agent string
-    user_agent = browser_template.format(platform=platform, firefox_version=firefox_version,
-                                         chrome_version=chrome_version, edge_version=edge_version)
-    return user_agent
-
-
-def check_url(url: str, url_title: str, in_title: Optional[Union[str, List[str]]] = None,
-              blacklisted_websites: Optional[list] = None) -> Optional[str]:
-    if in_title is not None and not isinstance(in_title, list):
-        in_title = [in_title]
-
-    if in_title is None or all([str(x).lower() in url_title.lower() for x in in_title]):
-        # Checking if the URL is accessible or leads to a 404 error
+class WebPage:
+    def __init__(self, url: str, in_url_keywords: Optional[List[str]] = None):
+        self.url = url
+        self.user_agent = self.generate_user_agent()
+        self.headers = {"User-Agent": self.user_agent}
+
+        self.crawlable = self.is_crawlable(url)
+        self.in_url = all(keyword.lower() in url.lower() for keyword in in_url_keywords) if in_url_keywords else True
+        self.accessible, self.status_code = self.check_url(url, [])
+
+        self.page = None
+        self.soup = None
+
+        if self.accessible and self.crawlable:
+            self.fetch_page()
+
+    @staticmethod
+    def is_crawlable(url: str) -> bool:
+        """
+        Check if the URL can be crawled by checking the robots.txt file of the website.
+        """
         try:
-            response = requests.head(url, allow_redirects=True)  # Using HEAD request to get the headers
-            if response.status_code == 404:
-                print(f"The URL {url} leads to a 404 error, checking next result...")
-                return None
-        except requests.RequestException as e:
-            print(f"Error accessing URL {url}: {e}, checking next result...")
-            return None
-
-        if is_crawlable(url):
-            if blacklisted_websites is None or not url.split("/")[2] in blacklisted_websites:
-                return url
+            # Parse the given URL to get the netloc (domain) part
+            domain = urlparse(url).netloc
+            robots_txt_url = urljoin(f'https://{domain}', 'robots.txt')
+            response = requests.get(robots_txt_url)
+
+            if response.status_code == 200:
+                # If "Disallow: /" is found for User-agent: *, it means the website can't be crawled
+                if 'User-agent: *\nDisallow: /' in response.text:
+                    return False
+                return True
             else:
-                print("Blacklisted URL:", url)
-        else:
-            print(f"The URL {url} cannot be crawled, checking next result...")
-    return None
+                print(f"Failed to retrieve the robots.txt file, status code: {response.status_code}")
+        except Exception as e:
+            print(f"An error occurred while checking the robots.txt file: {e}")
+        return False  # Return False if there was an error or the robots.txt file couldn't be retrieved
+
+    @staticmethod
+    def check_url(url: str, blacklisted_websites: Optional[list] = None) -> (bool, Optional[int]):
+        """
+        Check if the URL is accessible and not blacklisted, return a tuple (accessible, status_code).
+        """
+        try:
+            response = requests.head(url, allow_redirects=True)
+            status_code = response.status_code
 
+            if blacklisted_websites and any(blacklisted in url for blacklisted in blacklisted_websites):
+                print(f"Blacklisted URL: {url}")
+                return False, status_code
+
+            if status_code == 404:
+                print(f"The URL {url} leads to a 404 error.")
+                return False, status_code
 
-def is_crawlable(url: str) -> bool:
-    """
-    Check if the URL can be crawled by checking the robots.txt file of the website.
-    """
-    try:
-        # Parse the given URL to get the netloc (domain) part
-        domain = urlparse(url).netloc
-        robots_txt_url = urljoin(f'https://{domain}', 'robots.txt')
-        response = requests.get(robots_txt_url)
-
-        if response.status_code == 200:
-            # If "Disallow: /" is found for User-agent: *, it means the website can't be crawled
-            if 'User-agent: *\nDisallow: /' in response.text:
-                return False
-            return True
-        else:
-            print(f"Failed to retrieve the robots.txt file, status code: {response.status_code}")
-    except Exception as e:
-        print(f"An error occurred while checking the robots.txt file: {e}")
-    return False  # Return False if there was an error or the robots.txt file couldn't be retrieved
+            return True, status_code
+        except requests.RequestException as e:
+            print(f"Error accessing URL {url}: {e}")
+            return False, None
+
+    @staticmethod
+    def generate_user_agent():
+        platforms = [
+            f"Windows NT {random.choice([10, 11])}.0; Win64; x64",
+            "Macintosh; Intel Mac OS X 10_15_7",
+            "X11; Linux x86_64",
+            f"iPhone; CPU iPhone OS {random.choice(range(10, 13))}_{random.choice(range(0, 7))} like Mac OS X",
+            f"Android {random.choice(range(8, 12))}; Mobile"
+        ]
+
+        browsers = [
+            "Mozilla/5.0 ({platform}) Gecko/20100101 Firefox/{firefox_version}",
+            "Mozilla/5.0 ({platform}) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{chrome_version} Safari/537.36",
+            "Mozilla/5.0 ({platform}) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/{chrome_version} Safari/537.36 Edg/{edge_version}",
+            "Mozilla/5.0 ({platform}) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Safari/605.1.15",
+            "Mozilla/5.0 ({platform}) AppleWebKit/537.36 (KHTML, like Gecko) Opera/{opera_version} Safari/537.36"
+        ]
+
+        # Randomly select components
+        platform = random.choice(platforms)
+        browser_template = random.choice(browsers)
+        firefox_version = f"{random.randint(50, 90)}.0"
+        chrome_version = f"{random.randint(70, 110)}.0.0.0"
+        edge_version = f"{random.randint(70, 100)}.0.{random.randrange(1000, 2000)}.{random.randrange(50, 99)}"
+        opera_version = f"{random.randint(60, 75)}.0.0.0"
+
+        # Generate the final user agent string
+        user_agent = browser_template.format(platform=platform, firefox_version=firefox_version,
+                                             chrome_version=chrome_version, edge_version=edge_version,
+                                             opera_version=opera_version)
+        return user_agent
 
+    def fetch_page(self):
+        try:
+            self.page = requests.get(self.url, headers=self.headers)
+            self.soup = BeautifulSoup(self.page.content, 'html.parser')
+        except requests.RequestException as e:
+            print(f"Failed to fetch page content: {e}")
 
-class Search:
-    def __init__(self, core=None, local_user_agent_num: int = 5):
-        self.core = core
-        self.local_user_agent_list = [get_user_agent() for _ in range(local_user_agent_num)]
-
-    def get_useragent(self) -> str:
-        return random.choice(self.local_user_agent_list)
-
-    def replace_core(self, new_core):
-        self.core = new_core
-
-    def search(self, prompt: str, num_results: int = 10):
-        if self.core:
-            return self.core.search(query=prompt, num_results=num_results, user_agent=self.get_useragent())
-        return prompt
-
-    def api_search(self, prompt: str, api_key: str, num_results: int = 10):
-        if self.core:
-            return self.core.api_search(query=prompt, api_key=api_key, num_results=num_results)
-        return prompt
-
-
-class BingSearchCore:
-    def search(self, prompt, user_agent):
-        return prompt
-
-    def api_search(self, query, api_key, custom_config_id: str = "", num_results=10):
-        search_url = "https://api.bing.microsoft.com/v7.0/search"
-        headers = {"Ocp-Apim-Subscription-Key": api_key}
-        params = {
-            "q": query,
-            "customconfig": custom_config_id,
-            "count": num_results
-        }
-        response = requests.get(search_url, headers=headers, params=params)
-        response.raise_for_status()
-        return response.json()
-
-
-class GoogleSearchCore:
-    def search(self, query: str, num_results: int = 10, user_agent: str = "", advanced: bool = False, check: bool = True,
-               blacklisted_websites: Optional[List[str]] = None) -> Union[List[str], List[Dict[str, str]]]:
-        proxies = None  # If you have proxy settings, configure them here
-        escaped_term = query.replace(" ", "+")
-        start = 0
-        results = []
-
-        while start < num_results:
-            resp = requests.get(
-                url="https://www.google.com/search",
-                headers={"User-Agent": user_agent},
-                params={
-                    "q": escaped_term,
-                    "num": num_results + 2,
-                    "start": start,
-                },
-                proxies=proxies,
-                timeout=5,
-            )
-            resp.raise_for_status()
-            soup = BeautifulSoup(resp.text, "html.parser")
-            result_block = soup.find_all("div", attrs={"class": "g"})
-
-            for result in result_block:
-                link = result.find("a", href=True)
-                title = result.find("h3")
-                description_box = result.find("div", {"style": "-webkit-line-clamp:2"})
-
-                if description_box:
-                    description = description_box.text
-
-                    if link and title and description:
-                        url = link["href"]
-                        if check and blacklisted_websites and any(
-                                blacklisted_website in url for blacklisted_website in blacklisted_websites):
-                            continue
-                        start += 1
-                        if advanced:
-                            results.append({"url": url, "title": title.text, "description": description})
-                        else:
-                            results.append(url)
-                        if len(results) == num_results:
-                            break
-
-            time.sleep(1)  # Sleep interval to prevent rapid requests
-
-        return results
-
-    def api_search(query, api_key, cse_id, num_results=10, start=1):
-        url = "https://www.googleapis.com/customsearch/v1"
-        params = {
-            "key": api_key,
-            "cx": cse_id,
-            "q": query,
-            "num": num_results,
-            "start": start
-        }
-        response = requests.get(url, params=params)
-        response.raise_for_status()  # Raises an exception for HTTP errors
-        return response.json()
+    def get_by_tag(self, tag: str) -> List[element.Tag]:
+        """Retrieve a list of all elements with the specified tag."""
+        if self.soup:
+            return self.soup.find_all(tag)
+        return []
+
+    def get_by_class(self, class_name: str) -> List[element.Tag]:
+        """Retrieve a list of all elements with the specified class."""
+        if self.soup:
+            return self.soup.find_all(class_=class_name)
+        return []
+
+    def get_soup(self, func: str, *args, **kwargs):
+        """Dynamically call a method from the BeautifulSoup instance with provided arguments."""
+        if self.soup and hasattr(self.soup, func):
+            method = getattr(self.soup, func)
+            if callable(method):
+                try:
+                    return method(*args, **kwargs)
+                except Exception as e:
+                    print(f"Error calling soup method {func}: {e}")
+        return None
+
+    def __repr__(self):
+        return (f"WebPage(url={self.url}, crawlable={self.crawlable}, in_url={self.in_url}, "
+                f"accessible={self.accessible}, status_code={self.status_code}, user_agent={self.user_agent})")
 
 
-class DuckDuckGoSearchCore:
-    pass
+def local_test():
+    try:
+        web_page = WebPage("https://github.com")
+        tags = web_page.get_by_tag('a')  # Get all anchor tags
+        classes = web_page.get_by_class('menu-item')  # Get all elements with class 'menu-item'
+        dynamic_call = web_page.get_soup('find_all', 'div',
+                                         class_='sidebar')  # Dynamically find all divs with class 'sidebar'
+        print(web_page, tags, classes, dynamic_call)
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return False
+    print("Test completed successfully.")
+    return True
 
 
 if __name__ == "__main__":
-    searcher = Search()#BingSearchCore())
-    #searcher.search("Hello World")
-    searcher.replace_core(GoogleSearchCore())
-    searcher.search("Hello World")
+    local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools/web/new_webtools.py` & `aplustools-1.4.8/aplustools/web/new_webtools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.6.2/aplustools/web/web_request.py` & `aplustools-1.4.8/aplustools/web/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,29 +67,28 @@
         adv_handler = UnifiedRequestHandlerAdvanced()  # It can also handle image content
 
         # Synchronous GET request
         adv_handler.request('GET', 'http://example.com', async_mode=False)
         # Asynchronous GET request
         adv_handler.request('GET', 'http://example.com', async_mode=True)
 
-        folder_path = "../test_data/images"
+        folder_path = "./test_data/images"
         os.makedirs(folder_path, exist_ok=True)
 
         # Synchronous binary request (e.g., image)
         image_content = adv_handler.request('GET', 'https://huggingface.co/p1atdev/MangaLineExtraction-hf/resolve/main/images/sample.jpg', async_mode=False, return_type='binary')
         with open(os.path.join(folder_path, './image.jpg'), 'wb') as file:
             file.write(image_content)
 
         # Asynchronous binary request (e.g., image)
         image_content_async = adv_handler.request('GET', 'https://huggingface.co/p1atdev/MangaLineExtraction-hf/resolve/main/images/sample.jpg', async_mode=True, return_type='binary')
         with open(os.path.join(folder_path, './image_async.jpg'), 'wb') as file:
             file.write(image_content_async)
     except Exception as e:
         print(f"An error occurred {e}")
         return False
-    else:
-        print("All tests succeeded successfully")
-        return True
+    print("All tests succeeded successfully")
+    return True
 
 
 if __name__ == "__main__":
     local_test()
```

### Comparing `aplustools-1.4.6.2/aplustools.egg-info/PKG-INFO` & `aplustools-1.4.8/aplustools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.6.2
+Version: 1.4.8
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -17,23 +17,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: BeautifulSoup4>=4.12.2
 Requires-Dist: winreg; os_name != "nt"
 Provides-Extra: data
 Requires-Dist: PySide6>=6.6.1; extra == "data"
-Requires-Dist: Pillow>=10.1.0; extra == "data"
+Requires-Dist: Pillow>=10.3.0; extra == "data"
 Requires-Dist: aiohttp>=3.9.3; extra == "data"
 Requires-Dist: opencv-python>=4.9.0.80; extra == "data"
 Requires-Dist: pillow_heif==0.15.0; extra == "data"
 Provides-Extra: web
 Requires-Dist: duckduckgo_search>=3.9.6; extra == "web"
 Provides-Extra: utils
-Requires-Dist: rich>=13.7.0; extra == "utils"
-Requires-Dist: pycryptodome>=3.19.0; extra == "utils"
+Requires-Dist: cryptography>=42.0.5; extra == "utils"
 Requires-Dist: brotli>=1.1.0; extra == "utils"
 Requires-Dist: zstandard>=0.22.0; extra == "utils"
 Requires-Dist: py7zr>=0.21.0; extra == "utils"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 
 # aplustools
@@ -71,62 +70,88 @@
 
 ## Usage
 
 Here are a few quick examples of how to use aplustools:
 
 ### Search Engine usage
 ```python
-from aplustools.web import new_webtools as wt
+from aplustools.web.search import Search, GoogleSearchCore
 
-# Call the `google_search` function with a query
-result = wt.search.google_provider.google_search("Cute puppies", wt.get_useragent(), 1)
+# Call the `google_provider` function with a query
+searcher = Search(GoogleSearchCore(advanced=True))
+results = searcher.search("Cute puppies", num_results=10)
 
 # Print the result
-print(result)
-```
+print(results)
 
-### Search Engine usage 2
-```python
-from aplustools.web import webtools as wt
+from aplustools.web.utils import WebPage
 
-# Call the `google_provider` function with a query
-searcher = wt.Search()
-result = searcher.google_provider("Cute puppies")
+web_page = WebPage(results[0].get("url"))
+
+response = None
+if web_page.crawlable:  # Google search does this automatically at the moment
+    response = web_page.page.content
+print(response)
 
-# Print the result
-print(result)
 ```
 
-### Logger
+### web requests
 ```python
-from aplustools.io import environment as env
-from aplustools.io import loggers
+from aplustools.web.request import UnifiedRequestHandler, UnifiedRequestHandlerAdvanced
+import os
 
-# Set the current working directory to the main script or executable
-env.set_working_dir_to_main_script_location()
+# Default request handler
+handler = UnifiedRequestHandler()
 
-# Create an instance of Logger
-p_logger = loggers.PrintLogger("my_logs_file.log", show_time=True, capture_print=False, 
-                     overwrite_print=True, print_passthrough=False, print_log_to_stdout=True)
-# Shows the time in the logs (Like this [12:33:21]) and overwrites the normal sys.stdout
+# Synchronous request
+handler.fetch('http://example.com', async_mode=False)
+# Asynchronous request
+handler.fetch('http://example.com', async_mode=True)
 
-# Call the `monitor_stdout` method and pass the logger object, this will overwrite sys.stdout from Text I/O to the logger object
-logger = loggers.monitor_stdout(logger=p_logger) # Return sys.stdout, so you can make sure it worked
+# Advanced request handler (you can pass extra keyword arguments, and it automatically raises for status)
+adv_handler = UnifiedRequestHandlerAdvanced()  # It can also handle image content
 
-# Log something
-p_logger.log("Hello, world!")
+# Synchronous GET request
+adv_handler.request('GET', 'http://example.com', async_mode=False)
+# Asynchronous GET request
+adv_handler.request('GET', 'http://example.com', async_mode=True)
 
-# Print something, it won't get captured or displayed
-print("Hello, beautiful world!")
+folder_path = "./test_data/images"
+os.makedirs(folder_path, exist_ok=True)
+
+# Synchronous binary request (e.g., image)
+image_content = adv_handler.request('GET', 'http://example.com/image.png', async_mode=False, return_type='binary')
+with open(os.path.join(folder_path, './image.png'), 'wb') as file:
+    file.write(image_content)
+
+# Asynchronous binary request (e.g., image)
+image_content_async = adv_handler.request('GET', 'http://example.com/image.png', async_mode=True, return_type='binary')
+with open(os.path.join(folder_path, './image_async.png'), 'wb') as file:
+    file.write(image_content_async)
 
-# Close the Logger object (returns sys.stdout to it's normal state)
-p_logger.close()
 ```
 
-### OnlineImage
+### ImageManager
+````python
+from aplustools.data.imagetools import ImageManager, OnlineImage
+import os
+
+os.makedirs("./test", exist_ok=True)
+manager = ImageManager("./test", use_async=True)
+image_index = manager.add_image(OnlineImage, "somewhere.com/image.jpg")
+
+manager.execute_func(image_index, "download_image")
+manager.execute_func(image_index, "convert_to_grayscale")
+manager.execute_func(image_index, "apply_filter")  # Default is blur
+manager.execute_func(image_index, "rotate_image", 12)
+manager.execute_func(image_index, "save_image_to_disk")  # Overwrites downloaded file
+
+````
+
+### ImageTypes
 ```python
 from aplustools.data.imagetools import OnlineImage, OfflineImage, ImageFilter, SVGCompatibleImage
 import os
 
 # Setup
 folder_path = "./images"
 os.makedirs(folder_path, exist_ok=True)
@@ -156,92 +181,25 @@
 offline_image.save_image_to_disk(os.path.join(folder_path, "transformed_image.png"))
 
 # Example svg image usage
 image_processor = SVGCompatibleImage("someSvg.svg", 300,
                                      (667, 800), magick_path=r".\ImageMagick",
                                      base_location='./')
 image_processor.save_image_to_disk()
-```
-
-### Git-Updater
-```python
-from aplustools.data.updaters import GithubUpdater, VersionNumber
-from aplustools.io.environment import get_temp
-from aplustools import set_dir_to_ex
-import sys
-import os
-
-set_dir_to_ex()
-
-__version__ = VersionNumber("0.0.1")
-
-# Initialize an updater
-updater = GithubUpdater("Adalfarus", "unicode-writer", "py")  # If you want to use exe
-latest_version = updater.get_latest_tag_version()             # you need to compile them
-                                                              # yourself, otherwise it
-# Check if an update is needed                                # won't work
-if __version__ >= latest_version:
-    sys.exit()
-
-# Updater method
-path, zip_path = os.path.join(os.getcwd(), "update"), os.path.join(get_temp(), f"apt-update_{latest_version}")
-
-os.makedirs(path, exist_ok=True)
-os.makedirs(zip_path, exist_ok=True)
-
-# Start the update in a separate thread
-update_thread = updater.update(path, zip_path, latest_version, implementation="none", 
-                               host="localhost", port=1264, non_blocking=True, wait_for_connection=True)
-update_thread.start()
-
-# Receive the update status generator and print them
-progress_bar = 1
-for i in updater.receive_update_status():
-    print(f"{i}%", end=f" PB{progress_bar}\n")
-    if i == 100:
-        progress_bar += 1  # Switch to second progress bar, when the downloading is finished
-update_thread.join()
-```
-
-### Webtools
-```python
-... # Continuing the first two examples
-
-# Print the result
-print(result)
 
-from aplustools.web.webtools import check_url, is_crawlable
-import requests
-
-if check_url(result, ''): # Not really nessesary, search does this automatically
-	response = requests.get(result)
-	...
-```
-
-### Environment
-```python
-... # Continuing the image example
-
-_, img_name, img_path = image2.download_image(base_path=str(folder_path))  # Make sure this directory exists
 
 from aplustools.io.environment import absolute_path, remv, copy
-from aplustools.childsplay import ImportClass  # Could be switched out to adultswork, but the string would need to get converted
-
-importer = ImportClass(hard=True)
-importer.import_all()  # Destroys your runtime python
 
-a_img_path = absolute_path(img_path)
+a_img_path = absolute_path(os.path.join(folder_path, "downloaded_image.jpg"))
 
-try:
-    copy(a_img_path, str(folder_path) + str(img_name).remove(".png") + str(" - Copy.png"))
-except ValueError:
-    copy(a_img_path, str(folder_path) + str(img_name.split(".")[-1]) + str(" - Copy.png"))
+copy(a_img_path, str(folder_path) + "downloaded_image" + " - Copy.jpg")
 
 remv(a_img_path)  # Remove the original image
-remv(str(folder_path))  # Remove the base directory
+remv(folder_path)  # Remove the base directory
+
 ```
 
 ### Faker
 ```python
 from aplustools.data.faker import TestDataGenerator
 
 test_data = TestDataGenerator()
@@ -250,20 +208,21 @@
 print("\n", end="")
 print(test_data.generate_random_name())
 print(test_data.generate_random_email())
 print(test_data.generate_random_password())
 print(test_data.generate_random_phone_number())
 print(test_data.generate_random_address())
 print(test_data.generate_random_birth_date())
+
 ```
 
 ### Dummy
 ```python
-from aplustools.utils.dummy import Dummy3 # Dummy3 is for Python 3
-import math, sys
+from aplustools.utils.dummy import Dummy3  # Dummy3 is for Python 3
+import math
 
 dummy = Dummy3()
 
 # Do a bunch of operations that would normally throw errors
 dummy.attr.func("", int3="")
 dummy["Hello"] = 1
 del dummy[1]
@@ -289,23 +248,24 @@
 dummy << dummy
 dummy >> dummy
 dummy -= 1_000_000
 num = 1
 num *= dummy
 
 if dummy:
-	print(True)
+    print(True)
 else:
-	print(False)
+    print(False)
 
 for x in dummy:
-	print(x)
+    print(x)
 
 type(dummy)
 print(dummy, "->", int(dummy), list(dummy), tuple(dummy), float(dummy))
+
 ```
 
 ### Hasher
 ```python
 from aplustools.utils.hasher import hashed_latest, hashed_wrapper_latest, reducer, big_reducer, num_hasher
 
 inp = "Hello beautiful world, how are you today, lovely star?"
@@ -325,62 +285,128 @@
 
 acceptable_chars = range(100, 200)
 
 num_hashed_inp_uni = num_hasher(inp, desired_length, acceptable_chars)
 num_hashed_inp_uni_2 = num_hasher(inp2, desired_length, acceptable_chars)
 
 print(f"{inp} ({len(inp)}) -> {num_hashed_inp_uni} ({len(num_hashed_inp_uni)})\n{inp2} ({len(inp2)}) -> {num_hashed_inp_uni_2} ({len(num_hashed_inp_uni_2)})")
+
 ```
 
 ### GenPass
 ```python
-from aplustools.utils.genpass import GeneratePasswords
+from aplustools.utils.genpass import SecurePasswordManager, GeneratePasswords
+
+manager = SecurePasswordManager()
+password = manager.generate_ratio_based_password_v2(length=26, letters_ratio=0.5, numbers_ratio=0.3,
+                                                    punctuations_ratio=0.2, exclude_similar=True)
+manager.add_password("example.com", "json-the-greatest", password)
+manager.store_in_buffer("example.com", 0)  # Stores unencrypted password in a buffer
+print(manager.get_password("example.com"), "|", manager.use_from_buffer(0))  # for faster access.
+
+print(GeneratePasswords.generate_custom_sentence_based_password_v1(
+    "Exploring the unknown -- discovering new horizons...", random_case=True, extra_char="_",
+    char_position="keep" or 0, num_length=5, special_chars_length=2))
+# "keep" just sets it to 0
+
+# These classes are mostly meant for secure interprocess bidirectional
+# communication using networks.
+from aplustools.utils.genpass import ControlCodeProtocol, SecureSocketServer, SecureSocketClient
+
+# Initialize the protocol
+prot = ControlCodeProtocol()
+
+# Create a client and a server
+client = SecureSocketClient(prot)
+sock = client.get_socket()
+server = SecureSocketServer(sock, prot)
+
+# Start key exchange and communication between server and client
+client.start_and_exchange_keys()  # Client has to start first
+server.start_and_exchange_keys()
+
+# Client sends a message and a control code to the server
+client.add_control_code("shutdown")
+client.add_message("HELLO SERVER")
+client.sendall()  # The message is still received as it sends one chunk here
+# which then get's decoded in one piece. The decoder decodes everything
+# into chunks and control codes are always put behind messages.
+
+# Server shuts down the client connection
+server.shutdown_client()
+print("DONE1")
+
+# There are also classes for one directional communication that are
+# more integrated.
+from aplustools.utils.genpass import ControlCodeProtocol, ServerMessageHandler, ClientMessageHandler
+import threading
+
+prot = ControlCodeProtocol()
+
+# Create message handlers for server and client
+encoder = ClientMessageHandler(prot)
+
+# Make a connection using the clients host and chosen port
+connection = encoder.get_socket()
+
+decoder = ServerMessageHandler(connection, prot)
+
+# Client prepares and sends a message
+encoder.add_message("Hello Server")
+encoder.send_control_message("shutdown")
+
+# Server receives and processes each chunk
+encoder.start()
+threading.Thread(decoder.listen_for_messages()).start()  # Blocking
+encoder.flush()  # Blocking until connection is established
 
-gen = GeneratePasswords(debug=True)
-password = gen.generate_ratio_based_password_v2(length=10, letters_ratio=0.5, numbers_ratio=0.3, punctuations_ratio=0.2, secure_random=True, exclude_similar=True)
-print(password)
 ```
 
-### web_requests
+### Github-Updater
 ```python
-from aplustools.web.web_request import UnifiedRequestHandler, UnifiedRequestHandlerAdvanced
+from aplustools.data.updaters import GithubUpdater, VersionNumber
+from aplustools.io.environment import get_temp
+from aplustools import set_dir_to_ex
+import sys
 import os
 
-# Default request handler
-handler = UnifiedRequestHandler()
+set_dir_to_ex()
 
-# Synchronous request
-handler.fetch('http://example.com', async_mode=False)
-# Asynchronous request
-handler.fetch('http://example.com', async_mode=True)
+__version__ = VersionNumber("0.0.1")
 
-# Advanced request handler (you can pass extra keyword arguments, and it automatically raises for status)
-adv_handler = UnifiedRequestHandlerAdvanced()  # It can also handle image content
+# Initialize an updater
+updater = GithubUpdater("Adalfarus", "unicode-writer", "py")  # If you want to use exe
+latest_version = updater.get_latest_tag_version()             # you need to compile them
+                                                              # yourself, otherwise it
+# Check if an update is needed                                # won't work
+if __version__ >= latest_version:
+    sys.exit()
 
-# Synchronous GET request
-adv_handler.request('GET', 'http://example.com', async_mode=False)
-# Asynchronous GET request
-adv_handler.request('GET', 'http://example.com', async_mode=True)
+# Updater method
+path, zip_path = os.path.join(os.getcwd(), "update"), os.path.join(get_temp(), f"apt-update_{latest_version}")
 
-folder_path = "../test_data/images"
-os.makedirs(folder_path, exist_ok=True)
+os.makedirs(path, exist_ok=True)
+os.makedirs(zip_path, exist_ok=True)
 
-# Synchronous binary request (e.g., image)
-image_content = adv_handler.request('GET', 'http://example.com/image.png', async_mode=False, return_type='binary')
-with open(os.path.join(folder_path, './image.png'), 'wb') as file:
-    file.write(image_content)
+# Start the update in a separate thread
+update_thread = updater.update(path, zip_path, latest_version, implementation="none", 
+                               host="localhost", port=1264, non_blocking=True, wait_for_connection=True)
+update_thread.start()
+
+# Receive the update status generator and print them
+progress_bar = 1
+for i in updater.receive_update_status():
+    print(f"{i}%", end=f" PB{progress_bar}\n")
+    if i == 100:
+        progress_bar += 1  # Switch to second progress bar, when the downloading is finished
+update_thread.join()
 
-# Asynchronous binary request (e.g., image)
-image_content_async = adv_handler.request('GET', 'http://example.com/image.png', async_mode=True, return_type='binary')
-with open(os.path.join(folder_path, './image_async.png'), 'wb') as file:
-    file.write(image_content_async)
 ```
 
 ### ArguMint
-
 ```python
 from aplustools.package.argumint import ArgStruct, ArguMint
 from typing import Literal
 import sys
 
 
 def sorry(*args, **kwargs):
@@ -430,73 +456,163 @@
 sys.argv[0] = "apt"
 
 # Testing
 # sys.argv = ["apt", "help"]
 # sys.argv = ["apt", "build", "file", "./file.py", "--num=19"]
 parser.parse_cli(sys, "native_light")
 print(timer.end())
+
+```
+
+### compressor
+```python
+from aplustools.data.compressor import FileContainerV3, BrotliChunkCompressor
+import os
+
+
+compressor = BrotliChunkCompressor()
+container = FileContainerV3(compressor, block_size=2048*2048)
+
+image_data = {}
+for file in os.listdir("./images"):
+    if file.lower().endswith(".png"):
+        with open(os.path.join("./images", file), "rb") as f:
+            image_file_data = b''.join(f.readlines())
+            image_data[file] = image_file_data
+
+for file_name, image in image_data.items():
+    container.add_file(file_name, image)
+
+# Get the compressed data
+compressed_data = container.get_compressed_container()
+
+print("Compression done")
+
+with open("./files.bin", "wb") as f:
+    f.write(compressed_data)
+
+print("Wrote bin")
+
+# To extract a specific file from the compressed data
+try:
+    decompressed_images = []
+    for i in range(len(image_data)):
+        decompressed_image = container.extract_file(compressed_data, i)
+        decompressed_images.append(decompressed_image)
+except Exception as e:
+    print("Indexing not possible, error", e, "\n")
+    decompressed_images = []
+    for file_name in image_data.keys():
+        decompressed_image = container.extract_file(compressed_data, file_name)
+        decompressed_images.append(decompressed_image)
+compression_ratio = len(compressed_data) / sum(len(x) for x in image_data.values())
+
+print(f"Original size: {sum(len(x) for x in image_data.values())} bytes")
+print(f"Compressed size: {len(compressed_data)} bytes")
+print(f"Compression ratio: {compression_ratio:.2f}")
+
+for i, decompressed_image in enumerate(decompressed_images):
+    with open(f"./decompressed_images/image{i}.png", "wb") as f:
+        f.write(decompressed_image)
+
+```
+
+### Logger
+```python
+from aplustools.io import environment as env
+from aplustools.io import loggers
+
+# Set the current working directory to the main script or executable
+env.set_working_dir_to_main_script_location()
+
+# Create an instance of Logger
+p_logger = loggers.PrintLogger("my_logs_file.log", show_time=True, capture_print=False, 
+                     overwrite_print=True, print_passthrough=False, print_log_to_stdout=True)
+# Shows the time in the logs (Like this [12:33:21]) and overwrites the normal sys.stdout
+
+# Call the `monitor_stdout` method and pass the logger object, this will overwrite sys.stdout from Text I/O to the logger object
+logger = loggers.monitor_stdout(logger=p_logger) # Return sys.stdout, so you can make sure it worked
+
+# Log something
+p_logger.log("Hello, world!")
+
+# Print something, it won't get captured or displayed
+print("Hello, beautiful world!")
+
+# Close the Logger object (returns sys.stdout to it's normal state)
+p_logger.close()
+
 ```
+
 (Correct shortform for aplustools is apt, so please use ```import aplustools as apt``` for consistency)
 
 There are multiple clis added through this package:
 
 ### pype (python pipe)
 ```bash
 C:\Users\user_>pype
-Enter Python expression: 1+2
+Enter Python expression: 1 + 2
 3
 
-C:\Users\user_>pype 1//3
+C:\Users\user_>pype 1 // 3
 0
 ```
 ### upype (unified python pipe)
 ```bash
 C:\Users\user_>upype import aplustools; print(aplustools.__version__)
 1.4.4
 
 C:\Users\user_>upype
 Enter Python code (type 'end' on a new line to finish):
 ... class Test:
 ...     def hello_word(self):
-...             print("Hello, ya dunce!")
+...             print("Hello, you!")
 ... test = Test()
 ... test.hello_word()
 ... end
-Hello, ya dunce!
+Hello, you!
 ```
 ### apt
 Can currently run tests with ```apt tests run``` and show a basic help using ```apt help```.
 
 
 For more detailed usage and examples, check out our [documentation](https://github.com/adalfarus/aplustools/wiki).
 
 ## Naming convention, dependencies and more
 [PEP 8 -- Style Guide for Python Code](https://peps.python.org/pep-0008/#naming-conventions)
 
 For modules I use 'lowercase', classes are 'CapitalizedWords' and functions and methods are 'lower_case_with_underscores'.
 
-Dependencies (except for the standart libraries) are: 
-- data.database, io.environment, io.loggers, utils.mappers, data.faker, utils.dummy, utils.hasher, package.lazy_loader, package.timid, adultswork, childsplay - none
-- data.github-updater-cmd - requests
-- data.github-updater-gui - requests, PySide6
-- data.github-updater, data.updaters - requests
-- data.imagetools - Pillow, aiohttp, requests, wand
-- data.advanced_imagetools - opencv-python, aiohttp, wand, pillow_heif
-- web.webtools - requests, duckduckgo_search, BeautifulSoup4 - duckduckgo_search is only used for Search.duckduckgo_provider, if you don't want to use it, use Search._duckduckgo_provider instead.
-- utils.genpass - pycryptodome, rich
-- web.new_webtools, web.actual_webtools - requests, BeautifulSoup4
-- web.web_request - requests, aiohttp
-- utils.compressor - brotli, zstandard, py7zr
+Dependencies (except for the standard libraries) are: 
+- [`none`]
+  - data.database
+  - io.environment
+  - io.loggers
+  - data.faker
+  - utils.dummy
+  - utils.hasher
+  - package.lazy_loader
+  - package.timid
+- [`requests`]
+  - data.github-updater-none
+  - data.updaters
+  - data.github-updater-cmd
+- data.github-updater-gui - [`requests`, `PySide6`]
+- data.imagetools - [`Pillow`, `aiohttp`, `requests`, `wand`]
+- data.advanced_imagetools - [`opencv-python`, `aiohttp`, `wand`, `pillow_heif`]
+- web.search, web.utils - [`requests`, `BeautifulSoup4`]
+- utils.genpass - [`cryptography`]
+- web.request - [`requests`, `aiohttp`]
+- utils.compressor - [`brotli`, `zstandard`, `py7zr`]
+- io.gui - [`PySide6`]
 
 Sub-Modules that may be removed in future updates due to being hard to support or simply unneeded.
 
-- database (maybe unneeded and hard to support if more dbs are added)
-- actual_webtools, new_webtools, webtools search-machines (hard to support)
+- database (maybe unneeded and hard to support if more dbs are added -> new_database is being developed)
 - loggers (maybe unneeded)
-- childsplay & adultswork (maybe unneeded)
 
 ## Contributing
 
 We welcome contributions! Please see our [contributing guidelines](https://github.com/adalfarus/aplustools/blob/main/CONTRIBUTING.md) for more details on how you can contribute to aplustools.
 
 1. Fork the repository
 2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
```

### Comparing `aplustools-1.4.6.2/aplustools.egg-info/SOURCES.txt` & `aplustools-1.4.8/aplustools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 LICENSE
 README.md
 pyproject.toml
 aplustools/__init__.py
 aplustools/_direct_functions.py
-aplustools/adultswork.py
-aplustools/childsplay.py
 aplustools/cli.py
 aplustools.egg-info/PKG-INFO
 aplustools.egg-info/SOURCES.txt
 aplustools.egg-info/dependency_links.txt
 aplustools.egg-info/entry_points.txt
 aplustools.egg-info/requires.txt
 aplustools.egg-info/top_level.txt
 aplustools/data/__init__.py
 aplustools/data/_direct_functions.py
 aplustools/data/advanced_imagetools.py
+aplustools/data/compressor.py
 aplustools/data/database.py
+aplustools/data/database_new.py
 aplustools/data/faker.py
 aplustools/data/github-updater-cmd.py
 aplustools/data/github-updater-gui.py
 aplustools/data/github-updater-none.py
 aplustools/data/imagetools.py
 aplustools/data/updaters.py
 aplustools/io/__init__.py
 aplustools/io/environment.py
 aplustools/io/loggers.py
+aplustools/io/system_Test.py
 aplustools/package/__init__.py
+aplustools/package/_direct_functions.py
 aplustools/package/argu_mint_old.py
 aplustools/package/argumint.py
-aplustools/package/lazy_loader.py
 aplustools/package/timid.py
 aplustools/tests/__init__.py
 aplustools/tests/test_data.py
 aplustools/tests/test_general.py
 aplustools/tests/test_io.py
 aplustools/tests/test_package.py
 aplustools/tests/test_utils.py
 aplustools/tests/test_web.py
 aplustools/utils/__init__.py
 aplustools/utils/_direct_functions.py
-aplustools/utils/compressor.py
 aplustools/utils/dummy.py
 aplustools/utils/genpass.py
 aplustools/utils/hasher.py
-aplustools/utils/mappers.py
 aplustools/web/__init__.py
 aplustools/web/_direct_functions.py
-aplustools/web/actual_webtools.py
 aplustools/web/new_webtools.py
-aplustools/web/web_request.py
-aplustools/web/webtools.py
+aplustools/web/request.py
+aplustools/web/search.py
+aplustools/web/utils.py
```

### Comparing `aplustools-1.4.6.2/pyproject.toml` & `aplustools-1.4.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["aplustools", "aplustools.data", "aplustools.io", "aplustools.utils", "aplustools.web", "aplustools.package", "aplustools.tests"]
 
 [project]
 name = "aplustools"
-version = "1.4.6.2"
+version = "1.4.8"
 dependencies = [
   "requests>=2.31.0",
   "BeautifulSoup4>=4.12.2",
   "winreg; os_name != 'nt'",
 ]
 requires-python = ">= 3.9"
 authors = [
@@ -29,23 +29,22 @@
 	"Programming Language :: Python",
 	"Natural Language :: English"
 ]
 
 [project.optional-dependencies]
 data = [
   "PySide6>=6.6.1",
-  "Pillow>=10.1.0",
+  "Pillow>=10.3.0",
   "aiohttp>=3.9.3",
   "opencv-python>=4.9.0.80",
   "pillow_heif==0.15.0"
 ]
 web = ["duckduckgo_search>=3.9.6"]
 utils = [
-  "rich>=13.7.0",
-  "pycryptodome>=3.19.0",
+  "cryptography>=42.0.5",
   "brotli>=1.1.0",
   "zstandard>=0.22.0",
   "py7zr>=0.21.0"
 ]
 dev = ["pytest"]
 
 [project.urls]
```

