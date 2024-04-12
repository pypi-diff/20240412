# Comparing `tmp/Mopidy-Spotify-5.0.0a1.tar.gz` & `tmp/Mopidy-Spotify-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-Spotify-5.0.0a1.tar", last modified: Fri Mar  1 16:22:22 2024, max compression
+gzip compressed data, was "Mopidy-Spotify-5.0.0a2.tar", last modified: Fri Apr 12 13:28:31 2024, max compression
```

## Comparing `Mopidy-Spotify-5.0.0a1.tar` & `Mopidy-Spotify-5.0.0a2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.802193 Mopidy-Spotify-5.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.794193 Mopidy-Spotify-5.0.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.794193 Mopidy-Spotify-5.0.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/.github/ISSUE_TEMPLATE/issue-template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.794193 Mopidy-Spotify-5.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.802193 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-01 16:22:22.000000 Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-03-01 16:22:22.802193 Mopidy-Spotify-5.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.798193 Mopidy-Spotify-5.0.0a1/mopidy_spotify/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/browse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/distinct.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/ext.conf
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/mopidy_spotify/web.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-01 16:22:22.802193 Mopidy-Spotify-5.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:22.798193 Mopidy-Spotify-5.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_browse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_distinct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_playback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_playlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    24751 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42856 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tests/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-01 16:22:19.000000 Mopidy-Spotify-5.0.0a1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.676510 Mopidy-Spotify-5.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.668510 Mopidy-Spotify-5.0.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.668510 Mopidy-Spotify-5.0.0a2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/.github/ISSUE_TEMPLATE/issue-template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.668510 Mopidy-Spotify-5.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.676510 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 13:28:31.000000 Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-12 13:28:31.676510 Mopidy-Spotify-5.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.672510 Mopidy-Spotify-5.0.0a2/mopidy_spotify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/distinct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20943 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/mopidy_spotify/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-12 13:28:31.676510 Mopidy-Spotify-5.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:28:31.676510 Mopidy-Spotify-5.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_browse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_distinct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_playback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_playlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24552 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44392 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tests/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 13:28:25.000000 Mopidy-Spotify-5.0.0a2/tox.ini
```

### Comparing `Mopidy-Spotify-5.0.0a1/.github/workflows/ci.yml` & `Mopidy-Spotify-5.0.0a2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/LICENSE` & `Mopidy-Spotify-5.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/PKG-INFO` & `Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-Spotify
-Version: 5.0.0a1
+Version: 5.0.0a2
 Summary: Mopidy extension for playing music from Spotify
 Home-page: https://github.com/mopidy/mopidy-spotify
 Author: Stein Magnus Jodal
 Author-email: stein.magnus@jodal.no
 License: Apache License, Version 2.0
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
@@ -134,17 +134,15 @@
 
 
 Installation
 ============
 
 Install by running::
 
-    sudo python3 -m pip install --break-system-packages https://github.com/mopidy/mopidy-spotify/archive/refs/tags/v5.0.0a1.zip
-
-This is currently the only supported installation method.
+    sudo python3 -m pip install --break-system-packages Mopidy-Spotify==5.0.0a2
 
 
 Configuration
 =============
 
 Before starting Mopidy, you must add your Spotify Premium username and password
 to your Mopidy configuration file and also visit
```

### Comparing `Mopidy-Spotify-5.0.0a1/Mopidy_Spotify.egg-info/SOURCES.txt` & `Mopidy-Spotify-5.0.0a2/Mopidy_Spotify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/PKG-INFO` & `Mopidy-Spotify-5.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-Spotify
-Version: 5.0.0a1
+Version: 5.0.0a2
 Summary: Mopidy extension for playing music from Spotify
 Home-page: https://github.com/mopidy/mopidy-spotify
 Author: Stein Magnus Jodal
 Author-email: stein.magnus@jodal.no
 License: Apache License, Version 2.0
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
@@ -134,17 +134,15 @@
 
 
 Installation
 ============
 
 Install by running::
 
-    sudo python3 -m pip install --break-system-packages https://github.com/mopidy/mopidy-spotify/archive/refs/tags/v5.0.0a1.zip
-
-This is currently the only supported installation method.
+    sudo python3 -m pip install --break-system-packages Mopidy-Spotify==5.0.0a2
 
 
 Configuration
 =============
 
 Before starting Mopidy, you must add your Spotify Premium username and password
 to your Mopidy configuration file and also visit
