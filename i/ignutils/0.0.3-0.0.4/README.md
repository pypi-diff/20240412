# Comparing `tmp/ignutils-0.0.3.tar.gz` & `tmp/ignutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignutils-0.0.3.tar", last modified: Thu Apr 11 09:16:53 2024, max compression
+gzip compressed data, was "ignutils-0.0.4.tar", last modified: Thu Apr 11 11:47:06 2024, max compression
```

## Comparing `ignutils-0.0.3.tar` & `ignutils-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 09:16:53.361853 ignutils-0.0.3/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-11 07:58:25.000000 ignutils-0.0.3/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-11 09:16:53.361853 ignutils-0.0.3/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      602 2024-04-11 09:16:46.000000 ignutils-0.0.3/README.md
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 09:16:53.361853 ignutils-0.0.3/ignutils/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       33 2024-04-11 07:58:25.000000 ignutils-0.0.3/ignutils/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3070 2024-04-11 07:58:25.000000 ignutils-0.0.3/ignutils/json_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 09:16:53.361853 ignutils-0.0.3/ignutils.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      252 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       10 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-11 09:16:53.000000 ignutils-0.0.3/ignutils.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      806 2024-04-11 09:16:46.000000 ignutils-0.0.3/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-11 07:58:25.000000 ignutils-0.0.3/requirements.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-11 09:16:53.361853 ignutils-0.0.3/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 11:47:06.451787 ignutils-0.0.4/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)    11356 2024-04-11 07:58:25.000000 ignutils-0.0.4/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-11 11:47:06.451787 ignutils-0.0.4/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      602 2024-04-11 09:16:46.000000 ignutils-0.0.4/README.md
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 11:47:06.451787 ignutils-0.0.4/ignutils/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       33 2024-04-11 07:58:25.000000 ignutils-0.0.4/ignutils/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)     3070 2024-04-11 07:58:25.000000 ignutils-0.0.4/ignutils/json_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (997)        0 2024-04-11 11:47:06.451787 ignutils-0.0.4/ignutils.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (997)     1221 2024-04-11 11:47:06.000000 ignutils-0.0.4/ignutils.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      252 2024-04-11 11:47:06.000000 ignutils-0.0.4/ignutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        1 2024-04-11 11:47:06.000000 ignutils-0.0.4/ignutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       10 2024-04-11 11:47:06.000000 ignutils-0.0.4/ignutils.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-11 11:47:06.000000 ignutils-0.0.4/ignutils.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)      806 2024-04-11 11:47:00.000000 ignutils-0.0.4/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)        9 2024-04-11 07:58:25.000000 ignutils-0.0.4/requirements.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (997)       38 2024-04-11 11:47:06.451787 ignutils-0.0.4/setup.cfg
```

### Comparing `ignutils-0.0.3/LICENSE` & `ignutils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.3/PKG-INFO` & `ignutils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/ignutils/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/ignutils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ignutils-0.0.3/README.md` & `ignutils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.3/ignutils/json_utils.py` & `ignutils-0.0.4/ignutils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ignutils-0.0.3/ignutils.egg-info/PKG-INFO` & `ignutils-0.0.4/ignutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/ignutils/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/ignutils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ignutils-0.0.3/pyproject.toml` & `ignutils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ignutils"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

