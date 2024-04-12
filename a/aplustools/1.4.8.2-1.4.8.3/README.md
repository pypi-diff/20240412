# Comparing `tmp/aplustools-1.4.8.2.tar.gz` & `tmp/aplustools-1.4.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplustools-1.4.8.2.tar", last modified: Fri Apr 12 10:57:38 2024, max compression
+gzip compressed data, was "aplustools-1.4.8.3.tar", last modified: Fri Apr 12 11:16:09 2024, max compression
```

## Comparing `aplustools-1.4.8.2.tar` & `aplustools-1.4.8.3.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.437554 aplustools-1.4.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-12 10:57:38.437554 aplustools-1.4.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19478 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.425554 aplustools-1.4.8.2/aplustools/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.429554 aplustools-1.4.8.2/aplustools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28389 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/advanced_imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/database_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/github-updater-cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/github-updater-gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/github-updater-none.py
--rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/data/updaters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.429554 aplustools-1.4.8.2/aplustools/io/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/io/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/io/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/io/system_Test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.433554 aplustools-1.4.8.2/aplustools/package/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/package/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/package/argu_mint_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/package/argumint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/package/timid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.433554 aplustools-1.4.8.2/aplustools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/tests/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.433554 aplustools-1.4.8.2/aplustools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/utils/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/utils/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/utils/genpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/utils/hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.433554 aplustools-1.4.8.2/aplustools/web/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/web/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/web/new_webtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/web/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/web/search.py
--rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/aplustools/web/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:57:38.437554 aplustools-1.4.8.2/aplustools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20395 2024-04-12 10:57:38.000000 aplustools-1.4.8.2/aplustools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 10:57:38.000000 aplustools-1.4.8.2/aplustools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:57:38.000000 aplustools-1.4.8.2/aplustools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 10:57:38.000000 aplustools-1.4.8.2/aplustools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 10:57:38.000000 aplustools-1.4.8.2/aplustools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 10:57:38.000000 aplustools-1.4.8.2/aplustools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-12 10:57:33.000000 aplustools-1.4.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:57:38.437554 aplustools-1.4.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.593285 aplustools-1.4.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-04-12 11:16:09.593285 aplustools-1.4.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19488 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.585286 aplustools-1.4.8.3/aplustools/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.585286 aplustools-1.4.8.3/aplustools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28389 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/advanced_imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/database_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/github-updater-cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/github-updater-gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/github-updater-none.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/data/updaters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.589285 aplustools-1.4.8.3/aplustools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.589285 aplustools-1.4.8.3/aplustools/io/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/gui/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41238 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/gui/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188419 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/gui/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/io/system_Test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.589285 aplustools-1.4.8.3/aplustools/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/package/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/package/argu_mint_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/package/argumint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/package/timid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.589285 aplustools-1.4.8.3/aplustools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.593285 aplustools-1.4.8.3/aplustools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/utils/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/utils/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/utils/genpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/utils/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.593285 aplustools-1.4.8.3/aplustools/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/web/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/web/new_webtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/web/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/web/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/aplustools/web/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:16:09.593285 aplustools-1.4.8.3/aplustools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-04-12 11:16:09.000000 aplustools-1.4.8.3/aplustools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-12 11:16:09.000000 aplustools-1.4.8.3/aplustools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:16:09.000000 aplustools-1.4.8.3/aplustools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 11:16:09.000000 aplustools-1.4.8.3/aplustools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 11:16:09.000000 aplustools-1.4.8.3/aplustools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 11:16:09.000000 aplustools-1.4.8.3/aplustools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-12 11:16:05.000000 aplustools-1.4.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:16:09.593285 aplustools-1.4.8.3/setup.cfg
```

### Comparing `aplustools-1.4.8.2/LICENSE` & `aplustools-1.4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/PKG-INFO` & `aplustools-1.4.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.8.2
+Version: 1.4.8.3
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -53,15 +53,15 @@
 - Comprehensive documentation
 
 ## Installation
 
 You can install aplustools via pip:
 
 ```sh
-pip install aplustools
+pip install aplustools --upgrade
 ```
 
 Or clone the repository and install manually:
 
 ```sh
 git clone https://github.com/Adalfarus/aplustools.git
 cd aplustools
```

### Comparing `aplustools-1.4.8.2/README.md` & `aplustools-1.4.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 - Comprehensive documentation
 
 ## Installation
 
 You can install aplustools via pip:
 
 ```sh
-pip install aplustools
+pip install aplustools --upgrade
 ```
 
 Or clone the repository and install manually:
 
 ```sh
 git clone https://github.com/Adalfarus/aplustools.git
 cd aplustools
```

### Comparing `aplustools-1.4.8.2/aplustools/__init__.py` & `aplustools-1.4.8.3/aplustools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # aplustools __init__
-__version__ = "1.4.8.2"
+__version__ = "1.4.8.3"
 
 from aplustools.package import LazyModuleLoader as _LazyModuleLoader
 
 # Lazy loading modules
 io = _LazyModuleLoader('aplustools.io')
 data = _LazyModuleLoader('aplustools.data')
 utils = _LazyModuleLoader('aplustools.utils')