```

### Comparing `Mopidy-Spotify-5.0.0a1/README.rst` & `Mopidy-Spotify-5.0.0a2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -86,17 +86,15 @@
 
 
 Installation
 ============
 
 Install by running::
 
-    sudo python3 -m pip install --break-system-packages https://github.com/mopidy/mopidy-spotify/archive/refs/tags/v5.0.0a1.zip
-
-This is currently the only supported installation method.
+    sudo python3 -m pip install --break-system-packages Mopidy-Spotify==5.0.0a2
 
 
 Configuration
 =============
 
 Before starting Mopidy, you must add your Spotify Premium username and password
 to your Mopidy configuration file and also visit
```

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/__init__.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/backend.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/backend.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/browse.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/browse.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/distinct.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/distinct.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/images.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/images.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/library.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/library.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/lookup.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/lookup.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/playlists.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/playlists.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import logging
+import threading
 
 from mopidy import backend
+from mopidy.core import listener
 
 from mopidy_spotify import translator, utils
 
 
 logger = logging.getLogger(__name__)
 
 
 class SpotifyPlaylistsProvider(backend.PlaylistsProvider):
     def __init__(self, backend):
         self._backend = backend
         self._timeout = self._backend._config["spotify"]["timeout"]
-        self._loaded = False
+        self._refresh_mutex = threading.Lock()
 
     def as_list(self):
         with utils.time_logger("playlists.as_list()", logging.DEBUG):
-            if not self._loaded:
-                return []
-
             return list(self._get_flattened_playlist_refs())
 
-    def _get_flattened_playlist_refs(self):
+    def _get_flattened_playlist_refs(self, *, refresh=False):
         if not self._backend._web_client.logged_in:
             return []
 
-        user_playlists = self._backend._web_client.get_user_playlists()
+        user_playlists = self._backend._web_client.get_user_playlists(
+            refresh=refresh
+        )
         return translator.to_playlist_refs(
             user_playlists, self._backend._web_client.user_id
         )
 
     def get_items(self, uri):
         with utils.time_logger(f"playlist.get_items({uri!r})", logging.DEBUG):
             return self._get_playlist(uri, as_items=True)
@@ -45,26 +46,56 @@
             self._backend._bitrate,
             as_items,
         )
 
     def refresh(self):
         if not self._backend._web_client.logged_in:
             return
-
-        logger.info("Refreshing Spotify playlists")
-
-        with utils.time_logger("playlists.refresh()", logging.DEBUG):
-            self._backend._web_client.clear_cache()
-            count = 0
-            for playlist_ref in self._get_flattened_playlist_refs():
-                self._get_playlist(playlist_ref.uri)
-                count = count + 1
-            logger.info(f"Refreshed {count} Spotify playlists")
-
-        self._loaded = True
+        if not self._refresh_mutex.acquire(blocking=False):
+            logger.info("Refreshing Spotify playlists already in progress")
+            return
+        try:
+            uris = [
+                ref.uri
+                for ref in self._get_flattened_playlist_refs(refresh=True)
+            ]
+            logger.info(
+                f"Refreshing {len(uris)} Spotify playlists in background"
+            )
+            threading.Thread(
+                target=self._refresh_tracks,
+                args=(uris,),
+                daemon=True,
+            ).start()
+        except Exception:
+            logger.exception(
+                "Error occurred while refreshing Spotify playlists"
+            )
+            self._refresh_mutex.release()
+
+    def _refresh_tracks(self, playlist_uris):
+        if not self._refresh_mutex.locked():
+            logger.error("Lock must be held before calling this method")
+            return []
+        try:
+            with utils.time_logger(
+                "playlists._refresh_tracks()", logging.DEBUG
+            ):
+                refreshed = [uri for uri in playlist_uris if self.lookup(uri)]
+                logger.info(f"Refreshed {len(refreshed)} Spotify playlists")
+
+            listener.CoreListener.send("playlists_loaded")
+        except Exception:
+            logger.exception(
+                "Error occurred while refreshing Spotify playlists tracks"
+            )
+        else:
+            return refreshed  # For test
+        finally:
+            self._refresh_mutex.release()
 
     def create(self, name):
         pass  # TODO
 
     def delete(self, uri):
         pass  # TODO
```

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/search.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/search.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/translator.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/translator.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/utils.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/utils.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/mopidy_spotify/web.py` & `Mopidy-Spotify-5.0.0a2/mopidy_spotify/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import copy
 import logging
 import os
 import re
