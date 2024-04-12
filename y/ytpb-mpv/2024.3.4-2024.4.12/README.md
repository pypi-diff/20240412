# Comparing `tmp/ytpb_mpv-2024.3.4.tar.gz` & `tmp/ytpb_mpv-2024.4.12.tar.gz`

## Comparing `ytpb_mpv-2024.3.4.tar` & `ytpb_mpv-2024.4.12.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/src/ytpb_mpv/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/src/ytpb_mpv/__main__.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/src/ytpb_mpv/cli.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/LICENSE
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/LICENSE~
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/pyproject.toml
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 ytpb_mpv-2024.3.4/PKG-INFO
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/src/ytpb_mpv/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/src/ytpb_mpv/__main__.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/src/ytpb_mpv/cli.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/src/ytpb_mpv/listener.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/LICENSE
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/LICENSE~
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/README.md
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/pyproject.toml
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 ytpb_mpv-2024.4.12/PKG-INFO
```

### Comparing `ytpb_mpv-2024.3.4/.gitignore` & `ytpb_mpv-2024.4.12/.gitignore`

 * *Files identical despite different names*

### Comparing `ytpb_mpv-2024.3.4/LICENSE` & `ytpb_mpv-2024.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `ytpb_mpv-2024.3.4/LICENSE~` & `ytpb_mpv-2024.4.12/LICENSE~`

 * *Files identical despite different names*

### Comparing `ytpb_mpv-2024.3.4/pyproject.toml` & `ytpb_mpv-2024.4.12/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 requires = [ "hatchling", "hatch-vcs" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "ytpb-mpv"
 description = "A socket listener to complement mpv-ytpb"
 readme = "README.md"
-version = "2024.3.4"
+version = "2024.4.12"
 authors = [ { name = "Maxim Stolyarchuk" } ]
 keywords = [ "mpv", "youtube" ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Console",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.11"
 dependencies = [
-    "ytpb",
+    "ytpb>=2024.4.12",
     "python-mpv-jsonipc>=1.2.0",
 ]
 
 [project.scripts]
 ytpb-mpv = "ytpb_mpv.__main__:main"
```

### Comparing `ytpb_mpv-2024.3.4/PKG-INFO` & `ytpb_mpv-2024.4.12/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytpb-mpv
-Version: 2024.3.4
+Version: 2024.4.12
 Summary: A socket listener to complement mpv-ytpb
 Author: Maxim Stolyarchuk
 License: MIT License
         
         Copyright (c) 2024 Maxim Stolyarchuk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,13 +30,13 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Requires-Dist: python-mpv-jsonipc>=1.2.0
-Requires-Dist: ytpb
+Requires-Dist: ytpb>=2024.4.12
 Description-Content-Type: text/markdown
 
 # ytpb-mpv
 
 See [mpv-ytpb](https://github.com/xymaxim/mpv-ytpb) for more information.
```

