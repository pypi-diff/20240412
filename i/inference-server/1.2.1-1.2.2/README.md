# Comparing `tmp/inference-server-1.2.1.tar.gz` & `tmp/inference-server-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inference-server-1.2.1.tar", last modified: Thu Mar 21 10:18:00 2024, max compression
+gzip compressed data, was "inference-server-1.2.2.tar", last modified: Fri Apr 12 10:13:48 2024, max compression
```

## Comparing `inference-server-1.2.1.tar` & `inference-server-1.2.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.892659 inference-server-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-21 10:17:55.000000 inference-server-1.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-21 10:17:55.000000 inference-server-1.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.884659 inference-server-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.884659 inference-server-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-21 10:17:55.000000 inference-server-1.2.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-03-21 10:17:55.000000 inference-server-1.2.1/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-03-21 10:17:55.000000 inference-server-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-21 10:17:55.000000 inference-server-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-21 10:17:55.000000 inference-server-1.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-03-21 10:17:55.000000 inference-server-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 10:17:55.000000 inference-server-1.2.1/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-03-21 10:18:00.888659 inference-server-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-21 10:17:55.000000 inference-server-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.888659 inference-server-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.888659 inference-server-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/batch_transform.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/inference_server.rst
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/inference_server_testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-21 10:17:55.000000 inference-server-1.2.1/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-21 10:17:55.000000 inference-server-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:18:00.892659 inference-server-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.884659 inference-server-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.888659 inference-server-1.2.1/src/inference_server/
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-03-21 10:17:55.000000 inference-server-1.2.1/src/inference_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-03-21 10:17:55.000000 inference-server-1.2.1/src/inference_server/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-21 10:17:55.000000 inference-server-1.2.1/src/inference_server/default_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-21 10:17:55.000000 inference-server-1.2.1/src/inference_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-03-21 10:17:55.000000 inference-server-1.2.1/src/inference_server/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.888659 inference-server-1.2.1/src/inference_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-03-21 10:18:00.000000 inference-server-1.2.1/src/inference_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-21 10:18:00.000000 inference-server-1.2.1/src/inference_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:18:00.000000 inference-server-1.2.1/src/inference_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-21 10:18:00.000000 inference-server-1.2.1/src/inference_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-21 10:18:00.000000 inference-server-1.2.1/src/inference_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:18:00.888659 inference-server-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-21 10:17:55.000000 inference-server-1.2.1/tests/test_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-21 10:17:55.000000 inference-server-1.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.890920 inference-server-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 10:13:41.000000 inference-server-1.2.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 10:13:41.000000 inference-server-1.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.882920 inference-server-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.886920 inference-server-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-12 10:13:41.000000 inference-server-1.2.2/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-12 10:13:41.000000 inference-server-1.2.2/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-12 10:13:41.000000 inference-server-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 10:13:41.000000 inference-server-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 10:13:41.000000 inference-server-1.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-04-12 10:13:41.000000 inference-server-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-12 10:13:41.000000 inference-server-1.2.2/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-04-12 10:13:48.890920 inference-server-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-12 10:13:41.000000 inference-server-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.886920 inference-server-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.886920 inference-server-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/batch_transform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/inference_server.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/inference_server_testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 10:13:41.000000 inference-server-1.2.2/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-12 10:13:41.000000 inference-server-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:13:48.890920 inference-server-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.882920 inference-server-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.890920 inference-server-1.2.2/src/inference_server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-12 10:13:41.000000 inference-server-1.2.2/src/inference_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-12 10:13:41.000000 inference-server-1.2.2/src/inference_server/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-12 10:13:41.000000 inference-server-1.2.2/src/inference_server/default_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 10:13:41.000000 inference-server-1.2.2/src/inference_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-12 10:13:41.000000 inference-server-1.2.2/src/inference_server/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.890920 inference-server-1.2.2/src/inference_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14841 2024-04-12 10:13:48.000000 inference-server-1.2.2/src/inference_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-12 10:13:48.000000 inference-server-1.2.2/src/inference_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:13:48.000000 inference-server-1.2.2/src/inference_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 10:13:48.000000 inference-server-1.2.2/src/inference_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 10:13:48.000000 inference-server-1.2.2/src/inference_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:13:48.890920 inference-server-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-12 10:13:41.000000 inference-server-1.2.2/tests/test_inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-12 10:13:41.000000 inference-server-1.2.2/tox.ini
```

### Comparing `inference-server-1.2.1/.flake8` & `inference-server-1.2.2/.flake8`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/.github/workflows/release-package.yml` & `inference-server-1.2.2/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/.github/workflows/test-package.yml` & `inference-server-1.2.2/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/.gitignore` & `inference-server-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/.pre-commit-config.yaml` & `inference-server-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/.readthedocs.yaml` & `inference-server-1.2.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/LICENSE` & `inference-server-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/LICENSE_HEADER.txt` & `inference-server-1.2.2/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/PKG-INFO` & `inference-server-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.2.1
+Version: 1.2.2
 Summary: Deploy your AI/ML model to Amazon SageMaker for Real-Time Inference and Batch Transform using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.2.1/README.md` & `inference-server-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/docs/batch_transform.rst` & `inference-server-1.2.2/docs/batch_transform.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/docs/conf.py` & `inference-server-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/docs/deployment.rst` & `inference-server-1.2.2/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/docs/hooks.rst` & `inference-server-1.2.2/docs/hooks.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/docs/introduction.rst` & `inference-server-1.2.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/docs/testing.rst` & `inference-server-1.2.2/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/pyproject.toml` & `inference-server-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/src/inference_server/__init__.py` & `inference-server-1.2.2/src/inference_server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     import importlib_metadata as metadata  # type: ignore
 
 __all__ = (
     "BatchStrategy",
     "MIMEAccept",  # Exporting for plugin developers' convenience
     "create_app",
     "plugin_hook",
+    "warmup",
 )
 
 #: Library version, e.g. 1.0.0, taken from Git tags
 __version__ = metadata.version("inference-server")
 
 #: Well known location for model artifacts
 _MODEL_DIR = "/opt/ml/model"
@@ -66,20 +67,28 @@
     #: Batch Transform job to invoke the model with a single record per request
     SINGLE_RECORD = "SingleRecord"
     #: Batch Transform job to invoke the model with multiple records per request
     MULTI_RECORD = "MultiRecord"
 
 
 def create_app() -> "WSGIApplication":
-    """Initialize and return the WSGI application"""
+    """
+    Initialize and return the WSGI application
+
+    This is the WSGI application factory function that needs to be passed to a WSGI-compatible web server.
+    """
     return _app
 
 
 def warmup() -> None:
-    """Initialize any additional resources upfront"""
+    """
+    Initialize any additional resources upfront
+
+    This will call the ``model_fn`` plugin hook.
+    """
     _model()
 
 
 @werkzeug.Request.application
 def _app(request: werkzeug.Request) -> werkzeug.Response:
     """Return the WSGI application"""
     try:
```