+import threading
 import time
 import urllib.parse
 from dataclasses import dataclass
 from datetime import datetime
+from email.utils import parsedate_to_datetime
 from enum import Enum, unique
 from typing import Optional
-from email.utils import parsedate_to_datetime
+
 
 import requests
 
 from mopidy_spotify import utils
 
 logger = logging.getLogger(__name__)
 
@@ -59,70 +61,82 @@
         self._timeout = timeout
         self._number_of_retries = retries
         self._retry_statuses = retry_statuses
         self._backoff_factor = 0.5
 
         self._headers = {"Content-Type": "application/json"}
         self._session = utils.get_requests_session(proxy_config or {})
+        # TODO: Move _cache_mutex to the object it actually protects.
+        self._cache_mutex = threading.Lock()  # Protects get() cache param.
+        self._refresh_mutex = (
+            threading.Lock()
+        )  # Protects _headers and _expires.
 
     def get(self, path, cache=None, *args, **kwargs):
         if self._authorization_failed:
             logger.debug("Blocking request as previous authorization failed.")
             return WebResponse(None, None)
 
         params = kwargs.pop("params", None)
         path = self._normalise_query_string(path, params)
 
         _trace(f"Get '{path}'")
 
-        ignore_expiry = kwargs.pop("ignore_expiry", False)
+        expiry_strategy = kwargs.pop("expiry_strategy", None)
         if cache is not None and path in cache:
             cached_result = cache.get(path)
-            if cached_result.still_valid(ignore_expiry):
+            if cached_result.still_valid(expiry_strategy=expiry_strategy):
                 return cached_result
             kwargs.setdefault("headers", {}).update(cached_result.etag_headers)
 
         # TODO: Factor this out once we add more methods.
         # TODO: Don't silently error out.
-        try:
-            if self._should_refresh_token():
-                self._refresh_token()
-        except OAuthTokenRefreshError as e:
-            logger.error(e)
-            return WebResponse(None, None)
+        with self._refresh_mutex:
+            try:
+                if self._should_refresh_token():
+                    self._refresh_token()
+            except OAuthTokenRefreshError as e:
+                logger.error(e)  # noqa: TRY400
+                return WebResponse(None, None)
 
         # Make sure our headers always override user supplied ones.
         kwargs.setdefault("headers", {}).update(self._headers)
         result = self._request_with_retries("GET", path, *args, **kwargs)
 
         if result is None or "error" in result:
             logger.error(
                 "Spotify Web API request failed: "
                 f"{result.get('error','Unknown') if result else 'Unknown'}"
             )
             return WebResponse(None, None)
 
-        if self._should_cache_response(cache, result):
-            previous_result = cache.get(path)
-            if previous_result and previous_result.updated(result):
-                result = previous_result
-            cache[path] = result
+        with self._cache_mutex:
+            if self._should_cache_response(cache, result):
+                previous_result = cache.get(path)
+                if previous_result and previous_result.updated(result):
+                    result = previous_result
+                cache[path] = result
 
         return result
 
     def _should_cache_response(self, cache, response):
         return cache is not None and response.status_ok
 
     def _should_refresh_token(self):
         # TODO: Add jitter to margin?
+        if not self._refresh_mutex.locked():
+            raise OAuthTokenRefreshError("Lock must be held before calling.")
         return not self._auth or time.time() > self._expires - self._margin
 
     def _refresh_token(self):
         logger.debug(f"Fetching OAuth token from {self._refresh_url}")
 
+        if not self._refresh_mutex.locked():
+            raise OAuthTokenRefreshError("Lock must be held before calling.")
+
         data = {"grant_type": "client_credentials"}
         result = self._request_with_retries(
             "POST", self._refresh_url, auth=self._auth, data=data
         )
 
         if result is None:
             raise OAuthTokenRefreshError("Unknown error.")
@@ -262,14 +276,20 @@
                 date_tuple = parsedate_to_datetime(value)
                 seconds = (date_tuple - now).total_seconds()
             except Exception:
                 seconds = 0
         return max(0, seconds)
 
 
