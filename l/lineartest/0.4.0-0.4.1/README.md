# Comparing `tmp/lineartest-0.4.0.tar.gz` & `tmp/lineartest-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.4.0.tar", max compression
+gzip compressed data, was "lineartest-0.4.1.tar", max compression
```

## Comparing `lineartest-0.4.0.tar` & `lineartest-0.4.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.4.0/LICENSE
--rw-r--r--   0        0        0     1930 2024-04-11 10:51:08.025696 lineartest-0.4.0/README.md
--rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.4.0/lineartest/__init__.py
--rw-r--r--   0        0        0      520 2024-04-10 01:05:25.711594 lineartest-0.4.0/lineartest/_log.py
--rw-r--r--   0        0        0     7405 2024-04-11 10:46:29.727763 lineartest-0.4.0/lineartest/client.py
--rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.4.0/lineartest/schedule.py
--rw-r--r--   0        0        0     1196 2024-04-11 10:51:49.865980 lineartest-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2792 1970-01-01 00:00:00.000000 lineartest-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1953 2024-04-11 19:09:25.024079 lineartest-0.4.1/README.md
+-rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.4.1/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-11 18:49:51.313315 lineartest-0.4.1/lineartest/_log.py
+-rw-r--r--   0        0        0      342 2024-04-11 18:49:58.939025 lineartest-0.4.1/lineartest/_util.py
+-rw-r--r--   0        0        0     4061 2024-04-11 19:06:43.803735 lineartest-0.4.1/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.4.1/lineartest/schedule.py
+-rw-r--r--   0        0        0     1218 2024-04-11 19:10:09.341406 lineartest-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 lineartest-0.4.1/PKG-INFO
```

### Comparing `lineartest-0.4.0/LICENSE` & `lineartest-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.0/README.md` & `lineartest-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # LinearTest
-A testing framework working with httpx.
+A testing framework working with Starlette TestClient.
 
 - **Source code**: https://github.com/fanyf22/lineartest/
 - **Documentation**: https://fanyf22.github.io/lineartest/
 
 ## Dependencies
 
-```requirements
-python>=3.10
-pydantic>=2.6.4
-pyyaml>=6.0.1
-httpx>=0.27.0
+```toml
+python = "^3.10"
+pydantic = "^2.6.4"
+pyyaml = "^6.0.1"
+httpx = "^0.27.0"
 ```
 
 ## Installing
 
 The package is published on https://pypi.org/lineartest.
 
 Use `pip` or similar commands to install it:
```

### Comparing `lineartest-0.4.0/lineartest/_log.py` & `lineartest-0.4.1/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.0/lineartest/schedule.py` & `lineartest-0.4.1/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.0/pyproject.toml` & `lineartest-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.4.0"
+version = "0.4.1"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -28,14 +28,15 @@
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.21.3"
 ruff = "^0.3.5"
 pre-commit = "^3.7.0"
 isort = "^5.13.2"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.17"
+starlette = "^0.37.2"
 
 
 [tool.poetry.group.test.dependencies]
 fastapi = "^0.110.1"
 python-multipart = "^0.0.9"
 starlette = "^0.37.2"
```

### Comparing `lineartest-0.4.0/PKG-INFO` & `lineartest-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.4.0
+Version: 0.4.1
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,26 +18,26 @@
 Classifier: Programming Language :: Python :: 3.13
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # LinearTest
-A testing framework working with httpx.
+A testing framework working with Starlette TestClient.
 
 - **Source code**: https://github.com/fanyf22/lineartest/
 - **Documentation**: https://fanyf22.github.io/lineartest/
 
 ## Dependencies
 
-```requirements
-python>=3.10
-pydantic>=2.6.4
-pyyaml>=6.0.1
-httpx>=0.27.0
+```toml
+python = "^3.10"
+pydantic = "^2.6.4"
+pyyaml = "^6.0.1"
+httpx = "^0.27.0"
 ```
 
 ## Installing
 
 The package is published on https://pypi.org/lineartest.
 
 Use `pip` or similar commands to install it:
```

