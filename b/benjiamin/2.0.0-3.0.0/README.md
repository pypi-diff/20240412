# Comparing `tmp/benjiamin-2.0.0.tar.gz` & `tmp/benjiamin-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benjiamin-2.0.0.tar", last modified: Wed Mar 27 18:51:27 2024, max compression
+gzip compressed data, was "benjiamin-3.0.0.tar", last modified: Fri Apr 12 19:59:57 2024, max compression
```

## Comparing `benjiamin-2.0.0.tar` & `benjiamin-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-03-27 18:51:27.018191 benjiamin-2.0.0/
--rw-r--r--   0 jli17      (501) staff       (20)      322 2024-03-27 18:51:27.017459 benjiamin-2.0.0/PKG-INFO
-drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-03-27 18:51:27.017116 benjiamin-2.0.0/benjiamin.egg-info/
--rw-r--r--   0 jli17      (501) staff       (20)      322 2024-03-27 18:51:26.000000 benjiamin-2.0.0/benjiamin.egg-info/PKG-INFO
--rw-r--r--   0 jli17      (501) staff       (20)      140 2024-03-27 18:51:27.000000 benjiamin-2.0.0/benjiamin.egg-info/SOURCES.txt
--rw-r--r--   0 jli17      (501) staff       (20)        1 2024-03-27 18:51:26.000000 benjiamin-2.0.0/benjiamin.egg-info/dependency_links.txt
--rw-r--r--   0 jli17      (501) staff       (20)        1 2024-03-27 18:51:26.000000 benjiamin-2.0.0/benjiamin.egg-info/top_level.txt
--rw-r--r--   0 jli17      (501) staff       (20)       38 2024-03-27 18:51:27.018249 benjiamin-2.0.0/setup.cfg
--rw-r--r--   0 jli17      (501) staff       (20)      406 2024-03-27 18:49:15.000000 benjiamin-2.0.0/setup.py
+drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 19:59:57.727742 benjiamin-3.0.0/
+-rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 19:59:57.727619 benjiamin-3.0.0/PKG-INFO
+drwxr-xr-x   0 jli17      (501) staff       (20)        0 2024-04-12 19:59:57.727434 benjiamin-3.0.0/benjiamin.egg-info/
+-rw-r--r--   0 jli17      (501) staff       (20)      322 2024-04-12 19:59:57.000000 benjiamin-3.0.0/benjiamin.egg-info/PKG-INFO
+-rw-r--r--   0 jli17      (501) staff       (20)      140 2024-04-12 19:59:57.000000 benjiamin-3.0.0/benjiamin.egg-info/SOURCES.txt
+-rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 19:59:57.000000 benjiamin-3.0.0/benjiamin.egg-info/dependency_links.txt
+-rw-r--r--   0 jli17      (501) staff       (20)        1 2024-04-12 19:59:57.000000 benjiamin-3.0.0/benjiamin.egg-info/top_level.txt
+-rw-r--r--   0 jli17      (501) staff       (20)       38 2024-04-12 19:59:57.727785 benjiamin-3.0.0/setup.cfg
+-rw-r--r--   0 jli17      (501) staff       (20)      406 2024-04-12 19:57:22.000000 benjiamin-3.0.0/setup.py
```

