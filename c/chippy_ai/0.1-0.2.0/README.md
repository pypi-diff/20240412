# Comparing `tmp/chippy-ai-0.1.tar.gz` & `tmp/chippy_ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chippy-ai-0.1.tar", last modified: Thu Apr 11 19:08:51 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `chippy-ai-0.1.tar` & `chippy_ai-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,37 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-11 19:08:51.977347 chippy-ai-0.1/
--rw-r--r--   0 alex       (501) staff       (20)      557 2024-04-11 18:18:36.000000 chippy-ai-0.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)       37 2024-04-11 17:50:29.000000 chippy-ai-0.1/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)       73 2024-04-11 19:08:51.977133 chippy-ai-0.1/PKG-INFO
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-11 19:08:51.975859 chippy-ai-0.1/chip/
--rw-r--r--   0 alex       (501) staff       (20)       24 2024-04-05 21:10:06.000000 chippy-ai-0.1/chip/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    12235 2024-04-11 18:13:57.000000 chippy-ai-0.1/chip/main.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-11 19:08:51.976933 chippy-ai-0.1/chippy_ai.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)       73 2024-04-11 19:08:51.000000 chippy-ai-0.1/chippy_ai.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      226 2024-04-11 19:08:51.000000 chippy-ai-0.1/chippy_ai.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-04-11 19:08:51.000000 chippy-ai-0.1/chippy_ai.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       45 2024-04-11 19:08:51.000000 chippy-ai-0.1/chippy_ai.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)        5 2024-04-11 19:08:51.000000 chippy-ai-0.1/chippy_ai.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-11 19:08:51.977388 chippy-ai-0.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      326 2024-04-11 19:06:19.000000 chippy-ai-0.1/setup.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/git.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/setup.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/shell.txt
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/build/lib/chip/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/build/lib/chip/config.ini
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/build/lib/chip/main.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/build/lib/chippy_ai/__init__.py
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/build/lib/chippy_ai/main.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip.egg-info/top_level.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chip_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai/.gitignore
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai/README.MD
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai/config.ini
+-rw-r--r--   0        0        0    12439 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai/main.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai/pyproject.toml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai.egg-info/entry_points.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/chippy_ai.egg-info/top_level.txt
+-rw-r--r--   0        0        0   340261 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/images/chip1.png
+-rw-r--r--   0        0        0   376104 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/images/chip2.png
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/README.md
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 chippy_ai-0.2.0/PKG-INFO
```

### Comparing `chippy-ai-0.1/LICENSE` & `chippy_ai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chippy-ai-0.1/chip/main.py` & `chippy_ai-0.2.0/build/lib/chip/main.py`

 * *Files identical despite different names*

