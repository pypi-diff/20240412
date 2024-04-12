# Comparing `tmp/lineartest-0.4.1.tar.gz` & `tmp/lineartest-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lineartest-0.4.1.tar", max compression
+gzip compressed data, was "lineartest-0.4.2.tar", max compression
```

## Comparing `lineartest-0.4.1.tar` & `lineartest-0.4.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.4.1/LICENSE
--rw-r--r--   0        0        0     1953 2024-04-11 19:09:25.024079 lineartest-0.4.1/README.md
--rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.4.1/lineartest/__init__.py
--rw-r--r--   0        0        0      520 2024-04-11 18:49:51.313315 lineartest-0.4.1/lineartest/_log.py
--rw-r--r--   0        0        0      342 2024-04-11 18:49:58.939025 lineartest-0.4.1/lineartest/_util.py
--rw-r--r--   0        0        0     4061 2024-04-11 19:06:43.803735 lineartest-0.4.1/lineartest/client.py
--rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.4.1/lineartest/schedule.py
--rw-r--r--   0        0        0     1218 2024-04-11 19:10:09.341406 lineartest-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 lineartest-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 12:01:35.618800 lineartest-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1953 2024-04-11 19:09:25.024079 lineartest-0.4.2/README.md
+-rw-r--r--   0        0        0      270 2024-04-10 16:52:53.048727 lineartest-0.4.2/lineartest/__init__.py
+-rw-r--r--   0        0        0      520 2024-04-11 18:49:51.313315 lineartest-0.4.2/lineartest/_log.py
+-rw-r--r--   0        0        0      342 2024-04-11 18:49:58.939025 lineartest-0.4.2/lineartest/_util.py
+-rw-r--r--   0        0        0     4119 2024-04-12 05:38:17.065487 lineartest-0.4.2/lineartest/client.py
+-rw-r--r--   0        0        0     6288 2024-04-10 01:05:25.712505 lineartest-0.4.2/lineartest/schedule.py
+-rw-r--r--   0        0        0     1218 2024-04-12 05:38:49.710828 lineartest-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 lineartest-0.4.2/PKG-INFO
```

### Comparing `lineartest-0.4.1/LICENSE` & `lineartest-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.1/README.md` & `lineartest-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.1/lineartest/_log.py` & `lineartest-0.4.2/lineartest/_log.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.1/lineartest/client.py` & `lineartest-0.4.2/lineartest/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,17 @@
             print(prefix, line, sep='')
 
     @overload
     @wraps(Client.request)
     def request(self, *args, **kwargs) -> Response: ...
 
     @overload
-    def request(self, method, url, *args, response_model: T, **kwargs) -> T: ...
+    def request(
+        self, method: str, url: str, *args, response_model: T, **kwargs
+    ) -> T: ...
 
     def request(
         self, method: str, url: str, *args, response_model: T | None = None, **kwargs
     ) -> T | Response:
         """Perform a request with request and response data logged."""
         # log the start of the request
         print(f' REQUEST START: {method} {url} '.center(self.logging_width, '-'))
@@ -103,21 +105,23 @@
     @overload
     @wraps(Client.get)
     def get(self, *args, **kwargs) -> Response: ...
 
     @overload
     def get(self, *args, response_model: T, **kwargs) -> T: ...
 
-    def get(self, *args, response_model: T | None = None, **kwargs) -> T | Response:
+    def get(
+        self, url: str, *args, response_model: T | None = None, **kwargs
+    ) -> T | Response:
         """Perform a GET request with request and response data logged."""
         return self.request('GET', *args, response_model=response_model, **kwargs)
 
     @overload
     @wraps(Client.post)
     def post(self, *args, **kwargs) -> Response: ...
 
     @overload
-    def post(self, *args, response_model: T, **kwargs) -> T: ...
+    def post(self, url: str, *args, response_model: T, **kwargs) -> T: ...
 
     def post(self, *args, response_model: T | None = None, **kwargs) -> T | Response:
         """Perform a POST request with request and response data logged."""
         return self.request('POST', *args, response_model=response_model, **kwargs)
```

### Comparing `lineartest-0.4.1/lineartest/schedule.py` & `lineartest-0.4.2/lineartest/schedule.py`

 * *Files identical despite different names*

### Comparing `lineartest-0.4.1/pyproject.toml` & `lineartest-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lineartest"
-version = "0.4.1"
+version = "0.4.2"
 description = "A testing framework working with Starlette TestClient."
 authors = ["Philip Fan <topfyf@qq.com>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `lineartest-0.4.1/PKG-INFO` & `lineartest-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lineartest
-Version: 0.4.1
+Version: 0.4.2
 Summary: A testing framework working with Starlette TestClient.
 License: MIT
 Author: Philip Fan
 Author-email: topfyf@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

