# Comparing `tmp/gptscript-0.4.1.tar.gz` & `tmp/gptscript-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptscript-0.4.1.tar", last modified: Thu Apr  4 04:01:09 2024, max compression
+gzip compressed data, was "gptscript-0.4.2.tar", last modified: Fri Apr 12 18:14:06 2024, max compression
```

## Comparing `gptscript-0.4.1.tar` & `gptscript-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.632605 gptscript-0.4.1/
--rw-r--r--   0 wmaxwell   (501) staff       (20)    10175 2024-03-08 22:16:36.000000 gptscript-0.4.1/LICENSE
--rw-r--r--   0 wmaxwell   (501) staff       (20)    19243 2024-04-04 04:01:09.632370 gptscript-0.4.1/PKG-INFO
--rw-r--r--   0 wmaxwell   (501) staff       (20)     7029 2024-04-04 03:59:06.000000 gptscript-0.4.1/README.md
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.631341 gptscript-0.4.1/gptscript/
--rw-r--r--   0 wmaxwell   (501) staff       (20)        0 2024-03-08 22:16:36.000000 gptscript-0.4.1/gptscript/__init__.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     2782 2024-03-08 22:16:36.000000 gptscript-0.4.1/gptscript/command.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)      927 2024-03-08 22:16:36.000000 gptscript-0.4.1/gptscript/exec_utils.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     5452 2024-04-04 03:59:06.000000 gptscript-0.4.1/gptscript/install.py
--rw-r--r--   0 wmaxwell   (501) staff       (20)     1867 2024-04-01 18:37:22.000000 gptscript-0.4.1/gptscript/tool.py
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.632171 gptscript-0.4.1/gptscript.egg-info/
--rw-r--r--   0 wmaxwell   (501) staff       (20)    19243 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/PKG-INFO
--rw-r--r--   0 wmaxwell   (501) staff       (20)      362 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/SOURCES.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)        1 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/dependency_links.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       64 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/entry_points.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       99 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/requires.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)       10 2024-04-04 04:01:09.000000 gptscript-0.4.1/gptscript.egg-info/top_level.txt
--rw-r--r--   0 wmaxwell   (501) staff       (20)      802 2024-04-04 03:59:06.000000 gptscript-0.4.1/pyproject.toml
--rw-r--r--   0 wmaxwell   (501) staff       (20)       38 2024-04-04 04:01:09.632641 gptscript-0.4.1/setup.cfg
-drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-04 04:01:09.632022 gptscript-0.4.1/tests/
--rw-r--r--   0 wmaxwell   (501) staff       (20)     3232 2024-03-08 22:16:36.000000 gptscript-0.4.1/tests/test_gptscript.py
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-12 18:14:06.080641 gptscript-0.4.2/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    10175 2024-03-08 22:16:36.000000 gptscript-0.4.2/LICENSE
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    19243 2024-04-12 18:14:06.080461 gptscript-0.4.2/PKG-INFO
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     7029 2024-04-04 03:59:06.000000 gptscript-0.4.2/README.md
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-12 18:14:06.079277 gptscript-0.4.2/gptscript/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)        0 2024-03-08 22:16:36.000000 gptscript-0.4.2/gptscript/__init__.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     2782 2024-03-08 22:16:36.000000 gptscript-0.4.2/gptscript/command.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      927 2024-03-08 22:16:36.000000 gptscript-0.4.2/gptscript/exec_utils.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     5452 2024-04-12 18:12:33.000000 gptscript-0.4.2/gptscript/install.py
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     1867 2024-04-01 18:37:22.000000 gptscript-0.4.2/gptscript/tool.py
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-12 18:14:06.080265 gptscript-0.4.2/gptscript.egg-info/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)    19243 2024-04-12 18:14:06.000000 gptscript-0.4.2/gptscript.egg-info/PKG-INFO
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      362 2024-04-12 18:14:06.000000 gptscript-0.4.2/gptscript.egg-info/SOURCES.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)        1 2024-04-12 18:14:06.000000 gptscript-0.4.2/gptscript.egg-info/dependency_links.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       64 2024-04-12 18:14:06.000000 gptscript-0.4.2/gptscript.egg-info/entry_points.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       99 2024-04-12 18:14:06.000000 gptscript-0.4.2/gptscript.egg-info/requires.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       10 2024-04-12 18:14:06.000000 gptscript-0.4.2/gptscript.egg-info/top_level.txt
+-rw-r--r--   0 wmaxwell   (501) staff       (20)      802 2024-04-12 18:12:33.000000 gptscript-0.4.2/pyproject.toml
+-rw-r--r--   0 wmaxwell   (501) staff       (20)       38 2024-04-12 18:14:06.080676 gptscript-0.4.2/setup.cfg
+drwxr-xr-x   0 wmaxwell   (501) staff       (20)        0 2024-04-12 18:14:06.080143 gptscript-0.4.2/tests/
+-rw-r--r--   0 wmaxwell   (501) staff       (20)     3232 2024-03-08 22:16:36.000000 gptscript-0.4.2/tests/test_gptscript.py
```

### Comparing `gptscript-0.4.1/LICENSE` & `gptscript-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gptscript-0.4.1/PKG-INFO` & `gptscript-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptscript
-Version: 0.4.1
+Version: 0.4.2
 Summary: Run gptscripts from Python apps
 Author-email: Bill Maxwell <bill@acorn.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gptscript-0.4.1/README.md` & `gptscript-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gptscript-0.4.1/gptscript/command.py` & `gptscript-0.4.2/gptscript/command.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.4.1/gptscript/exec_utils.py` & `gptscript-0.4.2/gptscript/exec_utils.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.4.1/gptscript/install.py` & `gptscript-0.4.2/gptscript/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     # Handle other architectures or set a default/fallback
     arch = "unknown"
     print(f"Warning: Unhandled architecture '{machine}'. This may not be supported.")
 
 gptscript_info = {
     "name": "gptscript",
     "url": "https://github.com/gptscript-ai/gptscript/releases/download/",
-    "version": "v0.4.1",
+    "version": "v0.4.2",
 }
 
 pltfm = {"windows": "windows", "linux": "linux", "darwin": "macOS"}.get(
     platform_name, None
 )
 
 if platform_name == "darwin":
```

### Comparing `gptscript-0.4.1/gptscript/tool.py` & `gptscript-0.4.2/gptscript/tool.py`

 * *Files identical despite different names*

### Comparing `gptscript-0.4.1/gptscript.egg-info/PKG-INFO` & `gptscript-0.4.2/gptscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptscript
-Version: 0.4.1
+Version: 0.4.2
 Summary: Run gptscripts from Python apps
 Author-email: Bill Maxwell <bill@acorn.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gptscript-0.4.1/pyproject.toml` & `gptscript-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.9.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gptscript"
-version = "0.4.1"
+version = "0.4.2"
 description = "Run gptscripts from Python apps"
 readme = "README.md"
 authors = [{ name = "Bill Maxwell", email = "bill@acorn.io" }]
 license = { file = "LICENSE" }
 dependencies = [
     "certifi==2024.2.2",
     "charset-normalizer==3.3.2",
```

### Comparing `gptscript-0.4.1/tests/test_gptscript.py` & `gptscript-0.4.2/tests/test_gptscript.py`

 * *Files identical despite different names*