### Comparing `inference-server-1.2.1/src/inference_server/_plugin.py` & `inference-server-1.2.2/src/inference_server/_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/src/inference_server/default_plugin.py` & `inference-server-1.2.2/src/inference_server/default_plugin.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/src/inference_server/testing.py` & `inference-server-1.2.2/src/inference_server/testing.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/src/inference_server.egg-info/PKG-INFO` & `inference-server-1.2.2/src/inference_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inference-server
-Version: 1.2.1
+Version: 1.2.2
 Summary: Deploy your AI/ML model to Amazon SageMaker for Real-Time Inference and Batch Transform using your own Docker container image.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `inference-server-1.2.1/src/inference_server.egg-info/SOURCES.txt` & `inference-server-1.2.2/src/inference_server.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pyproject.toml
 tox.ini
 .github/workflows/release-package.yml
 .github/workflows/test-package.yml
 docs/batch_transform.rst
 docs/conf.py
 docs/deployment.rst
+docs/faq.rst
 docs/hooks.rst
 docs/index.rst
 docs/inference_server.rst
 docs/inference_server_testing.rst
 docs/introduction.rst
 docs/modules.rst
 docs/testing.rst
```

### Comparing `inference-server-1.2.1/tests/test_inference_server.py` & `inference-server-1.2.2/tests/test_inference_server.py`

 * *Files identical despite different names*

### Comparing `inference-server-1.2.1/tox.ini` & `inference-server-1.2.2/tox.ini`

 * *Files identical despite different names*

