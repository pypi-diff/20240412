# Comparing `tmp/aplustools-1.4.8.tar.gz` & `tmp/aplustools-1.4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplustools-1.4.8.tar", last modified: Fri Apr 12 10:00:48 2024, max compression
+gzip compressed data, was "aplustools-1.4.8.1.tar", last modified: Fri Apr 12 10:44:33 2024, max compression
```

## Comparing `aplustools-1.4.8.tar` & `aplustools-1.4.8.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.797835 aplustools-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 10:00:44.000000 aplustools-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-12 10:00:48.797835 aplustools-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19343 2024-04-12 10:00:44.000000 aplustools-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.789835 aplustools-1.4.8/aplustools/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.789835 aplustools-1.4.8/aplustools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28389 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/advanced_imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/database_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/github-updater-cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/github-updater-gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/github-updater-none.py
--rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/data/updaters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.789835 aplustools-1.4.8/aplustools/io/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/io/system_Test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/package/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/argu_mint_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    19452 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/argumint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/package/timid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/tests/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/genpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/utils/hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools/web/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/new_webtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/search.py
--rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-04-12 10:00:44.000000 aplustools-1.4.8/aplustools/web/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:00:48.793835 aplustools-1.4.8/aplustools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 10:00:48.000000 aplustools-1.4.8/aplustools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-12 10:00:44.000000 aplustools-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:00:48.797835 aplustools-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.421985 aplustools-1.4.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20299 2024-04-12 10:44:33.421985 aplustools-1.4.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19343 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.409985 aplustools-1.4.8.1/aplustools/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.413985 aplustools-1.4.8.1/aplustools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28389 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/advanced_imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/database_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/github-updater-cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/github-updater-gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/github-updater-none.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/data/updaters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.413985 aplustools-1.4.8.1/aplustools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/io/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/io/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/io/system_Test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.417985 aplustools-1.4.8.1/aplustools/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/package/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/package/argu_mint_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/package/argumint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/package/timid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.417985 aplustools-1.4.8.1/aplustools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.417985 aplustools-1.4.8.1/aplustools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/utils/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/utils/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/utils/genpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/utils/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.421985 aplustools-1.4.8.1/aplustools/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/web/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/web/new_webtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/web/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/web/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/aplustools/web/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:44:33.421985 aplustools-1.4.8.1/aplustools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20299 2024-04-12 10:44:33.000000 aplustools-1.4.8.1/aplustools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 10:44:33.000000 aplustools-1.4.8.1/aplustools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:44:33.000000 aplustools-1.4.8.1/aplustools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:44:33.000000 aplustools-1.4.8.1/aplustools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 10:44:33.000000 aplustools-1.4.8.1/aplustools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 10:44:33.000000 aplustools-1.4.8.1/aplustools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-12 10:44:28.000000 aplustools-1.4.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:44:33.421985 aplustools-1.4.8.1/setup.cfg
```

### Comparing `aplustools-1.4.8/LICENSE` & `aplustools-1.4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/PKG-INFO` & `aplustools-1.4.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.8
+Version: 1.4.8.1
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -14,21 +14,22 @@
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: BeautifulSoup4>=4.12.2
-Requires-Dist: winreg; os_name != "nt"
+Requires-Dist: winreg; os_name == "nt"
 Provides-Extra: data
 Requires-Dist: PySide6>=6.6.1; extra == "data"
 Requires-Dist: Pillow>=10.3.0; extra == "data"
 Requires-Dist: aiohttp>=3.9.3; extra == "data"
 Requires-Dist: opencv-python>=4.9.0.80; extra == "data"
 Requires-Dist: pillow_heif==0.15.0; extra == "data"
+Requires-Dist: numpy==1.26.4; extra == "data"
 Provides-Extra: web
 Requires-Dist: duckduckgo_search>=3.9.6; extra == "web"
 Provides-Extra: utils
 Requires-Dist: cryptography>=42.0.5; extra == "utils"
 Requires-Dist: brotli>=1.1.0; extra == "utils"
 Requires-Dist: zstandard>=0.22.0; extra == "utils"
 Requires-Dist: py7zr>=0.21.0; extra == "utils"
