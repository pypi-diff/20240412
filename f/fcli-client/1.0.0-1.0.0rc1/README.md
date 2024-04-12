# Comparing `tmp/fcli_client-1.tar.gz` & `tmp/fcli_client-1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcli_client-1.tar", last modified: Fri Apr 12 18:28:56 2024, max compression
+gzip compressed data, was "fcli_client-1rc1.tar", last modified: Fri Apr 12 18:48:07 2024, max compression
```

## Comparing `fcli_client-1.tar` & `fcli_client-1rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-12 18:28:56.160657 fcli_client-1/
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     1068 2023-11-25 20:33:36.000000 fcli_client-1/LICENSE
--rw-r--r--   0 philcowans  (1000) philcowans  (1000)      183 2024-04-12 18:28:56.160657 fcli_client-1/PKG-INFO
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     3147 2024-03-31 17:16:45.000000 fcli_client-1/README.md
-drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-12 18:28:56.156657 fcli_client-1/fcli_client.egg-info/
--rw-r--r--   0 philcowans  (1000) philcowans  (1000)      183 2024-04-12 18:28:56.000000 fcli_client-1/fcli_client.egg-info/PKG-INFO
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      206 2024-04-12 18:28:56.000000 fcli_client-1/fcli_client.egg-info/SOURCES.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-12 18:28:56.000000 fcli_client-1/fcli_client.egg-info/dependency_links.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       31 2024-04-12 18:28:56.000000 fcli_client-1/fcli_client.egg-info/requires.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-12 18:28:56.000000 fcli_client-1/fcli_client.egg-info/top_level.txt
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      216 2024-04-12 18:28:18.000000 fcli_client-1/pyproject.toml
--rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       38 2024-04-12 18:28:56.160657 fcli_client-1/setup.cfg
+drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-12 18:48:07.447929 fcli_client-1rc1/
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     1068 2023-11-25 20:33:36.000000 fcli_client-1rc1/LICENSE
+-rw-r--r--   0 philcowans  (1000) philcowans  (1000)     3777 2024-04-12 18:48:07.443930 fcli_client-1rc1/PKG-INFO
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)     3147 2024-03-31 17:16:45.000000 fcli_client-1rc1/README.md
+drwxrwxr-x   0 philcowans  (1000) philcowans  (1000)        0 2024-04-12 18:48:07.443930 fcli_client-1rc1/fcli_client.egg-info/
+-rw-r--r--   0 philcowans  (1000) philcowans  (1000)     3777 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/PKG-INFO
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      206 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       31 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/requires.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)        1 2024-04-12 18:48:07.000000 fcli_client-1rc1/fcli_client.egg-info/top_level.txt
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)      673 2024-04-12 18:46:28.000000 fcli_client-1rc1/pyproject.toml
+-rw-rw-r--   0 philcowans  (1000) philcowans  (1000)       38 2024-04-12 18:48:07.447929 fcli_client-1rc1/setup.cfg
```

### Comparing `fcli_client-1/LICENSE` & `fcli_client-1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fcli_client-1/README.md` & `fcli_client-1rc1/README.md`

 * *Files identical despite different names*

