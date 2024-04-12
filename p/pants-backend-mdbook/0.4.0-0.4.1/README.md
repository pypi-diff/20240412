# Comparing `tmp/pants_backend_mdbook-0.4.0.tar.gz` & `tmp/pants_backend_mdbook-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pants_backend_mdbook-0.4.0.tar", last modified: Fri Apr  5 14:47:07 2024, max compression
+gzip compressed data, was "pants_backend_mdbook-0.4.1.tar", last modified: Fri Apr 12 13:13:57 2024, max compression
```

## Comparing `pants_backend_mdbook-0.4.0.tar` & `pants_backend_mdbook-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/LICENSE-MIT.txt
--rw-r--r--   0        0        0      726 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/README.md
--rw-r--r--   0        0        0        9 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/__init__.py
--rw-r--r--   0        0        0       99 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/goals/__init__.py
--rw-r--r--   0        0        0     1022 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/goals/package.py
--rw-r--r--   0        0        0      255 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/register.py
--rw-r--r--   0        0        0     1440 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/subsystem.py
--rw-r--r--   0        0        0      727 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/targets.py
--rw-r--r--   0        0        0      153 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/build.py
--rw-r--r--   0        0        0     2379 2024-04-05 14:47:07.753885 pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/prepare.py
--rw-r--r--   0        0        0     1093 2024-04-05 14:47:07.983885 pants_backend_mdbook-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 pants_backend_mdbook-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/LICENSE-MIT.txt
+-rw-r--r--   0        0        0      726 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/README.md
+-rw-r--r--   0        0        0        9 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/goals/__init__.py
+-rw-r--r--   0        0        0     1022 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/goals/package.py
+-rw-r--r--   0        0        0      255 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/register.py
+-rw-r--r--   0        0        0     1611 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/subsystem.py
+-rw-r--r--   0        0        0      727 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/targets.py
+-rw-r--r--   0        0        0      153 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/util_rules/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/util_rules/build.py
+-rw-r--r--   0        0        0     2379 2024-04-12 13:13:57.098229 pants_backend_mdbook-0.4.1/pants_backend_mdbook/util_rules/prepare.py
+-rw-r--r--   0        0        0     1093 2024-04-12 13:13:57.218228 pants_backend_mdbook-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2648 1970-01-01 00:00:00.000000 pants_backend_mdbook-0.4.1/PKG-INFO
```

### Comparing `pants_backend_mdbook-0.4.0/LICENSE-MIT.txt` & `pants_backend_mdbook-0.4.1/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `pants_backend_mdbook-0.4.0/README.md` & `pants_backend_mdbook-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pants_backend_mdbook-0.4.0/pants_backend_mdbook/goals/package.py` & `pants_backend_mdbook-0.4.1/pants_backend_mdbook/goals/package.py`

 * *Files identical despite different names*

### Comparing `pants_backend_mdbook-0.4.0/pants_backend_mdbook/subsystem.py` & `pants_backend_mdbook-0.4.1/pants_backend_mdbook/subsystem.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 from pants.core.util_rules.external_tool import ExternalTool
 from pants.engine.platform import Platform
 
 _mdbook_platform_mapping = {
     "linux_x86_64": "x86_64-unknown-linux-gnu",
     "linux_arm64": "aarch64-unknown-linux-musl",
     "macos_x86_64": "x86_64-apple-darwin",
+    "macos_arm64": "x86_64-apple-darwin",
 }
 
 
 class MdBookTool(ExternalTool):
     options_scope = "mdbook"
     help = "The MdBook tool used to build static webpages."
 
     default_version = "v0.4.35"
     default_known_versions = [
+        # using rosetta
+        "v0.4.35|macos_arm64 |ca3281c2b5437a1ccd9079ed8121b3dd97c49be74dae32ea803b540a38c334bb|4701269",
         "v0.4.35|macos_x86_64|ca3281c2b5437a1ccd9079ed8121b3dd97c49be74dae32ea803b540a38c334bb|4701269",
         "v0.4.35|linux_x86_64|4ef777bfcb3fd01687deed990372a6eb5e125f79b592014b0ac09b61595f0b34|5348678",
         "v0.4.35|linux_arm64 |359af01b77fbd6bf6243a3f2b2491a37b5480bbb2674eb2d94f91354253b34f4|5442606",
         "v0.4.21|macos_x86_64|c1f3e8235f8b3128f6020397061c97444007e090ac42358402d3f25eee8499bd|4292102",
         "v0.4.21|linux_x86_64|ec3c978a255b444987fd6e0805147f4ea75d221f68c6e27dbf3e8a28aba166b7|4861607",
     ]
```

### Comparing `pants_backend_mdbook-0.4.0/pants_backend_mdbook/targets.py` & `pants_backend_mdbook-0.4.1/pants_backend_mdbook/targets.py`

 * *Files identical despite different names*

### Comparing `pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/build.py` & `pants_backend_mdbook-0.4.1/pants_backend_mdbook/util_rules/build.py`

 * *Files identical despite different names*

### Comparing `pants_backend_mdbook-0.4.0/pants_backend_mdbook/util_rules/prepare.py` & `pants_backend_mdbook-0.4.1/pants_backend_mdbook/util_rules/prepare.py`

 * *Files identical despite different names*

### Comparing `pants_backend_mdbook-0.4.0/pyproject.toml` & `pants_backend_mdbook-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pants_backend_mdbook"
 description = "A  MdBook documentation builder plugin for the Pants buildsystem."
-version = "0.4.0"
+version = "0.4.1"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = []
 readme = "README.md"
 keywords = [
     "pantsbuild",
```

### Comparing `pants_backend_mdbook-0.4.0/PKG-INFO` & `pants_backend_mdbook-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pants_backend_mdbook
-Version: 0.4.0
+Version: 0.4.1
 Summary: A  MdBook documentation builder plugin for the Pants buildsystem.
 Keywords: pantsbuild pants backend mdbook markdown
 Author-Email: Tom Solberg <me@sbg.dev>
 License: MIT License
         
         Copyright (c) 2022 Tom Solberg
```

