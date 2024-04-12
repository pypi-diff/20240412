# Comparing `tmp/playwrightcapture-1.24.2.tar.gz` & `tmp/playwrightcapture-1.24.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.24.2.tar", max compression
+gzip compressed data, was "playwrightcapture-1.24.3.tar", max compression
```

## Comparing `playwrightcapture-1.24.2.tar` & `playwrightcapture-1.24.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/LICENSE
--rw-r--r--   0        0        0     1441 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/README.md
--rw-r--r--   0        0        0      511 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    61274 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1764 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1487 2024-04-09 15:25:43.894777 playwrightcapture-1.24.2/pyproject.toml
--rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.2/PKG-INFO
+-rw-r--r--   0        0        0     1775 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/LICENSE
+-rw-r--r--   0        0        0     1441 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/README.md
+-rw-r--r--   0        0        0      511 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    61485 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1764 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1487 2024-04-12 13:07:39.841951 playwrightcapture-1.24.3/pyproject.toml
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 playwrightcapture-1.24.3/PKG-INFO
```

### Comparing `playwrightcapture-1.24.2/LICENSE` & `playwrightcapture-1.24.3/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.2/README.md` & `playwrightcapture-1.24.3/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.2/playwrightcapture/capture.py` & `playwrightcapture-1.24.3/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1077,14 +1077,18 @@
         if '\n' in exception.message:
             name, _ = exception.message.split('\n', maxsplit=1)
             if ' at ' in name:
                 name, _ = name.split(' at ', maxsplit=1)
             elif '; ' in name:
                 name, _ = name.split('; ', maxsplit=1)
             # This is kinda dirty.
+
+            # The format changed in Playwright 1.43.0, the name of the method that failed is set before the exception itself.
+            if ': ' in name:
+                _, name = name.split(': ', maxsplit=1)
             exception._name = name.strip()
 
     def _exception_is_network_error(self, exception: Error) -> bool:
         if exception.name in [
                 'NS_ERROR_ABORT',
                 'NS_ERROR_CONNECTION_REFUSED',
                 'NS_ERROR_NET_INTERRUPT',
```

### Comparing `playwrightcapture-1.24.2/playwrightcapture/helpers.py` & `playwrightcapture-1.24.3/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.24.2/pyproject.toml` & `playwrightcapture-1.24.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.24.2"
+version = "1.24.3"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.24.2/PKG-INFO` & `playwrightcapture-1.24.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlaywrightCapture
-Version: 1.24.2
+Version: 1.24.3
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

