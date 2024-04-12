# Comparing `tmp/poetry_aws_plugin-0.1.6.tar.gz` & `tmp/poetry_aws_plugin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.6.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.7.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.6.tar` & `poetry_aws_plugin-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.6/LICENSE
--rw-r--r--   0        0        0     2831 2024-04-12 00:00:11.575002 poetry_aws_plugin-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.6/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     7219 2024-04-12 01:34:59.890781 poetry_aws_plugin-0.1.6/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-12 01:06:27.466848 poetry_aws_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2831 2024-04-12 00:00:11.575002 poetry_aws_plugin-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.7/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     7005 2024-04-12 15:04:04.161620 poetry_aws_plugin-0.1.7/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-12 15:04:19.085619 poetry_aws_plugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.7/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.6/LICENSE` & `poetry_aws_plugin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.6/README.md` & `poetry_aws_plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.6/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.7/poetry_aws_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 
 
     def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
         return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
 
     def patched_session_send(self: requests.Session, request: requests.PreparedRequest, **kwargs: Any) -> requests.Response:
-        response = requests.Session.send(self, request, **kwargs)
+        response = requests.Session.send(self, request.copy(), **kwargs)
         if not is_retryable(response):
             return response
 
         io.write_line(
             "Failed to get authorization for CodeArtifact",
             verbosity=Verbosity.VERBOSE,
         )
@@ -163,19 +163,15 @@
         io.write_line("Successfully got CodeArtifact authorization token\nRetrying request", verbosity=Verbosity.VERBOSE)
 
         # Use the received auth token for the session
         self.auth = ("aws", auth_token)
 
         # And create a new request using the new auth
         new_request = request.copy()
-
-        # We must call prepare_hook after prepare_auth
-        # https://github.com/psf/requests/blob/31ebb8102c00f8cf8b396a6356743cca4362e07b/src/requests/models.py#L376
         new_request.prepare_auth(self.auth, request.url)
-        new_request.prepare_hooks(request.hooks)
 
         # And finally we retry the request
         return requests.Session.send(self, new_request, **kwargs)
 
 
     def patched_authenticator_create_session(self: Authenticator) -> requests.Session:
         session = authenticator_create_session(self)
```

### Comparing `poetry_aws_plugin-0.1.6/pyproject.toml` & `poetry_aws_plugin-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.6"
+version = "0.1.7"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.6/PKG-INFO` & `poetry_aws_plugin-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
```

