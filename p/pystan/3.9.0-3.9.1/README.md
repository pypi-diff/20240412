# Comparing `tmp/pystan-3.9.0.tar.gz` & `tmp/pystan-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystan-3.9.0.tar", max compression
+gzip compressed data, was "pystan-3.9.1.tar", max compression
```

## Comparing `pystan-3.9.0.tar` & `pystan-3.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      749 2024-02-07 14:29:00.091608 pystan-3.9.0/LICENSE
--rw-r--r--   0        0        0     2720 2024-02-07 14:29:00.091608 pystan-3.9.0/README.rst
--rw-r--r--   0        0        0     1295 2024-02-07 14:29:00.095608 pystan-3.9.0/pyproject.toml
--rw-r--r--   0        0        0      160 2024-02-07 14:29:00.095608 pystan-3.9.0/stan/__init__.py
--rw-r--r--   0        0        0     1748 2024-02-07 14:29:00.095608 pystan-3.9.0/stan/common.py
--rw-r--r--   0        0        0    10011 2024-02-07 14:29:00.095608 pystan-3.9.0/stan/fit.py
--rw-r--r--   0        0        0    23351 2024-02-07 14:29:00.095608 pystan-3.9.0/stan/model.py
--rw-r--r--   0        0        0     1353 2024-02-07 14:29:00.095608 pystan-3.9.0/stan/plugins.py
--rw-r--r--   0        0        0     3733 1970-01-01 00:00:00.000000 pystan-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0      749 2024-04-12 14:20:28.625630 pystan-3.9.1/LICENSE
+-rw-r--r--   0        0        0     2720 2024-04-12 14:20:28.625630 pystan-3.9.1/README.rst
+-rw-r--r--   0        0        0     1268 2024-04-12 14:20:28.629631 pystan-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-12 14:20:28.629631 pystan-3.9.1/stan/__init__.py
+-rw-r--r--   0        0        0     1748 2024-04-12 14:20:28.629631 pystan-3.9.1/stan/common.py
+-rw-r--r--   0        0        0    10011 2024-04-12 14:20:28.629631 pystan-3.9.1/stan/fit.py
+-rw-r--r--   0        0        0    23351 2024-04-12 14:20:28.629631 pystan-3.9.1/stan/model.py
+-rw-r--r--   0        0        0     1353 2024-04-12 14:20:28.629631 pystan-3.9.1/stan/plugins.py
+-rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 pystan-3.9.1/PKG-INFO
```

### Comparing `pystan-3.9.0/LICENSE` & `pystan-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystan-3.9.0/README.rst` & `pystan-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pystan-3.9.0/pyproject.toml` & `pystan-3.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pystan"
-version = "3.9.0"
+version = "3.9.1"
 description = "Python interface to Stan, a package for Bayesian inference"
 authors = [
   "Allen Riddell <riddella@indiana.edu>",
   "Ari Hartikainen <ahartikainen@users.noreply.github.com>",
   "Matthew Carter <m.j.carter2@liverpool.ac.uk>",
 ]
 license = "ISC"
@@ -21,29 +21,27 @@
   "License :: OSI Approved :: ISC License (ISCL)",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.6"
 httpstan = "~4.12"
-pysimdjson = "^5.0.2"
+pysimdjson = ">=5.0.2,<7"
 numpy = "^1.19"
 clikit = "^0.6"
 setuptools = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
 pytest-asyncio = "^0.18.3"
-pandas = "^1.0"
-autoflake = "^1.4"
+pandas = ">=1.0,<3"
 black = "22.6.0"
 isort = "^5.9"
 mypy = "0.982"
 types-setuptools = "^57.4"
-flake8 = "^4.0"
 # documentation
 # NOTE: when changing these, update docs-requirements.txt
 sphinx = "^7.2"
 sphinx-rtd-theme = "^2.0"
 
 [tool.black]
 line-length = 119
```

### Comparing `pystan-3.9.0/stan/common.py` & `pystan-3.9.1/stan/common.py`

 * *Files identical despite different names*

### Comparing `pystan-3.9.0/stan/fit.py` & `pystan-3.9.1/stan/fit.py`

 * *Files identical despite different names*

### Comparing `pystan-3.9.0/stan/model.py` & `pystan-3.9.1/stan/model.py`

 * *Files identical despite different names*

### Comparing `pystan-3.9.0/stan/plugins.py` & `pystan-3.9.1/stan/plugins.py`

 * *Files identical despite different names*

### Comparing `pystan-3.9.0/PKG-INFO` & `pystan-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystan
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python interface to Stan, a package for Bayesian inference
 Home-page: https://mc-stan.org
 License: ISC
 Author: Allen Riddell
 Author-email: riddella@indiana.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.6,<4.0)
 Requires-Dist: clikit (>=0.6,<0.7)
 Requires-Dist: httpstan (>=4.12,<4.13)
 Requires-Dist: numpy (>=1.19,<2.0)
-Requires-Dist: pysimdjson (>=5.0.2,<6.0.0)
+Requires-Dist: pysimdjson (>=5.0.2,<7)
 Requires-Dist: setuptools
 Project-URL: Documentation, https://pystan.readthedocs.io
 Project-URL: Repository, https://github.com/stan-dev/pystan
 Description-Content-Type: text/x-rst
 
 ******
 PyStan
```