+@unique
+class ExpiryStrategy(Enum):
+    FORCE_FRESH = "force-fresh"
+    FORCE_EXPIRED = "force-expired"
+
+
 class WebResponse(dict):
     def __init__(self, url, data, expires=0.0, etag=None, status_code=400):
         self._from_cache = False
         self.url = url
         self._expires = expires
         self._etag = etag
         self._status_code = status_code
@@ -320,27 +340,30 @@
             # currently ignoring this.
             # Format is string of ASCII characters placed between double quotes
             # but can seemingly also include hyphen characters.
             etag = re.match(r'^(W/)?("[!#-~]+")$', value)
             if etag and len(etag.groups()) == 2:
                 return etag.groups()[1]
 
-    def still_valid(self, ignore_expiry=False):
-        if ignore_expiry:
-            result = True
-            status = "forced"
-        elif self._expires >= time.time():
-            result = True
-            status = "fresh"
+        return None
+
+    def still_valid(self, *, expiry_strategy=None):
+        if expiry_strategy is None:
+            if self._expires >= time.time():
+                valid = True
+                status = "fresh"
+            else:
+                valid = False
+                status = "expired"
         else:
-            result = False
-            status = "expired"
-        self._from_cache = result
+            valid = expiry_strategy is ExpiryStrategy.FORCE_FRESH
+            status = expiry_strategy.value
+        self._from_cache = valid
         _trace("Cached data %s for %s", status, self)
-        return result
+        return valid
 
     @property
     def status_unchanged(self):
         return self._from_cache or 304 == self._status_code
 
     @property
     def status_ok(self):
@@ -428,29 +451,34 @@
             logger.info(f"Logged into Spotify Web API as {self.user_id}")
             return True
 
     @property
     def logged_in(self):
         return self.user_id is not None
 
-    def get_user_playlists(self):
+    def get_user_playlists(self, *, refresh=False):
+        expiry_strategy = ExpiryStrategy.FORCE_EXPIRED if refresh else None
         pages = self.get_all(
-            f"users/{self.user_id}/playlists", params={"limit": 50}
+            f"users/{self.user_id}/playlists",
+            params={"limit": 50},
+            expiry_strategy=expiry_strategy,
         )
         for page in pages:
             yield from page.get("items", [])
 
     def _with_all_tracks(self, obj, params=None):
         if params is None:
             params = {}
         tracks_path = obj.get("tracks", {}).get("next")
         track_pages = self.get_all(
             tracks_path,
             params=params,
-            ignore_expiry=obj.status_unchanged,
+            expiry_strategy=(
+                ExpiryStrategy.FORCE_FRESH if obj.status_unchanged else None
+            ),
         )
 
         more_tracks = []
         for page in track_pages:
             if "items" not in page:
                 return {}  # Return nothing on error, or what we have so far?
             more_tracks += page["items"]
@@ -527,17 +555,14 @@
             logger.error("Expecting Spotify track URI")
             return {}
 
         return self.get_one(
             f"tracks/{web_link.id}", params={"market": "from_token"}
         )
 
-    def clear_cache(self, extra_expiry=None):
-        self._cache.clear()
-
 
 @unique
 class LinkType(Enum):
     TRACK = "track"
     ALBUM = "album"
     ARTIST = "artist"
     PLAYLIST = "playlist"
```

### Comparing `Mopidy-Spotify-5.0.0a1/setup.cfg` & `Mopidy-Spotify-5.0.0a2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Mopidy-Spotify
-version = 5.0.0a1
+version = 5.0.0a2
 url = https://github.com/mopidy/mopidy-spotify
 author = Stein Magnus Jodal
 author_email = stein.magnus@jodal.no
 license = Apache License, Version 2.0
 license_file = LICENSE
 description = Mopidy extension for playing music from Spotify
 long_description = file: README.rst
```

### Comparing `Mopidy-Spotify-5.0.0a1/tests/conftest.py` & `Mopidy-Spotify-5.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_backend.py` & `Mopidy-Spotify-5.0.0a2/tests/test_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from unittest import skip
 
 from mopidy import backend as backend_api
 
 from mopidy_spotify import backend, library, playlists
 from mopidy_spotify.backend import SpotifyPlaybackProvider
 
+from tests import ThreadJoiner
+
 
 def get_backend(config):
     obj = backend.SpotifyBackend(config=config, audio=None)
     obj._web_client = mock.Mock()
     return obj
 
 
@@ -56,15 +58,16 @@
         "scheme": "https",
         "hostname": "my-proxy.example.com",
         "port": 8080,
         "username": "alice",
         "password": "s3cret",
     }
     backend = get_backend(config)
