# Comparing `tmp/wr-cloner-1.9.3.tar.gz` & `tmp/wr-cloner-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wr-cloner-1.9.3.tar", last modified: Wed Oct 18 14:20:25 2023, max compression
+gzip compressed data, was "wr-cloner-1.9.4.tar", last modified: Fri Apr 12 09:57:59 2024, max compression
```

## Comparing `wr-cloner-1.9.3.tar` & `wr-cloner-1.9.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:20:25.089407 wr-cloner-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-10-18 14:20:25.089407 wr-cloner-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:20:25.081407 wr-cloner-1.9.3/cloner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/clone_repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/cloner_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/cpu_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/obtain_repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/put_repos_in_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/cloner/split_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 14:20:25.089407 wr-cloner-1.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:20:25.085407 wr-cloner-1.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/tests/test_cloner_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    19223 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/tests/test_obtain_repos.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/tests/test_put_repos_in_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-10-18 14:20:08.000000 wr-cloner-1.9.3/tests/test_split_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:20:25.085407 wr-cloner-1.9.3/wr_cloner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-10-18 14:20:25.000000 wr-cloner-1.9.3/wr_cloner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-10-18 14:20:25.000000 wr-cloner-1.9.3/wr_cloner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 14:20:25.000000 wr-cloner-1.9.3/wr_cloner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-18 14:20:25.000000 wr-cloner-1.9.3/wr_cloner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-18 14:20:25.000000 wr-cloner-1.9.3/wr_cloner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-18 14:20:25.000000 wr-cloner-1.9.3/wr_cloner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:57:59.675154 wr-cloner-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-12 09:57:59.675154 wr-cloner-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:57:59.671154 wr-cloner-1.9.4/cloner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/clone_repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/cloner_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/cpu_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/obtain_repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/put_repos_in_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/cloner/split_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:57:59.675154 wr-cloner-1.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:57:59.671154 wr-cloner-1.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/tests/test_cloner_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/tests/test_obtain_repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/tests/test_put_repos_in_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-12 09:57:51.000000 wr-cloner-1.9.4/tests/test_split_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:57:59.671154 wr-cloner-1.9.4/wr_cloner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-12 09:57:59.000000 wr-cloner-1.9.4/wr_cloner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-12 09:57:59.000000 wr-cloner-1.9.4/wr_cloner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:57:59.000000 wr-cloner-1.9.4/wr_cloner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 09:57:59.000000 wr-cloner-1.9.4/wr_cloner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-12 09:57:59.000000 wr-cloner-1.9.4/wr_cloner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 09:57:59.000000 wr-cloner-1.9.4/wr_cloner.egg-info/top_level.txt
```

### Comparing `wr-cloner-1.9.3/LICENSE` & `wr-cloner-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/PKG-INFO` & `wr-cloner-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wr-cloner
-Version: 1.9.3
+Version: 1.9.4
 Summary: A tool to clone efficiently all the repos in an organization
 Author: w0rmr1d3r
 License: MIT
 Project-URL: Homepage, https://github.com/w0rmr1d3r/cloner
 Project-URL: Repository, https://github.com/w0rmr1d3r/cloner
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/cloner/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/cloner
@@ -18,26 +18,27 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.0.3
 Requires-Dist: Deprecated>=1.2.13
 Requires-Dist: requests>=2.27.1
 Provides-Extra: dev
