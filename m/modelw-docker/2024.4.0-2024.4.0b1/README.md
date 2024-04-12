# Comparing `tmp/modelw_docker-2024.4.0.tar.gz` & `tmp/modelw_docker-2024.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_docker-2024.4.0.tar", max compression
+gzip compressed data, was "modelw_docker-2024.4.0b1.tar", max compression
```

## Comparing `modelw_docker-2024.4.0.tar` & `modelw_docker-2024.4.0b1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      484 2024-04-12 13:11:14.688662 modelw_docker-2024.4.0/LICENSE
--rw-r--r--   0        0        0     4666 2024-04-12 13:11:14.688662 modelw_docker-2024.4.0/README.md
--rw-r--r--   0        0        0     1199 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/__init__.py
--rw-r--r--   0        0        0     2753 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/__main__.py
--rw-r--r--   0        0        0     1494 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/build.py
--rw-r--r--   0        0        0     7307 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/config.py
--rw-r--r--   0        0        0      209 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/exceptions.py
--rw-r--r--   0        0        0     5229 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/install.py
--rw-r--r--   0        0        0     7755 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/output.py
--rw-r--r--   0        0        0     1662 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/platform.py
--rw-r--r--   0        0        0        0 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/py.typed
--rw-r--r--   0        0        0     2580 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/run.py
--rw-r--r--   0        0        0     5865 2024-04-12 13:11:14.692662 modelw_docker-2024.4.0/src/model_w/docker/serve.py
--rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 modelw_docker-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0      484 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/LICENSE
+-rw-r--r--   0        0        0     4666 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/README.md
+-rw-r--r--   0        0        0     1201 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/src/model_w/docker/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-09 15:43:34.520246 modelw_docker-2024.4.0b1/src/model_w/docker/__main__.py
+-rw-r--r--   0        0        0     1494 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/build.py
+-rw-r--r--   0        0        0     7307 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/config.py
+-rw-r--r--   0        0        0      209 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/exceptions.py
+-rw-r--r--   0        0        0     5229 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/install.py
+-rw-r--r--   0        0        0     7755 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/output.py
+-rw-r--r--   0        0        0     1662 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/platform.py
+-rw-r--r--   0        0        0        0 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/py.typed
+-rw-r--r--   0        0        0     2580 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/run.py
+-rw-r--r--   0        0        0     5865 2024-04-09 15:43:34.524246 modelw_docker-2024.4.0b1/src/model_w/docker/serve.py
+-rw-r--r--   0        0        0     5810 1970-01-01 00:00:00.000000 modelw_docker-2024.4.0b1/PKG-INFO
```

### Comparing `modelw_docker-2024.4.0/README.md` & `modelw_docker-2024.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/pyproject.toml` & `modelw_docker-2024.4.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-docker"
-version = "2024.4.0"
+version = "2024.4.0b1"
 description = "Utility to simplify Dockerfiles"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
 readme = "README.md"
 packages = [{include = "model_w/docker", from = "src"}]
 repository = "https://github.com/ModelW/docker/"
 documentation = "https://github.com/ModelW/docker/"
```

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/__main__.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/build.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/build.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/config.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/config.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/install.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/install.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/output.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/output.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/platform.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/platform.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/run.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/run.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/src/model_w/docker/serve.py` & `modelw_docker-2024.4.0b1/src/model_w/docker/serve.py`

 * *Files identical despite different names*

### Comparing `modelw_docker-2024.4.0/PKG-INFO` & `modelw_docker-2024.4.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-docker
-Version: 2024.4.0
+Version: 2024.4.0b1
 Summary: Utility to simplify Dockerfiles
 Home-page: https://github.com/ModelW/docker/
 License: WTFPL
 Keywords: docker,django,nuxt,dockerfile
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.11,<4.0
```