-    backend.on_start()
+    with ThreadJoiner():
+        backend.on_start()
 
     assert True
 
     web_mock.SpotifyOAuthClient.assert_called_once_with(
         client_id=mock.ANY,
         client_secret=mock.ANY,
         proxy_config=config["proxy"],
@@ -72,15 +75,16 @@
 
 
 def test_on_start_configures_web_client(web_mock, config):
     config["spotify"]["client_id"] = "1234567"
     config["spotify"]["client_secret"] = "AbCdEfG"
 
     backend = get_backend(config)
-    backend.on_start()
+    with ThreadJoiner():
+        backend.on_start()
 
     web_mock.SpotifyOAuthClient.assert_called_once_with(
         client_id="1234567",
         client_secret="AbCdEfG",
         proxy_config=mock.ANY,
     )
 
@@ -90,20 +94,21 @@
     backend.on_start()
 
     web_mock.SpotifyOAuthClient.return_value.login.assert_called_once()
 
 
 def test_on_start_refreshes_playlists(web_mock, config, caplog):
     backend = get_backend(config)
-    backend.on_start()
+    with ThreadJoiner():
+        backend.on_start()
 
     client_mock = web_mock.SpotifyOAuthClient.return_value
-    client_mock.get_user_playlists.assert_called_once()
+    client_mock.get_user_playlists.assert_called_once_with(refresh=True)
+    assert "Refreshing 0 Spotify playlists in background" in caplog.text
     assert "Refreshed 0 Spotify playlists" in caplog.text
-    assert backend.playlists._loaded
 
 
 def test_on_start_doesnt_refresh_playlists_if_not_allowed(
     web_mock, config, caplog
 ):
     config["spotify"]["allow_playlists"] = False
```

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_browse.py` & `Mopidy-Spotify-5.0.0a2/tests/test_browse.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_distinct.py` & `Mopidy-Spotify-5.0.0a2/tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_extension.py` & `Mopidy-Spotify-5.0.0a2/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_images.py` & `Mopidy-Spotify-5.0.0a2/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_lookup.py` & `Mopidy-Spotify-5.0.0a2/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_playback.py` & `Mopidy-Spotify-5.0.0a2/tests/test_playback.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_playlists.py` & `Mopidy-Spotify-5.0.0a2/tests/test_playlists.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import logging
 from unittest import mock
 
 import pytest
 from mopidy import backend as backend_api
 from mopidy.models import Ref
 
 from mopidy_spotify import playlists
 
+from tests import ThreadJoiner
+
 
 @pytest.fixture
 def web_client_mock(web_client_mock, web_track_mock):
     web_playlist1 = {
         "owner": {"id": "alice"},
         "name": "Foo",
         "tracks": {"items": [{"track": web_track_mock}]},
@@ -39,17 +42,15 @@
     web_client_mock.get_playlist.side_effect = get_playlist
     return web_client_mock
 
 
 @pytest.fixture
 def provider(backend_mock, web_client_mock):
     backend_mock._web_client = web_client_mock
-    provider = playlists.SpotifyPlaylistsProvider(backend_mock)
-    provider._loaded = True
-    return provider
+    return playlists.SpotifyPlaylistsProvider(backend_mock)
 
 
 def test_is_a_playlists_provider(provider):
     assert isinstance(provider, backend_api.PlaylistsProvider)
 
 
 def test_as_list_when_not_logged_in(web_client_mock, provider):
@@ -64,22 +65,14 @@
     web_client_mock.get_user_playlists.return_value = {}
 
     result = provider.as_list()
 
     assert len(result) == 0
 
 
-def test_as_list_when_not_loaded(provider):
-    provider._loaded = False
-
-    result = provider.as_list()
-
-    assert len(result) == 0
-
-
 def test_as_list_when_playlist_wont_translate(provider):
     result = provider.as_list()
 
     assert len(result) == 2
 
     assert result[0] == Ref.playlist(
         uri="spotify:user:alice:playlist:foo", name="Foo"
@@ -116,78 +109,128 @@
     assert provider.get_items("spotify:user:alice:playlist:foo") is None
     assert (
         "Failed to lookup Spotify playlist URI "
         "'spotify:user:alice:playlist:foo'" in caplog.text
     )
 
 
-def test_get_items_when_not_loaded(provider):
-    provider._loaded = False
-
-    result = provider.get_items("spotify:user:alice:playlist:foo")
-
-    assert len(result) == 1
-    assert result[0] == Ref.track(uri="spotify:track:abc", name="ABC 123")
-
-
 def test_get_items_when_playlist_wont_translate(provider):
     assert provider.get_items("spotify:user:alice:playlist:malformed") is None
 
 
 def test_get_items_when_playlist_is_unknown(provider, caplog):
     assert provider.get_items("spotify:user:alice:playlist:unknown") is None
     assert (
         "Failed to lookup Spotify playlist URI "
         "'spotify:user:alice:playlist:unknown'" in caplog.text
     )
 
 
 def test_refresh_loads_all_playlists(provider, web_client_mock):
-    provider.refresh()
+    with ThreadJoiner():
+        provider.refresh()
 
     web_client_mock.get_user_playlists.assert_called_once()
     assert web_client_mock.get_playlist.call_count == 2
     expected_calls = [
         mock.call("spotify:user:alice:playlist:foo"),
         mock.call("spotify:user:bob:playlist:baz"),
     ]
     web_client_mock.get_playlist.assert_has_calls(expected_calls)
 
 
 def test_refresh_when_not_logged_in(provider, web_client_mock):
-    provider._loaded = False
     web_client_mock.logged_in = False
 
-    provider.refresh()
+    with ThreadJoiner():
+        provider.refresh()
 
     web_client_mock.get_user_playlists.assert_not_called()
     web_client_mock.get_playlist.assert_not_called()
-    assert not provider._loaded
 
 
-def test_refresh_sets_loaded(provider, web_client_mock):
-    provider._loaded = False
+def test_refresh_in_progress(provider, web_client_mock, caplog):
+    assert provider._refresh_mutex.acquire(blocking=False)
 
-    provider.refresh()
+    with ThreadJoiner():
+        provider.refresh()
 
-    web_client_mock.get_user_playlists.assert_called_once()
-    web_client_mock.get_playlist.assert_called()
-    assert provider._loaded
+    web_client_mock.get_user_playlists.assert_not_called()
+    web_client_mock.get_playlist.assert_not_called()
+    assert provider._refresh_mutex.locked()
+    assert "Refreshing Spotify playlists already in progress" in caplog.text
 
 
-def test_refresh_counts_playlists(provider, caplog):
-    provider.refresh()
+def test_refresh_counts_valid_playlists(provider, caplog):
+    caplog.set_level(
+        logging.INFO
+    )  # To avoid log corruption from debug logging.
+    with ThreadJoiner():
+        provider.refresh()
 
+    assert "Refreshing 2 Spotify playlists in background" in caplog.text
     assert "Refreshed 2 Spotify playlists" in caplog.text
 
 
-def test_refresh_clears_caches(provider, web_client_mock):
-    provider.refresh()
+@mock.patch("mopidy.core.listener.CoreListener.send")
+def test_refresh_triggers_playlists_loaded_event(send, provider):
+    with ThreadJoiner():
+        provider.refresh()
+
+    send.assert_called_once_with("playlists_loaded")
+
+
+def test_refresh_with_refresh_true_arg(provider, web_client_mock):
+    with ThreadJoiner():
+        provider.refresh()
+
+    web_client_mock.get_user_playlists.assert_called_once_with(refresh=True)
+
+
+def test_refresh_handles_error(provider, web_client_mock, caplog):
+    web_client_mock.get_user_playlists.side_effect = Exception()
+
+    with ThreadJoiner():
+        provider.refresh()
+
+    assert "Error occurred while refreshing Spotify playlists" in caplog.text
+    assert not provider._refresh_mutex.locked()
 
-    web_client_mock.clear_cache.assert_called_once()
+
+def test_refresh_tracks_handles_error(provider, web_client_mock, caplog):
+    web_client_mock.get_playlist.side_effect = Exception()
+
+    with ThreadJoiner():
+        provider.refresh()
+
+    assert (
+        "Error occurred while refreshing Spotify playlists tracks"
+        in caplog.text
+    )
+    assert not provider._refresh_mutex.locked()
+
+
+def test_refresh_tracks_needs_lock(provider, web_client_mock, caplog):
+    assert provider._refresh_tracks("foo") == []
+
+    assert "Lock must be held before calling this method" in caplog.text
+    web_client_mock.get_playlist.assert_not_called()
+
+
+def test_refresh_tracks(provider, web_client_mock, caplog):
+    uris = ["spotify:user:alice:playlist:foo", "spotify:user:bob:playlist:baz"]
+
+    assert provider._refresh_mutex.acquire(blocking=False)
+    assert provider._refresh_tracks(uris) == uris
+
+    expected_calls = [
+        mock.call("spotify:user:alice:playlist:foo"),
+        mock.call("spotify:user:bob:playlist:baz"),
+    ]
+    web_client_mock.get_playlist.assert_has_calls(expected_calls)
 
 
 def test_lookup(provider):
     playlist = provider.lookup("spotify:user:alice:playlist:foo")
 
     assert playlist.uri == "spotify:user:alice:playlist:foo"
     assert playlist.name == "Foo"
@@ -198,23 +241,14 @@
     web_client_mock.logged_in = False
 
     playlist = provider.lookup("spotify:user:alice:playlist:foo")
 
     assert playlist is None
 
 
-def test_lookup_when_not_loaded(provider):
-    provider._loaded = False
-
-    playlist = provider.lookup("spotify:user:alice:playlist:foo")
-
-    assert playlist.uri == "spotify:user:alice:playlist:foo"
-    assert playlist.name == "Foo"
-
-
 def test_lookup_when_playlist_is_empty(provider, caplog):
     assert provider.lookup("nothing") is None
     assert "Failed to lookup Spotify playlist URI 'nothing'" in caplog.text
 
 
 def test_lookup_of_playlist_with_other_owner(provider):
     playlist = provider.lookup("spotify:user:bob:playlist:baz")
```

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_search.py` & `Mopidy-Spotify-5.0.0a2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_translator.py` & `Mopidy-Spotify-5.0.0a2/tests/test_translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,20 +564,14 @@
     ):
         web_album_mock["artists"] = []
 
         album = translator.web_to_album(web_album_mock)
 
         assert list(album.artists) == []
 
