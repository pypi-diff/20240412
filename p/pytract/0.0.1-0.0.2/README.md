# Comparing `tmp/pytract-0.0.1.tar.gz` & `tmp/pytract-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytract-0.0.1.tar", last modified: Tue Apr  9 14:00:58 2024, max compression
+gzip compressed data, was "pytract-0.0.2.tar", last modified: Fri Apr 12 08:18:45 2024, max compression
```

## Comparing `pytract-0.0.1.tar` & `pytract-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,23 @@
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-09 14:00:58.210000 pytract-0.0.1/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      711 2024-04-09 14:00:58.210000 pytract-0.0.1/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      381 2024-04-09 02:57:12.000000 pytract-0.0.1/README.md
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-09 14:00:58.200000 pytract-0.0.1/pytract/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       39 2024-04-09 13:48:07.000000 pytract-0.0.1/pytract/__init__.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-09 14:00:58.210000 pytract-0.0.1/pytract.egg-info/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      711 2024-04-09 14:00:57.000000 pytract-0.0.1/pytract.egg-info/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      162 2024-04-09 14:00:57.000000 pytract-0.0.1/pytract.egg-info/SOURCES.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-09 14:00:57.000000 pytract-0.0.1/pytract.egg-info/dependency_links.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        8 2024-04-09 14:00:57.000000 pytract-0.0.1/pytract.egg-info/top_level.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-09 14:00:58.210000 pytract-0.0.1/setup.cfg
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      368 2024-04-09 13:47:04.000000 pytract-0.0.1/setup.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.540000 pytract-0.0.2/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     4354 2024-04-12 08:18:45.540000 pytract-0.0.2/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3166 2024-04-12 08:09:44.000000 pytract-0.0.2/README.md
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.530000 pytract-0.0.2/pytract/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      115 2024-04-11 17:26:05.000000 pytract-0.0.2/pytract/__init__.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      801 2024-04-11 19:26:57.000000 pytract-0.0.2/pytract/__main__.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)    11708 2024-04-12 07:24:01.000000 pytract-0.0.2/pytract/abi2api.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      224 2024-04-10 01:41:33.000000 pytract-0.0.2/pytract/classes.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       60 2024-04-11 15:00:14.000000 pytract-0.0.2/pytract/compile.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       83 2024-04-11 05:38:49.000000 pytract-0.0.2/pytract/constants.py
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       61 2024-04-11 13:46:32.000000 pytract-0.0.2/pytract/datatypes.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.540000 pytract-0.0.2/pytract/templates/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3335 2024-04-12 07:27:18.000000 pytract-0.0.2/pytract/templates/api.py.j2
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      234 2024-04-11 14:59:51.000000 pytract-0.0.2/pytract/utils.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-12 08:18:45.540000 pytract-0.0.2/pytract.egg-info/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     4354 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      390 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/SOURCES.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/dependency_links.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       51 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/entry_points.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       37 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/requires.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)        8 2024-04-12 08:18:45.000000 pytract-0.0.2/pytract.egg-info/top_level.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-12 08:18:45.540000 pytract-0.0.2/setup.cfg
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      746 2024-04-11 19:29:10.000000 pytract-0.0.2/setup.py
```