```

### Comparing `aplustools-1.4.8.2/aplustools/_direct_functions.py` & `aplustools-1.4.8.3/aplustools/_direct_functions.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/cli.py` & `aplustools-1.4.8.3/aplustools/cli.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/__init__.py` & `aplustools-1.4.8.3/aplustools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/advanced_imagetools.py` & `aplustools-1.4.8.3/aplustools/data/advanced_imagetools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/compressor.py` & `aplustools-1.4.8.3/aplustools/data/compressor.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/database.py` & `aplustools-1.4.8.3/aplustools/data/database.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/database_new.py` & `aplustools-1.4.8.3/aplustools/data/database_new.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/faker.py` & `aplustools-1.4.8.3/aplustools/data/faker.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/github-updater-cmd.py` & `aplustools-1.4.8.3/aplustools/data/github-updater-cmd.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/github-updater-gui.py` & `aplustools-1.4.8.3/aplustools/data/github-updater-gui.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/github-updater-none.py` & `aplustools-1.4.8.3/aplustools/data/github-updater-none.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/imagetools.py` & `aplustools-1.4.8.3/aplustools/data/imagetools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/data/updaters.py` & `aplustools-1.4.8.3/aplustools/data/updaters.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/io/environment.py` & `aplustools-1.4.8.3/aplustools/io/environment.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/io/loggers.py` & `aplustools-1.4.8.3/aplustools/io/loggers.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/io/system_Test.py` & `aplustools-1.4.8.3/aplustools/io/system_Test.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/package/__init__.py` & `aplustools-1.4.8.3/aplustools/package/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/package/_direct_functions.py` & `aplustools-1.4.8.3/aplustools/package/_direct_functions.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/package/argu_mint_old.py` & `aplustools-1.4.8.3/aplustools/package/argu_mint_old.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/package/argumint.py` & `aplustools-1.4.8.3/aplustools/package/argumint.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/package/timid.py` & `aplustools-1.4.8.3/aplustools/package/timid.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/tests/test_data.py` & `aplustools-1.4.8.3/aplustools/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/utils/__init__.py` & `aplustools-1.4.8.3/aplustools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/utils/_direct_functions.py` & `aplustools-1.4.8.3/aplustools/utils/_direct_functions.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/utils/dummy.py` & `aplustools-1.4.8.3/aplustools/utils/dummy.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/utils/genpass.py` & `aplustools-1.4.8.3/aplustools/utils/genpass.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/utils/hasher.py` & `aplustools-1.4.8.3/aplustools/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/web/__init__.py` & `aplustools-1.4.8.3/aplustools/web/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/web/new_webtools.py` & `aplustools-1.4.8.3/aplustools/web/new_webtools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/web/request.py` & `aplustools-1.4.8.3/aplustools/web/request.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/web/search.py` & `aplustools-1.4.8.3/aplustools/web/search.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools/web/utils.py` & `aplustools-1.4.8.3/aplustools/web/utils.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.2/aplustools.egg-info/PKG-INFO` & `aplustools-1.4.8.3/aplustools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.8.2
+Version: 1.4.8.3
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -53,15 +53,15 @@
 - Comprehensive documentation
 
 ## Installation
 
 You can install aplustools via pip:
 
 ```sh
-pip install aplustools
+pip install aplustools --upgrade
 ```
 
 Or clone the repository and install manually:
 
 ```sh
 git clone https://github.com/Adalfarus/aplustools.git
 cd aplustools
```

### Comparing `aplustools-1.4.8.2/aplustools.egg-info/SOURCES.txt` & `aplustools-1.4.8.3/aplustools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 aplustools/data/github-updater-none.py
 aplustools/data/imagetools.py
 aplustools/data/updaters.py
 aplustools/io/__init__.py
 aplustools/io/environment.py
 aplustools/io/loggers.py
 aplustools/io/system_Test.py
+aplustools/io/gui/__init__.py
+aplustools/io/gui/_direct_functions.py
+aplustools/io/gui/calendar.py
+aplustools/io/gui/chat.py
 aplustools/package/__init__.py
 aplustools/package/_direct_functions.py
 aplustools/package/argu_mint_old.py
 aplustools/package/argumint.py
 aplustools/package/timid.py
 aplustools/tests/__init__.py
 aplustools/tests/test_data.py
```

### Comparing `aplustools-1.4.8.2/pyproject.toml` & `aplustools-1.4.8.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-packages = ["aplustools", "aplustools.data", "aplustools.io", "aplustools.utils", "aplustools.web", "aplustools.package", "aplustools.tests"]
+packages = ["aplustools", "aplustools.data", "aplustools.io", "aplustools.utils", "aplustools.web", "aplustools.package", "aplustools.tests", "aplustools.io.gui"]
 
 [project]
 name = "aplustools"
-version = "1.4.8.2"
+version = "1.4.8.3"
 dependencies = [
   "requests>=2.31.0",
   "BeautifulSoup4>=4.12.2",
 #   "win32api; os_name == 'nt'",
 ]
 requires-python = ">= 3.9"
 authors = [
```