```

### Comparing `aplustools-1.4.8/README.md` & `aplustools-1.4.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/__init__.py` & `aplustools-1.4.8.1/aplustools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # aplustools __init__
-__version__ = "1.4.8"
+__version__ = "1.4.8.1"
 
 from aplustools.package import LazyModuleLoader as _LazyModuleLoader
 
 # Lazy loading modules
 io = _LazyModuleLoader('aplustools.io')
 data = _LazyModuleLoader('aplustools.data')
 utils = _LazyModuleLoader('aplustools.utils')
```

### Comparing `aplustools-1.4.8/aplustools/_direct_functions.py` & `aplustools-1.4.8.1/aplustools/_direct_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     exit(-1073741510)  # 130 / 0xC000013A
 
 
 def install_all_dependencies():
     success = _install_dependencies_lst(["requests==2.31.0", "Pillow==10.3.0", "BeautifulSoup4==4.12.3",
                                          "duckduckgo_search==3.9.3", "cryptography==42.0.5", "PySide6==6.6.1",
                                          "aiohttp==3.9.3", "opencv-python==4.9.0.80", "brotli==1.1.0",
-                                         "zstandard==0.22.0", "py7zr==0.21.0", "pillow_heif==0.15.0"])
+                                         "zstandard==0.22.0", "py7zr==0.21.0", "pillow_heif==0.15.0", "numpy==1.26.4"])
     if not success:
         return
     print("Done, all possible dependencies installed ...")
 
 
 def set_dir_to_ex():
     import __main__
```

### Comparing `aplustools-1.4.8/aplustools/cli.py` & `aplustools-1.4.8.1/aplustools/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from aplustools import execute_python_command
 from aplustools.io.environment import change_working_dir_to_script_location
 import subprocess
 import os
 import shutil
 import sys
-from aplustools.package.argu_mint_old import ArguMint, ArgStruct
+from aplustools.package.argumint import ArguMint, ArgStruct
 
 
 def pype_command():
     """Pype"""
     if len(sys.argv) > 1:
         expression = ' '.join(sys.argv[1:])
         try:
```

### Comparing `aplustools-1.4.8/aplustools/data/__init__.py` & `aplustools-1.4.8.1/aplustools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/advanced_imagetools.py` & `aplustools-1.4.8.1/aplustools/data/advanced_imagetools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/compressor.py` & `aplustools-1.4.8.1/aplustools/data/compressor.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/database.py` & `aplustools-1.4.8.1/aplustools/data/database.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/database_new.py` & `aplustools-1.4.8.1/aplustools/data/database_new.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/faker.py` & `aplustools-1.4.8.1/aplustools/data/faker.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/github-updater-cmd.py` & `aplustools-1.4.8.1/aplustools/data/github-updater-cmd.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/github-updater-gui.py` & `aplustools-1.4.8.1/aplustools/data/github-updater-gui.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/github-updater-none.py` & `aplustools-1.4.8.1/aplustools/data/github-updater-none.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/imagetools.py` & `aplustools-1.4.8.1/aplustools/data/imagetools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/data/updaters.py` & `aplustools-1.4.8.1/aplustools/data/updaters.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/io/environment.py` & `aplustools-1.4.8.1/aplustools/io/environment.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/io/loggers.py` & `aplustools-1.4.8.1/aplustools/io/loggers.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/io/system_Test.py` & `aplustools-1.4.8.1/aplustools/io/system_Test.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/package/__init__.py` & `aplustools-1.4.8.1/aplustools/package/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/package/_direct_functions.py` & `aplustools-1.4.8.1/aplustools/package/_direct_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         try:
             proc = _execute_python_command(arguments=["-m", "pip", "install", dep])
             if proc.returncode != 0:
                 raise
         except Exception as e:
             print("An error occurred:" + str(e))
             return False
-        return True
+    return True
 
 
 def install_dependencies():
     success = install_dependencies_lst([])
     if not success:
         return
     print("Done, all possible dependencies for the package module installed ...")
