# Comparing `tmp/dedl_stack_client-2024.2.3.tar.gz` & `tmp/dedl_stack_client-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedl_stack_client-2024.2.3.tar", max compression
+gzip compressed data, was "dedl_stack_client-2024.4.1.tar", max compression
```

## Comparing `dedl_stack_client-2024.2.3.tar` & `dedl_stack_client-2024.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10273 2024-02-27 11:52:22.210153 dedl_stack_client-2024.2.3/LICENSE
--rw-r--r--   0        0        0     1178 2024-02-27 11:52:22.210153 dedl_stack_client-2024.2.3/README.md
--rw-r--r--   0        0        0      583 2024-02-27 11:52:22.210153 dedl_stack_client-2024.2.3/dedl_stack_client/__init__.py
--rw-r--r--   0        0        0     2624 2024-02-27 11:52:22.210153 dedl_stack_client-2024.2.3/dedl_stack_client/authn.py
--rw-r--r--   0        0        0     3009 2024-02-27 11:52:22.210153 dedl_stack_client-2024.2.3/dedl_stack_client/dask.py
--rw-r--r--   0        0        0      667 2024-02-27 11:52:22.210153 dedl_stack_client-2024.2.3/pyproject.toml
--rw-r--r--   0        0        0     1813 1970-01-01 00:00:00.000000 dedl_stack_client-2024.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10273 2024-04-12 15:46:49.767080 dedl_stack_client-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     1178 2024-04-12 15:46:49.767080 dedl_stack_client-2024.4.1/README.md
+-rw-r--r--   0        0        0      583 2024-04-12 15:46:49.767080 dedl_stack_client-2024.4.1/dedl_stack_client/__init__.py
+-rw-r--r--   0        0        0     2624 2024-04-12 15:46:49.767080 dedl_stack_client-2024.4.1/dedl_stack_client/authn.py
+-rw-r--r--   0        0        0     3009 2024-04-12 15:46:49.767080 dedl_stack_client-2024.4.1/dedl_stack_client/dask.py
+-rw-r--r--   0        0        0      835 2024-04-12 15:46:49.767080 dedl_stack_client-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 dedl_stack_client-2024.4.1/PKG-INFO
```

### Comparing `dedl_stack_client-2024.2.3/LICENSE` & `dedl_stack_client-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dedl_stack_client-2024.2.3/README.md` & `dedl_stack_client-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dedl_stack_client-2024.2.3/dedl_stack_client/__init__.py` & `dedl_stack_client-2024.4.1/dedl_stack_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dedl_stack_client-2024.2.3/dedl_stack_client/authn.py` & `dedl_stack_client-2024.4.1/dedl_stack_client/authn.py`

 * *Files identical despite different names*

### Comparing `dedl_stack_client-2024.2.3/dedl_stack_client/dask.py` & `dedl_stack_client-2024.4.1/dedl_stack_client/dask.py`

 * *Files identical despite different names*

### Comparing `dedl_stack_client-2024.2.3/pyproject.toml` & `dedl_stack_client-2024.4.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 [tool.poetry]
 name = "dedl-stack-client"
-version = "2024.02.3"
+version = "2024.04.1"
 description = "Python client for DEDL Stack services"
 authors = ["Christoph Reimer <christoph.reimer@eodc.eu>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "dedl_stack_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pyjwt = {extras = ["crypto"], version = ">=2.8.0"}
 dask-gateway = "==2023.1.1"
+requests = ">=2.31.0"
 rich = {extras = ["jupyter"], version = ">=13.6.0"}
 ipykernel = ">=6.26.0"
+cloudpickle = "==2.2.1"
+dask = "==2023.8.0"
+distributed = "==2023.8.0"
+lz4 = "==4.3.2"
+tornado = "==6.3.2"
+msgpack = "==1.0.5"
+toolz = "==0.12.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 pre-commit = "^3.4.0"
```

