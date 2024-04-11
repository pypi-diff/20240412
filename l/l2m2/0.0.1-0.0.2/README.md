# Comparing `tmp/l2m2-0.0.1.tar.gz` & `tmp/l2m2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2m2-0.0.1.tar", last modified: Thu Apr 11 22:08:52 2024, max compression
+gzip compressed data, was "l2m2-0.0.2.tar", last modified: Thu Apr 11 22:32:21 2024, max compression
```

## Comparing `l2m2-0.0.1.tar` & `l2m2-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:08:52.047487 l2m2-0.0.1/
--rw-r--r--   0 pierce     (503) staff       (20)      167 2024-04-11 22:08:52.047280 l2m2-0.0.1/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-11 21:52:46.000000 l2m2-0.0.1/README.md
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:08:52.046216 l2m2-0.0.1/l2m2/
--rw-r--r--   0 pierce     (503) staff       (20)       35 2024-04-11 20:10:27.000000 l2m2-0.0.1/l2m2/__init__.py
--rw-r--r--   0 pierce     (503) staff       (20)     4365 2024-04-11 20:09:11.000000 l2m2-0.0.1/l2m2/llm_manager.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:08:52.047040 l2m2-0.0.1/l2m2.egg-info/
--rw-r--r--   0 pierce     (503) staff       (20)      167 2024-04-11 22:08:52.000000 l2m2-0.0.1/l2m2.egg-info/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      194 2024-04-11 22:08:52.000000 l2m2-0.0.1/l2m2.egg-info/SOURCES.txt
--rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-11 22:08:52.000000 l2m2-0.0.1/l2m2.egg-info/dependency_links.txt
--rw-r--r--   0 pierce     (503) staff       (20)       59 2024-04-11 22:08:52.000000 l2m2-0.0.1/l2m2.egg-info/requires.txt
--rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-11 22:08:52.000000 l2m2-0.0.1/l2m2.egg-info/top_level.txt
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-11 22:08:52.047548 l2m2-0.0.1/setup.cfg
--rw-r--r--   0 pierce     (503) staff       (20)      255 2024-04-11 21:59:29.000000 l2m2-0.0.1/setup.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:32:21.983569 l2m2-0.0.2/
+-rw-r--r--   0 pierce     (503) staff       (20)      371 2024-04-11 22:32:21.983357 l2m2-0.0.2/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      163 2024-04-11 22:30:56.000000 l2m2-0.0.2/README.md
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:32:21.982283 l2m2-0.0.2/l2m2/
+-rw-r--r--   0 pierce     (503) staff       (20)       35 2024-04-11 20:10:27.000000 l2m2-0.0.2/l2m2/__init__.py
+-rw-r--r--   0 pierce     (503) staff       (20)     4365 2024-04-11 20:09:11.000000 l2m2-0.0.2/l2m2/llm_manager.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:32:21.983132 l2m2-0.0.2/l2m2.egg-info/
+-rw-r--r--   0 pierce     (503) staff       (20)      371 2024-04-11 22:32:21.000000 l2m2-0.0.2/l2m2.egg-info/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      194 2024-04-11 22:32:21.000000 l2m2-0.0.2/l2m2.egg-info/SOURCES.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-11 22:32:21.000000 l2m2-0.0.2/l2m2.egg-info/dependency_links.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       59 2024-04-11 22:32:21.000000 l2m2-0.0.2/l2m2.egg-info/requires.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-11 22:32:21.000000 l2m2-0.0.2/l2m2.egg-info/top_level.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-11 22:32:21.983618 l2m2-0.0.2/setup.cfg
+-rw-r--r--   0 pierce     (503) staff       (20)      392 2024-04-11 22:32:14.000000 l2m2-0.0.2/setup.py
```

### Comparing `l2m2-0.0.1/l2m2/llm_manager.py` & `l2m2-0.0.2/l2m2/llm_manager.py`

 * *Files identical despite different names*

