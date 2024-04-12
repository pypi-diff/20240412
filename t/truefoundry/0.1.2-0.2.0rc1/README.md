# Comparing `tmp/truefoundry-0.1.2.tar.gz` & `tmp/truefoundry-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.1.2.tar", max compression
+gzip compressed data, was "truefoundry-0.2.0rc1.tar", max compression
```

## Comparing `truefoundry-0.1.2.tar` & `truefoundry-0.2.0rc1.tar`

### file list

```diff
@@ -1,9 +1,31 @@
--rw-r--r--   0        0        0      871 2024-04-05 17:00:29.485450 truefoundry-0.1.2/README.md
--rw-r--r--   0        0        0      655 2024-04-05 17:00:40.725604 truefoundry-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 17:00:29.485450 truefoundry-0.1.2/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      794 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       29 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0       39 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      151 2024-04-05 17:00:29.489450 truefoundry-0.1.2/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 truefoundry-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/README.md
+-rw-r--r--   0        0        0     1487 2024-04-12 05:58:10.178581 truefoundry-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6321 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4428 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2289 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    10660 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0      435 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0       54 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-04-12 05:57:59.986424 truefoundry-0.2.0rc1/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5823 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     5059 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     1751 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0     5358 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0        0 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0     1585 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       29 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-12 05:57:59.990424 truefoundry-0.2.0rc1/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 truefoundry-0.2.0rc1/PKG-INFO
```

### Comparing `truefoundry-0.1.2/README.md` & `truefoundry-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.1.2/PKG-INFO` & `truefoundry-0.2.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.1.2
+Version: 0.2.0rc1
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: autodeploy
 Provides-Extra: ml
+Requires-Dist: docker (>=7.0.0,<8.0.0) ; extra == "autodeploy"
+Requires-Dist: gitignorefile (>=1.1.2,<2.0.0) ; extra == "autodeploy"
+Requires-Dist: gitpython (>=3.1.43,<4.0.0) ; extra == "autodeploy"
 Requires-Dist: mlfoundry (==0.10.9) ; extra == "ml"
+Requires-Dist: openai (>=1.16.2,<2.0.0) ; extra == "autodeploy"
+Requires-Dist: pydantic (>=2.6.4,<3.0.0) ; extra == "autodeploy"
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0) ; extra == "autodeploy"
+Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "autodeploy"
+Requires-Dist: rich (>=13.7.1,<14.0.0) ; extra == "autodeploy"
 Requires-Dist: servicefoundry (==0.10.6)
 Description-Content-Type: text/markdown
 
 # Truefoundry
 
 TrueFoundry library to help you interact with the platform programmatically by
```