-    def test_caches_results(self, web_album_mock):
-        album1 = translator.web_to_album(web_album_mock)
-        album2 = translator.web_to_album(web_album_mock)
-
-        assert album1 is album2
-
     def test_web_to_album_tracks(self, web_album_mock):
         tracks = translator.web_to_album_tracks(web_album_mock)
 
         assert len(tracks) == 10
         track = tracks[0]
         assert track.album.name == "DEF 456"
         assert track.album.artists == track.artists
```

### Comparing `Mopidy-Spotify-5.0.0a1/tests/test_web.py` & `Mopidy-Spotify-5.0.0a2/tests/test_web.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,28 +46,41 @@
     patcher = mock.patch.object(
         web.OAuthClient, "_should_refresh_token", return_value=False
     )
     yield patcher.start()
     patcher.stop()
 
 
+def test_should_refresh_token_requires_lock(oauth_client):
+    with pytest.raises(web.OAuthTokenRefreshError):
+        oauth_client._should_refresh_token()
+
+
+def test_refresh_token_requires_lock(oauth_client):
+    with pytest.raises(web.OAuthTokenRefreshError):
+        oauth_client._refresh_token()
+
+
 def test_initial_refresh_token(oauth_client):
-    assert oauth_client._should_refresh_token()
+    with oauth_client._refresh_mutex:
+        assert oauth_client._should_refresh_token()
 
 
 def test_expired_refresh_token(oauth_client, mock_time):
     oauth_client._expires = 1060
     mock_time.return_value = 1001
