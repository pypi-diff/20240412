# Comparing `tmp/trial_IGNchinmay-0.0.3.tar.gz` & `tmp/trial_IGNchinmay-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trial_IGNchinmay-0.0.3.tar", last modified: Thu Apr 11 10:44:52 2024, max compression
+gzip compressed data, was "trial_IGNchinmay-0.0.4.tar", last modified: Fri Apr 12 05:26:05 2024, max compression
```

## Comparing `trial_IGNchinmay-0.0.3.tar` & `trial_IGNchinmay-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 10:44:52.274470 trial_IGNchinmay-0.0.3/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)    11356 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.3/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      830 2024-04-11 10:44:52.274470 trial_IGNchinmay-0.0.3/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      212 2024-04-11 07:36:58.000000 trial_IGNchinmay-0.0.3/README.md
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      688 2024-04-11 10:44:10.000000 trial_IGNchinmay-0.0.3/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       38 2024-04-11 10:44:52.274470 trial_IGNchinmay-0.0.3/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 10:44:52.274470 trial_IGNchinmay-0.0.3/trial_IGNchinmay/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       41 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.3/trial_IGNchinmay/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)     3078 2024-04-11 07:16:32.000000 trial_IGNchinmay-0.0.3/trial_IGNchinmay/json_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 10:44:52.274470 trial_IGNchinmay-0.0.3/trial_IGNchinmay.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      830 2024-04-11 10:44:52.000000 trial_IGNchinmay-0.0.3/trial_IGNchinmay.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      252 2024-04-11 10:44:52.000000 trial_IGNchinmay-0.0.3/trial_IGNchinmay.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)        1 2024-04-11 10:44:52.000000 trial_IGNchinmay-0.0.3/trial_IGNchinmay.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       17 2024-04-11 10:44:52.000000 trial_IGNchinmay-0.0.3/trial_IGNchinmay.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 05:26:05.046627 trial_IGNchinmay-0.0.4/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)    11356 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.4/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      828 2024-04-12 05:26:05.046627 trial_IGNchinmay-0.0.4/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      210 2024-04-11 11:08:55.000000 trial_IGNchinmay-0.0.4/README.md
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      688 2024-04-12 05:25:21.000000 trial_IGNchinmay-0.0.4/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       38 2024-04-12 05:26:05.046627 trial_IGNchinmay-0.0.4/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 05:26:05.046627 trial_IGNchinmay-0.0.4/trial_IGNchinmay/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       41 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.4/trial_IGNchinmay/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)     3058 2024-04-11 16:19:19.000000 trial_IGNchinmay-0.0.4/trial_IGNchinmay/json_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 05:26:05.046627 trial_IGNchinmay-0.0.4/trial_IGNchinmay.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      828 2024-04-12 05:26:05.000000 trial_IGNchinmay-0.0.4/trial_IGNchinmay.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      252 2024-04-12 05:26:05.000000 trial_IGNchinmay-0.0.4/trial_IGNchinmay.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)        1 2024-04-12 05:26:05.000000 trial_IGNchinmay-0.0.4/trial_IGNchinmay.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       17 2024-04-12 05:26:05.000000 trial_IGNchinmay-0.0.4/trial_IGNchinmay.egg-info/top_level.txt
```

### Comparing `trial_IGNchinmay-0.0.3/LICENSE` & `trial_IGNchinmay-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trial_IGNchinmay-0.0.3/PKG-INFO` & `trial_IGNchinmay-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trial_IGNchinmay
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,10 +13,10 @@
 License-File: LICENSE
 
 # icutils
 <div align="center">
   <img src="ignitarium-logo.png">
 </div>
 
-[![PyPI version](https://badge.fury.io/py/icutil-IGNchinmay.svg)](https://badge.fury.io/py/icutil-IGNchinmay)
+[![PyPI version](https://badge.fury.io/py/trial-IGNchinmay.svg)](https://badge.fury.io/py/trial-IGNchinmay)
 
 A sample test package for CV
```

### Comparing `trial_IGNchinmay-0.0.3/pyproject.toml` & `trial_IGNchinmay-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trial_IGNchinmay"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `trial_IGNchinmay-0.0.3/trial_IGNchinmay/json_utils.py` & `trial_IGNchinmay-0.0.4/trial_IGNchinmay/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 class TestJsonUtils(unittest.TestCase):
     """test json utils"""
 
     @classmethod
     def setUpClass(cls):
         """Edit sample docker daemon config file with nvidia runtime."""
-        cls.FILENAME = "trial_IGNchinmay/samples/daemon_sample.json"
+        cls.FILENAME = "test/daemon_sample.json"
         cls.key_list = ("runtimes", "nvidia", "path")
         cls.val = random.random()
         cls.VALUE = "/usr/bin/nvidia-container-runtime - " + str(cls.val)
 
     def test_edit_json(self):
         """tests the edit json function"""
         print("Testing edit json function \n")
```

### Comparing `trial_IGNchinmay-0.0.3/trial_IGNchinmay.egg-info/PKG-INFO` & `trial_IGNchinmay-0.0.4/trial_IGNchinmay.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trial_IGNchinmay
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,10 +13,10 @@
 License-File: LICENSE
 
 # icutils
 <div align="center">
   <img src="ignitarium-logo.png">
 </div>
 
-[![PyPI version](https://badge.fury.io/py/icutil-IGNchinmay.svg)](https://badge.fury.io/py/icutil-IGNchinmay)
+[![PyPI version](https://badge.fury.io/py/trial-IGNchinmay.svg)](https://badge.fury.io/py/trial-IGNchinmay)
 
 A sample test package for CV
```

