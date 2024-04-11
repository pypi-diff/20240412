# Comparing `tmp/l2m2-0.0.3.tar.gz` & `tmp/l2m2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2m2-0.0.3.tar", last modified: Thu Apr 11 22:35:08 2024, max compression
+gzip compressed data, was "l2m2-0.0.4.tar", last modified: Thu Apr 11 22:35:37 2024, max compression
```

## Comparing `l2m2-0.0.3.tar` & `l2m2-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:35:08.490375 l2m2-0.0.3/
--rw-r--r--   0 pierce     (503) staff       (20)      443 2024-04-11 22:35:08.490117 l2m2-0.0.3/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      235 2024-04-11 22:34:18.000000 l2m2-0.0.3/README.md
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:35:08.488991 l2m2-0.0.3/l2m2/
--rw-r--r--   0 pierce     (503) staff       (20)       35 2024-04-11 20:10:27.000000 l2m2-0.0.3/l2m2/__init__.py
--rw-r--r--   0 pierce     (503) staff       (20)     4365 2024-04-11 20:09:11.000000 l2m2-0.0.3/l2m2/llm_manager.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:35:08.489880 l2m2-0.0.3/l2m2.egg-info/
--rw-r--r--   0 pierce     (503) staff       (20)      443 2024-04-11 22:35:08.000000 l2m2-0.0.3/l2m2.egg-info/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      194 2024-04-11 22:35:08.000000 l2m2-0.0.3/l2m2.egg-info/SOURCES.txt
--rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-11 22:35:08.000000 l2m2-0.0.3/l2m2.egg-info/dependency_links.txt
--rw-r--r--   0 pierce     (503) staff       (20)       59 2024-04-11 22:35:08.000000 l2m2-0.0.3/l2m2.egg-info/requires.txt
--rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-11 22:35:08.000000 l2m2-0.0.3/l2m2.egg-info/top_level.txt
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-11 22:35:08.490436 l2m2-0.0.3/setup.cfg
--rw-r--r--   0 pierce     (503) staff       (20)      392 2024-04-11 22:35:05.000000 l2m2-0.0.3/setup.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:35:37.925270 l2m2-0.0.4/
+-rw-r--r--   0 pierce     (503) staff       (20)      411 2024-04-11 22:35:37.925042 l2m2-0.0.4/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      203 2024-04-11 22:35:34.000000 l2m2-0.0.4/README.md
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:35:37.923960 l2m2-0.0.4/l2m2/
+-rw-r--r--   0 pierce     (503) staff       (20)       35 2024-04-11 20:10:27.000000 l2m2-0.0.4/l2m2/__init__.py
+-rw-r--r--   0 pierce     (503) staff       (20)     4365 2024-04-11 20:09:11.000000 l2m2-0.0.4/l2m2/llm_manager.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:35:37.924834 l2m2-0.0.4/l2m2.egg-info/
+-rw-r--r--   0 pierce     (503) staff       (20)      411 2024-04-11 22:35:37.000000 l2m2-0.0.4/l2m2.egg-info/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      194 2024-04-11 22:35:37.000000 l2m2-0.0.4/l2m2.egg-info/SOURCES.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-11 22:35:37.000000 l2m2-0.0.4/l2m2.egg-info/dependency_links.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       59 2024-04-11 22:35:37.000000 l2m2-0.0.4/l2m2.egg-info/requires.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-11 22:35:37.000000 l2m2-0.0.4/l2m2.egg-info/top_level.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-11 22:35:37.925328 l2m2-0.0.4/setup.cfg
+-rw-r--r--   0 pierce     (503) staff       (20)      392 2024-04-11 22:35:27.000000 l2m2-0.0.4/setup.py
```

### Comparing `l2m2-0.0.3/l2m2/llm_manager.py` & `l2m2-0.0.4/l2m2/llm_manager.py`

 * *Files identical despite different names*