-    assert oauth_client._should_refresh_token()
+    with oauth_client._refresh_mutex:
+        assert oauth_client._should_refresh_token()
 
 
 def test_still_valid_refresh_token(oauth_client, mock_time):
     oauth_client._expires = 1060
     mock_time.return_value = 1000
-    assert not oauth_client._should_refresh_token()
+    with oauth_client._refresh_mutex:
+        assert not oauth_client._should_refresh_token()
 
 
 def test_user_agent(oauth_client):
     assert oauth_client._session.headers["user-agent"].startswith(
         f"Mopidy-Spotify/{mopidy_spotify.__version__}"
     )
 
@@ -374,15 +387,15 @@
 
 
 def test_web_response_status_unchanged_from_cache():
     response = web.WebResponse("https://foo.com", {})
 
     assert not response.status_unchanged
 
-    response.still_valid(ignore_expiry=True)
+    response.still_valid(expiry_strategy=web.ExpiryStrategy.FORCE_FRESH)
 
     assert response.status_unchanged
 
     response.updated(response)
 
     assert not response.status_unchanged
 
@@ -528,32 +541,54 @@
     assert "Cached data expired for" in caplog.text
 
     result = oauth_client.get("https://api.spotify.com/v1/tracks/abc", cache)
     assert len(responses.calls) == 1
     assert result["uri"] == "new"
 
 
