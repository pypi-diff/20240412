# Comparing `tmp/poetry_aws_plugin-0.1.7.tar.gz` & `tmp/poetry_aws_plugin-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_aws_plugin-0.1.7.tar", max compression
+gzip compressed data, was "poetry_aws_plugin-0.1.8.tar", max compression
```

## Comparing `poetry_aws_plugin-0.1.7.tar` & `poetry_aws_plugin-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.7/LICENSE
--rw-r--r--   0        0        0     2831 2024-04-12 00:00:11.575002 poetry_aws_plugin-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.7/poetry_aws_plugin/__init__.py
--rw-r--r--   0        0        0     7005 2024-04-12 15:04:04.161620 poetry_aws_plugin-0.1.7/poetry_aws_plugin/plugin.py
--rw-r--r--   0        0        0      684 2024-04-12 15:04:19.085619 poetry_aws_plugin-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2831 2024-04-12 00:00:11.575002 poetry_aws_plugin-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 17:43:20.828413 poetry_aws_plugin-0.1.8/poetry_aws_plugin/__init__.py
+-rw-r--r--   0        0        0     6099 2024-04-12 16:09:16.337468 poetry_aws_plugin-0.1.8/poetry_aws_plugin/plugin.py
+-rw-r--r--   0        0        0      684 2024-04-12 16:09:55.405467 poetry_aws_plugin-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3604 1970-01-01 00:00:00.000000 poetry_aws_plugin-0.1.8/PKG-INFO
```

### Comparing `poetry_aws_plugin-0.1.7/LICENSE` & `poetry_aws_plugin-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.7/README.md` & `poetry_aws_plugin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `poetry_aws_plugin-0.1.7/poetry_aws_plugin/plugin.py` & `poetry_aws_plugin-0.1.8/poetry_aws_plugin/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+import logging
 import os
 import re
 from typing import Any
 
 import boto3
 import requests
+from requests.utils import rewind_body
 
 from botocore.exceptions import ClientError
-from cleo.io.io import IO, Verbosity
 from poetry.exceptions import PoetryException
-from poetry.poetry import Poetry
 from poetry.plugins import Plugin
 from poetry.publishing.uploader import Uploader
 from poetry.utils.authenticator import Authenticator
 
 POETRY_AWS_PLUGIN_ROLE_ARN_VAR = "POETRY_AWS_PLUGIN_ROLE_ARN"
 POETRY_AWS_PLUGIN_SESSION_NAME = "poetry-aws-plugin"
 POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR = "POETRY_AWS_PLUGIN_AUTH_TOKEN"
@@ -25,171 +25,153 @@
 
 Then make sure you have atleast one of the following:
     1. Authorization for CodeArtifact with your current credentials
     2. Authorization for an IAM role that has access to CodeArtifact and
        environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' set to that role's ARN
 """
 
+logger = logging.getLogger("PoetryAwsPlugin")
 
-def patch(io: IO):
 
-    def is_retryable(response: requests.Response) -> bool:
-        if response.status_code not in UNAUTHORIZED_STATUS_CODES:
-            return False
-        if not re.match(CODEARTIFACT_URL_REGEX, response.url):
-            return False
-        return True
+authenticator_create_session = Authenticator.create_session
+uploader_make_session = Uploader.make_session
 
 
-    def get_auth_token(domain: str, domain_owner: str) -> str:
-        io.write_line(
-            "Getting new CodeArtifact authorization token for "
-            f"domain '{domain}' and domain owner '{domain_owner}'",
-            verbosity=Verbosity.VERBOSE,
-        )
-
-        is_valid = validate_credentials()
-        if not is_valid:
-            return ""
-
-        # We'll try these methods to get the CodeArtifact token
-        methods = [
-            get_auth_token_with_current_credentials,
-            get_auth_token_with_iam_role,
-            get_auth_token_from_env,
-        ]
-        for method in methods:
-            auth_token = method(domain, domain_owner)
-            if auth_token:
-                return auth_token
+def is_retryable(response: requests.Response) -> bool:
+    if response.status_code not in UNAUTHORIZED_STATUS_CODES:
+        return False
+    if not re.match(CODEARTIFACT_URL_REGEX, response.url):
+        return False
+    return True
 
-        return ""
 
+def get_auth_token(domain: str, domain_owner: str) -> str:
+    logger.debug(
+        f"Getting new CodeArtifact authorization token for domain '{domain}' and domain owner '{domain_owner}'"
+    )
 
-    def validate_credentials() -> bool:
-        try:
-            boto3.client("sts").get_caller_identity()
-            return True
-        except ClientError as err:
-            io.write_line(f"Error using current credentials: {err}")
-            return False
-        except Exception as err:
-            io.write_line("Unexpected error while validating AWS credentials")
-            io.write_line(RETRY_ERROR_MESSAGE)
-            raise err
-
-
-    def get_auth_token_with_current_credentials(domain: str, domain_owner: str) -> str:
-        try:
-            token_response = boto3.client("codeartifact").get_authorization_token(
-                domain=domain,
-                domainOwner=domain_owner,
-            )
-            return token_response["authorizationToken"]
-        except ClientError as err:
-            io.write_line(
-                f"Error getting CodeArtifact token using current credentials: {err}",
-                verbosity=Verbosity.VERBOSE,
-            )
-        except Exception as err:
-            io.write_line(
-                f"Unexpected error while getting CodeArtifact authorization token: {err}",
-                verbosity=Verbosity.VERBOSE,
-            )
+    is_valid = validate_credentials()
+    if not is_valid:
         return ""
 
+    # We'll try these methods to get the CodeArtifact token
+    methods = [
+        get_auth_token_with_current_credentials,
+        get_auth_token_with_iam_role,
+        get_auth_token_from_env,
+    ]
+    for method in methods:
+        auth_token = method(domain, domain_owner)
+        if auth_token:
+            return auth_token
+    return ""
+
+
+def validate_credentials() -> bool:
+    try:
+        boto3.client("sts").get_caller_identity()
+        return True
+    except ClientError as err:
+        logger.debug(f"Error using current credentials: {err}")
+        return False
+    except Exception as err:
+        logger.debug(f"Unexpected error while validating AWS credentials\n{RETRY_ERROR_MESSAGE}")
+        raise err
 
-    def get_auth_token_with_iam_role(domain: str, domain_owner: str) -> str:
-        role_arn = os.environ.get(POETRY_AWS_PLUGIN_ROLE_ARN_VAR)
-        if not role_arn:
-            io.write_line(
-                f"Error getting CodeArtifact token using IAM role: "
-                f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found",
-                verbosity=Verbosity.VERBOSE,
-            )
-            return ""
-
-        try:
-            assume_role_response = boto3.client("sts").assume_role(
-                RoleArn=role_arn,
-                RoleSessionName=POETRY_AWS_PLUGIN_SESSION_NAME,
-            )
-            credentials = assume_role_response["Credentials"]
-            session = boto3.Session(
-                aws_access_key_id=credentials["AccessKeyId"],
-                aws_secret_access_key=credentials["SecretAccessKey"],
-                aws_session_token=credentials["SessionToken"],
-            )
-
-            token_response = session.client("codeartifact").get_authorization_token(
-                domain=domain,
-                domainOwner=domain_owner,
-            )
-            return token_response["authorizationToken"]
-        except ClientError as err:
-            io.write_line(
-                f"Error getting CodeArtifact token using IAM role '{role_arn}': {err}",
-                verbosity=Verbosity.VERBOSE,
-            )
-        except Exception as err:
-            io.write_line(
-                "Unexpected error while assuming CodeArtifact role "
-                f"and getting CodeArtifact authorization token: {err}",
-                verbosity=Verbosity.VERBOSE,
-            )
-        return ""
 
+def get_auth_token_with_current_credentials(domain: str, domain_owner: str) -> str:
+    try:
+        token_response = boto3.client("codeartifact").get_authorization_token(
+            domain=domain,
+            domainOwner=domain_owner,
+        )
+        return token_response["authorizationToken"]
+    except ClientError as err:
+        logger.debug(f"Error getting CodeArtifact token using current credentials: {err}")
+    except Exception as err:
+        logger.debug(f"Unexpected error while getting CodeArtifact authorization token: {err}")
+    return ""
 
-    def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
-        return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
 
+def get_auth_token_with_iam_role(domain: str, domain_owner: str) -> str:
+    role_arn = os.environ.get(POETRY_AWS_PLUGIN_ROLE_ARN_VAR)
+    if not role_arn:
+        logger.debug(
+            f"Error getting CodeArtifact token using IAM role: "
+            f"Environment variable '{POETRY_AWS_PLUGIN_ROLE_ARN_VAR}' not found"
+        )
+        return ""
 
-    def patched_session_send(self: requests.Session, request: requests.PreparedRequest, **kwargs: Any) -> requests.Response:
-        response = requests.Session.send(self, request.copy(), **kwargs)
-        if not is_retryable(response):
-            return response
+    try:
+        assume_role_response = boto3.client("sts").assume_role(
+            RoleArn=role_arn,
+            RoleSessionName=POETRY_AWS_PLUGIN_SESSION_NAME,
+        )
+        credentials = assume_role_response["Credentials"]
+        session = boto3.Session(
+            aws_access_key_id=credentials["AccessKeyId"],
+            aws_secret_access_key=credentials["SecretAccessKey"],
+            aws_session_token=credentials["SessionToken"],
+        )
 
-        io.write_line(
-            "Failed to get authorization for CodeArtifact",
-            verbosity=Verbosity.VERBOSE,
+        token_response = session.client("codeartifact").get_authorization_token(
+            domain=domain,
+            domainOwner=domain_owner,
         )
+        return token_response["authorizationToken"]
+    except ClientError as err:
+        logger.debug(f"Error getting CodeArtifact token using IAM role '{role_arn}': {err}")
+    except Exception as err:
+        logger.debug(
+            f"Unexpected error while assuming CodeArtifact role and getting CodeArtifact authorization token: {err}"
+        )
+    return ""
+
+
+def get_auth_token_from_env(*args: Any, **kwargs: Any) -> str:
+    return os.environ.get(POETRY_AWS_PLUGIN_AUTH_TOKEN_VAR, "")
+
+
+def patched_session_send(self: requests.Session, request: requests.PreparedRequest, **kwargs: Any) -> requests.Response:
+    response = requests.Session.send(self, request.copy(), **kwargs.copy())
+    if not is_retryable(response):
+        return response
 
-        match = re.match(CODEARTIFACT_URL_REGEX, response.url)
-        domain, domain_owner = match.groups()
+    logger.debug("Failed to get authorization for CodeArtifact")
 
-        auth_token = get_auth_token(domain, domain_owner)
-        if not auth_token:
-            raise PoetryException(RETRY_ERROR_MESSAGE)
+    match = re.match(CODEARTIFACT_URL_REGEX, response.url)
+    domain, domain_owner = match.groups()
 
-        io.write_line("Successfully got CodeArtifact authorization token\nRetrying request", verbosity=Verbosity.VERBOSE)
+    auth_token = get_auth_token(domain, domain_owner)
+    if not auth_token:
+        raise PoetryException(RETRY_ERROR_MESSAGE)
 
-        # Use the received auth token for the session
-        self.auth = ("aws", auth_token)
+    logger.debug("Successfully got CodeArtifact authorization token\nRetrying request")
 
-        # And create a new request using the new auth
-        new_request = request.copy()
-        new_request.prepare_auth(self.auth, request.url)
+    # Use the received auth token for the session
+    self.auth = ("aws", auth_token)
 
-        # And finally we retry the request
-        return requests.Session.send(self, new_request, **kwargs)
+    # And create a new request using the new auth
+    new_request = request.copy()
+    rewind_body(new_request)
+    new_request.prepare_auth(self.auth, request.url)
 
+    # And finally we retry the request
+    return requests.Session.send(self, new_request, **kwargs)
 
-    def patched_authenticator_create_session(self: Authenticator) -> requests.Session:
-        session = authenticator_create_session(self)
-        session.send = patched_session_send.__get__(session)
-        return session
 
-    def patched_uploader_make_session(self: Uploader) -> requests.Session:
-        session = uploader_make_session(self)
-        session.send = patched_session_send.__get__(session)
-        return session
+def patched_authenticator_create_session(self: Authenticator) -> requests.Session:
+    session = authenticator_create_session(self)
+    session.send = patched_session_send.__get__(session)
+    return session
 
-    authenticator_create_session = Authenticator.create_session
-    uploader_make_session = Uploader.make_session
 
-    Authenticator.create_session = patched_authenticator_create_session
-    Uploader.make_session = patched_uploader_make_session
+def patched_uploader_make_session(self: Uploader) -> requests.Session:
+    session = uploader_make_session(self)
+    session.send = patched_session_send.__get__(session)
+    return session
 
 
 class PoetryAwsPlugin(Plugin):
-    def activate(self, _: Poetry, io: IO) -> None:
-        patch(io)
+    def activate(self, *args: Any, **kwargs: Any) -> None:
+        Authenticator.create_session = patched_authenticator_create_session
+        Uploader.make_session = patched_uploader_make_session
```

### Comparing `poetry_aws_plugin-0.1.7/pyproject.toml` & `poetry_aws_plugin-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-aws-plugin"
-version = "0.1.7"
+version = "0.1.8"
 description = "A poetry plugin to help with AWS CodeArtifact authorization automatically"
 license = "MIT"
 authors = ["Song Huang <xiasongh@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/xiasongh/poetry-aws-plugin"
 keywords = ["aws", "codeartifact", "poetry"]
 packages = [{include = "poetry_aws_plugin"}]
```

### Comparing `poetry_aws_plugin-0.1.7/PKG-INFO` & `poetry_aws_plugin-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-aws-plugin
-Version: 0.1.7
+Version: 0.1.8
 Summary: A poetry plugin to help with AWS CodeArtifact authorization automatically
 Home-page: https://github.com/xiasongh/poetry-aws-plugin
 License: MIT
 Keywords: aws,codeartifact,poetry
 Author: Song Huang
 Author-email: xiasongh@gmail.com
 Requires-Python: >=3.10,<4.0
```