```

### Comparing `aplustools-1.4.8/aplustools/package/argu_mint_old.py` & `aplustools-1.4.8.1/aplustools/package/argu_mint_old.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/package/argumint.py` & `aplustools-1.4.8.1/aplustools/package/argumint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, Callable, Union, Literal, List, get_type_hints, Any
-from pydantic import BaseModel, ValidationError, Field, create_model
+# from pydantic import BaseModel, ValidationError, Field, create_model
 from argparse import ArgumentParser
 import sys
 import re
 
 
 class ArgumentParsingError(Exception):
     def __init__(self, message: str, index: int):
```

### Comparing `aplustools-1.4.8/aplustools/package/timid.py` & `aplustools-1.4.8.1/aplustools/package/timid.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/tests/test_data.py` & `aplustools-1.4.8.1/aplustools/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/utils/__init__.py` & `aplustools-1.4.8.1/aplustools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/utils/_direct_functions.py` & `aplustools-1.4.8.1/aplustools/utils/_direct_functions.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/utils/dummy.py` & `aplustools-1.4.8.1/aplustools/utils/dummy.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/utils/genpass.py` & `aplustools-1.4.8.1/aplustools/utils/genpass.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/utils/hasher.py` & `aplustools-1.4.8.1/aplustools/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/web/__init__.py` & `aplustools-1.4.8.1/aplustools/web/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/web/new_webtools.py` & `aplustools-1.4.8.1/aplustools/web/new_webtools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/web/request.py` & `aplustools-1.4.8.1/aplustools/web/request.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/web/search.py` & `aplustools-1.4.8.1/aplustools/web/search.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools/web/utils.py` & `aplustools-1.4.8.1/aplustools/web/utils.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/aplustools.egg-info/PKG-INFO` & `aplustools-1.4.8.1/aplustools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.8
+Version: 1.4.8.1
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -14,21 +14,22 @@
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: BeautifulSoup4>=4.12.2
-Requires-Dist: winreg; os_name != "nt"
+Requires-Dist: winreg; os_name == "nt"
 Provides-Extra: data
 Requires-Dist: PySide6>=6.6.1; extra == "data"
 Requires-Dist: Pillow>=10.3.0; extra == "data"
 Requires-Dist: aiohttp>=3.9.3; extra == "data"
 Requires-Dist: opencv-python>=4.9.0.80; extra == "data"
 Requires-Dist: pillow_heif==0.15.0; extra == "data"
+Requires-Dist: numpy==1.26.4; extra == "data"
 Provides-Extra: web
 Requires-Dist: duckduckgo_search>=3.9.6; extra == "web"
 Provides-Extra: utils
 Requires-Dist: cryptography>=42.0.5; extra == "utils"
 Requires-Dist: brotli>=1.1.0; extra == "utils"
 Requires-Dist: zstandard>=0.22.0; extra == "utils"
 Requires-Dist: py7zr>=0.21.0; extra == "utils"
```

### Comparing `aplustools-1.4.8/aplustools.egg-info/SOURCES.txt` & `aplustools-1.4.8.1/aplustools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8/pyproject.toml` & `aplustools-1.4.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["aplustools", "aplustools.data", "aplustools.io", "aplustools.utils", "aplustools.web", "aplustools.package", "aplustools.tests"]
 
 [project]
 name = "aplustools"
-version = "1.4.8"
+version = "1.4.8.1"
 dependencies = [
   "requests>=2.31.0",
   "BeautifulSoup4>=4.12.2",
-  "winreg; os_name != 'nt'",
+  "winreg; os_name == 'nt'",
 ]
 requires-python = ">= 3.9"
 authors = [
   {name = "Cariel Becker", email = "cariel.becker@gmx.de"},
 ]
 maintainers = [
   {name = "Cariel Becker", email = "cariel.becker@gmx.de"},
@@ -32,15 +32,16 @@
 
 [project.optional-dependencies]
 data = [
   "PySide6>=6.6.1",
   "Pillow>=10.3.0",
   "aiohttp>=3.9.3",
   "opencv-python>=4.9.0.80",
-  "pillow_heif==0.15.0"
+  "pillow_heif==0.15.0",
+  "numpy==1.26.4"
 ]
 web = ["duckduckgo_search>=3.9.6"]
 utils = [
   "cryptography>=42.0.5",
   "brotli>=1.1.0",
   "zstandard>=0.22.0",
   "py7zr>=0.21.0"
```