+def test_cache_response_still_valid_strategy(mock_time):
+    response = web.WebResponse("foo", {}, expires=9999 + 1)
+    mock_time.return_value = 9999
+
+    assert response.still_valid() is True
+    assert response.still_valid(expiry_strategy=None) is True
+    assert (
+        response.still_valid(expiry_strategy=web.ExpiryStrategy.FORCE_FRESH)
+        is True
+    )
+    assert (
+        response.still_valid(expiry_strategy=web.ExpiryStrategy.FORCE_EXPIRED)
+        is False
+    )
+
+
 @responses.activate
-def test_cache_response_ignore_expiry(
+def test_cache_response_force_fresh(
     web_response_mock, skip_refresh_token, oauth_client, mock_time, caplog
 ):
     cache = {"https://api.spotify.com/v1/tracks/abc": web_response_mock}
     responses.add(
         responses.GET,
         "https://api.spotify.com/v1/tracks/abc",
         json={"uri": "new"},
     )
     mock_time.return_value = 9999
 
     assert not web_response_mock.still_valid()
-    assert web_response_mock.still_valid(True)
-    assert "Cached data forced for" in caplog.text
+    assert "Cached data expired for" in caplog.text
+
+    assert web_response_mock.still_valid(
+        expiry_strategy=web.ExpiryStrategy.FORCE_FRESH
+    )
+    assert "Cached data force-fresh for" in caplog.text
 
     result = oauth_client.get(
-        "https://api.spotify.com/v1/tracks/abc", cache, ignore_expiry=True
+        "https://api.spotify.com/v1/tracks/abc",
+        cache,
+        expiry_strategy=web.ExpiryStrategy.FORCE_FRESH,
     )
     assert len(responses.calls) == 0
     assert result["uri"] == "spotify:track:abc"
 
 
 @responses.activate
 def test_dont_cache_bad_status(
@@ -970,14 +1005,35 @@
         responses.add(responses.GET, url("users/alice/playlists"), json={})
 
         result = list(spotify_client.get_user_playlists())
 
         assert len(responses.calls) == 1
         assert len(result) == 0
 
+    @pytest.mark.parametrize(
+        ("refresh", "strategy"),
+        [
+            (True, web.ExpiryStrategy.FORCE_EXPIRED),
+            (False, None),
+        ],
+    )
+    def test_get_user_playlists_get_all(
+        self, spotify_client, refresh, strategy
+    ):
+        spotify_client.get_all = mock.Mock(return_value=[])
+
+        result = list(spotify_client.get_user_playlists(refresh=refresh))
+
+        spotify_client.get_all.assert_called_once_with(
+            "users/alice/playlists",
+            params={"limit": 50},
+            expiry_strategy=strategy,
+        )
+        assert len(result) == 0
+
     @responses.activate
     def test_get_user_playlists_sets_params(self, spotify_client):
         responses.add(responses.GET, url("users/alice/playlists"), json={})
 
         list(spotify_client.get_user_playlists())
 
         assert len(responses.calls) == 1
@@ -1175,23 +1231,16 @@
             ("my-bad-uri", "Spotify"),
         ],
     )
     def test_get_playlist_error_msg(self, spotify_client, caplog, uri, msg):
         assert spotify_client.get_playlist(uri) == {}
         assert f"Could not parse {uri!r} as a {msg} URI" in caplog.text
 
-    def test_clear_cache(self, spotify_client):
-        spotify_client._cache = {"foo": "bar"}
-
-        spotify_client.clear_cache()
-
-        assert {} == spotify_client._cache
-
     @pytest.mark.parametrize(
-        "user_id,expected", [("alice", True), (None, False)]
+        ("user_id", "expected"), [("alice", True), (None, False)]
     )
     def test_logged_in(self, spotify_client, user_id, expected):
         spotify_client.user_id = user_id
 
         assert spotify_client.logged_in is expected
 
     @responses.activate
```