-Requires-Dist: black>=22.3.0; extra == "dev"
+Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: coverage>=6.3.2; extra == "dev"
 Requires-Dist: docformatter>=1.5.1; extra == "dev"
 Requires-Dist: faker>=12.0.1; extra == "dev"
 Requires-Dist: pip-tools>=6.5.0; extra == "dev"
 Requires-Dist: pylint>=2.15.10; extra == "dev"
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: responses>=0.20.0; extra == "dev"
```

### Comparing `wr-cloner-1.9.3/README.md` & `wr-cloner-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/cli.py` & `wr-cloner-1.9.4/cloner/cli.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/clone_repos.py` & `wr-cloner-1.9.4/cloner/clone_repos.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/cloner_process.py` & `wr-cloner-1.9.4/cloner/cloner_process.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/cpu_config.py` & `wr-cloner-1.9.4/cloner/cpu_config.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/obtain_repos.py` & `wr-cloner-1.9.4/cloner/obtain_repos.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/put_repos_in_queue.py` & `wr-cloner-1.9.4/cloner/put_repos_in_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/repository.py` & `wr-cloner-1.9.4/cloner/repository.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/cloner/split_queue.py` & `wr-cloner-1.9.4/cloner/split_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/pyproject.toml` & `wr-cloner-1.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,24 @@
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Security",
     "Topic :: Software Development :: Version Control",
     "Topic :: Software Development :: Version Control :: Git",
     "Topic :: System",
 ]
 # Make sure this matches the keywords in GitHub
 keywords = ["github", "python", "git", "clone", "organization", "multiprocessing", "multithreading", "python3"]
 # Make sure this matches the version in __version__.py
-version = "1.9.3"
+version = "1.9.4"
 # Supported Python 3.9 and above
 # If supporting newer versions, update ->  CI and classifiers
 # If minimum version supported changes, update -> CI, coverage, classifiers, pylint, release, contributing.
 requires-python = ">=3.9.0"
 
 # Always try to be compatible with these versions and above
 dependencies = [
@@ -41,15 +42,15 @@
     "Deprecated>=1.2.13",
     "requests>=2.27.1"
 ]
 
 [project.optional-dependencies]
 # Always try to be compatible with these versions and above
 dev = [
-    "black>=22.3.0",
+    "black>=24.3.0",
     "coverage>=6.3.2",
     "docformatter>=1.5.1",
     "faker>=12.0.1",
     "pip-tools>=6.5.0",
     "pylint>=2.15.10",
     "pytest>=6.2.5",
     "responses>=0.20.0",
```

### Comparing `wr-cloner-1.9.3/tests/test_cloner_process.py` & `wr-cloner-1.9.4/tests/test_cloner_process.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/tests/test_obtain_repos.py` & `wr-cloner-1.9.4/tests/test_obtain_repos.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/tests/test_put_repos_in_queue.py` & `wr-cloner-1.9.4/tests/test_put_repos_in_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/tests/test_repository.py` & `wr-cloner-1.9.4/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/tests/test_split_queue.py` & `wr-cloner-1.9.4/tests/test_split_queue.py`

 * *Files identical despite different names*

### Comparing `wr-cloner-1.9.3/wr_cloner.egg-info/PKG-INFO` & `wr-cloner-1.9.4/wr_cloner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wr-cloner
-Version: 1.9.3
+Version: 1.9.4
 Summary: A tool to clone efficiently all the repos in an organization
 Author: w0rmr1d3r
 License: MIT
 Project-URL: Homepage, https://github.com/w0rmr1d3r/cloner
 Project-URL: Repository, https://github.com/w0rmr1d3r/cloner
 Project-URL: Bug Tracker, https://github.com/w0rmr1d3r/cloner/issues
 Project-URL: Documentation, https://github.com/w0rmr1d3r/cloner
@@ -18,26 +18,27 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: System
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.0.3
 Requires-Dist: Deprecated>=1.2.13
 Requires-Dist: requests>=2.27.1
 Provides-Extra: dev
-Requires-Dist: black>=22.3.0; extra == "dev"
+Requires-Dist: black>=24.3.0; extra == "dev"
 Requires-Dist: coverage>=6.3.2; extra == "dev"
 Requires-Dist: docformatter>=1.5.1; extra == "dev"
 Requires-Dist: faker>=12.0.1; extra == "dev"
 Requires-Dist: pip-tools>=6.5.0; extra == "dev"
 Requires-Dist: pylint>=2.15.10; extra == "dev"
 Requires-Dist: pytest>=6.2.5; extra == "dev"
 Requires-Dist: responses>=0.20.0; extra == "dev"
```

### Comparing `wr-cloner-1.9.3/wr_cloner.egg-info/SOURCES.txt` & `wr-cloner-1.9.4/wr_cloner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

