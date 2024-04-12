# Comparing `tmp/haskellian-either-0.1.6.tar.gz` & `tmp/haskellian_either-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-either-0.1.6.tar", last modified: Tue Apr  9 15:05:50 2024, max compression
+gzip compressed data, was "haskellian_either-0.1.7.tar", last modified: Fri Apr 12 17:46:53 2024, max compression
```

## Comparing `haskellian-either-0.1.6.tar` & `haskellian_either-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.930682 haskellian-either-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-09 15:05:50.930682 haskellian-either-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-09 15:05:48.000000 haskellian-either-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-09 15:05:50.930682 haskellian-either-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      278 2024-04-05 17:36:56.000000 haskellian-either-0.1.6/src/haskellian/either/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian/either/extras/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian-either-0.1.6/src/haskellian/either/extras/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian-either-0.1.6/src/haskellian/either/extras/pydantic.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1228 2024-04-08 10:51:36.000000 haskellian-either-0.1.6/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-04-08 13:18:48.000000 haskellian-either-0.1.6/src/haskellian/either/narrowing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2082 2024-04-09 09:12:43.000000 haskellian-either-0.1.6/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-09 15:05:50.920682 haskellian-either-0.1.6/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-09 15:05:50.000000 haskellian-either-0.1.6/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.787777 haskellian_either-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian_either-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-12 17:46:51.000000 haskellian_either-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-12 17:46:53.787777 haskellian_either-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-12 17:17:47.000000 haskellian_either-0.1.7/src/haskellian/either/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian/either/extras/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       78 2024-04-05 16:46:47.000000 haskellian_either-0.1.7/src/haskellian/either/extras/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-05 16:46:28.000000 haskellian_either-0.1.7/src/haskellian/either/extras/pydantic.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1283 2024-04-12 17:17:42.000000 haskellian_either-0.1.7/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      300 2024-04-08 13:18:48.000000 haskellian_either-0.1.7/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2082 2024-04-09 09:12:43.000000 haskellian_either-0.1.7/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-12 17:46:53.777776 haskellian_either-0.1.7/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      319 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-12 17:46:53.000000 haskellian_either-0.1.7/src/haskellian_either.egg-info/top_level.txt
```

### Comparing `haskellian-either-0.1.6/pyproject.toml` & `haskellian_either-0.1.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian-either"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple Either type"
 dependencies = []
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `haskellian-either-0.1.6/src/haskellian/either/funcs.py` & `haskellian_either-0.1.7/src/haskellian/either/funcs.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     try:
       return Right(func())
     except Exc as e:
       return Left(e)
     
 def maybe(x: R | None) -> 'Either[None, R]':
   return Left(None) if x is None else Right(x)
+
+def unsafe(x: Either[L, R]) -> R:
+  return x.unsafe()
     
 def sequence(eithers: Iterable[Either[L, R]]) -> Either[list[L], list[R]]:
   """List of lefts if any (thus with length in `[1, len(eithers)]`), otherwise list of all rights (with length `len(eithers)`)"""
   lefts: list[L] = []
   rights: list[R] = []
   for x in eithers:
     x.match(lefts.append, rights.append)
```

### Comparing `haskellian-either-0.1.6/src/haskellian/either/type.py` & `haskellian_either-0.1.7/src/haskellian/either/type.py`

 * *Files identical despite different names*

