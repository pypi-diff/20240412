# Comparing `tmp/pytzen-1.0.4.tar.gz` & `tmp/pytzen-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytzen-1.0.4.tar", last modified: Fri Mar  1 22:13:46 2024, max compression
+gzip compressed data, was "pytzen-1.0.5.tar", last modified: Fri Apr 12 11:26:04 2024, max compression
```

## Comparing `pytzen-1.0.4.tar` & `pytzen-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:13:46.393721 pytzen-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-01 22:13:31.000000 pytzen-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-03-01 22:13:46.393721 pytzen-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-03-01 22:13:31.000000 pytzen-1.0.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-03-01 22:13:31.000000 pytzen-1.0.4/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      613 2024-03-01 22:13:46.393721 pytzen-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:13:46.389721 pytzen-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:13:46.389721 pytzen-1.0.4/src/pytzen/
--rw-r--r--   0 runner    (1001) docker     (127)     7084 2024-03-01 22:13:31.000000 pytzen-1.0.4/src/pytzen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 22:13:46.393721 pytzen-1.0.4/src/pytzen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-03-01 22:13:46.000000 pytzen-1.0.4/src/pytzen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-01 22:13:46.000000 pytzen-1.0.4/src/pytzen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 22:13:46.000000 pytzen-1.0.4/src/pytzen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-01 22:13:46.000000 pytzen-1.0.4/src/pytzen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:26:04.314706 pytzen-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-12 11:25:53.000000 pytzen-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-04-12 11:26:04.314706 pytzen-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25995 2024-04-12 11:25:53.000000 pytzen-1.0.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-04-12 11:25:53.000000 pytzen-1.0.5/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      613 2024-04-12 11:26:04.314706 pytzen-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:26:04.310706 pytzen-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:26:04.314706 pytzen-1.0.5/src/pytzen/
+-rw-r--r--   0 runner    (1001) docker     (127)    22382 2024-04-12 11:25:53.000000 pytzen-1.0.5/src/pytzen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:26:04.314706 pytzen-1.0.5/src/pytzen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26543 2024-04-12 11:26:04.000000 pytzen-1.0.5/src/pytzen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 11:26:04.000000 pytzen-1.0.5/src/pytzen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:26:04.000000 pytzen-1.0.5/src/pytzen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 11:26:04.000000 pytzen-1.0.5/src/pytzen.egg-info/top_level.txt
```

### Comparing `pytzen-1.0.4/LICENSE` & `pytzen-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytzen-1.0.4/setup.cfg` & `pytzen-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytzen
-version = 1.0.4
+version = 1.0.5
 author = PYTZEN
 description = PYTZEN Metaprogramming Study Package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://pytzen.com
 project_urls = 
 	Source Code = https://github.com/pytzen/pytzen
```

