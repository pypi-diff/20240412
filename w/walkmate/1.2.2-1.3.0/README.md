# Comparing `tmp/walkmate-1.2.2.tar.gz` & `tmp/walkmate-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walkmate-1.2.2.tar", last modified: Thu Jul 30 16:47:45 2020, max compression
+gzip compressed data, was "walkmate-1.3.0.tar", last modified: Thu Apr 11 23:06:29 2024, max compression
```

## Comparing `walkmate-1.2.2.tar` & `walkmate-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2020-07-30 16:47:45.000000 walkmate-1.2.2/
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/
--rw-r--r--   0 joel       (501) staff       (20)     4704 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)      240 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/SOURCES.txt
--rw-r--r--   0 joel       (501) staff       (20)      238 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/requires.txt
--rw-r--r--   0 joel       (501) staff       (20)        9 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/top_level.txt
--rw-r--r--   0 joel       (501) staff       (20)        1 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/dependency_links.txt
--rw-r--r--   0 joel       (501) staff       (20)     4704 2020-07-30 16:47:45.000000 walkmate-1.2.2/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)     1071 2020-07-30 16:15:15.000000 walkmate-1.2.2/LICENSE.md
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate/
--rw-r--r--   0 joel       (501) staff       (20)       56 2020-07-30 16:42:32.000000 walkmate-1.2.2/walkmate/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)     1805 2020-07-30 16:42:14.000000 walkmate-1.2.2/walkmate/__main__.py
--rw-r--r--   0 joel       (501) staff       (20)     3169 2020-07-30 16:15:15.000000 walkmate-1.2.2/README.md
--rw-r--r--   0 joel       (501) staff       (20)      733 2020-07-30 16:15:15.000000 walkmate-1.2.2/setup.py
--rw-r--r--   0 joel       (501) staff       (20)     1069 2020-07-30 16:47:45.000000 walkmate-1.2.2/setup.cfg
+drwxr-xr-x   0 joel.lefkowitz   (502) staff       (20)        0 2024-04-11 23:06:29.029669 walkmate-1.3.0/
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)      971 2024-04-11 23:06:29.029758 walkmate-1.3.0/PKG-INFO
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)      470 2024-04-11 22:59:05.000000 walkmate-1.3.0/README.md
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)      732 2024-04-11 23:06:29.030093 walkmate-1.3.0/setup.cfg
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)       88 2024-04-11 23:03:42.000000 walkmate-1.3.0/setup.py
+drwxr-xr-x   0 joel.lefkowitz   (502) staff       (20)        0 2024-04-11 23:06:29.028615 walkmate-1.3.0/src/
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)       30 2024-04-11 22:48:59.000000 walkmate-1.3.0/src/__init__.py
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)     1568 2024-04-11 22:55:29.000000 walkmate-1.3.0/src/files.py
+drwxr-xr-x   0 joel.lefkowitz   (502) staff       (20)        0 2024-04-11 23:06:29.029015 walkmate-1.3.0/test/
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)        0 2023-12-03 14:46:23.000000 walkmate-1.3.0/test/__init__.py
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)       34 2024-04-11 22:50:04.000000 walkmate-1.3.0/test/conftest.py
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)      303 2024-04-11 22:49:53.000000 walkmate-1.3.0/test/test_files.py
+drwxr-xr-x   0 joel.lefkowitz   (502) staff       (20)        0 2024-04-11 23:06:29.029551 walkmate-1.3.0/walkmate.egg-info/
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)      971 2024-04-11 23:06:29.000000 walkmate-1.3.0/walkmate.egg-info/PKG-INFO
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)      238 2024-04-11 23:06:29.000000 walkmate-1.3.0/walkmate.egg-info/SOURCES.txt
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)        1 2024-04-11 23:06:29.000000 walkmate-1.3.0/walkmate.egg-info/dependency_links.txt
+-rw-r--r--   0 joel.lefkowitz   (502) staff       (20)        9 2024-04-11 23:06:29.000000 walkmate-1.3.0/walkmate.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

